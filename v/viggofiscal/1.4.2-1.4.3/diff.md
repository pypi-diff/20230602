# Comparing `tmp/viggofiscal-1.4.2.tar.gz` & `tmp/viggofiscal-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggofiscal-1.4.2.tar", last modified: Wed May 31 17:59:10 2023, max compression
+gzip compressed data, was "viggofiscal-1.4.3.tar", last modified: Fri Jun  2 18:46:03 2023, max compression
```

## Comparing `viggofiscal-1.4.2.tar` & `viggofiscal-1.4.3.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cfop/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cfop/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cfop/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstipi/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/natureza_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.455860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/origem/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/origem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/origem/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/portaria/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/portaria/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/portaria/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/regra_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/tipo_operacao/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/uficms/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/uficms/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.459860 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/unidade_medida/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-31 17:58:20.000000 viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:59:10.451860 viggofiscal-1.4.2/viggofiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 17:59:10.000000 viggofiscal-1.4.2/viggofiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-31 17:59:10.000000 viggofiscal-1.4.2/viggofiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:59:10.000000 viggofiscal-1.4.2/viggofiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 17:59:10.000000 viggofiscal-1.4.2/viggofiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 17:59:10.000000 viggofiscal-1.4.2/viggofiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-02 18:46:03.382021 viggofiscal-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.366021 viggofiscal-1.4.3/viggofiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.366021 viggofiscal-1.4.3/viggofiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.366021 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.370020 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_proprio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cfop/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cfop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cfop/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cfop/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstipi/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstipi/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.374021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/natureza_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/natureza_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/origem/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/origem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/origem/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/portaria/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/portaria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/portaria/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/portaria/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/regra_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/regra_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/tipo_operacao/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/tipo_operacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/uficms/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/uficms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/uficms/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.378021 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/unidade_medida/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/unidade_medida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-02 18:45:11.000000 viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:46:03.366021 viggofiscal-1.4.3/viggofiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 18:46:03.000000 viggofiscal-1.4.3/viggofiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-02 18:46:03.000000 viggofiscal-1.4.3/viggofiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:46:03.000000 viggofiscal-1.4.3/viggofiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 18:46:03.000000 viggofiscal-1.4.3/viggofiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 18:46:03.000000 viggofiscal-1.4.3/viggofiscal.egg-info/top_level.txt
```

### Comparing `viggofiscal-1.4.2/viggofiscal/__init__.py` & `viggofiscal-1.4.3/viggofiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_proprio.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/base_reduzida_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms00.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms10.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms101.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms20.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms201.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms202_203.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms30.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms51.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms70.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms90.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/icms900.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/icms/valor_icms_st.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/base_ipi.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_ad_valorem.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/ipi/ipi50_especifico.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/base_pis.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins01_02.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/pis/pis_cofins03.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/calculo_fiscal/utils.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/calculo_fiscal/utils.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/certificado_digital/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cfop/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cfop/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cfop/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cfop/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/codigo_seguranca_contribuinte/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstcofins/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/csticms/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/csticms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstipi/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstipi/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/cstpis/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/cstpis/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/domain_org/router.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/domain_org/router.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/forma_pagamento_sefaz/router.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/natureza_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/ncm_ibpt_erro/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/origem/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/origem/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/portaria/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/portaria/manager.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/portaria/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/portaria/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/regra_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/tipo_operacao/manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,48 @@
-from sqlalchemy import and_, or_
-from viggocore.common import exception, manager
 from viggocore.common.subsystem import operation
 from viggocore.common.subsystem.pagination import Pagination
+from viggocore.common import manager
 
-from viggofiscal.subsystem.parametrizacao.serial_fiscal.resource import \
-    SerieFiscal
-from viggofiscal.subsystem.parametrizacao.terminal.resource import Terminal
+from viggofiscal.subsystem.parametrizacao.tipo_operacao.resource \
+    import TipoOperacao
 
 
-class Update(operation.Update):
+class Create(operation.Create):
 
-    def do(self, session, **kwargs):
-        kwargs.pop('ambiente', None)
-        kwargs.pop('serie', None)
-        kwargs.pop('modelo', None)
-        return super().do(session=session, **kwargs)
-
-
-class GetNextUltimoDoc(operation.Operation):
-    def pre(self, session, id, **kwargs):
-        serie_fiscal = self.manager.get(id=id)
-        if not serie_fiscal:
-            raise exception.NotFound('ERROR! serie_fiscal not found')
-        self.serie_fiscal_id = serie_fiscal.id
-
-        return True
-
-    def do(self, session, **kwargs):
-        next_ultimo_doc = self.driver.get_next_ultimo_doc(
-            session, self.serie_fiscal_id)
+    def pre(self, session, **kwargs):
+        codigo = kwargs.get('codigo', None)
+        domain_id = kwargs.get('domain_org_id', None)
 
