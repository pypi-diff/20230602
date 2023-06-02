# Comparing `tmp/sysnet-persons-1.0.1.tar.gz` & `tmp/sysnet-persons-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-persons-1.0.1.tar", last modified: Fri May 19 08:09:12 2023, max compression
+gzip compressed data, was "sysnet-persons-1.0.2.tar", last modified: Fri Jun  2 18:22:56 2023, max compression
```

## Comparing `sysnet-persons-1.0.1.tar` & `sysnet-persons-1.0.2.tar`

### file list

```diff
@@ -1,88 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/
--rw-rw-rw-   0        0        0    11558 2022-09-22 12:06:50.000000 sysnet-persons-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    28378 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    14312 2023-05-19 08:07:51.000000 sysnet-persons-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.764594 sysnet-persons-1.0.1/persons/
--rw-rw-rw-   0        0        0     2230 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.780231 sysnet-persons-1.0.1/persons/api/
--rw-rw-rw-   0        0        0      316 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/persons/api/__init__.py
--rw-rw-rw-   0        0        0    25661 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api/admins_api.py
--rw-rw-rw-   0        0        0     6822 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api/developers_api.py
--rw-rw-rw-   0        0        0    38477 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api/link_api.py
--rw-rw-rw-   0        0        0    53758 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/persons/api/manage_api.py
--rw-rw-rw-   0        0        0    72247 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/persons/api/public_api.py
--rw-rw-rw-   0        0        0    25005 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api_client.py
--rw-rw-rw-   0        0        0     8212 2023-05-19 08:05:47.000000 sysnet-persons-1.0.1/persons/configuration.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.836197 sysnet-persons-1.0.1/persons/models/
--rw-rw-rw-   0        0        0     1863 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/__init__.py
--rw-rw-rw-   0        0        0     3703 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/code_value_type.py
--rw-rw-rw-   0        0        0     2987 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/config_body.py
--rw-rw-rw-   0        0        0    13229 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/contact_type.py
--rw-rw-rw-   0        0        0     5277 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/context_type.py
--rw-rw-rw-   0        0        0     5903 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/context_type_persons.py
--rw-rw-rw-   0        0        0     3959 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/context_type_roles.py
--rw-rw-rw-   0        0        0     5128 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/department_type.py
--rw-rw-rw-   0        0        0     5839 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/document_entry.py
--rw-rw-rw-   0        0        0     7568 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/document_entry_list.py
--rw-rw-rw-   0        0        0     8241 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/document_metadata_type.py
--rw-rw-rw-   0        0        0     3621 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/geo_point_jtsk_type.py
--rw-rw-rw-   0        0        0     3693 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/geo_point_type.py
--rw-rw-rw-   0        0        0    13655 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/individual_type.py
--rw-rw-rw-   0        0        0     5363 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/issuing_type.py
--rw-rw-rw-   0        0        0     9273 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/location_type.py
--rw-rw-rw-   0        0        0     3859 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/mail_address_type.py
--rw-rw-rw-   0        0        0     5498 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/member_type.py
--rw-rw-rw-   0        0        0     5363 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/person_link_type.py
--rw-rw-rw-   0        0        0     6767 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/person_list_item.py
--rw-rw-rw-   0        0        0    17547 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/person_type.py
--rw-rw-rw-   0        0        0     4586 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/phone_number_type.py
--rw-rw-rw-   0        0        0     5231 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/reference_registry.py
--rw-rw-rw-   0        0        0     5405 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/role_category_type.py
--rw-rw-rw-   0        0        0     5206 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/role_list_item.py
--rw-rw-rw-   0        0        0    10766 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/role_type.py
--rw-rw-rw-   0        0        0     3761 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/tag_item_type.py
--rw-rw-rw-   0        0        0     3042 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/tag_type.py
--rw-rw-rw-   0        0        0    12985 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/rest.py
--rw-rw-rw-   0        0        0      673 2023-05-19 08:07:51.000000 sysnet-persons-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-05-19 07:57:55.000000 sysnet-persons-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.851858 sysnet-persons-1.0.1/sysnet_persons.egg-info/
--rw-rw-rw-   0        0        0    28378 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2324 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/test/
--rw-rw-rw-   0        0        0       15 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     1673 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_admins_api.py
--rw-rw-rw-   0        0        0      862 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_code_value_type.py
--rw-rw-rw-   0        0        0      836 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_config_body.py
--rw-rw-rw-   0        0        0      844 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_contact_type.py
--rw-rw-rw-   0        0        0      844 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_context_type.py
--rw-rw-rw-   0        0        0      902 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_context_type_persons.py
--rw-rw-rw-   0        0        0      886 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_context_type_roles.py
--rw-rw-rw-   0        0        0      868 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_department_type.py
--rw-rw-rw-   0        0        0      955 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_developers_api.py
--rw-rw-rw-   0        0        0      860 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_document_entry.py
--rw-rw-rw-   0        0        0      894 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_document_entry_list.py
--rw-rw-rw-   0        0        0      918 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_document_metadata_type.py
--rw-rw-rw-   0        0        0      888 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_geo_point_jtsk_type.py
--rw-rw-rw-   0        0        0      854 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_geo_point_type.py
--rw-rw-rw-   0        0        0      868 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_individual_type.py
--rw-rw-rw-   0        0        0      844 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_issuing_type.py
--rw-rw-rw-   0        0        0     2080 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_link_api.py
--rw-rw-rw-   0        0        0      852 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_location_type.py
--rw-rw-rw-   0        0        0      878 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_mail_address_type.py
--rw-rw-rw-   0        0        0     3163 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_manage_api.py
--rw-rw-rw-   0        0        0      836 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_member_type.py
--rw-rw-rw-   0        0        0      870 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_person_link_type.py
--rw-rw-rw-   0        0        0      870 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_person_list_item.py
--rw-rw-rw-   0        0        0      836 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_person_type.py
--rw-rw-rw-   0        0        0      878 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_phone_number_type.py
--rw-rw-rw-   0        0        0     3629 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_public_api.py
--rw-rw-rw-   0        0        0      892 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_reference_registry.py
--rw-rw-rw-   0        0        0      886 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_role_category_type.py
--rw-rw-rw-   0        0        0      854 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_role_list_item.py
--rw-rw-rw-   0        0        0      820 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_role_type.py
--rw-rw-rw-   0        0        0      846 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_tag_item_type.py
--rw-rw-rw-   0        0        0      812 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_tag_type.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:22:56.358207 sysnet-persons-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2022-09-22 12:06:50.000000 sysnet-persons-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    29120 2023-06-02 18:22:56.357615 sysnet-persons-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15046 2023-06-02 18:19:00.000000 sysnet-persons-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 18:22:56.183925 sysnet-persons-1.0.2/persons/
+-rw-rw-rw-   0        0        0     2511 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:22:56.196825 sysnet-persons-1.0.2/persons/api/
+-rw-rw-rw-   0        0        0      363 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/api/__init__.py
+-rw-rw-rw-   0        0        0    25661 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/api/admins_api.py
+-rw-rw-rw-   0        0        0     6822 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/api/developers_api.py
+-rw-rw-rw-   0        0        0    38477 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/api/link_api.py
+-rw-rw-rw-   0        0        0    16179 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/api/manage2_api.py
+-rw-rw-rw-   0        0        0    53758 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/api/manage_api.py
+-rw-rw-rw-   0        0        0    72247 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/api/public_api.py
+-rw-rw-rw-   0        0        0    25005 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/api_client.py
+-rw-rw-rw-   0        0        0     8212 2023-06-02 18:19:00.000000 sysnet-persons-1.0.2/persons/configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:22:56.271269 sysnet-persons-1.0.2/persons/models/
+-rw-rw-rw-   0        0        0     2097 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/__init__.py
+-rw-rw-rw-   0        0        0     3703 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/code_value_type.py
+-rw-rw-rw-   0        0        0     2987 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/config_body.py
+-rw-rw-rw-   0        0        0    13229 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/contact_type.py
+-rw-rw-rw-   0        0        0     5277 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/context_type.py
+-rw-rw-rw-   0        0        0     5903 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/context_type_persons.py
+-rw-rw-rw-   0        0        0     3959 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/context_type_roles.py
+-rw-rw-rw-   0        0        0     5128 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/department_type.py
+-rw-rw-rw-   0        0        0     5839 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/document_entry.py
+-rw-rw-rw-   0        0        0     7568 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/document_entry_list.py
+-rw-rw-rw-   0        0        0     8241 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/document_metadata_type.py
+-rw-rw-rw-   0        0        0     3621 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/geo_point_jtsk_type.py
+-rw-rw-rw-   0        0        0     3693 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/models/geo_point_type.py
+-rw-rw-rw-   0        0        0     6083 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/individual_list_type.py
+-rw-rw-rw-   0        0        0    13655 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/individual_type.py
+-rw-rw-rw-   0        0        0     5363 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/issuing_type.py
+-rw-rw-rw-   0        0        0     9273 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/location_type.py
+-rw-rw-rw-   0        0        0     3859 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/mail_address_type.py
+-rw-rw-rw-   0        0        0     5498 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/member_type.py
+-rw-rw-rw-   0        0        0     5363 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/person_link_type.py
+-rw-rw-rw-   0        0        0     6767 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/person_list_item.py
+-rw-rw-rw-   0        0        0     5975 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/person_list_type.py
+-rw-rw-rw-   0        0        0    17547 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/person_type.py
+-rw-rw-rw-   0        0        0     4586 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/phone_number_type.py
+-rw-rw-rw-   0        0        0     5231 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/reference_registry.py
+-rw-rw-rw-   0        0        0     5405 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/role_category_type.py
+-rw-rw-rw-   0        0        0     5206 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/role_list_item.py
+-rw-rw-rw-   0        0        0     5921 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/role_list_type.py
+-rw-rw-rw-   0        0        0    10766 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/role_type.py
+-rw-rw-rw-   0        0        0     3761 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/tag_item_type.py
+-rw-rw-rw-   0        0        0     5894 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/tag_list_type.py
+-rw-rw-rw-   0        0        0     3042 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/persons/models/tag_type.py
+-rw-rw-rw-   0        0        0    12985 2023-06-02 07:43:58.000000 sysnet-persons-1.0.2/persons/rest.py
+-rw-rw-rw-   0        0        0      673 2023-06-02 18:19:00.000000 sysnet-persons-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 18:22:56.358713 sysnet-persons-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-06-02 07:44:00.000000 sysnet-persons-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:22:56.280269 sysnet-persons-1.0.2/sysnet_persons.egg-info/
+-rw-rw-rw-   0        0        0    29120 2023-06-02 18:22:56.000000 sysnet-persons-1.0.2/sysnet_persons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2023-06-02 18:22:56.000000 sysnet-persons-1.0.2/sysnet_persons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 18:22:56.000000 sysnet-persons-1.0.2/sysnet_persons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-02 18:22:56.000000 sysnet-persons-1.0.2/sysnet_persons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 18:22:56.000000 sysnet-persons-1.0.2/sysnet_persons.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 18:22:56.355502 sysnet-persons-1.0.2/test/
+-rw-rw-rw-   0        0        0       15 2023-05-19 07:57:54.000000 sysnet-persons-1.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     1673 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_admins_api.py
+-rw-rw-rw-   0        0        0      862 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_code_value_type.py
+-rw-rw-rw-   0        0        0      836 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_config_body.py
+-rw-rw-rw-   0        0        0      844 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_contact_type.py
+-rw-rw-rw-   0        0        0      844 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_context_type.py
+-rw-rw-rw-   0        0        0      902 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_context_type_persons.py
+-rw-rw-rw-   0        0        0      886 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_context_type_roles.py
+-rw-rw-rw-   0        0        0      868 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_department_type.py
+-rw-rw-rw-   0        0        0      955 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_developers_api.py
+-rw-rw-rw-   0        0        0      860 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_document_entry.py
+-rw-rw-rw-   0        0        0      894 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_document_entry_list.py
+-rw-rw-rw-   0        0        0      918 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_document_metadata_type.py
+-rw-rw-rw-   0        0        0      888 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_geo_point_jtsk_type.py
+-rw-rw-rw-   0        0        0      854 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_geo_point_type.py
+-rw-rw-rw-   0        0        0      902 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_individual_list_type.py
+-rw-rw-rw-   0        0        0      868 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_individual_type.py
+-rw-rw-rw-   0        0        0      844 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_issuing_type.py
+-rw-rw-rw-   0        0        0     2080 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_link_api.py
+-rw-rw-rw-   0        0        0      852 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_location_type.py
+-rw-rw-rw-   0        0        0      878 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_mail_address_type.py
+-rw-rw-rw-   0        0        0     1302 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_manage2_api.py
+-rw-rw-rw-   0        0        0     3163 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_manage_api.py
+-rw-rw-rw-   0        0        0      836 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_member_type.py
+-rw-rw-rw-   0        0        0      870 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_person_link_type.py
+-rw-rw-rw-   0        0        0      870 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_person_list_item.py
+-rw-rw-rw-   0        0        0      870 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_person_list_type.py
+-rw-rw-rw-   0        0        0      836 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_person_type.py
+-rw-rw-rw-   0        0        0      878 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_phone_number_type.py
+-rw-rw-rw-   0        0        0     3629 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_public_api.py
+-rw-rw-rw-   0        0        0      892 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_reference_registry.py
+-rw-rw-rw-   0        0        0      886 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_role_category_type.py
+-rw-rw-rw-   0        0        0      854 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_role_list_item.py
+-rw-rw-rw-   0        0        0      854 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_role_list_type.py
+-rw-rw-rw-   0        0        0      820 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_role_type.py
+-rw-rw-rw-   0        0        0      846 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_tag_item_type.py
+-rw-rw-rw-   0        0        0      846 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_tag_list_type.py
+-rw-rw-rw-   0        0        0      812 2023-06-02 07:43:59.000000 sysnet-persons-1.0.2/test/test_tag_type.py
```

### Comparing `sysnet-persons-1.0.1/LICENSE` & `sysnet-persons-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sysnet-persons-1.0.1/PKG-INFO` & `sysnet-persons-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-persons
-Version: 1.0.1
+Version: 1.0.2
 Summary: SYSNET Persons Registry REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,34 +212,34 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sysnet-persons
