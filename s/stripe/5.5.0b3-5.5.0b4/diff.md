# Comparing `tmp/stripe-5.5.0b3.tar.gz` & `tmp/stripe-5.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe-5.5.0b3.tar", last modified: Fri May 19 17:20:18 2023, max compression
+gzip compressed data, was "stripe-5.5.0b4.tar", last modified: Fri Jun  2 18:36:55 2023, max compression
```

## Comparing `stripe-5.5.0b3.tar` & `stripe-5.5.0b4.tar`

### file list

```diff
@@ -1,333 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 17:19:54.000000 stripe-5.5.0b3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-19 17:19:54.000000 stripe-5.5.0b3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    47658 2023-05-19 17:19:54.000000 stripe-5.5.0b3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-19 17:19:54.000000 stripe-5.5.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-19 17:19:54.000000 stripe-5.5.0b3/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 17:19:54.000000 stripe-5.5.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-19 17:20:18.415509 stripe-5.5.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-05-19 17:19:54.000000 stripe-5.5.0b3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 17:19:54.000000 stripe-5.5.0b3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.375510 stripe-5.5.0b3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-19 17:19:54.000000 stripe-5.5.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 17:20:18.415509 stripe-5.5.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-19 17:19:54.000000 stripe-5.5.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.379510 stripe-5.5.0b3/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.387509 stripe-5.5.0b3/stripe/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/verify_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/account_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/application_fee_refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/apps/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/bank_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/billing_portal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/billing_portal/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/capital/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/financing_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/financing_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/financing_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/cash_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/charge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/checkout/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/credit_note_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/customer_cash_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/error_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/file_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/financial_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/account_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/account_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/inferred_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/funding_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/gift_cards/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/gift_cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/gift_cards/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/gift_cards/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/identity/verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/identity/verification_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/invoice_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/card.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/card_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/card_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/login_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/quote_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/value_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/recipient_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reporting/report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reporting/report_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/shipping_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/sigma/scheduled_query_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/subscription_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/api_resources/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/test_helpers/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/api_resources/treasury/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/credit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/debit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/financial_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/inbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/outbound_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/outbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/received_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/received_debit.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/transaction_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/data/
--rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/data/ca-certificates.crt
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/request_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.379510 stripe-5.5.0b3/stripe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.403509 stripe-5.5.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_test_helpers_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_updateable_api_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/billing_portal/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/billing_portal/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/checkout/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/identity/test_verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/identity/test_verification_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/test_early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/test_value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/test_value_list_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/reporting/test_report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/reporting/test_report_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/sigma/test_scheduled_query_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/test_connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_application_fee_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_capability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_file_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_subscription_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/stripe_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    25396 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)   102848 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_generated_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.739111 stripe-5.5.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 18:36:33.000000 stripe-5.5.0b4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-02 18:36:33.000000 stripe-5.5.0b4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    47974 2023-06-02 18:36:33.000000 stripe-5.5.0b4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-02 18:36:33.000000 stripe-5.5.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-02 18:36:33.000000 stripe-5.5.0b4/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 18:36:33.000000 stripe-5.5.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-02 18:36:55.739111 stripe-5.5.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-02 18:36:33.000000 stripe-5.5.0b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 18:36:33.000000 stripe-5.5.0b4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.659109 stripe-5.5.0b4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 18:36:33.000000 stripe-5.5.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 18:36:55.739111 stripe-5.5.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-02 18:36:33.000000 stripe-5.5.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.663109 stripe-5.5.0b4/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.687110 stripe-5.5.0b4/stripe/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.687110 stripe-5.5.0b4/stripe/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/verify_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/account_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/application_fee_refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/apps/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/bank_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/billing_portal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/billing_portal/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/capital/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/financing_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/financing_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/financing_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/cash_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/charge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/checkout/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/credit_note_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/customer_cash_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/error_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/file_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.695110 stripe-5.5.0b4/stripe/api_resources/financial_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/account_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/account_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/inferred_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/funding_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.695110 stripe-5.5.0b4/stripe/api_resources/gift_cards/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/gift_cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/gift_cards/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/gift_cards/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.695110 stripe-5.5.0b4/stripe/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/identity/verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/identity/verification_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/invoice_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/card_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/card_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/login_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/quote_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/value_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/recipient_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reporting/report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reporting/report_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/shipping_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/sigma/scheduled_query_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/subscription_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.703110 stripe-5.5.0b4/stripe/api_resources/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.703110 stripe-5.5.0b4/stripe/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.703110 stripe-5.5.0b4/stripe/api_resources/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/test_helpers/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.707110 stripe-5.5.0b4/stripe/api_resources/treasury/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/credit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/debit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/financial_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/inbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/outbound_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/outbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/received_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/received_debit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/transaction_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.707110 stripe-5.5.0b4/stripe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/data/ca-certificates.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/request_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.667110 stripe-5.5.0b4/stripe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.711110 stripe-5.5.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.727110 stripe-5.5.0b4/tests/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_test_helpers_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_updateable_api_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/billing_portal/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/billing_portal/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/checkout/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/identity/test_verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/identity/test_verification_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/test_early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/test_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/test_value_list_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/reporting/test_report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/reporting/test_report_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/sigma/test_scheduled_query_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.739111 stripe-5.5.0b4/tests/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/test_connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_application_fee_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_file_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_subscription_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/stripe_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103511 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_generated_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tox.ini
```

### Comparing `stripe-5.5.0b3/CHANGELOG.md` & `stripe-5.5.0b4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 5.5.0b4 - 2023-06-02
+* [#973](https://github.com/stripe/stripe-python/pull/973) Update generated code for beta
+* [#969](https://github.com/stripe/stripe-python/pull/969) Update generated code for beta
+* [#971](https://github.com/stripe/stripe-python/pull/971) Handle developer message in preview error responses
+
 ## 5.5.0b3 - 2023-05-19
 * [#966](https://github.com/stripe/stripe-python/pull/966) Update generated code for beta
   * Add support for `subscribe` and `unsubscribe` methods on resource `FinancialConnections.Account`
 * [#965](https://github.com/stripe/stripe-python/pull/965) Add raw_request
 * [#964](https://github.com/stripe/stripe-python/pull/964) Update generated code for beta
 * [#961](https://github.com/stripe/stripe-python/pull/961) Update generated code for beta
```

### Comparing `stripe-5.5.0b3/LICENSE` & `stripe-5.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/LONG_DESCRIPTION.rst` & `stripe-5.5.0b4/LONG_DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/PKG-INFO` & `stripe-5.5.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b3
+Version: 5.5.0b4
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b3/README.md` & `stripe-5.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/examples/oauth.py` & `stripe-5.5.0b4/examples/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/examples/proxy.py` & `stripe-5.5.0b4/examples/proxy.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/examples/webhooks.py` & `stripe-5.5.0b4/examples/webhooks.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/setup.py` & `stripe-5.5.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/__init__.py` & `stripe-5.5.0b4/stripe/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_requestor.py` & `stripe-5.5.0b4/stripe/api_requestor.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,65 +173,89 @@
             err = self.specific_api_error(
                 rbody, rcode, resp, rheaders, error_data
             )
 
         raise err
 
     def specific_api_error(self, rbody, rcode, resp, rheaders, error_data):
+        message = error_data.get("message") or error_data.get(
+            "developer_message"
+        )
+
         util.log_info(
             "Stripe API error received",
             error_code=error_data.get("code"),
             error_type=error_data.get("type"),
-            error_message=error_data.get("message"),
+            error_message=message,
             error_param=error_data.get("param"),
         )
 
         # Rate limits were previously coded as 400's with code 'rate_limit'
         if rcode == 429 or (
             rcode == 400 and error_data.get("code") == "rate_limit"
         ):
             return error.RateLimitError(
-                error_data.get("message"), rbody, rcode, resp, rheaders
+                message,
+                rbody,
+                rcode,
+                resp,
+                rheaders,
             )
         elif rcode in [400, 404]:
             if error_data.get("type") == "idempotency_error":
                 return error.IdempotencyError(
-                    error_data.get("message"), rbody, rcode, resp, rheaders
+                    message,
+                    rbody,
+                    rcode,
+                    resp,
+                    rheaders,
                 )
             else:
                 return error.InvalidRequestError(
-                    error_data.get("message"),
+                    message,
                     error_data.get("param"),
                     error_data.get("code"),
                     rbody,
                     rcode,
                     resp,
                     rheaders,
                 )
         elif rcode == 401:
             return error.AuthenticationError(
-                error_data.get("message"), rbody, rcode, resp, rheaders
+                message,
+                rbody,
+                rcode,
+                resp,
+                rheaders,
             )
         elif rcode == 402:
             return error.CardError(
-                error_data.get("message"),
+                message,
                 error_data.get("param"),
                 error_data.get("code"),
                 rbody,
                 rcode,
                 resp,
                 rheaders,
             )
         elif rcode == 403:
             return error.PermissionError(
-                error_data.get("message"), rbody, rcode, resp, rheaders
+                message,
+                rbody,
+                rcode,
+                resp,
+                rheaders,
             )
         else:
             return error.APIError(
-                error_data.get("message"), rbody, rcode, resp, rheaders
+                message,
+                rbody,
+                rcode,
+                resp,
+                rheaders,
             )
 
     def specific_oauth_error(self, rbody, rcode, resp, rheaders, error_code):
         description = resp.get("error_description", error_code)
 
         util.log_info(
             "Stripe OAuth error received",
```

### Comparing `stripe-5.5.0b3/stripe/api_resources/__init__.py` & `stripe-5.5.0b4/stripe/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/__init__.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/api_resource.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/createable_api_resource.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/custom_method.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/deletable_api_resource.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/listable_api_resource.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/nested_resource_class_methods.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/searchable_api_resource.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/singleton_api_resource.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/test_helpers.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/test_helpers.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/abstract/updateable_api_resource.py` & `stripe-5.5.0b4/stripe/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/account.py` & `stripe-5.5.0b4/stripe/api_resources/account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/account_link.py` & `stripe-5.5.0b4/stripe/api_resources/account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/account_session.py` & `stripe-5.5.0b4/stripe/api_resources/account_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/apple_pay_domain.py` & `stripe-5.5.0b4/stripe/api_resources/apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/application_fee.py` & `stripe-5.5.0b4/stripe/api_resources/application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/application_fee_refund.py` & `stripe-5.5.0b4/stripe/api_resources/application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/apps/secret.py` & `stripe-5.5.0b4/stripe/api_resources/apps/secret.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/balance.py` & `stripe-5.5.0b4/stripe/api_resources/balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/balance_transaction.py` & `stripe-5.5.0b4/stripe/api_resources/balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/bank_account.py` & `stripe-5.5.0b4/stripe/api_resources/bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/billing_portal/configuration.py` & `stripe-5.5.0b4/stripe/api_resources/billing_portal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/billing_portal/session.py` & `stripe-5.5.0b4/stripe/api_resources/billing_portal/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/capability.py` & `stripe-5.5.0b4/stripe/api_resources/capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/capital/financing_offer.py` & `stripe-5.5.0b4/stripe/api_resources/capital/financing_offer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/capital/financing_summary.py` & `stripe-5.5.0b4/stripe/api_resources/capital/financing_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/card.py` & `stripe-5.5.0b4/stripe/api_resources/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/cash_balance.py` & `stripe-5.5.0b4/stripe/api_resources/cash_balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/charge.py` & `stripe-5.5.0b4/stripe/api_resources/charge.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 class Charge(
     CreateableAPIResource,
     ListableAPIResource,
     SearchableAPIResource,
     UpdateableAPIResource,
 ):
     """
-    To charge a credit or a debit card, you create a `Charge` object. You can
-    retrieve and refund individual charges as well as list all charges. Charges
-    are identified by a unique, random ID.
-
-    Related guide: [Accept a payment with the Charges API](https://stripe.com/docs/payments/accept-a-payment-charges)
+    The `Charge` object represents a single attempt to move money into your Stripe account.
+    PaymentIntent confirmation is the most common way to create Charges, but transferring
+    money to a different Stripe account through Connect also creates Charges.
+    Some legacy payment flows create Charges directly, which is not recommended for new integrations.
     """
 
     OBJECT_NAME = "charge"
 
     @classmethod
     def _cls_capture(
         cls,
```

### Comparing `stripe-5.5.0b3/stripe/api_resources/checkout/session.py` & `stripe-5.5.0b4/stripe/api_resources/checkout/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/country_spec.py` & `stripe-5.5.0b4/stripe/api_resources/country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/coupon.py` & `stripe-5.5.0b4/stripe/api_resources/coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/credit_note.py` & `stripe-5.5.0b4/stripe/api_resources/credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/customer.py` & `stripe-5.5.0b4/stripe/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/customer_balance_transaction.py` & `stripe-5.5.0b4/stripe/api_resources/customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/customer_cash_balance_transaction.py` & `stripe-5.5.0b4/stripe/api_resources/customer_cash_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/dispute.py` & `stripe-5.5.0b4/stripe/api_resources/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/ephemeral_key.py` & `stripe-5.5.0b4/stripe/api_resources/ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/error_object.py` & `stripe-5.5.0b4/stripe/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/event.py` & `stripe-5.5.0b4/stripe/api_resources/event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/exchange_rate.py` & `stripe-5.5.0b4/stripe/api_resources/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/file.py` & `stripe-5.5.0b4/stripe/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/file_link.py` & `stripe-5.5.0b4/stripe/api_resources/file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/financial_connections/__init__.py` & `stripe-5.5.0b4/stripe/api_resources/financial_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/financial_connections/account.py` & `stripe-5.5.0b4/stripe/api_resources/financial_connections/account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/funding_instructions.py` & `stripe-5.5.0b4/stripe/api_resources/funding_instructions.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/gift_cards/card.py` & `stripe-5.5.0b4/stripe/api_resources/gift_cards/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/gift_cards/transaction.py` & `stripe-5.5.0b4/stripe/api_resources/gift_cards/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/identity/verification_report.py` & `stripe-5.5.0b4/stripe/api_resources/identity/verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/identity/verification_session.py` & `stripe-5.5.0b4/stripe/api_resources/identity/verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/invoice.py` & `stripe-5.5.0b4/stripe/api_resources/invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/invoice_item.py` & `stripe-5.5.0b4/stripe/api_resources/invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/issuing/__init__.py` & `stripe-5.5.0b4/stripe/api_resources/issuing/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/issuing/authorization.py` & `stripe-5.5.0b4/stripe/api_resources/issuing/authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/issuing/card.py` & `stripe-5.5.0b4/stripe/api_resources/issuing/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/issuing/card_design.py` & `stripe-5.5.0b4/stripe/api_resources/issuing/card_design.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/issuing/cardholder.py` & `stripe-5.5.0b4/stripe/api_resources/issuing/cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/issuing/dispute.py` & `stripe-5.5.0b4/stripe/api_resources/issuing/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/issuing/transaction.py` & `stripe-5.5.0b4/stripe/api_resources/issuing/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/list_object.py` & `stripe-5.5.0b4/stripe/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/order.py` & `stripe-5.5.0b4/stripe/api_resources/order.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/payment_intent.py` & `stripe-5.5.0b4/stripe/api_resources/payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/payment_link.py` & `stripe-5.5.0b4/stripe/api_resources/payment_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/payment_method.py` & `stripe-5.5.0b4/stripe/api_resources/payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/payout.py` & `stripe-5.5.0b4/stripe/api_resources/payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/person.py` & `stripe-5.5.0b4/stripe/api_resources/person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/plan.py` & `stripe-5.5.0b4/stripe/api_resources/plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/price.py` & `stripe-5.5.0b4/stripe/api_resources/price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/product.py` & `stripe-5.5.0b4/stripe/api_resources/product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/promotion_code.py` & `stripe-5.5.0b4/stripe/api_resources/promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/quote.py` & `stripe-5.5.0b4/stripe/api_resources/quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/quote_phase.py` & `stripe-5.5.0b4/stripe/api_resources/quote_phase.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/radar/early_fraud_warning.py` & `stripe-5.5.0b4/stripe/api_resources/radar/early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/radar/value_list.py` & `stripe-5.5.0b4/stripe/api_resources/radar/value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/radar/value_list_item.py` & `stripe-5.5.0b4/stripe/api_resources/radar/value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/refund.py` & `stripe-5.5.0b4/stripe/api_resources/refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/reporting/report_run.py` & `stripe-5.5.0b4/stripe/api_resources/reporting/report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/reporting/report_type.py` & `stripe-5.5.0b4/stripe/api_resources/reporting/report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/reversal.py` & `stripe-5.5.0b4/stripe/api_resources/reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/review.py` & `stripe-5.5.0b4/stripe/api_resources/review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/search_result_object.py` & `stripe-5.5.0b4/stripe/api_resources/search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/setup_attempt.py` & `stripe-5.5.0b4/stripe/api_resources/setup_attempt.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/setup_intent.py` & `stripe-5.5.0b4/stripe/api_resources/setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/shipping_rate.py` & `stripe-5.5.0b4/stripe/api_resources/shipping_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/sigma/scheduled_query_run.py` & `stripe-5.5.0b4/stripe/api_resources/sigma/scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/source.py` & `stripe-5.5.0b4/stripe/api_resources/source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/source_transaction.py` & `stripe-5.5.0b4/stripe/api_resources/source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/subscription.py` & `stripe-5.5.0b4/stripe/api_resources/subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/subscription_item.py` & `stripe-5.5.0b4/stripe/api_resources/subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/subscription_schedule.py` & `stripe-5.5.0b4/stripe/api_resources/subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/tax/calculation.py` & `stripe-5.5.0b4/stripe/api_resources/tax/calculation.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/tax/registration.py` & `stripe-5.5.0b4/stripe/api_resources/tax/registration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/tax/settings.py` & `stripe-5.5.0b4/stripe/api_resources/tax/settings.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/tax/transaction.py` & `stripe-5.5.0b4/stripe/api_resources/tax/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/tax_id.py` & `stripe-5.5.0b4/stripe/api_resources/tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/tax_rate.py` & `stripe-5.5.0b4/stripe/api_resources/tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/terminal/configuration.py` & `stripe-5.5.0b4/stripe/api_resources/terminal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/terminal/location.py` & `stripe-5.5.0b4/stripe/api_resources/terminal/location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/terminal/reader.py` & `stripe-5.5.0b4/stripe/api_resources/terminal/reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/test_helpers/test_clock.py` & `stripe-5.5.0b4/stripe/api_resources/test_helpers/test_clock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/token.py` & `stripe-5.5.0b4/stripe/api_resources/token.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,12 +23,10 @@
     Stripe, so we cannot determine how it is handled or stored.
 
     Tokens cannot be stored or used more than once. To store card or bank account
     information for later use, you can create [Customer](https://stripe.com/docs/api#customers)
     objects or [Custom accounts](https://stripe.com/docs/api#external_accounts). Note that
     [Radar](https://stripe.com/docs/radar), our integrated solution for automatic fraud protection,
     performs best with integrations that use client-side tokenization.
-
-    Related guide: [Accept a payment with Charges and Tokens](https://stripe.com/docs/payments/accept-a-payment-charges#web-create-token)
     """
 
     OBJECT_NAME = "token"
```

### Comparing `stripe-5.5.0b3/stripe/api_resources/topup.py` & `stripe-5.5.0b4/stripe/api_resources/topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/transfer.py` & `stripe-5.5.0b4/stripe/api_resources/transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/__init__.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/credit_reversal.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/credit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/debit_reversal.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/debit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/financial_account.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/financial_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/inbound_transfer.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/outbound_payment.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/outbound_payment.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/outbound_transfer.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/received_credit.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/received_credit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/received_debit.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/received_debit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/treasury/transaction_entry.py` & `stripe-5.5.0b4/stripe/api_resources/treasury/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/usage_record.py` & `stripe-5.5.0b4/stripe/api_resources/usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/api_resources/webhook_endpoint.py` & `stripe-5.5.0b4/stripe/api_resources/webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/data/ca-certificates.crt` & `stripe-5.5.0b4/stripe/data/ca-certificates.crt`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/error.py` & `stripe-5.5.0b4/stripe/error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/http_client.py` & `stripe-5.5.0b4/stripe/http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/multipart_data_generator.py` & `stripe-5.5.0b4/stripe/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/oauth.py` & `stripe-5.5.0b4/stripe/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/oauth_error.py` & `stripe-5.5.0b4/stripe/oauth_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/object_classes.py` & `stripe-5.5.0b4/stripe/object_classes.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/preview.py` & `stripe-5.5.0b4/stripe/preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/raw_request.py` & `stripe-5.5.0b4/stripe/raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/six.py` & `stripe-5.5.0b4/stripe/six.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/stripe_object.py` & `stripe-5.5.0b4/stripe/stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/stripe_response.py` & `stripe-5.5.0b4/stripe/stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/util.py` & `stripe-5.5.0b4/stripe/util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe/webhook.py` & `stripe-5.5.0b4/stripe/webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/stripe.egg-info/PKG-INFO` & `stripe-5.5.0b4/stripe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b3
+Version: 5.5.0b4
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b3/stripe.egg-info/SOURCES.txt` & `stripe-5.5.0b4/stripe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_createable_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_custom_method.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_deletable_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_listable_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_nested_resource_class_methods.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_searchable_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_singleton_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_test_helpers_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_test_helpers_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/abstract/test_updateable_api_resource.py` & `stripe-5.5.0b4/tests/api_resources/abstract/test_updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/billing_portal/test_configuration.py` & `stripe-5.5.0b4/tests/api_resources/billing_portal/test_configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/checkout/test_session.py` & `stripe-5.5.0b4/tests/api_resources/checkout/test_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/identity/test_verification_report.py` & `stripe-5.5.0b4/tests/api_resources/identity/test_verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/identity/test_verification_session.py` & `stripe-5.5.0b4/tests/api_resources/identity/test_verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/issuing/test_authorization.py` & `stripe-5.5.0b4/tests/api_resources/issuing/test_authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/issuing/test_card.py` & `stripe-5.5.0b4/tests/api_resources/issuing/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/issuing/test_cardholder.py` & `stripe-5.5.0b4/tests/api_resources/issuing/test_cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/issuing/test_dispute.py` & `stripe-5.5.0b4/tests/api_resources/issuing/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/issuing/test_transaction.py` & `stripe-5.5.0b4/tests/api_resources/issuing/test_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/radar/test_early_fraud_warning.py` & `stripe-5.5.0b4/tests/api_resources/radar/test_early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/radar/test_value_list.py` & `stripe-5.5.0b4/tests/api_resources/radar/test_value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/radar/test_value_list_item.py` & `stripe-5.5.0b4/tests/api_resources/radar/test_value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/reporting/test_report_run.py` & `stripe-5.5.0b4/tests/api_resources/reporting/test_report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/reporting/test_report_type.py` & `stripe-5.5.0b4/tests/api_resources/reporting/test_report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/sigma/test_scheduled_query_run.py` & `stripe-5.5.0b4/tests/api_resources/sigma/test_scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/terminal/test_location.py` & `stripe-5.5.0b4/tests/api_resources/terminal/test_location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/terminal/test_reader.py` & `stripe-5.5.0b4/tests/api_resources/terminal/test_reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_account.py` & `stripe-5.5.0b4/tests/api_resources/test_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_account_link.py` & `stripe-5.5.0b4/tests/api_resources/test_account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_apple_pay_domain.py` & `stripe-5.5.0b4/tests/api_resources/test_apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_application_fee.py` & `stripe-5.5.0b4/tests/api_resources/test_application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_application_fee_refund.py` & `stripe-5.5.0b4/tests/api_resources/test_application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_balance_transaction.py` & `stripe-5.5.0b4/tests/api_resources/test_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_bank_account.py` & `stripe-5.5.0b4/tests/api_resources/test_bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_capability.py` & `stripe-5.5.0b4/tests/api_resources/test_capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_card.py` & `stripe-5.5.0b4/tests/api_resources/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_charge.py` & `stripe-5.5.0b4/tests/api_resources/test_charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_country_spec.py` & `stripe-5.5.0b4/tests/api_resources/test_country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_coupon.py` & `stripe-5.5.0b4/tests/api_resources/test_coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_credit_note.py` & `stripe-5.5.0b4/tests/api_resources/test_credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_customer.py` & `stripe-5.5.0b4/tests/api_resources/test_customer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_customer_balance_transaction.py` & `stripe-5.5.0b4/tests/api_resources/test_customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_dispute.py` & `stripe-5.5.0b4/tests/api_resources/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_ephemeral_key.py` & `stripe-5.5.0b4/tests/api_resources/test_ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_event.py` & `stripe-5.5.0b4/tests/api_resources/test_event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_exchange_rate.py` & `stripe-5.5.0b4/tests/api_resources/test_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_file.py` & `stripe-5.5.0b4/tests/api_resources/test_file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_file_link.py` & `stripe-5.5.0b4/tests/api_resources/test_file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_file_upload.py` & `stripe-5.5.0b4/tests/api_resources/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_invoice.py` & `stripe-5.5.0b4/tests/api_resources/test_invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_invoice_item.py` & `stripe-5.5.0b4/tests/api_resources/test_invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_list_object.py` & `stripe-5.5.0b4/tests/api_resources/test_list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_payment_intent.py` & `stripe-5.5.0b4/tests/api_resources/test_payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_payment_method.py` & `stripe-5.5.0b4/tests/api_resources/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_payout.py` & `stripe-5.5.0b4/tests/api_resources/test_payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_person.py` & `stripe-5.5.0b4/tests/api_resources/test_person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_plan.py` & `stripe-5.5.0b4/tests/api_resources/test_plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_price.py` & `stripe-5.5.0b4/tests/api_resources/test_price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_product.py` & `stripe-5.5.0b4/tests/api_resources/test_product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_promotion_code.py` & `stripe-5.5.0b4/tests/api_resources/test_promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_quote.py` & `stripe-5.5.0b4/tests/api_resources/test_quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_refund.py` & `stripe-5.5.0b4/tests/api_resources/test_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_reversal.py` & `stripe-5.5.0b4/tests/api_resources/test_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_review.py` & `stripe-5.5.0b4/tests/api_resources/test_review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_search_result_object.py` & `stripe-5.5.0b4/tests/api_resources/test_search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_setup_intent.py` & `stripe-5.5.0b4/tests/api_resources/test_setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_source.py` & `stripe-5.5.0b4/tests/api_resources/test_source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_source_transaction.py` & `stripe-5.5.0b4/tests/api_resources/test_source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_subscription.py` & `stripe-5.5.0b4/tests/api_resources/test_subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_subscription_item.py` & `stripe-5.5.0b4/tests/api_resources/test_subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_subscription_schedule.py` & `stripe-5.5.0b4/tests/api_resources/test_subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_tax_code.py` & `stripe-5.5.0b4/tests/api_resources/test_tax_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_tax_id.py` & `stripe-5.5.0b4/tests/api_resources/test_tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_tax_rate.py` & `stripe-5.5.0b4/tests/api_resources/test_tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_topup.py` & `stripe-5.5.0b4/tests/api_resources/test_topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_transfer.py` & `stripe-5.5.0b4/tests/api_resources/test_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_usage_record.py` & `stripe-5.5.0b4/tests/api_resources/test_usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_usage_record_summary.py` & `stripe-5.5.0b4/tests/api_resources/test_usage_record_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/api_resources/test_webhook_endpoint.py` & `stripe-5.5.0b4/tests/api_resources/test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/conftest.py` & `stripe-5.5.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/request_mock.py` & `stripe-5.5.0b4/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/stripe_mock.py` & `stripe-5.5.0b4/tests/stripe_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_api_requestor.py` & `stripe-5.5.0b4/tests/test_api_requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -730,16 +730,20 @@
             urllib3.response.HTTPResponse(
                 body=util.io.BytesIO(b'{"error": "invalid_grant"}'),
                 preload_content=False,
             ),
             400,
         )
 
-        with pytest.raises(stripe.oauth_error.InvalidGrantError):
-            requestor.request_stream("get", self.valid_path, {})
+    def test_developer_message_in_error(self, requestor, mock_response):
+        mock_response('{"error": {"developer_message": "Unacceptable"}}', 400)
+
+        with pytest.raises(stripe.error.InvalidRequestError) as excinfo:
+            requestor.request("get", self.valid_path, {})
+        assert excinfo.value.user_message == "Unacceptable"
 
     def test_raw_request_with_file_param(self, requestor, mock_response):
         test_file = tempfile.NamedTemporaryFile()
         test_file.write("\u263A".encode("utf-16"))
         test_file.seek(0)
         params = {"file": test_file, "purpose": "dispute_evidence"}
         supplied_headers = {"Content-Type": "multipart/form-data"}
```

### Comparing `stripe-5.5.0b3/tests/test_error.py` & `stripe-5.5.0b4/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_generated_examples.py` & `stripe-5.5.0b4/tests/test_generated_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -3231,7 +3231,27 @@
 
     def test_quote_list_line_items(self, request_mock):
         stripe.Quote.list_line_items("qt_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/quotes/qt_xxxxxxxxxxxxx/line_items",
         )
+
+    def test_tax_calculation_create(self, request_mock):
+        stripe.tax.Calculation.create(
+            currency="usd",
+            line_items=[{"amount": 1000, "reference": "L1"}],
+            customer_details={
+                "address": {
+                    "line1": "354 Oyster Point Blvd",
+                    "city": "South San Francisco",
+                    "state": "CA",
+                    "postal_code": "94080",
+                    "country": "US",
+                },
+                "address_source": "shipping",
+            },
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/tax/calculations",
+        )
```

### Comparing `stripe-5.5.0b3/tests/test_http_client.py` & `stripe-5.5.0b4/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_integration.py` & `stripe-5.5.0b4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_multipart_data_generator.py` & `stripe-5.5.0b4/tests/test_multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_oauth.py` & `stripe-5.5.0b4/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_preview.py` & `stripe-5.5.0b4/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_raw_request.py` & `stripe-5.5.0b4/tests/test_raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_stripe_object.py` & `stripe-5.5.0b4/tests/test_stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_stripe_response.py` & `stripe-5.5.0b4/tests/test_stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_util.py` & `stripe-5.5.0b4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tests/test_webhook.py` & `stripe-5.5.0b4/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b3/tox.ini` & `stripe-5.5.0b4/tox.ini`

 * *Files identical despite different names*