-        if next_ultimo_doc is None:
-            raise exception.ViggoCoreException(
-                'Não foi possível retornar o próximo ultimo_doc ' +
-                'da serie_fiscal')
+        if not codigo and domain_id:
+            kwargs['codigo'] = self.manager.api.domain_sequences().\
+                get_nextval(id=domain_id, name=TipoOperacao.CODIGO_SEQUENCE)
 
-        return next_ultimo_doc
+        return super().pre(session=session, **kwargs)
 
 
-class GetDisponiveis(operation.List):
+class List(operation.List):
 
     def do(self, session, **kwargs):
-        serie_fiscal_id = kwargs.pop('serie_fiscal_id', None)
+        query = session.query(TipoOperacao)
 
-        query = session.query(SerieFiscal). \
-            join(Terminal, Terminal.serie_fiscal_id == SerieFiscal.id,
-                 isouter=True). \
-            filter(and_(or_(Terminal.serie_fiscal_id == None,  # noqa: E711
-                            SerieFiscal.id == serie_fiscal_id),
-                        SerieFiscal.modelo == 'NFCE',
-                        SerieFiscal.status == 'ATIVO'))
-        query = self.manager.apply_filters(query, SerieFiscal, **kwargs)
-
-        dict_compare = {"terminal.": Terminal}
-        query = self.manager.apply_filters_includes(
-            query, dict_compare, **kwargs)
+        query = self.manager.apply_filters(query, TipoOperacao, **kwargs)
         query = query.distinct()
 
         total_rows = None
         if self.manager.with_pagination(**kwargs):
             total_rows = query.count()
 
-        pagination = Pagination.get_pagination(SerieFiscal, **kwargs)
+        pagination = Pagination.get_pagination(TipoOperacao, **kwargs)
         if pagination.order_by is not None:
-            pagination.order_by = 'serie_fiscal.serie'
+            pagination.adjust_order_by(TipoOperacao)
         query = self.driver.apply_pagination(query, pagination)
         result = query.all()
 
         return (result, total_rows)
 
 
 class Manager(manager.CommonManager):
 
     def __init__(self, driver):
         super(Manager, self).__init__(driver)
-        self.update = Update(self)
-        self.get_next_ultimo_doc = GetNextUltimoDoc(self)
-        self.get_disponiveis = GetDisponiveis(self)
+        self.create = Create(self)
+        self.list = List(self)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/serial_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/controller.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/controller.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/manager.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from sqlalchemy import and_
 from viggocore.common import manager
 from viggocore.common.subsystem import operation
 from viggocore.subsystem.user.resource import User
 from viggofiscal.subsystem.parametrizacao.terminal.resource import (
     Terminal, TerminalOperador)
+from viggocore.common.subsystem.pagination import Pagination
 
 
 class Create(operation.Create):
 
     def do(self, session, **kwargs):
         super().do(session=session, **kwargs)
 
@@ -39,21 +40,45 @@
         operadores_em_uso = []
         if len(operadores) > 0:
             operadores_em_uso = self.manager.get_operadores_em_uso(
                 session, terminal_id, operadores)
         return operadores_em_uso
 
 
+class List(operation.List):
+
+    def do(self, session, **kwargs):
+        query = session.query(Terminal)
+        query = self.manager.apply_filters(query, Terminal, **kwargs)
+
+        dict_compare = {}
+        query = self.manager.apply_filters_includes(
+            query, dict_compare, **kwargs)
+
+        total_rows = None
+        if self.manager.with_pagination(**kwargs):
+            total_rows = query.count()
+
+        pagination = Pagination.get_pagination(Terminal, **kwargs)
+        if pagination.order_by is not None:
+            pagination.adjust_order_by(Terminal)
+        query = self.driver.apply_pagination(query, pagination)
+        result = query.all()
+
+        return (result, total_rows)
+
+
 class Manager(manager.CommonManager):
 
     def __init__(self, driver):
         super(Manager, self).__init__(driver)
         self.create = Create(self)
         self.update = Update(self)
         self.analisar = Analisar(self)
+        self.list = List(self)
 
     def remover_users_de_outros_terminais(self, terminal, session):
         if len(terminal.operadores) > 0:
             user_ids = terminal.get_user_id_dos_operadores()
 
             query = """
                 DELETE FROM terminal_operador
```

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/terminal/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/terminal/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/tipo_operacao/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/uficms/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/uficms/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py` & `viggofiscal-1.4.3/viggofiscal/subsystem/parametrizacao/unidade_medida/resource.py`

 * *Files identical despite different names*

### Comparing `viggofiscal-1.4.2/viggofiscal.egg-info/SOURCES.txt` & `viggofiscal-1.4.3/viggofiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