+# persons
 This is a API to Persons Registry
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.1
-- Package version: 1.0.1
+- API version: 1.0.2
+- Package version: 1.0.2
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 3.9+
+Python 2.7 and 3.4+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-persons
+pip install --upgrade sysnet-persons
 ```
 
 Then import the package:
 ```python
 import persons 
 ```
 
@@ -390,15 +390,15 @@
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_tag: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/persons/1.0.1*
+All URIs are relative to *https://service.sysnet.cz/persons/1.0.2*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**delete_tag**](docs/AdminsApi.md#delete_tag) | **DELETE** /tag/{name} | odstraní definici tagu  (cruD)
 *AdminsApi* | [**get_config**](docs/AdminsApi.md#get_config) | **GET** /config | získá konfiguraci konektoru
 *AdminsApi* | [**get_tag**](docs/AdminsApi.md#get_tag) | **GET** /tag/{name} | vrací definici tagu (cRud)
 *AdminsApi* | [**get_tag_list**](docs/AdminsApi.md#get_tag_list) | **GET** /tag | vrací seznam tagů v systému (autocomplete)
@@ -428,14 +428,18 @@
 *ManageApi* | [**import_individuals_replace**](docs/ManageApi.md#import_individuals_replace) | **POST** /individual/data | Nahradí všechny uživatele
 *ManageApi* | [**import_persons**](docs/ManageApi.md#import_persons) | **PUT** /person/data | Importuje subjekty
 *ManageApi* | [**import_persons_replace**](docs/ManageApi.md#import_persons_replace) | **POST** /person/data | Nahradí všechny subjekty
 *ManageApi* | [**import_roles**](docs/ManageApi.md#import_roles) | **PUT** /role/data | Importuje role
 *ManageApi* | [**import_roles_replace**](docs/ManageApi.md#import_roles_replace) | **POST** /role/data | Nahradí všechny role
 *ManageApi* | [**import_tags**](docs/ManageApi.md#import_tags) | **PUT** /tag/data | Importuje tagy
 *ManageApi* | [**import_tags_replace**](docs/ManageApi.md#import_tags_replace) | **POST** /tag/data | Nahradí všechny tagy
+*Manage2Api* | [**get_all_idividuals**](docs/Manage2Api.md#get_all_idividuals) | **GET** /all/individuals | Vrací všechny uživatele pro Admin Portal
+*Manage2Api* | [**get_all_persons**](docs/Manage2Api.md#get_all_persons) | **GET** /all/persons | Vrací všechny subjekty pro Admin Portal
+*Manage2Api* | [**get_all_roles**](docs/Manage2Api.md#get_all_roles) | **GET** /all/roles | Vrací všechny role pro Admin Portal
+*Manage2Api* | [**get_all_tags**](docs/Manage2Api.md#get_all_tags) | **GET** /all/tags | Vrací všechny tagy pro Admin Portal
 *PublicApi* | [**delete_individual**](docs/PublicApi.md#delete_individual) | **DELETE** /individual/{identifier} | odstraní registrační dokument jednotlivce s daným identifikátorem (cruD)
 *PublicApi* | [**delete_person**](docs/PublicApi.md#delete_person) | **DELETE** /person/{identifier} | odstraní registrační dokument subjektu s daným identifikátorem (cruD)
 *PublicApi* | [**delete_role**](docs/PublicApi.md#delete_role) | **DELETE** /role/{identifier} | odstraní roli s daným identifikátorem (cruD)
 *PublicApi* | [**get_context**](docs/PublicApi.md#get_context) | **GET** /context/{identifier} | vrací kontext jednotlivce
 *PublicApi* | [**get_individual**](docs/PublicApi.md#get_individual) | **GET** /individual/{identifier} | vrací registrační dokument jednotlivce s daným identifikátorem (cRud)
 *PublicApi* | [**get_individual_list**](docs/PublicApi.md#get_individual_list) | **GET** /individual | vrací seznam jednotlivců (autocomplete)
 *PublicApi* | [**get_person**](docs/PublicApi.md#get_person) | **GET** /person/{identifier} | vrací registrační dokument subjektu s daným identifikátorem (cRud)
@@ -460,28 +464,32 @@
  - [ContextTypeRoles](docs/ContextTypeRoles.md)
  - [DepartmentType](docs/DepartmentType.md)
  - [DocumentEntry](docs/DocumentEntry.md)
  - [DocumentEntryList](docs/DocumentEntryList.md)
  - [DocumentMetadataType](docs/DocumentMetadataType.md)
  - [GeoPointJtskType](docs/GeoPointJtskType.md)
  - [GeoPointType](docs/GeoPointType.md)
+ - [IndividualListType](docs/IndividualListType.md)
  - [IndividualType](docs/IndividualType.md)
  - [IssuingType](docs/IssuingType.md)
  - [LocationType](docs/LocationType.md)
  - [MailAddressType](docs/MailAddressType.md)
  - [MemberType](docs/MemberType.md)
  - [PersonLinkType](docs/PersonLinkType.md)
  - [PersonListItem](docs/PersonListItem.md)
+ - [PersonListType](docs/PersonListType.md)
  - [PersonType](docs/PersonType.md)
  - [PhoneNumberType](docs/PhoneNumberType.md)
  - [ReferenceRegistry](docs/ReferenceRegistry.md)
  - [RoleCategoryType](docs/RoleCategoryType.md)
  - [RoleListItem](docs/RoleListItem.md)
+ - [RoleListType](docs/RoleListType.md)
  - [RoleType](docs/RoleType.md)
  - [TagItemType](docs/TagItemType.md)
+ - [TagListType](docs/TagListType.md)
  - [TagType](docs/TagType.md)
 
 ## Documentation For Authorization
 
 
 ## apiKey
```

### Comparing `sysnet-persons-1.0.1/README.md` & `sysnet-persons-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# sysnet-persons
+# persons
 This is a API to Persons Registry
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.1
-- Package version: 1.0.1
+- API version: 1.0.2
+- Package version: 1.0.2
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 3.9+
+Python 2.7 and 3.4+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-persons
+pip install --upgrade sysnet-persons
 ```
 
 Then import the package:
 ```python
 import persons 
 ```
 
@@ -172,15 +172,15 @@
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_tag: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/persons/1.0.1*
+All URIs are relative to *https://service.sysnet.cz/persons/1.0.2*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**delete_tag**](docs/AdminsApi.md#delete_tag) | **DELETE** /tag/{name} | odstraní definici tagu  (cruD)
 *AdminsApi* | [**get_config**](docs/AdminsApi.md#get_config) | **GET** /config | získá konfiguraci konektoru
 *AdminsApi* | [**get_tag**](docs/AdminsApi.md#get_tag) | **GET** /tag/{name} | vrací definici tagu (cRud)
 *AdminsApi* | [**get_tag_list**](docs/AdminsApi.md#get_tag_list) | **GET** /tag | vrací seznam tagů v systému (autocomplete)
@@ -210,14 +210,18 @@
 *ManageApi* | [**import_individuals_replace**](docs/ManageApi.md#import_individuals_replace) | **POST** /individual/data | Nahradí všechny uživatele
 *ManageApi* | [**import_persons**](docs/ManageApi.md#import_persons) | **PUT** /person/data | Importuje subjekty
 *ManageApi* | [**import_persons_replace**](docs/ManageApi.md#import_persons_replace) | **POST** /person/data | Nahradí všechny subjekty
 *ManageApi* | [**import_roles**](docs/ManageApi.md#import_roles) | **PUT** /role/data | Importuje role
 *ManageApi* | [**import_roles_replace**](docs/ManageApi.md#import_roles_replace) | **POST** /role/data | Nahradí všechny role
 *ManageApi* | [**import_tags**](docs/ManageApi.md#import_tags) | **PUT** /tag/data | Importuje tagy
 *ManageApi* | [**import_tags_replace**](docs/ManageApi.md#import_tags_replace) | **POST** /tag/data | Nahradí všechny tagy
+*Manage2Api* | [**get_all_idividuals**](docs/Manage2Api.md#get_all_idividuals) | **GET** /all/individuals | Vrací všechny uživatele pro Admin Portal
+*Manage2Api* | [**get_all_persons**](docs/Manage2Api.md#get_all_persons) | **GET** /all/persons | Vrací všechny subjekty pro Admin Portal
+*Manage2Api* | [**get_all_roles**](docs/Manage2Api.md#get_all_roles) | **GET** /all/roles | Vrací všechny role pro Admin Portal
+*Manage2Api* | [**get_all_tags**](docs/Manage2Api.md#get_all_tags) | **GET** /all/tags | Vrací všechny tagy pro Admin Portal
 *PublicApi* | [**delete_individual**](docs/PublicApi.md#delete_individual) | **DELETE** /individual/{identifier} | odstraní registrační dokument jednotlivce s daným identifikátorem (cruD)
 *PublicApi* | [**delete_person**](docs/PublicApi.md#delete_person) | **DELETE** /person/{identifier} | odstraní registrační dokument subjektu s daným identifikátorem (cruD)
 *PublicApi* | [**delete_role**](docs/PublicApi.md#delete_role) | **DELETE** /role/{identifier} | odstraní roli s daným identifikátorem (cruD)
 *PublicApi* | [**get_context**](docs/PublicApi.md#get_context) | **GET** /context/{identifier} | vrací kontext jednotlivce
 *PublicApi* | [**get_individual**](docs/PublicApi.md#get_individual) | **GET** /individual/{identifier} | vrací registrační dokument jednotlivce s daným identifikátorem (cRud)
 *PublicApi* | [**get_individual_list**](docs/PublicApi.md#get_individual_list) | **GET** /individual | vrací seznam jednotlivců (autocomplete)
 *PublicApi* | [**get_person**](docs/PublicApi.md#get_person) | **GET** /person/{identifier} | vrací registrační dokument subjektu s daným identifikátorem (cRud)
@@ -242,28 +246,32 @@
  - [ContextTypeRoles](docs/ContextTypeRoles.md)
  - [DepartmentType](docs/DepartmentType.md)
  - [DocumentEntry](docs/DocumentEntry.md)
  - [DocumentEntryList](docs/DocumentEntryList.md)
  - [DocumentMetadataType](docs/DocumentMetadataType.md)
  - [GeoPointJtskType](docs/GeoPointJtskType.md)
  - [GeoPointType](docs/GeoPointType.md)
+ - [IndividualListType](docs/IndividualListType.md)
  - [IndividualType](docs/IndividualType.md)
  - [IssuingType](docs/IssuingType.md)
  - [LocationType](docs/LocationType.md)
  - [MailAddressType](docs/MailAddressType.md)
  - [MemberType](docs/MemberType.md)
  - [PersonLinkType](docs/PersonLinkType.md)
  - [PersonListItem](docs/PersonListItem.md)
+ - [PersonListType](docs/PersonListType.md)
  - [PersonType](docs/PersonType.md)
  - [PhoneNumberType](docs/PhoneNumberType.md)
  - [ReferenceRegistry](docs/ReferenceRegistry.md)
  - [RoleCategoryType](docs/RoleCategoryType.md)
  - [RoleListItem](docs/RoleListItem.md)
+ - [RoleListType](docs/RoleListType.md)
  - [RoleType](docs/RoleType.md)
  - [TagItemType](docs/TagItemType.md)
+ - [TagListType](docs/TagListType.md)
  - [TagType](docs/TagType.md)
 
 ## Documentation For Authorization
 
 
 ## apiKey
```

### Comparing `sysnet-persons-1.0.1/persons/__init__.py` & `sysnet-persons-1.0.2/persons/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 # flake8: noqa
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
 from persons.api.admins_api import AdminsApi
 from persons.api.developers_api import DevelopersApi
 from persons.api.link_api import LinkApi
 from persons.api.manage_api import ManageApi
+from persons.api.manage2_api import Manage2Api
 from persons.api.public_api import PublicApi
 # import ApiClient
 from persons.api_client import ApiClient
 from persons.configuration import Configuration
 # import models into sdk package
 from persons.models.code_value_type import CodeValueType
 from persons.models.config_body import ConfigBody
@@ -32,22 +33,26 @@
 from persons.models.context_type_roles import ContextTypeRoles
 from persons.models.department_type import DepartmentType
 from persons.models.document_entry import DocumentEntry
 from persons.models.document_entry_list import DocumentEntryList
 from persons.models.document_metadata_type import DocumentMetadataType
 from persons.models.geo_point_jtsk_type import GeoPointJtskType
 from persons.models.geo_point_type import GeoPointType
+from persons.models.individual_list_type import IndividualListType
 from persons.models.individual_type import IndividualType
 from persons.models.issuing_type import IssuingType
 from persons.models.location_type import LocationType
 from persons.models.mail_address_type import MailAddressType
 from persons.models.member_type import MemberType
 from persons.models.person_link_type import PersonLinkType
 from persons.models.person_list_item import PersonListItem
+from persons.models.person_list_type import PersonListType
 from persons.models.person_type import PersonType
 from persons.models.phone_number_type import PhoneNumberType
 from persons.models.reference_registry import ReferenceRegistry
 from persons.models.role_category_type import RoleCategoryType
 from persons.models.role_list_item import RoleListItem
+from persons.models.role_list_type import RoleListType
 from persons.models.role_type import RoleType
 from persons.models.tag_item_type import TagItemType
+from persons.models.tag_list_type import TagListType
 from persons.models.tag_type import TagType
```

### Comparing `sysnet-persons-1.0.1/persons/api/admins_api.py` & `sysnet-persons-1.0.2/persons/api/admins_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/api/developers_api.py` & `sysnet-persons-1.0.2/persons/api/developers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/api/link_api.py` & `sysnet-persons-1.0.2/persons/api/link_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/api/manage_api.py` & `sysnet-persons-1.0.2/persons/api/manage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/api/public_api.py` & `sysnet-persons-1.0.2/persons/api/public_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/api_client.py` & `sysnet-persons-1.0.2/persons/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.1/python'
+        self.user_agent = 'Swagger-Codegen/1.0.2/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `sysnet-persons-1.0.1/persons/configuration.py` & `sysnet-persons-1.0.2/persons/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import copy
@@ -42,15 +42,15 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
         # Default Base url
-        self.host = "https://service.sysnet.cz/persons/1.0.1"
+        self.host = "https://service.sysnet.cz/persons/1.0.2"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
@@ -242,10 +242,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.1\n"\
-               "SDK Package Version: 1.0.1".\
+               "Version of the API: 1.0.2\n"\
+               "SDK Package Version: 1.0.2".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `sysnet-persons-1.0.1/persons/models/__init__.py` & `sysnet-persons-1.0.2/persons/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
@@ -22,22 +22,26 @@
 from persons.models.context_type_roles import ContextTypeRoles
 from persons.models.department_type import DepartmentType
 from persons.models.document_entry import DocumentEntry
 from persons.models.document_entry_list import DocumentEntryList
 from persons.models.document_metadata_type import DocumentMetadataType
 from persons.models.geo_point_jtsk_type import GeoPointJtskType
 from persons.models.geo_point_type import GeoPointType
+from persons.models.individual_list_type import IndividualListType
 from persons.models.individual_type import IndividualType
 from persons.models.issuing_type import IssuingType
 from persons.models.location_type import LocationType
 from persons.models.mail_address_type import MailAddressType
 from persons.models.member_type import MemberType
 from persons.models.person_link_type import PersonLinkType
 from persons.models.person_list_item import PersonListItem
+from persons.models.person_list_type import PersonListType
 from persons.models.person_type import PersonType
 from persons.models.phone_number_type import PhoneNumberType
 from persons.models.reference_registry import ReferenceRegistry
 from persons.models.role_category_type import RoleCategoryType
 from persons.models.role_list_item import RoleListItem
+from persons.models.role_list_type import RoleListType
 from persons.models.role_type import RoleType
 from persons.models.tag_item_type import TagItemType
+from persons.models.tag_list_type import TagListType
 from persons.models.tag_type import TagType
```

### Comparing `sysnet-persons-1.0.1/persons/models/code_value_type.py` & `sysnet-persons-1.0.2/persons/models/code_value_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/config_body.py` & `sysnet-persons-1.0.2/persons/models/config_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/contact_type.py` & `sysnet-persons-1.0.2/persons/models/contact_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/context_type.py` & `sysnet-persons-1.0.2/persons/models/context_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/context_type_persons.py` & `sysnet-persons-1.0.2/persons/models/context_type_persons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/context_type_roles.py` & `sysnet-persons-1.0.2/persons/models/context_type_roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/department_type.py` & `sysnet-persons-1.0.2/persons/models/department_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/document_entry.py` & `sysnet-persons-1.0.2/persons/models/document_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/document_entry_list.py` & `sysnet-persons-1.0.2/persons/models/document_entry_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/document_metadata_type.py` & `sysnet-persons-1.0.2/persons/models/document_metadata_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/geo_point_jtsk_type.py` & `sysnet-persons-1.0.2/persons/models/geo_point_jtsk_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/geo_point_type.py` & `sysnet-persons-1.0.2/persons/models/geo_point_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/individual_type.py` & `sysnet-persons-1.0.2/persons/models/individual_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/issuing_type.py` & `sysnet-persons-1.0.2/persons/models/issuing_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/location_type.py` & `sysnet-persons-1.0.2/persons/models/location_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/mail_address_type.py` & `sysnet-persons-1.0.2/persons/models/mail_address_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/member_type.py` & `sysnet-persons-1.0.2/persons/models/member_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/person_link_type.py` & `sysnet-persons-1.0.2/persons/models/person_link_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/person_list_item.py` & `sysnet-persons-1.0.2/persons/models/person_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/person_type.py` & `sysnet-persons-1.0.2/persons/models/person_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/phone_number_type.py` & `sysnet-persons-1.0.2/persons/models/phone_number_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/reference_registry.py` & `sysnet-persons-1.0.2/persons/models/reference_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/role_category_type.py` & `sysnet-persons-1.0.2/persons/models/role_category_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/role_list_item.py` & `sysnet-persons-1.0.2/persons/models/role_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/role_type.py` & `sysnet-persons-1.0.2/persons/models/role_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/tag_item_type.py` & `sysnet-persons-1.0.2/persons/models/tag_item_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/models/tag_type.py` & `sysnet-persons-1.0.2/persons/models/tag_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.1/persons/rest.py` & `sysnet-persons-1.0.2/persons/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `sysnet-persons-1.0.1/pyproject.toml` & `sysnet-persons-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-persons"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Radim Jaeger", email="rjaeger@sysnet.cz" },
 ]
 description = "SYSNET Persons Registry REST API client"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-persons-1.0.1/setup.py` & `sysnet-persons-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "persons"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `sysnet-persons-1.0.1/sysnet_persons.egg-info/PKG-INFO` & `sysnet-persons-1.0.2/sysnet_persons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-persons
-Version: 1.0.1
+Version: 1.0.2
 Summary: SYSNET Persons Registry REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,34 +212,34 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sysnet-persons
+# persons
 This is a API to Persons Registry
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.1
-- Package version: 1.0.1
+- API version: 1.0.2
+- Package version: 1.0.2
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 3.9+
+Python 2.7 and 3.4+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-persons
+pip install --upgrade sysnet-persons
 ```
 
 Then import the package:
 ```python
 import persons 
 ```
 
@@ -390,15 +390,15 @@
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_tag: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/persons/1.0.1*
+All URIs are relative to *https://service.sysnet.cz/persons/1.0.2*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**delete_tag**](docs/AdminsApi.md#delete_tag) | **DELETE** /tag/{name} | odstraní definici tagu  (cruD)
 *AdminsApi* | [**get_config**](docs/AdminsApi.md#get_config) | **GET** /config | získá konfiguraci konektoru
 *AdminsApi* | [**get_tag**](docs/AdminsApi.md#get_tag) | **GET** /tag/{name} | vrací definici tagu (cRud)
 *AdminsApi* | [**get_tag_list**](docs/AdminsApi.md#get_tag_list) | **GET** /tag | vrací seznam tagů v systému (autocomplete)
@@ -428,14 +428,18 @@
 *ManageApi* | [**import_individuals_replace**](docs/ManageApi.md#import_individuals_replace) | **POST** /individual/data | Nahradí všechny uživatele
 *ManageApi* | [**import_persons**](docs/ManageApi.md#import_persons) | **PUT** /person/data | Importuje subjekty
 *ManageApi* | [**import_persons_replace**](docs/ManageApi.md#import_persons_replace) | **POST** /person/data | Nahradí všechny subjekty
 *ManageApi* | [**import_roles**](docs/ManageApi.md#import_roles) | **PUT** /role/data | Importuje role
 *ManageApi* | [**import_roles_replace**](docs/ManageApi.md#import_roles_replace) | **POST** /role/data | Nahradí všechny role
 *ManageApi* | [**import_tags**](docs/ManageApi.md#import_tags) | **PUT** /tag/data | Importuje tagy
 *ManageApi* | [**import_tags_replace**](docs/ManageApi.md#import_tags_replace) | **POST** /tag/data | Nahradí všechny tagy
+*Manage2Api* | [**get_all_idividuals**](docs/Manage2Api.md#get_all_idividuals) | **GET** /all/individuals | Vrací všechny uživatele pro Admin Portal
+*Manage2Api* | [**get_all_persons**](docs/Manage2Api.md#get_all_persons) | **GET** /all/persons | Vrací všechny subjekty pro Admin Portal
+*Manage2Api* | [**get_all_roles**](docs/Manage2Api.md#get_all_roles) | **GET** /all/roles | Vrací všechny role pro Admin Portal
+*Manage2Api* | [**get_all_tags**](docs/Manage2Api.md#get_all_tags) | **GET** /all/tags | Vrací všechny tagy pro Admin Portal
 *PublicApi* | [**delete_individual**](docs/PublicApi.md#delete_individual) | **DELETE** /individual/{identifier} | odstraní registrační dokument jednotlivce s daným identifikátorem (cruD)
 *PublicApi* | [**delete_person**](docs/PublicApi.md#delete_person) | **DELETE** /person/{identifier} | odstraní registrační dokument subjektu s daným identifikátorem (cruD)
 *PublicApi* | [**delete_role**](docs/PublicApi.md#delete_role) | **DELETE** /role/{identifier} | odstraní roli s daným identifikátorem (cruD)
 *PublicApi* | [**get_context**](docs/PublicApi.md#get_context) | **GET** /context/{identifier} | vrací kontext jednotlivce
 *PublicApi* | [**get_individual**](docs/PublicApi.md#get_individual) | **GET** /individual/{identifier} | vrací registrační dokument jednotlivce s daným identifikátorem (cRud)
 *PublicApi* | [**get_individual_list**](docs/PublicApi.md#get_individual_list) | **GET** /individual | vrací seznam jednotlivců (autocomplete)
 *PublicApi* | [**get_person**](docs/PublicApi.md#get_person) | **GET** /person/{identifier} | vrací registrační dokument subjektu s daným identifikátorem (cRud)
@@ -460,28 +464,32 @@
  - [ContextTypeRoles](docs/ContextTypeRoles.md)
  - [DepartmentType](docs/DepartmentType.md)
  - [DocumentEntry](docs/DocumentEntry.md)
  - [DocumentEntryList](docs/DocumentEntryList.md)
  - [DocumentMetadataType](docs/DocumentMetadataType.md)
  - [GeoPointJtskType](docs/GeoPointJtskType.md)
  - [GeoPointType](docs/GeoPointType.md)
+ - [IndividualListType](docs/IndividualListType.md)
  - [IndividualType](docs/IndividualType.md)
  - [IssuingType](docs/IssuingType.md)
  - [LocationType](docs/LocationType.md)
  - [MailAddressType](docs/MailAddressType.md)
  - [MemberType](docs/MemberType.md)
  - [PersonLinkType](docs/PersonLinkType.md)
  - [PersonListItem](docs/PersonListItem.md)
+ - [PersonListType](docs/PersonListType.md)
  - [PersonType](docs/PersonType.md)
  - [PhoneNumberType](docs/PhoneNumberType.md)
  - [ReferenceRegistry](docs/ReferenceRegistry.md)
  - [RoleCategoryType](docs/RoleCategoryType.md)
  - [RoleListItem](docs/RoleListItem.md)
+ - [RoleListType](docs/RoleListType.md)
  - [RoleType](docs/RoleType.md)
  - [TagItemType](docs/TagItemType.md)
+ - [TagListType](docs/TagListType.md)
  - [TagType](docs/TagType.md)
 
 ## Documentation For Authorization
 
 
 ## apiKey
```

### Comparing `sysnet-persons-1.0.1/sysnet_persons.egg-info/SOURCES.txt` & `sysnet-persons-1.0.2/sysnet_persons.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 persons/api_client.py
 persons/configuration.py
 persons/rest.py
 persons/api/__init__.py
 persons/api/admins_api.py
 persons/api/developers_api.py
 persons/api/link_api.py
+persons/api/manage2_api.py
 persons/api/manage_api.py
 persons/api/public_api.py
 persons/models/__init__.py
 persons/models/code_value_type.py
 persons/models/config_body.py
 persons/models/contact_type.py
 persons/models/context_type.py
@@ -21,28 +22,32 @@
 persons/models/context_type_roles.py
 persons/models/department_type.py
 persons/models/document_entry.py
 persons/models/document_entry_list.py
 persons/models/document_metadata_type.py
 persons/models/geo_point_jtsk_type.py
 persons/models/geo_point_type.py
+persons/models/individual_list_type.py
 persons/models/individual_type.py
 persons/models/issuing_type.py
 persons/models/location_type.py
 persons/models/mail_address_type.py
 persons/models/member_type.py
 persons/models/person_link_type.py
 persons/models/person_list_item.py
+persons/models/person_list_type.py
 persons/models/person_type.py
 persons/models/phone_number_type.py
 persons/models/reference_registry.py
 persons/models/role_category_type.py
 persons/models/role_list_item.py
+persons/models/role_list_type.py
 persons/models/role_type.py
 persons/models/tag_item_type.py
+persons/models/tag_list_type.py
 persons/models/tag_type.py
 sysnet_persons.egg-info/PKG-INFO
 sysnet_persons.egg-info/SOURCES.txt
 sysnet_persons.egg-info/dependency_links.txt
 sysnet_persons.egg-info/requires.txt
 sysnet_persons.egg-info/top_level.txt
 test/__init__.py
@@ -56,25 +61,30 @@
 test/test_department_type.py
 test/test_developers_api.py
 test/test_document_entry.py
 test/test_document_entry_list.py
 test/test_document_metadata_type.py
 test/test_geo_point_jtsk_type.py
 test/test_geo_point_type.py
+test/test_individual_list_type.py
 test/test_individual_type.py
 test/test_issuing_type.py
 test/test_link_api.py
 test/test_location_type.py
 test/test_mail_address_type.py
+test/test_manage2_api.py
 test/test_manage_api.py
 test/test_member_type.py
 test/test_person_link_type.py
 test/test_person_list_item.py
+test/test_person_list_type.py
 test/test_person_type.py
 test/test_phone_number_type.py
 test/test_public_api.py
 test/test_reference_registry.py
 test/test_role_category_type.py
 test/test_role_list_item.py
+test/test_role_list_type.py
 test/test_role_type.py
 test/test_tag_item_type.py
+test/test_tag_list_type.py
 test/test_tag_type.py
```

### Comparing `sysnet-persons-1.0.1/test/test_admins_api.py` & `sysnet-persons-1.0.2/test/test_admins_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_code_value_type.py` & `sysnet-persons-1.0.2/test/test_code_value_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_config_body.py` & `sysnet-persons-1.0.2/test/test_config_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_contact_type.py` & `sysnet-persons-1.0.2/test/test_contact_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_context_type.py` & `sysnet-persons-1.0.2/test/test_context_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_context_type_persons.py` & `sysnet-persons-1.0.2/test/test_context_type_persons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_context_type_roles.py` & `sysnet-persons-1.0.2/test/test_context_type_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_department_type.py` & `sysnet-persons-1.0.2/test/test_department_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_developers_api.py` & `sysnet-persons-1.0.2/test/test_developers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_document_entry.py` & `sysnet-persons-1.0.2/test/test_document_entry_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import persons
-from persons.models.document_entry import DocumentEntry  # noqa: E501
+from persons.models.document_entry_list import DocumentEntryList  # noqa: E501
 from persons.rest import ApiException
 
 
-class TestDocumentEntry(unittest.TestCase):
-    """DocumentEntry unit test stubs"""
+class TestDocumentEntryList(unittest.TestCase):
+    """DocumentEntryList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDocumentEntry(self):
-        """Test DocumentEntry"""
+    def testDocumentEntryList(self):
+        """Test DocumentEntryList"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = persons.models.document_entry.DocumentEntry()  # noqa: E501
+        # model = persons.models.document_entry_list.DocumentEntryList()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-persons-1.0.1/test/test_document_entry_list.py` & `sysnet-persons-1.0.2/test/test_tag_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import persons
-from persons.models.document_entry_list import DocumentEntryList  # noqa: E501
+from persons.models.tag_type import TagType  # noqa: E501
 from persons.rest import ApiException
 
 
-class TestDocumentEntryList(unittest.TestCase):
-    """DocumentEntryList unit test stubs"""
+class TestTagType(unittest.TestCase):
+    """TagType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDocumentEntryList(self):
-        """Test DocumentEntryList"""
+    def testTagType(self):
+        """Test TagType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = persons.models.document_entry_list.DocumentEntryList()  # noqa: E501
+        # model = persons.models.tag_type.TagType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-persons-1.0.1/test/test_document_metadata_type.py` & `sysnet-persons-1.0.2/test/test_document_metadata_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_geo_point_jtsk_type.py` & `sysnet-persons-1.0.2/test/test_geo_point_jtsk_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_geo_point_type.py` & `sysnet-persons-1.0.2/test/test_geo_point_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_individual_type.py` & `sysnet-persons-1.0.2/test/test_member_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import persons
-from persons.models.individual_type import IndividualType  # noqa: E501
+from persons.models.member_type import MemberType  # noqa: E501
 from persons.rest import ApiException
 
 
-class TestIndividualType(unittest.TestCase):
-    """IndividualType unit test stubs"""
+class TestMemberType(unittest.TestCase):
+    """MemberType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIndividualType(self):
-        """Test IndividualType"""
+    def testMemberType(self):
+        """Test MemberType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = persons.models.individual_type.IndividualType()  # noqa: E501
+        # model = persons.models.member_type.MemberType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-persons-1.0.1/test/test_issuing_type.py` & `sysnet-persons-1.0.2/test/test_issuing_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_link_api.py` & `sysnet-persons-1.0.2/test/test_link_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_location_type.py` & `sysnet-persons-1.0.2/test/test_location_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_mail_address_type.py` & `sysnet-persons-1.0.2/test/test_mail_address_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_manage_api.py` & `sysnet-persons-1.0.2/test/test_manage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_member_type.py` & `sysnet-persons-1.0.2/test/test_role_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import persons
-from persons.models.member_type import MemberType  # noqa: E501
+from persons.models.role_type import RoleType  # noqa: E501
 from persons.rest import ApiException
 
 
-class TestMemberType(unittest.TestCase):
-    """MemberType unit test stubs"""
+class TestRoleType(unittest.TestCase):
+    """RoleType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMemberType(self):
-        """Test MemberType"""
+    def testRoleType(self):
+        """Test RoleType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = persons.models.member_type.MemberType()  # noqa: E501
+        # model = persons.models.role_type.RoleType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-persons-1.0.1/test/test_person_link_type.py` & `sysnet-persons-1.0.2/test/test_person_link_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_person_list_item.py` & `sysnet-persons-1.0.2/test/test_person_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_person_type.py` & `sysnet-persons-1.0.2/test/test_person_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_phone_number_type.py` & `sysnet-persons-1.0.2/test/test_phone_number_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_public_api.py` & `sysnet-persons-1.0.2/test/test_public_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_reference_registry.py` & `sysnet-persons-1.0.2/test/test_reference_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_role_category_type.py` & `sysnet-persons-1.0.2/test/test_role_category_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_role_list_item.py` & `sysnet-persons-1.0.2/test/test_role_list_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_role_type.py` & `sysnet-persons-1.0.2/test/test_individual_list_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import persons
-from persons.models.role_type import RoleType  # noqa: E501
+from persons.models.individual_list_type import IndividualListType  # noqa: E501
 from persons.rest import ApiException
 
 
-class TestRoleType(unittest.TestCase):
-    """RoleType unit test stubs"""
+class TestIndividualListType(unittest.TestCase):
+    """IndividualListType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRoleType(self):
-        """Test RoleType"""
+    def testIndividualListType(self):
+        """Test IndividualListType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = persons.models.role_type.RoleType()  # noqa: E501
+        # model = persons.models.individual_list_type.IndividualListType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-persons-1.0.1/test/test_tag_item_type.py` & `sysnet-persons-1.0.2/test/test_tag_item_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.1/test/test_tag_type.py` & `sysnet-persons-1.0.2/test/test_tag_list_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.1
+    OpenAPI spec version: 1.0.2
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import persons
-from persons.models.tag_type import TagType  # noqa: E501
+from persons.models.tag_list_type import TagListType  # noqa: E501
 from persons.rest import ApiException
 
 
-class TestTagType(unittest.TestCase):
-    """TagType unit test stubs"""
+class TestTagListType(unittest.TestCase):
+    """TagListType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTagType(self):
-        """Test TagType"""
+    def testTagListType(self):
+        """Test TagListType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = persons.models.tag_type.TagType()  # noqa: E501
+        # model = persons.models.tag_list_type.TagListType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

