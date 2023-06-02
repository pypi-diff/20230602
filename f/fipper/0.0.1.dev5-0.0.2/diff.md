# Comparing `tmp/fipper-0.0.1.dev5.tar.gz` & `tmp/fipper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fipper-0.0.1.dev5.tar", last modified: Tue May 23 08:34:57 2023, max compression
+gzip compressed data, was "fipper-0.0.2.tar", last modified: Fri Jun  2 04:42:08 2023, max compression
```

## Comparing `fipper-0.0.1.dev5.tar` & `fipper-0.0.2.tar`

### file list

```diff
@@ -1,486 +1,486 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.982007 fipper-0.0.1.dev5/
--rw-rw-rw-   0        0        0    35184 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/LICENSE
--rw-rw-rw-   0        0        0      291 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/MANIFEST.in
--rw-rw-rw-   0        0        0      781 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/NOTICE
--rw-rw-rw-   0        0        0     2202 2023-05-23 08:34:57.981007 fipper-0.0.1.dev5/PKG-INFO
--rw-rw-rw-   0        0        0     1297 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.266683 fipper-0.0.1.dev5/compiler/
--rw-rw-rw-   0        0        0      835 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.272682 fipper-0.0.1.dev5/compiler/api/
--rw-rw-rw-   0        0        0      835 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/api/__init__.py
--rw-rw-rw-   0        0        0    23018 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/api/compiler.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.331646 fipper-0.0.1.dev5/compiler/api/source/
--rw-rw-rw-   0        0        0     2273 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/api/source/auth_key.tl
--rw-rw-rw-   0        0        0   159892 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/api/source/main_api.tl
--rw-rw-rw-   0        0        0     3501 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/api/source/sys_msgs.tl
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.353630 fipper-0.0.1.dev5/compiler/api/template/
--rw-rw-rw-   0        0        0      772 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/api/template/combinator.txt
--rw-rw-rw-   0        0        0      652 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/api/template/type.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.370619 fipper-0.0.1.dev5/compiler/errors/
--rw-rw-rw-   0        0        0      835 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/__init__.py
--rw-rw-rw-   0        0        0     5055 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/compiler.py
--rw-rw-rw-   0        0        0     1298 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/sort.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.453313 fipper-0.0.1.dev5/compiler/errors/source/
--rw-rw-rw-   0        0        0      475 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/303_SEE_OTHER.tsv
--rw-rw-rw-   0        0        0    22646 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-rw-rw-   0        0        0      687 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-rw-rw-   0        0        0     2027 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/403_FORBIDDEN.tsv
--rw-rw-rw-   0        0        0     1189 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-rw-rw-   0        0        0      475 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/420_FLOOD.tsv
--rw-rw-rw-   0        0        0     4263 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-rw-rw-   0        0        0      157 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.472732 fipper-0.0.1.dev5/compiler/errors/template/
--rw-rw-rw-   0        0        0      190 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/template/class.txt
--rw-rw-rw-   0        0        0      127 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/compiler/errors/template/sub_class.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.596513 fipper-0.0.1.dev5/fipper/
--rw-rw-rw-   0        0        0     1447 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/__init__.py
--rw-rw-rw-   0        0        0    43136 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/client.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.671974 fipper-0.0.1.dev5/fipper/connection/
--rw-rw-rw-   0        0        0      873 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/__init__.py
--rw-rw-rw-   0        0        0     2916 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/connection.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.683969 fipper-0.0.1.dev5/fipper/connection/transport/
--rw-rw-rw-   0        0        0      857 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.775908 fipper-0.0.1.dev5/fipper/connection/transport/tcp/
--rw-rw-rw-   0        0        0     1068 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/tcp/__init__.py
--rw-rw-rw-   0        0        0     4225 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp.py
--rw-rw-rw-   0        0        0     1825 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_abridged.py
--rw-rw-rw-   0        0        0     2908 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_abridged_o.py
--rw-rw-rw-   0        0        0     1970 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_full.py
--rw-rw-rw-   0        0        0     1556 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_intermediate.py
--rw-rw-rw-   0        0        0     2530 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_intermediate_o.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.879843 fipper-0.0.1.dev5/fipper/crypto/
--rw-rw-rw-   0        0        0      835 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/crypto/__init__.py
--rw-rw-rw-   0        0        0     4143 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/crypto/aes.py
--rw-rw-rw-   0        0        0     4890 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/crypto/mtproto.py
--rw-rw-rw-   0        0        0     2528 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/crypto/prime.py
--rw-rw-rw-   0        0        0    11002 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/crypto/rsa.py
--rw-rw-rw-   0        0        0    10453 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/dispatcher.py
--rw-rw-rw-   0        0        0   212040 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/emoji.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:53.080716 fipper-0.0.1.dev5/fipper/enums/
--rw-rw-rw-   0        0        0     1785 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/auto_name.py
--rw-rw-rw-   0        0        0     2375 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/chat_action.py
--rw-rw-rw-   0        0        0     4328 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/chat_event_action.py
--rw-rw-rw-   0        0        0     1306 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/chat_member_status.py
--rw-rw-rw-   0        0        0     1484 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/chat_members_filter.py
--rw-rw-rw-   0        0        0     1276 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/chat_type.py
--rw-rw-rw-   0        0        0     2544 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/message_entity_type.py
--rw-rw-rw-   0        0        0     1667 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/message_media_type.py
--rw-rw-rw-   0        0        0     1971 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/message_service_type.py
--rw-rw-rw-   0        0        0     2475 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/messages_filter.py
--rw-rw-rw-   0        0        0     1456 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/next_code_type.py
--rw-rw-rw-   0        0        0     1225 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/parse_mode.py
--rw-rw-rw-   0        0        0     1076 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/poll_type.py
--rw-rw-rw-   0        0        0     1567 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/sent_code_type.py
--rw-rw-rw-   0        0        0     1340 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/enums/user_status.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:53.107700 fipper-0.0.1.dev5/fipper/errors/
--rw-rw-rw-   0        0        0     2659 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/errors/__init__.py
--rw-rw-rw-   0        0        0     3410 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/errors/rpc_error.py
--rw-rw-rw-   0        0        0    15633 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/file_id.py
--rw-rw-rw-   0        0        0    25461 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/filters.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:53.306308 fipper-0.0.1.dev5/fipper/handlers/
--rw-rw-rw-   0        0        0     1560 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0     2052 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/chat_join_request_handler.py
--rw-rw-rw-   0        0        0     2087 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/chat_member_updated_handler.py
--rw-rw-rw-   0        0        0     2143 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/chosen_inline_result_handler.py
--rw-rw-rw-   0        0        0     2502 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/conversation_handler.py
--rw-rw-rw-   0        0        0     2588 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/deleted_messages_handler.py
--rw-rw-rw-   0        0        0     1739 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/disconnect_handler.py
--rw-rw-rw-   0        0        0     2020 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/edited_message_handler.py
--rw-rw-rw-   0        0        0     1585 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/handler.py
--rw-rw-rw-   0        0        0     2025 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0     2902 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/message_handler.py
--rw-rw-rw-   0        0        0     1956 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/poll_handler.py
--rw-rw-rw-   0        0        0     2987 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/raw_update_handler.py
--rw-rw-rw-   0        0        0     2028 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/handlers/user_status_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:53.317982 fipper-0.0.1.dev5/fipper/methods/
--rw-rw-rw-   0        0        0     1365 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:53.377873 fipper-0.0.1.dev5/fipper/methods/advanced/
--rw-rw-rw-   0        0        0     1017 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     3206 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/advanced/invoke.py
--rw-rw-rw-   0        0        0     4673 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/advanced/resolve_peer.py
--rw-rw-rw-   0        0        0     8382 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/advanced/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:53.581746 fipper-0.0.1.dev5/fipper/methods/auth/
--rw-rw-rw-   0        0        0     1724 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     1506 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/accept_terms_of_service.py
--rw-rw-rw-   0        0        0     1990 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/check_password.py
--rw-rw-rw-   0        0        0     1794 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/connect.py
--rw-rw-rw-   0        0        0     1540 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/disconnect.py
--rw-rw-rw-   0        0        0     1339 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/get_password_hint.py
--rw-rw-rw-   0        0        0     1735 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/initialize.py
--rw-rw-rw-   0        0        0     1671 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/log_out.py
--rw-rw-rw-   0        0        0     1878 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/recover_password.py
--rw-rw-rw-   0        0        0     2202 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/resend_code.py
--rw-rw-rw-   0        0        0     2851 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/send_code.py
--rw-rw-rw-   0        0        0     1510 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/send_recovery_code.py
--rw-rw-rw-   0        0        0     3149 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/sign_in.py
--rw-rw-rw-   0        0        0     2788 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/sign_in_bot.py
--rw-rw-rw-   0        0        0     2416 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/sign_up.py
--rw-rw-rw-   0        0        0     1905 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/auth/terminate.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:53.811197 fipper-0.0.1.dev5/fipper/methods/bots/
--rw-rw-rw-   0        0        0     2096 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/__init__.py
--rw-rw-rw-   0        0        0     3386 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/answer_callback_query.py
--rw-rw-rw-   0        0        0     5090 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/answer_inline_query.py
--rw-rw-rw-   0        0        0     2030 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/answer_web_app_query.py
--rw-rw-rw-   0        0        0     2412 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/delete_bot_commands.py
--rw-rw-rw-   0        0        0     2628 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/get_bot_commands.py
--rw-rw-rw-   0        0        0     2102 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/get_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2377 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/get_chat_menu_button.py
--rw-rw-rw-   0        0        0     2860 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/get_game_high_scores.py
--rw-rw-rw-   0        0        0     3445 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/get_inline_bot_results.py
--rw-rw-rw-   0        0        0     2918 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/request_callback_answer.py
--rw-rw-rw-   0        0        0     4044 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/send_game.py
--rw-rw-rw-   0        0        0     2873 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/send_inline_bot_result.py
--rw-rw-rw-   0        0        0     2767 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/set_bot_commands.py
--rw-rw-rw-   0        0        0     3255 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/set_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2092 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/set_chat_menu_button.py
--rw-rw-rw-   0        0        0     4036 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/bots/set_game_score.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:54.345410 fipper-0.0.1.dev5/fipper/methods/chats/
--rw-rw-rw-   0        0        0     3540 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/__init__.py
--rw-rw-rw-   0        0        0     3448 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/add_chat_members.py
--rw-rw-rw-   0        0        0     2281 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/archive_chats.py
--rw-rw-rw-   0        0        0     4721 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/ban_chat_member.py
--rw-rw-rw-   0        0        0     1863 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/create_channel.py
--rw-rw-rw-   0        0        0     2336 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/create_group.py
--rw-rw-rw-   0        0        0     2003 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/create_supergroup.py
--rw-rw-rw-   0        0        0     1631 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/delete_channel.py
--rw-rw-rw-   0        0        0     2371 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/delete_chat_photo.py
--rw-rw-rw-   0        0        0     1649 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/delete_supergroup.py
--rw-rw-rw-   0        0        0     2018 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/delete_user_history.py
--rw-rw-rw-   0        0        0     3355 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_chat.py
--rw-rw-rw-   0        0        0     4129 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_chat_event_log.py
--rw-rw-rw-   0        0        0     3418 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_chat_member.py
--rw-rw-rw-   0        0        0     5420 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_chat_members.py
--rw-rw-rw-   0        0        0     2327 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_chat_members_count.py
--rw-rw-rw-   0        0        0     1768 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_chat_online_count.py
--rw-rw-rw-   0        0        0     3456 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_dialogs.py
--rw-rw-rw-   0        0        0     2153 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_dialogs_count.py
--rw-rw-rw-   0        0        0     2467 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_nearby_chats.py
--rw-rw-rw-   0        0        0     2191 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/get_send_as_chats.py
--rw-rw-rw-   0        0        0     2758 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/join_chat.py
--rw-rw-rw-   0        0        0     2676 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/leave_chat.py
--rw-rw-rw-   0        0        0     1569 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/mark_chat_unread.py
--rw-rw-rw-   0        0        0     3230 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/pin_chat_message.py
--rw-rw-rw-   0        0        0     3954 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/promote_chat_member.py
--rw-rw-rw-   0        0        0     4397 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/restrict_chat_member.py
--rw-rw-rw-   0        0        0     3215 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_administrator_title.py
--rw-rw-rw-   0        0        0     2307 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_chat_description.py
--rw-rw-rw-   0        0        0     3488 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_chat_permissions.py
--rw-rw-rw-   0        0        0     4708 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_chat_photo.py
--rw-rw-rw-   0        0        0     1774 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_chat_protected_content.py
--rw-rw-rw-   0        0        0     2644 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_chat_title.py
--rw-rw-rw-   0        0        0     2356 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_chat_username.py
--rw-rw-rw-   0        0        0     2031 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_send_as_chat.py
--rw-rw-rw-   0        0        0     2140 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/set_slow_mode.py
--rw-rw-rw-   0        0        0     2295 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/unarchive_chats.py
--rw-rw-rw-   0        0        0     2363 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/unban_chat_member.py
--rw-rw-rw-   0        0        0     1989 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/unpin_all_chat_messages.py
--rw-rw-rw-   0        0        0     2194 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/chats/unpin_chat_message.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:54.421825 fipper-0.0.1.dev5/fipper/methods/contacts/
--rw-rw-rw-   0        0        0     1187 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/contacts/__init__.py
--rw-rw-rw-   0        0        0     2634 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/contacts/add_contact.py
--rw-rw-rw-   0        0        0     2504 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/contacts/delete_contacts.py
--rw-rw-rw-   0        0        0     1642 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/contacts/get_contacts.py
--rw-rw-rw-   0        0        0     1457 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/contacts/get_contacts_count.py
--rw-rw-rw-   0        0        0     1980 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/contacts/import_contacts.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:54.598318 fipper-0.0.1.dev5/fipper/methods/decorators/
--rw-rw-rw-   0        0        0     1671 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0     2213 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_chat_join_request.py
--rw-rw-rw-   0        0        0     2234 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_chat_member_updated.py
--rw-rw-rw-   0        0        0     2262 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_chosen_inline_result.py
--rw-rw-rw-   0        0        0     2228 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_deleted_messages.py
--rw-rw-rw-   0        0        0     1584 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_disconnect.py
--rw-rw-rw-   0        0        0     2217 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_edited_message.py
--rw-rw-rw-   0        0        0     2212 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0     2183 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_message.py
--rw-rw-rw-   0        0        0     2165 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_poll.py
--rw-rw-rw-   0        0        0     1861 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_raw_update.py
--rw-rw-rw-   0        0        0     2197 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/decorators/on_user_status.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:54.835113 fipper-0.0.1.dev5/fipper/methods/invite_links/
--rw-rw-rw-   0        0        0     2493 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/approve_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1975 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/approve_chat_join_request.py
--rw-rw-rw-   0        0        0     3444 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/create_chat_invite_link.py
--rw-rw-rw-   0        0        0     1944 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/decline_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1976 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/decline_chat_join_request.py
--rw-rw-rw-   0        0        0     2079 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/delete_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     1797 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/delete_chat_invite_link.py
--rw-rw-rw-   0        0        0     3615 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/edit_chat_invite_link.py
--rw-rw-rw-   0        0        0     2637 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/export_chat_invite_link.py
--rw-rw-rw-   0        0        0     3654 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     2391 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-rw-rw-   0        0        0     2045 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-rw-rw-   0        0        0     1971 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_invite_link.py
--rw-rw-rw-   0        0        0     3003 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_invite_link_joiners.py
--rw-rw-rw-   0        0        0     1979 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-rw-rw-   0        0        0     3023 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_join_requests.py
--rw-rw-rw-   0        0        0     2387 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/invite_links/revoke_chat_invite_link.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:55.561740 fipper-0.0.1.dev5/fipper/methods/messages/
--rw-rw-rw-   0        0        0     4194 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/__init__.py
--rw-rw-rw-   0        0        0     6095 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/copy_media_group.py
--rw-rw-rw-   0        0        0     5280 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/copy_message.py
--rw-rw-rw-   0        0        0     3226 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/delete_messages.py
--rw-rw-rw-   0        0        0     7705 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/download_media.py
--rw-rw-rw-   0        0        0     2326 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_caption.py
--rw-rw-rw-   0        0        0     9990 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_media.py
--rw-rw-rw-   0        0        0     2519 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_reply_markup.py
--rw-rw-rw-   0        0        0     3189 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_text.py
--rw-rw-rw-   0        0        0     3040 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_message_caption.py
--rw-rw-rw-   0        0        0    12725 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_message_media.py
--rw-rw-rw-   0        0        0     3039 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_message_reply_markup.py
--rw-rw-rw-   0        0        0     3986 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/edit_message_text.py
--rw-rw-rw-   0        0        0     4662 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/forward_messages.py
--rw-rw-rw-   0        0        0     4152 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_chat_history.py
--rw-rw-rw-   0        0        0     2455 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_chat_history_count.py
--rw-rw-rw-   0        0        0     2023 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_custom_emoji_stickers.py
--rw-rw-rw-   0        0        0     2286 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_discussion_message.py
--rw-rw-rw-   0        0        0     2888 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_discussion_replies.py
--rw-rw-rw-   0        0        0     2006 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_discussion_replies_count.py
--rw-rw-rw-   0        0        0     3011 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_media_group.py
--rw-rw-rw-   0        0        0     4846 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/get_messages.py
--rw-rw-rw-   0        0        0     2227 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/inline_session.py
--rw-rw-rw-   0        0        0     2594 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/read_chat_history.py
--rw-rw-rw-   0        0        0     2175 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/retract_vote.py
--rw-rw-rw-   0        0        0     4259 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/search_global.py
--rw-rw-rw-   0        0        0     2208 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/search_global_count.py
--rw-rw-rw-   0        0        0     5486 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/search_messages.py
--rw-rw-rw-   0        0        0     3277 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/search_messages_count.py
--rw-rw-rw-   0        0        0    12513 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_animation.py
--rw-rw-rw-   0        0        0    11326 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_audio.py
--rw-rw-rw-   0        0        0     5579 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_cached_media.py
--rw-rw-rw-   0        0        0     2887 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_chat_action.py
--rw-rw-rw-   0        0        0     4970 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_contact.py
--rw-rw-rw-   0        0        0     4939 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_dice.py
--rw-rw-rw-   0        0        0    10656 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_document.py
--rw-rw-rw-   0        0        0     4671 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_location.py
--rw-rw-rw-   0        0        0    19643 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_media_group.py
--rw-rw-rw-   0        0        0     7418 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     9303 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_photo.py
--rw-rw-rw-   0        0        0     8222 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_poll.py
--rw-rw-rw-   0        0        0     2428 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_reaction.py
--rw-rw-rw-   0        0        0     8489 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_sticker.py
--rw-rw-rw-   0        0        0     5516 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_venue.py
--rw-rw-rw-   0        0        0    11877 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_video.py
--rw-rw-rw-   0        0        0     9487 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_video_note.py
--rw-rw-rw-   0        0        0     9600 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/send_voice.py
--rw-rw-rw-   0        0        0     2884 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/stop_poll.py
--rw-rw-rw-   0        0        0     4033 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/stream_media.py
--rw-rw-rw-   0        0        0     2563 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/vote_poll.py
--rw-rw-rw-   0        0        0     2895 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/wait_for_callback_query.py
--rw-rw-rw-   0        0        0     2816 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/messages/wait_for_message.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:55.614707 fipper-0.0.1.dev5/fipper/methods/password/
--rw-rw-rw-   0        0        0     1117 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/password/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/password/change_cloud_password.py
--rw-rw-rw-   0        0        0     3086 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/password/enable_cloud_password.py
--rw-rw-rw-   0        0        0     2199 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/password/remove_cloud_password.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:55.799104 fipper-0.0.1.dev5/fipper/methods/users/
--rw-rw-rw-   0        0        0     1708 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/__init__.py
--rw-rw-rw-   0        0        0     1819 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/block_user.py
--rw-rw-rw-   0        0        0     2288 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/delete_profile_photos.py
--rw-rw-rw-   0        0        0     4548 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/get_chat_photos.py
--rw-rw-rw-   0        0        0     2577 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/get_chat_photos_count.py
--rw-rw-rw-   0        0        0     2416 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/get_common_chats.py
--rw-rw-rw-   0        0        0     1701 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/get_default_emoji_statuses.py
--rw-rw-rw-   0        0        0     1604 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/get_me.py
--rw-rw-rw-   0        0        0     2621 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/get_users.py
--rw-rw-rw-   0        0        0     1930 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/set_emoji_status.py
--rw-rw-rw-   0        0        0     2787 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/set_profile_photo.py
--rw-rw-rw-   0        0        0     1925 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/set_username.py
--rw-rw-rw-   0        0        0     1829 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/unblock_user.py
--rw-rw-rw-   0        0        0     2442 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/users/update_profile.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:55.963004 fipper-0.0.1.dev5/fipper/methods/utilities/
--rw-rw-rw-   0        0        0     1292 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/add_handler.py
--rw-rw-rw-   0        0        0     2300 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/compose.py
--rw-rw-rw-   0        0        0     1593 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/export_session_string.py
--rw-rw-rw-   0        0        0     2833 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/idle.py
--rw-rw-rw-   0        0        0     2259 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/remove_handler.py
--rw-rw-rw-   0        0        0     2354 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/restart.py
--rw-rw-rw-   0        0        0     2925 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/run.py
--rw-rw-rw-   0        0        0     2432 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/start.py
--rw-rw-rw-   0        0        0     2178 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/stop.py
--rw-rw-rw-   0        0        0     1749 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/methods/utilities/stop_transmission.py
--rw-rw-rw-   0        0        0    63796 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/mime_types.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.025963 fipper-0.0.1.dev5/fipper/parser/
--rw-rw-rw-   0        0        0      865 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/parser/__init__.py
--rw-rw-rw-   0        0        0     7587 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/parser/html.py
--rw-rw-rw-   0        0        0     5937 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/parser/markdown.py
--rw-rw-rw-   0        0        0     2132 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/parser/parser.py
--rw-rw-rw-   0        0        0     1586 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/parser/utils.py
--rw-rw-rw-   0        0        0        0 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.038955 fipper-0.0.1.dev5/fipper/raw/
--rw-rw-rw-   0        0        0     1066 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.177737 fipper-0.0.1.dev5/fipper/raw/core/
--rw-rw-rw-   0        0        0     1343 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/__init__.py
--rw-rw-rw-   0        0        0     1745 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/future_salt.py
--rw-rw-rw-   0        0        0     1954 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/future_salts.py
--rw-rw-rw-   0        0        0     1876 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/gzip_packed.py
--rw-rw-rw-   0        0        0     1072 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/list.py
--rw-rw-rw-   0        0        0     1907 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/message.py
--rw-rw-rw-   0        0        0     1667 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/msg_container.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.267681 fipper-0.0.1.dev5/fipper/raw/core/primitives/
--rw-rw-rw-   0        0        0     1036 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/primitives/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/primitives/bool.py
--rw-rw-rw-   0        0        0     1814 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/primitives/bytes.py
--rw-rw-rw-   0        0        0     1225 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/primitives/double.py
--rw-rw-rw-   0        0        0     1403 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/primitives/int.py
--rw-rw-rw-   0        0        0     1225 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/primitives/string.py
--rw-rw-rw-   0        0        0     2081 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/primitives/vector.py
--rw-rw-rw-   0        0        0     2575 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/raw/core/tl_object.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.310653 fipper-0.0.1.dev5/fipper/session/
--rw-rw-rw-   0        0        0      891 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/__init__.py
--rw-rw-rw-   0        0        0    10760 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.373615 fipper-0.0.1.dev5/fipper/session/internals/
--rw-rw-rw-   0        0        0      938 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/internals/__init__.py
--rw-rw-rw-   0        0        0     2446 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/internals/data_center.py
--rw-rw-rw-   0        0        0     1406 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/internals/msg_factory.py
--rw-rw-rw-   0        0        0     1632 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/internals/msg_id.py
--rw-rw-rw-   0        0        0     1291 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/internals/seq_no.py
--rw-rw-rw-   0        0        0    12801 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/session/session.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.444588 fipper-0.0.1.dev5/fipper/storage/
--rw-rw-rw-   0        0        0      949 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/storage/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/storage/file_storage.py
--rw-rw-rw-   0        0        0     2823 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/storage/memory_storage.py
--rw-rw-rw-   0        0        0     6638 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/storage/sqlite_storage.py
--rw-rw-rw-   0        0        0     2872 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/storage/storage.py
--rw-rw-rw-   0        0        0     3846 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/sync.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.495596 fipper-0.0.1.dev5/fipper/types/
--rw-rw-rw-   0        0        0     1137 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.534523 fipper-0.0.1.dev5/fipper/types/authorization/
--rw-rw-rw-   0        0        0      960 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/authorization/__init__.py
--rw-rw-rw-   0        0        0     2336 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/authorization/sent_code.py
--rw-rw-rw-   0        0        0     1978 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/authorization/terms_of_service.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:56.874985 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/
--rw-rw-rw-   0        0        0     2901 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/__init__.py
--rw-rw-rw-   0        0        0     1789 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command.py
--rw-rw-rw-   0        0        0     2841 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope.py
--rw-rw-rw-   0        0        0     1319 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-rw-rw-   0        0        0     1284 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-rw-rw-   0        0        0     1275 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-rw-rw-   0        0        0     1599 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-rw-rw-   0        0        0     1676 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-rw-rw-   0        0        0     1859 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-rw-rw-   0        0        0     1335 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_default.py
--rw-rw-rw-   0        0        0     1058 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/callback_game.py
--rw-rw-rw-   0        0        0    13062 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/callback_query.py
--rw-rw-rw-   0        0        0     2443 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/force_reply.py
--rw-rw-rw-   0        0        0     2276 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/game_high_score.py
--rw-rw-rw-   0        0        0     8312 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/inline_keyboard_button.py
--rw-rw-rw-   0        0        0     2526 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-rw-rw-   0        0        0     3605 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/keyboard_button.py
--rw-rw-rw-   0        0        0     3800 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/login_url.py
--rw-rw-rw-   0        0        0     1633 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button.py
--rw-rw-rw-   0        0        0     1235 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button_commands.py
--rw-rw-rw-   0        0        0     1238 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button_default.py
--rw-rw-rw-   0        0        0     1850 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button_web_app.py
--rw-rw-rw-   0        0        0     4221 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-rw-rw-   0        0        0     2391 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-rw-rw-   0        0        0     1604 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/sent_web_app_message.py
--rw-rw-rw-   0        0        0     1350 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/web_app_info.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.153350 fipper-0.0.1.dev5/fipper/types/inline_mode/
--rw-rw-rw-   0        0        0     2802 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/chosen_inline_result.py
--rw-rw-rw-   0        0        0     7459 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query.py
--rw-rw-rw-   0        0        0     2434 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result.py
--rw-rw-rw-   0        0        0     5917 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_animation.py
--rw-rw-rw-   0        0        0     3391 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_article.py
--rw-rw-rw-   0        0        0     4611 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_audio.py
--rw-rw-rw-   0        0        0     4339 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_animation.py
--rw-rw-rw-   0        0        0     4116 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_audio.py
--rw-rw-rw-   0        0        0     4487 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_document.py
--rw-rw-rw-   0        0        0     4409 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_photo.py
--rw-rw-rw-   0        0        0     3099 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_sticker.py
--rw-rw-rw-   0        0        0     4494 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_video.py
--rw-rw-rw-   0        0        0     4296 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_voice.py
--rw-rw-rw-   0        0        0     4236 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_contact.py
--rw-rw-rw-   0        0        0     5371 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_document.py
--rw-rw-rw-   0        0        0     4731 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_location.py
--rw-rw-rw-   0        0        0     5394 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     4875 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_venue.py
--rw-rw-rw-   0        0        0     5611 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_video.py
--rw-rw-rw-   0        0        0     4460 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_voice.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.255792 fipper-0.0.1.dev5/fipper/types/input_media/
--rw-rw-rw-   0        0        0     1344 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/__init__.py
--rw-rw-rw-   0        0        0     1677 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/input_media.py
--rw-rw-rw-   0        0        0     3305 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/input_media_animation.py
--rw-rw-rw-   0        0        0     3358 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/input_media_audio.py
--rw-rw-rw-   0        0        0     2832 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/input_media_document.py
--rw-rw-rw-   0        0        0     2536 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/input_media_photo.py
--rw-rw-rw-   0        0        0     3500 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/input_media_video.py
--rw-rw-rw-   0        0        0     1782 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_media/input_phone_contact.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.293771 fipper-0.0.1.dev5/fipper/types/input_message_content/
--rw-rw-rw-   0        0        0     1030 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_message_content/__init__.py
--rw-rw-rw-   0        0        0     1441 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_message_content/input_message_content.py
--rw-rw-rw-   0        0        0     2696 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/input_message_content/input_text_message_content.py
--rw-rw-rw-   0        0        0     1121 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/list.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.615303 fipper-0.0.1.dev5/fipper/types/messages_and_media/
--rw-rw-rw-   0        0        0     1883 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/__init__.py
--rw-rw-rw-   0        0        0     4153 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/animation.py
--rw-rw-rw-   0        0        0     4178 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/audio.py
--rw-rw-rw-   0        0        0     2270 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/contact.py
--rw-rw-rw-   0        0        0     1628 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/dice.py
--rw-rw-rw-   0        0        0     3495 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/document.py
--rw-rw-rw-   0        0        0     3131 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/game.py
--rw-rw-rw-   0        0        0     1709 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/location.py
--rw-rw-rw-   0        0        0   150315 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/message.py
--rw-rw-rw-   0        0        0     4456 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/message_entity.py
--rw-rw-rw-   0        0        0     1846 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/message_reactions.py
--rw-rw-rw-   0        0        0     4427 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/photo.py
--rw-rw-rw-   0        0        0     7226 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/poll.py
--rw-rw-rw-   0        0        0     1578 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/poll_option.py
--rw-rw-rw-   0        0        0     2693 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/reaction.py
--rw-rw-rw-   0        0        0     7101 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/sticker.py
--rw-rw-rw-   0        0        0     1472 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/stripped_thumbnail.py
--rw-rw-rw-   0        0        0     3858 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/thumbnail.py
--rw-rw-rw-   0        0        0     2355 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/venue.py
--rw-rw-rw-   0        0        0     4511 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/video.py
--rw-rw-rw-   0        0        0     3697 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/video_note.py
--rw-rw-rw-   0        0        0     3292 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/voice.py
--rw-rw-rw-   0        0        0     1614 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/web_app_data.py
--rw-rw-rw-   0        0        0     6520 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/messages_and_media/web_page.py
--rw-rw-rw-   0        0        0     3973 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/object.py
--rw-rw-rw-   0        0        0     1023 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/update.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.932404 fipper-0.0.1.dev5/fipper/types/user_and_chats/
--rw-rw-rw-   0        0        0     2364 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/__init__.py
--rw-rw-rw-   0        0        0    33702 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat.py
--rw-rw-rw-   0        0        0     2289 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_admin_with_invite_links.py
--rw-rw-rw-   0        0        0    20240 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_event.py
--rw-rw-rw-   0        0        0     5687 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_event_filter.py
--rw-rw-rw-   0        0        0     4699 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_invite_link.py
--rw-rw-rw-   0        0        0     4364 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_join_request.py
--rw-rw-rw-   0        0        0     2634 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_joiner.py
--rw-rw-rw-   0        0        0     9647 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_member.py
--rw-rw-rw-   0        0        0     3756 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_member_updated.py
--rw-rw-rw-   0        0        0     4478 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_permissions.py
--rw-rw-rw-   0        0        0     4066 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_photo.py
--rw-rw-rw-   0        0        0     2659 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_preview.py
--rw-rw-rw-   0        0        0     5061 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_privileges.py
--rw-rw-rw-   0        0        0     2417 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_reactions.py
--rw-rw-rw-   0        0        0     2749 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/dialog.py
--rw-rw-rw-   0        0        0     2491 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/emoji_status.py
--rw-rw-rw-   0        0        0     2006 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/invite_link_importer.py
--rw-rw-rw-   0        0        0     1711 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/restriction.py
--rw-rw-rw-   0        0        0    13477 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/user.py
--rw-rw-rw-   0        0        0     1385 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_ended.py
--rw-rw-rw-   0        0        0     1656 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_members_invited.py
--rw-rw-rw-   0        0        0     1572 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_scheduled.py
--rw-rw-rw-   0        0        0     1072 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_started.py
--rw-rw-rw-   0        0        0    10933 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/fipper/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:52.647985 fipper-0.0.1.dev5/fipper.egg-info/
--rw-rw-rw-   0        0        0     2202 2023-05-23 08:34:51.000000 fipper-0.0.1.dev5/fipper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17932 2023-05-23 08:34:51.000000 fipper-0.0.1.dev5/fipper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:34:51.000000 fipper-0.0.1.dev5/fipper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 08:34:51.000000 fipper-0.0.1.dev5/fipper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       54 2023-05-23 08:34:51.000000 fipper-0.0.1.dev5/fipper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 08:34:51.000000 fipper-0.0.1.dev5/fipper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       57 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 08:34:57.982637 fipper-0.0.1.dev5/setup.cfg
--rw-rw-rw-   0        0        0     2106 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.949023 fipper-0.0.1.dev5/tests/
--rw-rw-rw-   0        0        0      835 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:34:57.978011 fipper-0.0.1.dev5/tests/filters/
--rw-rw-rw-   0        0        0     1237 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/tests/filters/__init__.py
--rw-rw-rw-   0        0        0     3518 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/tests/filters/test_command.py
--rw-rw-rw-   0        0        0     8400 2023-05-23 08:32:50.000000 fipper-0.0.1.dev5/tests/test_file_id.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:08.108312 fipper-0.0.2/
+-rw-rw-rw-   0        0        0    35184 2023-06-02 04:40:39.000000 fipper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      291 2023-06-02 04:40:39.000000 fipper-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      781 2023-06-02 04:40:39.000000 fipper-0.0.2/NOTICE
+-rw-rw-rw-   0        0        0     2197 2023-06-02 04:42:08.107313 fipper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-06-02 04:40:39.000000 fipper-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.573458 fipper-0.0.2/compiler/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.577458 fipper-0.0.2/compiler/api/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/api/__init__.py
+-rw-rw-rw-   0        0        0    23018 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/api/compiler.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.632426 fipper-0.0.2/compiler/api/source/
+-rw-rw-rw-   0        0        0     2273 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/api/source/auth_key.tl
+-rw-rw-rw-   0        0        0   159892 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/api/source/main_api.tl
+-rw-rw-rw-   0        0        0     3501 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/api/source/sys_msgs.tl
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.655408 fipper-0.0.2/compiler/api/template/
+-rw-rw-rw-   0        0        0      772 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/api/template/combinator.txt
+-rw-rw-rw-   0        0        0      652 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/api/template/type.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.672397 fipper-0.0.2/compiler/errors/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/__init__.py
+-rw-rw-rw-   0        0        0     5055 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/compiler.py
+-rw-rw-rw-   0        0        0     1298 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/sort.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.751857 fipper-0.0.2/compiler/errors/source/
+-rw-rw-rw-   0        0        0      475 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-rw-rw-   0        0        0    22646 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-rw-rw-   0        0        0      687 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-rw-rw-   0        0        0     2027 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-rw-rw-   0        0        0     1189 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-rw-rw-   0        0        0      475 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/420_FLOOD.tsv
+-rw-rw-rw-   0        0        0     4263 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-rw-rw-   0        0        0      157 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.769846 fipper-0.0.2/compiler/errors/template/
+-rw-rw-rw-   0        0        0      190 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/template/class.txt
+-rw-rw-rw-   0        0        0      127 2023-06-02 04:40:39.000000 fipper-0.0.2/compiler/errors/template/sub_class.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.887634 fipper-0.0.2/fipper/
+-rw-rw-rw-   0        0        0     1441 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/__init__.py
+-rw-rw-rw-   0        0        0    43136 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/client.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.957477 fipper-0.0.2/fipper/connection/
+-rw-rw-rw-   0        0        0      873 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/__init__.py
+-rw-rw-rw-   0        0        0     2916 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/connection.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.968465 fipper-0.0.2/fipper/connection/transport/
+-rw-rw-rw-   0        0        0      857 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.054453 fipper-0.0.2/fipper/connection/transport/tcp/
+-rw-rw-rw-   0        0        0     1068 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/tcp/__init__.py
+-rw-rw-rw-   0        0        0     4225 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/tcp/tcp.py
+-rw-rw-rw-   0        0        0     1825 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/tcp/tcp_abridged.py
+-rw-rw-rw-   0        0        0     2908 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/tcp/tcp_abridged_o.py
+-rw-rw-rw-   0        0        0     1970 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/tcp/tcp_full.py
+-rw-rw-rw-   0        0        0     1556 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/tcp/tcp_intermediate.py
+-rw-rw-rw-   0        0        0     2530 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/connection/transport/tcp/tcp_intermediate_o.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.154523 fipper-0.0.2/fipper/crypto/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/crypto/__init__.py
+-rw-rw-rw-   0        0        0     4143 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/crypto/aes.py
+-rw-rw-rw-   0        0        0     4890 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/crypto/mtproto.py
+-rw-rw-rw-   0        0        0     2528 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/crypto/prime.py
+-rw-rw-rw-   0        0        0    11002 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/crypto/rsa.py
+-rw-rw-rw-   0        0        0    10453 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/dispatcher.py
+-rw-rw-rw-   0        0        0   212040 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/emoji.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.347270 fipper-0.0.2/fipper/enums/
+-rw-rw-rw-   0        0        0     1785 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/auto_name.py
+-rw-rw-rw-   0        0        0     2375 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/chat_action.py
+-rw-rw-rw-   0        0        0     4328 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/chat_event_action.py
+-rw-rw-rw-   0        0        0     1306 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/chat_member_status.py
+-rw-rw-rw-   0        0        0     1484 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/chat_members_filter.py
+-rw-rw-rw-   0        0        0     1276 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/chat_type.py
+-rw-rw-rw-   0        0        0     2544 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/message_entity_type.py
+-rw-rw-rw-   0        0        0     1667 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/message_media_type.py
+-rw-rw-rw-   0        0        0     1971 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/message_service_type.py
+-rw-rw-rw-   0        0        0     2475 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/messages_filter.py
+-rw-rw-rw-   0        0        0     1456 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/next_code_type.py
+-rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/parse_mode.py
+-rw-rw-rw-   0        0        0     1076 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/poll_type.py
+-rw-rw-rw-   0        0        0     1567 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/sent_code_type.py
+-rw-rw-rw-   0        0        0     1340 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/enums/user_status.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.372255 fipper-0.0.2/fipper/errors/
+-rw-rw-rw-   0        0        0     2659 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/errors/__init__.py
+-rw-rw-rw-   0        0        0     3410 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/errors/rpc_error.py
+-rw-rw-rw-   0        0        0    15633 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/file_id.py
+-rw-rw-rw-   0        0        0    25461 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.570940 fipper-0.0.2/fipper/handlers/
+-rw-rw-rw-   0        0        0     1560 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0     2052 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/chat_join_request_handler.py
+-rw-rw-rw-   0        0        0     2087 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/chat_member_updated_handler.py
+-rw-rw-rw-   0        0        0     2143 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/chosen_inline_result_handler.py
+-rw-rw-rw-   0        0        0     2502 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/conversation_handler.py
+-rw-rw-rw-   0        0        0     2588 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/deleted_messages_handler.py
+-rw-rw-rw-   0        0        0     1739 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/disconnect_handler.py
+-rw-rw-rw-   0        0        0     2020 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/edited_message_handler.py
+-rw-rw-rw-   0        0        0     1585 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/handler.py
+-rw-rw-rw-   0        0        0     2025 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0     2902 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/message_handler.py
+-rw-rw-rw-   0        0        0     1956 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/poll_handler.py
+-rw-rw-rw-   0        0        0     2987 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/raw_update_handler.py
+-rw-rw-rw-   0        0        0     2028 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/handlers/user_status_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.581934 fipper-0.0.2/fipper/methods/
+-rw-rw-rw-   0        0        0     1365 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.632902 fipper-0.0.2/fipper/methods/advanced/
+-rw-rw-rw-   0        0        0     1017 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/advanced/__init__.py
+-rw-rw-rw-   0        0        0     3206 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/advanced/invoke.py
+-rw-rw-rw-   0        0        0     4673 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/advanced/resolve_peer.py
+-rw-rw-rw-   0        0        0     8382 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/advanced/save_file.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:03.831292 fipper-0.0.2/fipper/methods/auth/
+-rw-rw-rw-   0        0        0     1724 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     1506 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/accept_terms_of_service.py
+-rw-rw-rw-   0        0        0     1990 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/check_password.py
+-rw-rw-rw-   0        0        0     1794 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/connect.py
+-rw-rw-rw-   0        0        0     1540 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/disconnect.py
+-rw-rw-rw-   0        0        0     1339 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/get_password_hint.py
+-rw-rw-rw-   0        0        0     1735 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/initialize.py
+-rw-rw-rw-   0        0        0     1671 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/log_out.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/recover_password.py
+-rw-rw-rw-   0        0        0     2202 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/resend_code.py
+-rw-rw-rw-   0        0        0     2851 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/send_code.py
+-rw-rw-rw-   0        0        0     1510 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/send_recovery_code.py
+-rw-rw-rw-   0        0        0     3149 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/sign_in.py
+-rw-rw-rw-   0        0        0     2788 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/sign_in_bot.py
+-rw-rw-rw-   0        0        0     2416 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/sign_up.py
+-rw-rw-rw-   0        0        0     1905 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/auth/terminate.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:04.058808 fipper-0.0.2/fipper/methods/bots/
+-rw-rw-rw-   0        0        0     2096 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/__init__.py
+-rw-rw-rw-   0        0        0     3386 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/answer_callback_query.py
+-rw-rw-rw-   0        0        0     5090 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/answer_inline_query.py
+-rw-rw-rw-   0        0        0     2030 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/answer_web_app_query.py
+-rw-rw-rw-   0        0        0     2412 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/delete_bot_commands.py
+-rw-rw-rw-   0        0        0     2628 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/get_bot_commands.py
+-rw-rw-rw-   0        0        0     2102 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/get_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2377 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/get_chat_menu_button.py
+-rw-rw-rw-   0        0        0     2860 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/get_game_high_scores.py
+-rw-rw-rw-   0        0        0     3445 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/get_inline_bot_results.py
+-rw-rw-rw-   0        0        0     2918 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/request_callback_answer.py
+-rw-rw-rw-   0        0        0     4044 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/send_game.py
+-rw-rw-rw-   0        0        0     3056 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/send_inline_bot_result.py
+-rw-rw-rw-   0        0        0     2767 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/set_bot_commands.py
+-rw-rw-rw-   0        0        0     3255 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/set_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2092 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/set_chat_menu_button.py
+-rw-rw-rw-   0        0        0     4036 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/bots/set_game_score.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:04.564510 fipper-0.0.2/fipper/methods/chats/
+-rw-rw-rw-   0        0        0     3540 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0     3448 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/add_chat_members.py
+-rw-rw-rw-   0        0        0     2281 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/archive_chats.py
+-rw-rw-rw-   0        0        0     4721 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/ban_chat_member.py
+-rw-rw-rw-   0        0        0     1863 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/create_channel.py
+-rw-rw-rw-   0        0        0     2336 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/create_group.py
+-rw-rw-rw-   0        0        0     2003 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/create_supergroup.py
+-rw-rw-rw-   0        0        0     1631 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/delete_channel.py
+-rw-rw-rw-   0        0        0     2371 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/delete_chat_photo.py
+-rw-rw-rw-   0        0        0     1649 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/delete_supergroup.py
+-rw-rw-rw-   0        0        0     2018 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/delete_user_history.py
+-rw-rw-rw-   0        0        0     3355 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_chat.py
+-rw-rw-rw-   0        0        0     4129 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_chat_event_log.py
+-rw-rw-rw-   0        0        0     3418 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_chat_member.py
+-rw-rw-rw-   0        0        0     5420 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_chat_members.py
+-rw-rw-rw-   0        0        0     2327 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_chat_members_count.py
+-rw-rw-rw-   0        0        0     1768 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_chat_online_count.py
+-rw-rw-rw-   0        0        0     3456 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_dialogs.py
+-rw-rw-rw-   0        0        0     2153 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_dialogs_count.py
+-rw-rw-rw-   0        0        0     2467 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_nearby_chats.py
+-rw-rw-rw-   0        0        0     2191 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/get_send_as_chats.py
+-rw-rw-rw-   0        0        0     2758 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/join_chat.py
+-rw-rw-rw-   0        0        0     2676 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/leave_chat.py
+-rw-rw-rw-   0        0        0     1569 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/mark_chat_unread.py
+-rw-rw-rw-   0        0        0     3230 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/pin_chat_message.py
+-rw-rw-rw-   0        0        0     3954 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/promote_chat_member.py
+-rw-rw-rw-   0        0        0     4397 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/restrict_chat_member.py
+-rw-rw-rw-   0        0        0     3215 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_administrator_title.py
+-rw-rw-rw-   0        0        0     2307 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_chat_description.py
+-rw-rw-rw-   0        0        0     3488 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_chat_permissions.py
+-rw-rw-rw-   0        0        0     4708 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_chat_photo.py
+-rw-rw-rw-   0        0        0     1774 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_chat_protected_content.py
+-rw-rw-rw-   0        0        0     2644 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_chat_title.py
+-rw-rw-rw-   0        0        0     2356 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_chat_username.py
+-rw-rw-rw-   0        0        0     2031 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_send_as_chat.py
+-rw-rw-rw-   0        0        0     2140 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/set_slow_mode.py
+-rw-rw-rw-   0        0        0     2295 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/unarchive_chats.py
+-rw-rw-rw-   0        0        0     2363 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/unban_chat_member.py
+-rw-rw-rw-   0        0        0     1989 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/unpin_all_chat_messages.py
+-rw-rw-rw-   0        0        0     2194 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/chats/unpin_chat_message.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:04.638794 fipper-0.0.2/fipper/methods/contacts/
+-rw-rw-rw-   0        0        0     1187 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/contacts/__init__.py
+-rw-rw-rw-   0        0        0     2634 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/contacts/add_contact.py
+-rw-rw-rw-   0        0        0     2504 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/contacts/delete_contacts.py
+-rw-rw-rw-   0        0        0     1642 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/contacts/get_contacts.py
+-rw-rw-rw-   0        0        0     1457 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/contacts/get_contacts_count.py
+-rw-rw-rw-   0        0        0     1980 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/contacts/import_contacts.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:04.809685 fipper-0.0.2/fipper/methods/decorators/
+-rw-rw-rw-   0        0        0     1671 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2226 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0     2213 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_chat_join_request.py
+-rw-rw-rw-   0        0        0     2234 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_chat_member_updated.py
+-rw-rw-rw-   0        0        0     2262 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_chosen_inline_result.py
+-rw-rw-rw-   0        0        0     2228 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_deleted_messages.py
+-rw-rw-rw-   0        0        0     1584 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_disconnect.py
+-rw-rw-rw-   0        0        0     2217 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_edited_message.py
+-rw-rw-rw-   0        0        0     2212 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0     2183 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_message.py
+-rw-rw-rw-   0        0        0     2165 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_poll.py
+-rw-rw-rw-   0        0        0     1861 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_raw_update.py
+-rw-rw-rw-   0        0        0     2197 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/decorators/on_user_status.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:05.035546 fipper-0.0.2/fipper/methods/invite_links/
+-rw-rw-rw-   0        0        0     2493 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/approve_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1975 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/approve_chat_join_request.py
+-rw-rw-rw-   0        0        0     3444 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/create_chat_invite_link.py
+-rw-rw-rw-   0        0        0     1944 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/decline_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1976 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/decline_chat_join_request.py
+-rw-rw-rw-   0        0        0     2079 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     1797 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/delete_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3615 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/edit_chat_invite_link.py
+-rw-rw-rw-   0        0        0     2637 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/export_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3654 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/get_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     2391 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-rw-rw-   0        0        0     2045 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-rw-rw-   0        0        0     1971 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/get_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3003 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-rw-rw-   0        0        0     1979 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-rw-rw-   0        0        0     3023 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/get_chat_join_requests.py
+-rw-rw-rw-   0        0        0     2387 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/invite_links/revoke_chat_invite_link.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:05.734288 fipper-0.0.2/fipper/methods/messages/
+-rw-rw-rw-   0        0        0     4194 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0     6095 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/copy_media_group.py
+-rw-rw-rw-   0        0        0     5280 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/copy_message.py
+-rw-rw-rw-   0        0        0     3226 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/delete_messages.py
+-rw-rw-rw-   0        0        0     7705 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/download_media.py
+-rw-rw-rw-   0        0        0     2326 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_inline_caption.py
+-rw-rw-rw-   0        0        0     9990 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_inline_media.py
+-rw-rw-rw-   0        0        0     2519 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_inline_reply_markup.py
+-rw-rw-rw-   0        0        0     3189 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_inline_text.py
+-rw-rw-rw-   0        0        0     3040 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_message_caption.py
+-rw-rw-rw-   0        0        0    12725 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_message_media.py
+-rw-rw-rw-   0        0        0     3039 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_message_reply_markup.py
+-rw-rw-rw-   0        0        0     3986 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/edit_message_text.py
+-rw-rw-rw-   0        0        0     4662 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/forward_messages.py
+-rw-rw-rw-   0        0        0     4152 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_chat_history.py
+-rw-rw-rw-   0        0        0     2455 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_chat_history_count.py
+-rw-rw-rw-   0        0        0     2023 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_custom_emoji_stickers.py
+-rw-rw-rw-   0        0        0     2286 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_discussion_message.py
+-rw-rw-rw-   0        0        0     2888 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_discussion_replies.py
+-rw-rw-rw-   0        0        0     2006 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_discussion_replies_count.py
+-rw-rw-rw-   0        0        0     3011 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_media_group.py
+-rw-rw-rw-   0        0        0     4846 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/get_messages.py
+-rw-rw-rw-   0        0        0     2227 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/inline_session.py
+-rw-rw-rw-   0        0        0     2594 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/read_chat_history.py
+-rw-rw-rw-   0        0        0     2175 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/retract_vote.py
+-rw-rw-rw-   0        0        0     4259 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/search_global.py
+-rw-rw-rw-   0        0        0     2208 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/search_global_count.py
+-rw-rw-rw-   0        0        0     5486 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/search_messages.py
+-rw-rw-rw-   0        0        0     3277 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/search_messages_count.py
+-rw-rw-rw-   0        0        0    12513 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_animation.py
+-rw-rw-rw-   0        0        0    11326 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_audio.py
+-rw-rw-rw-   0        0        0     5579 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_cached_media.py
+-rw-rw-rw-   0        0        0     2887 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_chat_action.py
+-rw-rw-rw-   0        0        0     4970 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_contact.py
+-rw-rw-rw-   0        0        0     4939 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_dice.py
+-rw-rw-rw-   0        0        0    10656 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     4671 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_location.py
+-rw-rw-rw-   0        0        0    19643 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_media_group.py
+-rw-rw-rw-   0        0        0     7418 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     9303 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     8222 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_poll.py
+-rw-rw-rw-   0        0        0     2428 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_reaction.py
+-rw-rw-rw-   0        0        0     8489 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_sticker.py
+-rw-rw-rw-   0        0        0     5516 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_venue.py
+-rw-rw-rw-   0        0        0    11877 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     9487 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_video_note.py
+-rw-rw-rw-   0        0        0     9600 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/send_voice.py
+-rw-rw-rw-   0        0        0     2884 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/stop_poll.py
+-rw-rw-rw-   0        0        0     4033 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/stream_media.py
+-rw-rw-rw-   0        0        0     2563 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/vote_poll.py
+-rw-rw-rw-   0        0        0     2895 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/wait_for_callback_query.py
+-rw-rw-rw-   0        0        0     2816 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/messages/wait_for_message.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:05.785253 fipper-0.0.2/fipper/methods/password/
+-rw-rw-rw-   0        0        0     1117 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/password/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/password/change_cloud_password.py
+-rw-rw-rw-   0        0        0     3086 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/password/enable_cloud_password.py
+-rw-rw-rw-   0        0        0     2199 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/password/remove_cloud_password.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:05.958297 fipper-0.0.2/fipper/methods/users/
+-rw-rw-rw-   0        0        0     1708 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/__init__.py
+-rw-rw-rw-   0        0        0     1819 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/block_user.py
+-rw-rw-rw-   0        0        0     2288 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/delete_profile_photos.py
+-rw-rw-rw-   0        0        0     4548 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/get_chat_photos.py
+-rw-rw-rw-   0        0        0     2577 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/get_chat_photos_count.py
+-rw-rw-rw-   0        0        0     2416 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/get_common_chats.py
+-rw-rw-rw-   0        0        0     1701 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/get_default_emoji_statuses.py
+-rw-rw-rw-   0        0        0     1604 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/get_me.py
+-rw-rw-rw-   0        0        0     2621 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/get_users.py
+-rw-rw-rw-   0        0        0     1930 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/set_emoji_status.py
+-rw-rw-rw-   0        0        0     2787 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/set_profile_photo.py
+-rw-rw-rw-   0        0        0     1925 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/set_username.py
+-rw-rw-rw-   0        0        0     1829 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/unblock_user.py
+-rw-rw-rw-   0        0        0     2442 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/users/update_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.115060 fipper-0.0.2/fipper/methods/utilities/
+-rw-rw-rw-   0        0        0     1292 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/add_handler.py
+-rw-rw-rw-   0        0        0     2300 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/compose.py
+-rw-rw-rw-   0        0        0     1593 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/export_session_string.py
+-rw-rw-rw-   0        0        0     2833 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/idle.py
+-rw-rw-rw-   0        0        0     2259 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/remove_handler.py
+-rw-rw-rw-   0        0        0     2354 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/restart.py
+-rw-rw-rw-   0        0        0     2925 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     2432 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/start.py
+-rw-rw-rw-   0        0        0     2178 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/stop.py
+-rw-rw-rw-   0        0        0     1749 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/methods/utilities/stop_transmission.py
+-rw-rw-rw-   0        0        0    63796 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/mime_types.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.175705 fipper-0.0.2/fipper/parser/
+-rw-rw-rw-   0        0        0      865 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/parser/__init__.py
+-rw-rw-rw-   0        0        0     7587 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/parser/html.py
+-rw-rw-rw-   0        0        0     5937 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/parser/markdown.py
+-rw-rw-rw-   0        0        0     2132 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/parser/parser.py
+-rw-rw-rw-   0        0        0     1586 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/parser/utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.187703 fipper-0.0.2/fipper/raw/
+-rw-rw-rw-   0        0        0     1066 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.312624 fipper-0.0.2/fipper/raw/core/
+-rw-rw-rw-   0        0        0     1343 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/__init__.py
+-rw-rw-rw-   0        0        0     1745 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/future_salt.py
+-rw-rw-rw-   0        0        0     1954 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/future_salts.py
+-rw-rw-rw-   0        0        0     1876 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/gzip_packed.py
+-rw-rw-rw-   0        0        0     1072 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/list.py
+-rw-rw-rw-   0        0        0     1907 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/message.py
+-rw-rw-rw-   0        0        0     1667 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/msg_container.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.404568 fipper-0.0.2/fipper/raw/core/primitives/
+-rw-rw-rw-   0        0        0     1036 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/primitives/bool.py
+-rw-rw-rw-   0        0        0     1814 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/primitives/bytes.py
+-rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/primitives/double.py
+-rw-rw-rw-   0        0        0     1403 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/primitives/int.py
+-rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/primitives/string.py
+-rw-rw-rw-   0        0        0     2081 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/primitives/vector.py
+-rw-rw-rw-   0        0        0     2575 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/raw/core/tl_object.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.443544 fipper-0.0.2/fipper/session/
+-rw-rw-rw-   0        0        0      891 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/__init__.py
+-rw-rw-rw-   0        0        0    10760 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/auth.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.544481 fipper-0.0.2/fipper/session/internals/
+-rw-rw-rw-   0        0        0      938 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/internals/__init__.py
+-rw-rw-rw-   0        0        0     2446 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/internals/data_center.py
+-rw-rw-rw-   0        0        0     1406 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/internals/msg_factory.py
+-rw-rw-rw-   0        0        0     1632 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/internals/msg_id.py
+-rw-rw-rw-   0        0        0     1291 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/internals/seq_no.py
+-rw-rw-rw-   0        0        0    12801 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/session/session.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.610460 fipper-0.0.2/fipper/storage/
+-rw-rw-rw-   0        0        0      949 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/storage/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/storage/file_storage.py
+-rw-rw-rw-   0        0        0     2823 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/storage/memory_storage.py
+-rw-rw-rw-   0        0        0     6638 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/storage/sqlite_storage.py
+-rw-rw-rw-   0        0        0     2872 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/storage/storage.py
+-rw-rw-rw-   0        0        0     3846 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/sync.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.660424 fipper-0.0.2/fipper/types/
+-rw-rw-rw-   0        0        0     1137 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:06.695403 fipper-0.0.2/fipper/types/authorization/
+-rw-rw-rw-   0        0        0      960 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/authorization/__init__.py
+-rw-rw-rw-   0        0        0     2336 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/authorization/sent_code.py
+-rw-rw-rw-   0        0        0     1978 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/authorization/terms_of_service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:07.018713 fipper-0.0.2/fipper/types/bots_and_keyboards/
+-rw-rw-rw-   0        0        0     2901 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/__init__.py
+-rw-rw-rw-   0        0        0     1789 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command.py
+-rw-rw-rw-   0        0        0     2841 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope.py
+-rw-rw-rw-   0        0        0     1319 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-rw-rw-   0        0        0     1284 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-rw-rw-   0        0        0     1275 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-rw-rw-   0        0        0     1599 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-rw-rw-   0        0        0     1676 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-rw-rw-   0        0        0     1859 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-rw-rw-   0        0        0     1335 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-rw-rw-   0        0        0     1058 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/callback_game.py
+-rw-rw-rw-   0        0        0    13062 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/callback_query.py
+-rw-rw-rw-   0        0        0     2443 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/force_reply.py
+-rw-rw-rw-   0        0        0     2276 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/game_high_score.py
+-rw-rw-rw-   0        0        0     8312 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0     2526 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-rw-rw-   0        0        0     3605 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/keyboard_button.py
+-rw-rw-rw-   0        0        0     3800 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/login_url.py
+-rw-rw-rw-   0        0        0     1633 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button.py
+-rw-rw-rw-   0        0        0     1235 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button_commands.py
+-rw-rw-rw-   0        0        0     1238 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button_default.py
+-rw-rw-rw-   0        0        0     1850 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button_web_app.py
+-rw-rw-rw-   0        0        0     4221 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-rw-rw-   0        0        0     2391 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-rw-rw-   0        0        0     1604 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/sent_web_app_message.py
+-rw-rw-rw-   0        0        0     1350 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/bots_and_keyboards/web_app_info.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:07.286070 fipper-0.0.2/fipper/types/inline_mode/
+-rw-rw-rw-   0        0        0     2802 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/chosen_inline_result.py
+-rw-rw-rw-   0        0        0     7459 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query.py
+-rw-rw-rw-   0        0        0     2434 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result.py
+-rw-rw-rw-   0        0        0     5917 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_animation.py
+-rw-rw-rw-   0        0        0     3391 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     4611 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_audio.py
+-rw-rw-rw-   0        0        0     4339 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_animation.py
+-rw-rw-rw-   0        0        0     4116 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_audio.py
+-rw-rw-rw-   0        0        0     4487 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_document.py
+-rw-rw-rw-   0        0        0     4409 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_photo.py
+-rw-rw-rw-   0        0        0     3099 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-rw-rw-   0        0        0     4494 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_video.py
+-rw-rw-rw-   0        0        0     4296 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_voice.py
+-rw-rw-rw-   0        0        0     4236 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_contact.py
+-rw-rw-rw-   0        0        0     5371 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     4731 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_location.py
+-rw-rw-rw-   0        0        0     5394 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     4875 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_venue.py
+-rw-rw-rw-   0        0        0     5611 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_video.py
+-rw-rw-rw-   0        0        0     4460 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/inline_mode/inline_query_result_voice.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:07.385819 fipper-0.0.2/fipper/types/input_media/
+-rw-rw-rw-   0        0        0     1344 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/__init__.py
+-rw-rw-rw-   0        0        0     1677 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/input_media.py
+-rw-rw-rw-   0        0        0     3305 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/input_media_animation.py
+-rw-rw-rw-   0        0        0     3358 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/input_media_audio.py
+-rw-rw-rw-   0        0        0     2832 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/input_media_document.py
+-rw-rw-rw-   0        0        0     2536 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/input_media_photo.py
+-rw-rw-rw-   0        0        0     3500 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/input_media_video.py
+-rw-rw-rw-   0        0        0     1782 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_media/input_phone_contact.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:07.424791 fipper-0.0.2/fipper/types/input_message_content/
+-rw-rw-rw-   0        0        0     1030 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_message_content/__init__.py
+-rw-rw-rw-   0        0        0     1441 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_message_content/input_message_content.py
+-rw-rw-rw-   0        0        0     2696 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/input_message_content/input_text_message_content.py
+-rw-rw-rw-   0        0        0     1121 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/list.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:07.751532 fipper-0.0.2/fipper/types/messages_and_media/
+-rw-rw-rw-   0        0        0     1883 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/__init__.py
+-rw-rw-rw-   0        0        0     4153 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/animation.py
+-rw-rw-rw-   0        0        0     4178 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/audio.py
+-rw-rw-rw-   0        0        0     2270 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/contact.py
+-rw-rw-rw-   0        0        0     1628 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/dice.py
+-rw-rw-rw-   0        0        0     3495 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/document.py
+-rw-rw-rw-   0        0        0     3131 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/game.py
+-rw-rw-rw-   0        0        0     1709 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/location.py
+-rw-rw-rw-   0        0        0   150486 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/message.py
+-rw-rw-rw-   0        0        0     4456 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/message_entity.py
+-rw-rw-rw-   0        0        0     1846 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/message_reactions.py
+-rw-rw-rw-   0        0        0     4427 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/photo.py
+-rw-rw-rw-   0        0        0     7226 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/poll.py
+-rw-rw-rw-   0        0        0     1578 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/poll_option.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/reaction.py
+-rw-rw-rw-   0        0        0     7101 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/sticker.py
+-rw-rw-rw-   0        0        0     1472 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/stripped_thumbnail.py
+-rw-rw-rw-   0        0        0     3858 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/thumbnail.py
+-rw-rw-rw-   0        0        0     2355 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/venue.py
+-rw-rw-rw-   0        0        0     4511 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/video.py
+-rw-rw-rw-   0        0        0     3697 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/video_note.py
+-rw-rw-rw-   0        0        0     3292 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/voice.py
+-rw-rw-rw-   0        0        0     1614 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/web_app_data.py
+-rw-rw-rw-   0        0        0     6520 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/messages_and_media/web_page.py
+-rw-rw-rw-   0        0        0     3973 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/object.py
+-rw-rw-rw-   0        0        0     1023 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/update.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:08.056348 fipper-0.0.2/fipper/types/user_and_chats/
+-rw-rw-rw-   0        0        0     2364 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/__init__.py
+-rw-rw-rw-   0        0        0    33702 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat.py
+-rw-rw-rw-   0        0        0     2289 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-rw-rw-   0        0        0    20240 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_event.py
+-rw-rw-rw-   0        0        0     5687 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_event_filter.py
+-rw-rw-rw-   0        0        0     4699 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_invite_link.py
+-rw-rw-rw-   0        0        0     4364 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_join_request.py
+-rw-rw-rw-   0        0        0     2634 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_joiner.py
+-rw-rw-rw-   0        0        0     9647 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_member.py
+-rw-rw-rw-   0        0        0     3756 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_member_updated.py
+-rw-rw-rw-   0        0        0     4478 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_permissions.py
+-rw-rw-rw-   0        0        0     4066 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_photo.py
+-rw-rw-rw-   0        0        0     2659 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_preview.py
+-rw-rw-rw-   0        0        0     5061 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_privileges.py
+-rw-rw-rw-   0        0        0     2417 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/chat_reactions.py
+-rw-rw-rw-   0        0        0     2749 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/dialog.py
+-rw-rw-rw-   0        0        0     2491 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/emoji_status.py
+-rw-rw-rw-   0        0        0     2006 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/invite_link_importer.py
+-rw-rw-rw-   0        0        0     1711 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/restriction.py
+-rw-rw-rw-   0        0        0    13477 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/user.py
+-rw-rw-rw-   0        0        0     1385 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/video_chat_ended.py
+-rw-rw-rw-   0        0        0     1656 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/video_chat_members_invited.py
+-rw-rw-rw-   0        0        0     1572 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/video_chat_scheduled.py
+-rw-rw-rw-   0        0        0     1072 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/types/user_and_chats/video_chat_started.py
+-rw-rw-rw-   0        0        0    10933 2023-06-02 04:40:39.000000 fipper-0.0.2/fipper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:02.933487 fipper-0.0.2/fipper.egg-info/
+-rw-rw-rw-   0        0        0     2197 2023-06-02 04:42:01.000000 fipper-0.0.2/fipper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17932 2023-06-02 04:42:01.000000 fipper-0.0.2/fipper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 04:42:01.000000 fipper-0.0.2/fipper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 04:42:01.000000 fipper-0.0.2/fipper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       54 2023-06-02 04:42:01.000000 fipper-0.0.2/fipper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 04:42:01.000000 fipper-0.0.2/fipper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       57 2023-06-02 04:40:39.000000 fipper-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 04:42:08.109311 fipper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2106 2023-06-02 04:40:39.000000 fipper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:08.080336 fipper-0.0.2/tests/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 04:42:08.104316 fipper-0.0.2/tests/filters/
+-rw-rw-rw-   0        0        0     1237 2023-06-02 04:40:39.000000 fipper-0.0.2/tests/filters/__init__.py
+-rw-rw-rw-   0        0        0     3518 2023-06-02 04:40:39.000000 fipper-0.0.2/tests/filters/test_command.py
+-rw-rw-rw-   0        0        0     8400 2023-06-02 04:40:39.000000 fipper-0.0.2/tests/test_file_id.py
```

### Comparing `fipper-0.0.1.dev5/LICENSE` & `fipper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/NOTICE` & `fipper-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/PKG-INFO` & `fipper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fipper
-Version: 0.0.1.dev5
+Version: 0.0.2
 Summary: Fipper - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/AyiinXd/fipper
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/fipper/issues
 Project-URL: Documentation, https://fipper.tech
```

### Comparing `fipper-0.0.1.dev5/README.md` & `fipper-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/__init__.py` & `fipper-0.0.2/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/api/__init__.py` & `fipper-0.0.2/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/api/compiler.py` & `fipper-0.0.2/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/api/source/auth_key.tl` & `fipper-0.0.2/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/api/source/main_api.tl` & `fipper-0.0.2/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/api/source/sys_msgs.tl` & `fipper-0.0.2/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/api/template/combinator.txt` & `fipper-0.0.2/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/api/template/type.txt` & `fipper-0.0.2/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/__init__.py` & `fipper-0.0.2/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/compiler.py` & `fipper-0.0.2/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/sort.py` & `fipper-0.0.2/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/source/400_BAD_REQUEST.tsv` & `fipper-0.0.2/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/source/401_UNAUTHORIZED.tsv` & `fipper-0.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/source/403_FORBIDDEN.tsv` & `fipper-0.0.2/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `fipper-0.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `fipper-0.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/__init__.py` & `fipper-0.0.2/fipper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.0.1.dev05"
+__version__ = "0.0.2"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `fipper-0.0.1.dev5/fipper/client.py` & `fipper-0.0.2/fipper/client.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/__init__.py` & `fipper-0.0.2/fipper/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/connection.py` & `fipper-0.0.2/fipper/connection/connection.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/__init__.py` & `fipper-0.0.2/fipper/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/tcp/__init__.py` & `fipper-0.0.2/fipper/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp.py` & `fipper-0.0.2/fipper/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_abridged.py` & `fipper-0.0.2/fipper/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_abridged_o.py` & `fipper-0.0.2/fipper/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_full.py` & `fipper-0.0.2/fipper/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_intermediate.py` & `fipper-0.0.2/fipper/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/connection/transport/tcp/tcp_intermediate_o.py` & `fipper-0.0.2/fipper/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/crypto/__init__.py` & `fipper-0.0.2/fipper/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/crypto/aes.py` & `fipper-0.0.2/fipper/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/crypto/mtproto.py` & `fipper-0.0.2/fipper/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/crypto/prime.py` & `fipper-0.0.2/fipper/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/crypto/rsa.py` & `fipper-0.0.2/fipper/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/dispatcher.py` & `fipper-0.0.2/fipper/dispatcher.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/emoji.py` & `fipper-0.0.2/fipper/emoji.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/__init__.py` & `fipper-0.0.2/fipper/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/auto_name.py` & `fipper-0.0.2/fipper/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/chat_action.py` & `fipper-0.0.2/fipper/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/chat_event_action.py` & `fipper-0.0.2/fipper/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/chat_member_status.py` & `fipper-0.0.2/fipper/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/chat_members_filter.py` & `fipper-0.0.2/fipper/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/chat_type.py` & `fipper-0.0.2/fipper/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/message_entity_type.py` & `fipper-0.0.2/fipper/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/message_media_type.py` & `fipper-0.0.2/fipper/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/message_service_type.py` & `fipper-0.0.2/fipper/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/messages_filter.py` & `fipper-0.0.2/fipper/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/next_code_type.py` & `fipper-0.0.2/fipper/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/parse_mode.py` & `fipper-0.0.2/fipper/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/poll_type.py` & `fipper-0.0.2/fipper/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/sent_code_type.py` & `fipper-0.0.2/fipper/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/enums/user_status.py` & `fipper-0.0.2/fipper/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/errors/__init__.py` & `fipper-0.0.2/fipper/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/errors/rpc_error.py` & `fipper-0.0.2/fipper/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/file_id.py` & `fipper-0.0.2/fipper/file_id.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/filters.py` & `fipper-0.0.2/fipper/filters.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/__init__.py` & `fipper-0.0.2/fipper/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/callback_query_handler.py` & `fipper-0.0.2/fipper/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/chat_join_request_handler.py` & `fipper-0.0.2/fipper/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/chat_member_updated_handler.py` & `fipper-0.0.2/fipper/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/chosen_inline_result_handler.py` & `fipper-0.0.2/fipper/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/conversation_handler.py` & `fipper-0.0.2/fipper/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/deleted_messages_handler.py` & `fipper-0.0.2/fipper/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/disconnect_handler.py` & `fipper-0.0.2/fipper/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/edited_message_handler.py` & `fipper-0.0.2/fipper/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/handler.py` & `fipper-0.0.2/fipper/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/inline_query_handler.py` & `fipper-0.0.2/fipper/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/message_handler.py` & `fipper-0.0.2/fipper/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/poll_handler.py` & `fipper-0.0.2/fipper/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/raw_update_handler.py` & `fipper-0.0.2/fipper/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/handlers/user_status_handler.py` & `fipper-0.0.2/fipper/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/__init__.py` & `fipper-0.0.2/fipper/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/advanced/__init__.py` & `fipper-0.0.2/fipper/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/advanced/invoke.py` & `fipper-0.0.2/fipper/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/advanced/resolve_peer.py` & `fipper-0.0.2/fipper/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/advanced/save_file.py` & `fipper-0.0.2/fipper/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/__init__.py` & `fipper-0.0.2/fipper/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/accept_terms_of_service.py` & `fipper-0.0.2/fipper/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/check_password.py` & `fipper-0.0.2/fipper/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/connect.py` & `fipper-0.0.2/fipper/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/disconnect.py` & `fipper-0.0.2/fipper/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/get_password_hint.py` & `fipper-0.0.2/fipper/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/initialize.py` & `fipper-0.0.2/fipper/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/log_out.py` & `fipper-0.0.2/fipper/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/recover_password.py` & `fipper-0.0.2/fipper/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/resend_code.py` & `fipper-0.0.2/fipper/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/send_code.py` & `fipper-0.0.2/fipper/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/send_recovery_code.py` & `fipper-0.0.2/fipper/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/sign_in.py` & `fipper-0.0.2/fipper/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/sign_in_bot.py` & `fipper-0.0.2/fipper/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/sign_up.py` & `fipper-0.0.2/fipper/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/auth/terminate.py` & `fipper-0.0.2/fipper/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/__init__.py` & `fipper-0.0.2/fipper/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/answer_callback_query.py` & `fipper-0.0.2/fipper/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/answer_inline_query.py` & `fipper-0.0.2/fipper/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/answer_web_app_query.py` & `fipper-0.0.2/fipper/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/delete_bot_commands.py` & `fipper-0.0.2/fipper/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/get_bot_commands.py` & `fipper-0.0.2/fipper/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/get_bot_default_privileges.py` & `fipper-0.0.2/fipper/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/get_chat_menu_button.py` & `fipper-0.0.2/fipper/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/get_game_high_scores.py` & `fipper-0.0.2/fipper/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/get_inline_bot_results.py` & `fipper-0.0.2/fipper/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/request_callback_answer.py` & `fipper-0.0.2/fipper/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/send_game.py` & `fipper-0.0.2/fipper/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/send_inline_bot_result.py` & `fipper-0.0.2/fipper/methods/bots/send_inline_bot_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 class SendInlineBotResult:
     async def send_inline_bot_result(
         self: "fipper.Client",
         chat_id: Union[int, str],
         query_id: int,
         result_id: str,
         disable_notification: bool = None,
-        reply_to_message_id: int = None
+        reply_to_message_id: int = None,
+        hide_via: bool = None
     ):
         """Send an inline bot result.
         Bot results can be retrieved using :meth:`~fipper.Client.get_inline_bot_results`
 
         .. include:: /_includes/usable-by/users.rst
 
         Parameters:
@@ -50,14 +51,17 @@
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             reply_to_message_id (``bool``, *optional*):
                 If the message is a reply, ID of the original message.
+            
+            hide_via (``bool``):
+                Sends the message with *via @bot* hidden.
 
         Returns:
             :obj:`~fipper.types.Message`: On success, the sent inline result message is returned.
 
         Example:
             .. code-block:: python
 
@@ -66,10 +70,11 @@
         return await self.invoke(
             raw.functions.messages.SendInlineBotResult(
                 peer=await self.resolve_peer(chat_id),
                 query_id=query_id,
                 id=result_id,
                 random_id=self.rnd_id(),
                 silent=disable_notification or None,
-                reply_to_msg_id=reply_to_message_id
+                reply_to_msg_id=reply_to_message_id,
+                hide_via=hide_via or None
             )
         )
```

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/set_bot_commands.py` & `fipper-0.0.2/fipper/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/set_bot_default_privileges.py` & `fipper-0.0.2/fipper/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/set_chat_menu_button.py` & `fipper-0.0.2/fipper/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/bots/set_game_score.py` & `fipper-0.0.2/fipper/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/__init__.py` & `fipper-0.0.2/fipper/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/add_chat_members.py` & `fipper-0.0.2/fipper/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/archive_chats.py` & `fipper-0.0.2/fipper/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/ban_chat_member.py` & `fipper-0.0.2/fipper/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/create_channel.py` & `fipper-0.0.2/fipper/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/create_group.py` & `fipper-0.0.2/fipper/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/create_supergroup.py` & `fipper-0.0.2/fipper/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/delete_channel.py` & `fipper-0.0.2/fipper/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/delete_chat_photo.py` & `fipper-0.0.2/fipper/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/delete_supergroup.py` & `fipper-0.0.2/fipper/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/delete_user_history.py` & `fipper-0.0.2/fipper/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_chat.py` & `fipper-0.0.2/fipper/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_chat_event_log.py` & `fipper-0.0.2/fipper/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_chat_member.py` & `fipper-0.0.2/fipper/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_chat_members.py` & `fipper-0.0.2/fipper/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_chat_members_count.py` & `fipper-0.0.2/fipper/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_chat_online_count.py` & `fipper-0.0.2/fipper/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_dialogs.py` & `fipper-0.0.2/fipper/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_dialogs_count.py` & `fipper-0.0.2/fipper/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_nearby_chats.py` & `fipper-0.0.2/fipper/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/get_send_as_chats.py` & `fipper-0.0.2/fipper/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/join_chat.py` & `fipper-0.0.2/fipper/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/leave_chat.py` & `fipper-0.0.2/fipper/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/mark_chat_unread.py` & `fipper-0.0.2/fipper/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/pin_chat_message.py` & `fipper-0.0.2/fipper/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/promote_chat_member.py` & `fipper-0.0.2/fipper/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/restrict_chat_member.py` & `fipper-0.0.2/fipper/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_administrator_title.py` & `fipper-0.0.2/fipper/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_chat_description.py` & `fipper-0.0.2/fipper/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_chat_permissions.py` & `fipper-0.0.2/fipper/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_chat_photo.py` & `fipper-0.0.2/fipper/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_chat_protected_content.py` & `fipper-0.0.2/fipper/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_chat_title.py` & `fipper-0.0.2/fipper/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_chat_username.py` & `fipper-0.0.2/fipper/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_send_as_chat.py` & `fipper-0.0.2/fipper/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/set_slow_mode.py` & `fipper-0.0.2/fipper/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/unarchive_chats.py` & `fipper-0.0.2/fipper/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/unban_chat_member.py` & `fipper-0.0.2/fipper/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/unpin_all_chat_messages.py` & `fipper-0.0.2/fipper/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/chats/unpin_chat_message.py` & `fipper-0.0.2/fipper/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/contacts/__init__.py` & `fipper-0.0.2/fipper/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/contacts/add_contact.py` & `fipper-0.0.2/fipper/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/contacts/delete_contacts.py` & `fipper-0.0.2/fipper/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/contacts/get_contacts.py` & `fipper-0.0.2/fipper/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/contacts/get_contacts_count.py` & `fipper-0.0.2/fipper/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/contacts/import_contacts.py` & `fipper-0.0.2/fipper/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/__init__.py` & `fipper-0.0.2/fipper/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_callback_query.py` & `fipper-0.0.2/fipper/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_chat_join_request.py` & `fipper-0.0.2/fipper/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_chat_member_updated.py` & `fipper-0.0.2/fipper/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_chosen_inline_result.py` & `fipper-0.0.2/fipper/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_deleted_messages.py` & `fipper-0.0.2/fipper/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_disconnect.py` & `fipper-0.0.2/fipper/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_edited_message.py` & `fipper-0.0.2/fipper/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_inline_query.py` & `fipper-0.0.2/fipper/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_message.py` & `fipper-0.0.2/fipper/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_poll.py` & `fipper-0.0.2/fipper/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_raw_update.py` & `fipper-0.0.2/fipper/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/decorators/on_user_status.py` & `fipper-0.0.2/fipper/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/__init__.py` & `fipper-0.0.2/fipper/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/approve_all_chat_join_requests.py` & `fipper-0.0.2/fipper/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/approve_chat_join_request.py` & `fipper-0.0.2/fipper/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/create_chat_invite_link.py` & `fipper-0.0.2/fipper/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/decline_all_chat_join_requests.py` & `fipper-0.0.2/fipper/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/decline_chat_join_request.py` & `fipper-0.0.2/fipper/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/delete_chat_admin_invite_links.py` & `fipper-0.0.2/fipper/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/delete_chat_invite_link.py` & `fipper-0.0.2/fipper/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/edit_chat_invite_link.py` & `fipper-0.0.2/fipper/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/export_chat_invite_link.py` & `fipper-0.0.2/fipper/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_admin_invite_links.py` & `fipper-0.0.2/fipper/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_admin_invite_links_count.py` & `fipper-0.0.2/fipper/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_admins_with_invite_links.py` & `fipper-0.0.2/fipper/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_invite_link.py` & `fipper-0.0.2/fipper/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_invite_link_joiners.py` & `fipper-0.0.2/fipper/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py` & `fipper-0.0.2/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/get_chat_join_requests.py` & `fipper-0.0.2/fipper/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/invite_links/revoke_chat_invite_link.py` & `fipper-0.0.2/fipper/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/__init__.py` & `fipper-0.0.2/fipper/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/copy_media_group.py` & `fipper-0.0.2/fipper/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/copy_message.py` & `fipper-0.0.2/fipper/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/delete_messages.py` & `fipper-0.0.2/fipper/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/download_media.py` & `fipper-0.0.2/fipper/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_caption.py` & `fipper-0.0.2/fipper/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_media.py` & `fipper-0.0.2/fipper/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_reply_markup.py` & `fipper-0.0.2/fipper/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_inline_text.py` & `fipper-0.0.2/fipper/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_message_caption.py` & `fipper-0.0.2/fipper/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_message_media.py` & `fipper-0.0.2/fipper/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_message_reply_markup.py` & `fipper-0.0.2/fipper/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/edit_message_text.py` & `fipper-0.0.2/fipper/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/forward_messages.py` & `fipper-0.0.2/fipper/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_chat_history.py` & `fipper-0.0.2/fipper/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_chat_history_count.py` & `fipper-0.0.2/fipper/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_custom_emoji_stickers.py` & `fipper-0.0.2/fipper/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_discussion_message.py` & `fipper-0.0.2/fipper/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_discussion_replies.py` & `fipper-0.0.2/fipper/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_discussion_replies_count.py` & `fipper-0.0.2/fipper/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_media_group.py` & `fipper-0.0.2/fipper/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/get_messages.py` & `fipper-0.0.2/fipper/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/inline_session.py` & `fipper-0.0.2/fipper/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/read_chat_history.py` & `fipper-0.0.2/fipper/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/retract_vote.py` & `fipper-0.0.2/fipper/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/search_global.py` & `fipper-0.0.2/fipper/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/search_global_count.py` & `fipper-0.0.2/fipper/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/search_messages.py` & `fipper-0.0.2/fipper/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/search_messages_count.py` & `fipper-0.0.2/fipper/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_animation.py` & `fipper-0.0.2/fipper/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_audio.py` & `fipper-0.0.2/fipper/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_cached_media.py` & `fipper-0.0.2/fipper/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_chat_action.py` & `fipper-0.0.2/fipper/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_contact.py` & `fipper-0.0.2/fipper/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_dice.py` & `fipper-0.0.2/fipper/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_document.py` & `fipper-0.0.2/fipper/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_location.py` & `fipper-0.0.2/fipper/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_media_group.py` & `fipper-0.0.2/fipper/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_message.py` & `fipper-0.0.2/fipper/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_photo.py` & `fipper-0.0.2/fipper/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_poll.py` & `fipper-0.0.2/fipper/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_reaction.py` & `fipper-0.0.2/fipper/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_sticker.py` & `fipper-0.0.2/fipper/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_venue.py` & `fipper-0.0.2/fipper/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_video.py` & `fipper-0.0.2/fipper/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_video_note.py` & `fipper-0.0.2/fipper/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/send_voice.py` & `fipper-0.0.2/fipper/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/stop_poll.py` & `fipper-0.0.2/fipper/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/stream_media.py` & `fipper-0.0.2/fipper/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/vote_poll.py` & `fipper-0.0.2/fipper/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/wait_for_callback_query.py` & `fipper-0.0.2/fipper/methods/messages/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/messages/wait_for_message.py` & `fipper-0.0.2/fipper/methods/messages/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/password/__init__.py` & `fipper-0.0.2/fipper/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/password/change_cloud_password.py` & `fipper-0.0.2/fipper/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/password/enable_cloud_password.py` & `fipper-0.0.2/fipper/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/password/remove_cloud_password.py` & `fipper-0.0.2/fipper/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/__init__.py` & `fipper-0.0.2/fipper/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/block_user.py` & `fipper-0.0.2/fipper/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/delete_profile_photos.py` & `fipper-0.0.2/fipper/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/get_chat_photos.py` & `fipper-0.0.2/fipper/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/get_chat_photos_count.py` & `fipper-0.0.2/fipper/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/get_common_chats.py` & `fipper-0.0.2/fipper/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/get_default_emoji_statuses.py` & `fipper-0.0.2/fipper/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/get_me.py` & `fipper-0.0.2/fipper/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/get_users.py` & `fipper-0.0.2/fipper/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/set_emoji_status.py` & `fipper-0.0.2/fipper/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/set_profile_photo.py` & `fipper-0.0.2/fipper/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/set_username.py` & `fipper-0.0.2/fipper/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/unblock_user.py` & `fipper-0.0.2/fipper/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/users/update_profile.py` & `fipper-0.0.2/fipper/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/__init__.py` & `fipper-0.0.2/fipper/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/add_handler.py` & `fipper-0.0.2/fipper/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/compose.py` & `fipper-0.0.2/fipper/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/export_session_string.py` & `fipper-0.0.2/fipper/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/idle.py` & `fipper-0.0.2/fipper/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/remove_handler.py` & `fipper-0.0.2/fipper/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/restart.py` & `fipper-0.0.2/fipper/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/run.py` & `fipper-0.0.2/fipper/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/start.py` & `fipper-0.0.2/fipper/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/stop.py` & `fipper-0.0.2/fipper/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/methods/utilities/stop_transmission.py` & `fipper-0.0.2/fipper/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/mime_types.py` & `fipper-0.0.2/fipper/mime_types.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/parser/__init__.py` & `fipper-0.0.2/fipper/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/parser/html.py` & `fipper-0.0.2/fipper/parser/html.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/parser/markdown.py` & `fipper-0.0.2/fipper/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/parser/parser.py` & `fipper-0.0.2/fipper/parser/parser.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/parser/utils.py` & `fipper-0.0.2/fipper/parser/utils.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/__init__.py` & `fipper-0.0.2/fipper/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/__init__.py` & `fipper-0.0.2/fipper/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/future_salt.py` & `fipper-0.0.2/fipper/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/future_salts.py` & `fipper-0.0.2/fipper/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/gzip_packed.py` & `fipper-0.0.2/fipper/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/list.py` & `fipper-0.0.2/fipper/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/message.py` & `fipper-0.0.2/fipper/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/msg_container.py` & `fipper-0.0.2/fipper/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/primitives/__init__.py` & `fipper-0.0.2/fipper/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/primitives/bool.py` & `fipper-0.0.2/fipper/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/primitives/bytes.py` & `fipper-0.0.2/fipper/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/primitives/double.py` & `fipper-0.0.2/fipper/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/primitives/int.py` & `fipper-0.0.2/fipper/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/primitives/string.py` & `fipper-0.0.2/fipper/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/primitives/vector.py` & `fipper-0.0.2/fipper/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/raw/core/tl_object.py` & `fipper-0.0.2/fipper/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/__init__.py` & `fipper-0.0.2/fipper/session/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/auth.py` & `fipper-0.0.2/fipper/session/auth.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/internals/__init__.py` & `fipper-0.0.2/fipper/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/internals/data_center.py` & `fipper-0.0.2/fipper/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/internals/msg_factory.py` & `fipper-0.0.2/fipper/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/internals/msg_id.py` & `fipper-0.0.2/fipper/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/internals/seq_no.py` & `fipper-0.0.2/fipper/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/session/session.py` & `fipper-0.0.2/fipper/session/session.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/storage/__init__.py` & `fipper-0.0.2/fipper/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/storage/file_storage.py` & `fipper-0.0.2/fipper/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/storage/memory_storage.py` & `fipper-0.0.2/fipper/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/storage/sqlite_storage.py` & `fipper-0.0.2/fipper/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/storage/storage.py` & `fipper-0.0.2/fipper/storage/storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/sync.py` & `fipper-0.0.2/fipper/sync.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/__init__.py` & `fipper-0.0.2/fipper/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/authorization/__init__.py` & `fipper-0.0.2/fipper/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/authorization/sent_code.py` & `fipper-0.0.2/fipper/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/authorization/terms_of_service.py` & `fipper-0.0.2/fipper/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/__init__.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_chat.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/bot_command_scope_default.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/callback_game.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/callback_query.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/force_reply.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/game_high_score.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/inline_keyboard_button.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/inline_keyboard_markup.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/keyboard_button.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/login_url.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button_commands.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button_default.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/menu_button_web_app.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/reply_keyboard_markup.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/reply_keyboard_remove.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/sent_web_app_message.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/bots_and_keyboards/web_app_info.py` & `fipper-0.0.2/fipper/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/__init__.py` & `fipper-0.0.2/fipper/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/chosen_inline_result.py` & `fipper-0.0.2/fipper/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_animation.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_article.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_audio.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_animation.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_audio.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_document.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_photo.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_sticker.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_video.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_cached_voice.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_contact.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_document.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_location.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_photo.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_venue.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_video.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/inline_mode/inline_query_result_voice.py` & `fipper-0.0.2/fipper/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/__init__.py` & `fipper-0.0.2/fipper/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/input_media.py` & `fipper-0.0.2/fipper/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/input_media_animation.py` & `fipper-0.0.2/fipper/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/input_media_audio.py` & `fipper-0.0.2/fipper/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/input_media_document.py` & `fipper-0.0.2/fipper/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/input_media_photo.py` & `fipper-0.0.2/fipper/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/input_media_video.py` & `fipper-0.0.2/fipper/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_media/input_phone_contact.py` & `fipper-0.0.2/fipper/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_message_content/__init__.py` & `fipper-0.0.2/fipper/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_message_content/input_message_content.py` & `fipper-0.0.2/fipper/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/input_message_content/input_text_message_content.py` & `fipper-0.0.2/fipper/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/list.py` & `fipper-0.0.2/fipper/types/list.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/__init__.py` & `fipper-0.0.2/fipper/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/animation.py` & `fipper-0.0.2/fipper/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/audio.py` & `fipper-0.0.2/fipper/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/contact.py` & `fipper-0.0.2/fipper/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/dice.py` & `fipper-0.0.2/fipper/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/document.py` & `fipper-0.0.2/fipper/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/game.py` & `fipper-0.0.2/fipper/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/location.py` & `fipper-0.0.2/fipper/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/message.py` & `fipper-0.0.2/fipper/types/messages_and_media/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -4554,4842 +4554,4853 @@
 00011c90: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
 00011ca0: 7175 6f74 653a 2062 6f6f 6c20 3d20 4e6f  quote: bool = No
 00011cb0: 6e65 2c0d 0a20 2020 2020 2020 2064 6973  ne,..        dis
 00011cc0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
 00011cd0: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d  n: bool = None,.
 00011ce0: 0a20 2020 2020 2020 2072 6570 6c79 5f74  .        reply_t
 00011cf0: 6f5f 6d65 7373 6167 655f 6964 3a20 696e  o_message_id: in
-00011d00: 7420 3d20 4e6f 6e65 0d0a 2020 2020 2920  t = None..    ) 
-00011d10: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
-00011d20: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
-00011d30: 6d65 7468 6f64 202a 7265 706c 795f 696e  method *reply_in
-00011d40: 6c69 6e65 5f62 6f74 5f72 6573 756c 742a  line_bot_result*
-00011d50: 206f 6620 3a6f 626a 3a60 7e66 6970 7065   of :obj:`~fippe
-00011d60: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
-00011d70: 2e0d 0a0d 0a20 2020 2020 2020 2055 7365  .....        Use
-00011d80: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
-00011d90: 6f72 3a0d 0a0d 0a20 2020 2020 2020 202e  or:....        .
-00011da0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00011db0: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
-00011dc0: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
-00011dd0: 742e 7365 6e64 5f69 6e6c 696e 655f 626f  t.send_inline_bo
-00011de0: 745f 7265 7375 6c74 280d 0a20 2020 2020  t_result(..     
-00011df0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00011e00: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
-00011e10: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-00011e20: 2020 2020 2071 7565 7279 5f69 643d 7175       query_id=qu
-00011e30: 6572 795f 6964 2c0d 0a20 2020 2020 2020  ery_id,..       
-00011e40: 2020 2020 2020 2020 2072 6573 756c 745f           result_
-00011e50: 6964 3d72 6573 756c 745f 6964 0d0a 2020  id=result_id..  
-00011e60: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
-00011e70: 2020 2020 2020 2045 7861 6d70 6c65 3a0d         Example:.
-00011e80: 0a20 2020 2020 2020 2020 2020 202e 2e20  .            .. 
-00011e90: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-00011ea0: 686f 6e0d 0a0d 0a20 2020 2020 2020 2020  hon....         
-00011eb0: 2020 2020 2020 2061 7761 6974 206d 6573         await mes
-00011ec0: 7361 6765 2e72 6570 6c79 5f69 6e6c 696e  sage.reply_inlin
-00011ed0: 655f 626f 745f 7265 7375 6c74 2871 7565  e_bot_result(que
-00011ee0: 7279 5f69 642c 2072 6573 756c 745f 6964  ry_id, result_id
-00011ef0: 290d 0a0d 0a20 2020 2020 2020 2050 6172  )....        Par
-00011f00: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
-00011f10: 2020 2020 2020 7175 6572 795f 6964 2028        query_id (
-00011f20: 6060 696e 7460 6029 3a0d 0a20 2020 2020  ``int``):..     
-00011f30: 2020 2020 2020 2020 2020 2055 6e69 7175             Uniqu
-00011f40: 6520 6964 656e 7469 6669 6572 2066 6f72  e identifier for
-00011f50: 2074 6865 2061 6e73 7765 7265 6420 7175   the answered qu
-00011f60: 6572 792e 0d0a 0d0a 2020 2020 2020 2020  ery.....        
-00011f70: 2020 2020 7265 7375 6c74 5f69 6420 2860      result_id (`
-00011f80: 6073 7472 6060 293a 0d0a 2020 2020 2020  `str``):..      
-00011f90: 2020 2020 2020 2020 2020 556e 6971 7565            Unique
-00011fa0: 2069 6465 6e74 6966 6965 7220 666f 7220   identifier for 
-00011fb0: 7468 6520 7265 7375 6c74 2074 6861 7420  the result that 
-00011fc0: 7761 7320 6368 6f73 656e 2e0d 0a0d 0a20  was chosen..... 
-00011fd0: 2020 2020 2020 2020 2020 2071 756f 7465             quote
-00011fe0: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
-00011ff0: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
-00012000: 2020 2020 2020 2020 2020 4966 2060 6054            If ``T
-00012010: 7275 6560 602c 2074 6865 206d 6573 7361  rue``, the messa
-00012020: 6765 2077 696c 6c20 6265 2073 656e 7420  ge will be sent 
-00012030: 6173 2061 2072 6570 6c79 2074 6f20 7468  as a reply to th
-00012040: 6973 206d 6573 7361 6765 2e0d 0a20 2020  is message...   
-00012050: 2020 2020 2020 2020 2020 2020 2049 6620               If 
-00012060: 2a72 6570 6c79 5f74 6f5f 6d65 7373 6167  *reply_to_messag
-00012070: 655f 6964 2a20 6973 2070 6173 7365 642c  e_id* is passed,
-00012080: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
-00012090: 7769 6c6c 2062 6520 6967 6e6f 7265 642e  will be ignored.
-000120a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000120b0: 2020 4465 6661 756c 7473 2074 6f20 6060    Defaults to ``
-000120c0: 5472 7565 6060 2069 6e20 6772 6f75 7020  True`` in group 
-000120d0: 6368 6174 7320 616e 6420 6060 4661 6c73  chats and ``Fals
-000120e0: 6560 6020 696e 2070 7269 7661 7465 2063  e`` in private c
-000120f0: 6861 7473 2e0d 0a0d 0a20 2020 2020 2020  hats.....       
-00012100: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
-00012110: 6966 6963 6174 696f 6e20 2860 6062 6f6f  ification (``boo
-00012120: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
-00012130: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012140: 2020 2053 656e 6473 2074 6865 206d 6573     Sends the mes
-00012150: 7361 6765 2073 696c 656e 746c 792e 0d0a  sage silently...
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 5573 6572 7320 7769 6c6c 2072 6563 6569  Users will recei
-00012180: 7665 2061 206e 6f74 6966 6963 6174 696f  ve a notificatio
-00012190: 6e20 7769 7468 206e 6f20 736f 756e 642e  n with no sound.
-000121a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000121b0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-000121c0: 5f69 6420 2860 6062 6f6f 6c60 602c 202a  _id (``bool``, *
-000121d0: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
-000121e0: 2020 2020 2020 2020 2020 2020 2049 6620               If 
-000121f0: 7468 6520 6d65 7373 6167 6520 6973 2061  the message is a
-00012200: 2072 6570 6c79 2c20 4944 206f 6620 7468   reply, ID of th
-00012210: 6520 6f72 6967 696e 616c 206d 6573 7361  e original messa
-00012220: 6765 2e0d 0a0d 0a20 2020 2020 2020 2052  ge.....        R
-00012230: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00012240: 2020 2020 204f 6e20 7375 6363 6573 732c       On success,
-00012250: 2074 6865 2073 656e 7420 4d65 7373 6167   the sent Messag
-00012260: 6520 6973 2072 6574 7572 6e65 642e 0d0a  e is returned...
-00012270: 0d0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00012280: 3a0d 0a20 2020 2020 2020 2020 2020 2052  :..            R
-00012290: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
-000122a0: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
-000122b0: 5043 2065 7272 6f72 2e0d 0a20 2020 2020  PC error...     
-000122c0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000122d0: 6966 2071 756f 7465 2069 7320 4e6f 6e65  if quote is None
-000122e0: 3a0d 0a20 2020 2020 2020 2020 2020 2071  :..            q
-000122f0: 756f 7465 203d 2073 656c 662e 6368 6174  uote = self.chat
-00012300: 2e74 7970 6520 213d 2065 6e75 6d73 2e43  .type != enums.C
-00012310: 6861 7454 7970 652e 5052 4956 4154 450d  hatType.PRIVATE.
-00012320: 0a0d 0a20 2020 2020 2020 2069 6620 7265  ...        if re
-00012330: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00012340: 6420 6973 204e 6f6e 6520 616e 6420 7175  d is None and qu
-00012350: 6f74 653a 0d0a 2020 2020 2020 2020 2020  ote:..          
-00012360: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00012370: 6765 5f69 6420 3d20 7365 6c66 2e69 640d  ge_id = self.id.
-00012380: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00012390: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-000123a0: 6965 6e74 2e73 656e 645f 696e 6c69 6e65  ient.send_inline
-000123b0: 5f62 6f74 5f72 6573 756c 7428 0d0a 2020  _bot_result(..  
-000123c0: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
-000123d0: 643d 7365 6c66 2e63 6861 742e 6964 2c0d  d=self.chat.id,.
-000123e0: 0a20 2020 2020 2020 2020 2020 2071 7565  .            que
-000123f0: 7279 5f69 643d 7175 6572 795f 6964 2c0d  ry_id=query_id,.
-00012400: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00012410: 756c 745f 6964 3d72 6573 756c 745f 6964  ult_id=result_id
-00012420: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-00012430: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-00012440: 696f 6e3d 6469 7361 626c 655f 6e6f 7469  ion=disable_noti
-00012450: 6669 6361 7469 6f6e 2c0d 0a20 2020 2020  fication,..     
-00012460: 2020 2020 2020 2072 6570 6c79 5f74 6f5f         reply_to_
-00012470: 6d65 7373 6167 655f 6964 3d72 6570 6c79  message_id=reply
-00012480: 5f74 6f5f 6d65 7373 6167 655f 6964 0d0a  _to_message_id..
-00012490: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-000124a0: 2061 7379 6e63 2064 6566 2072 6570 6c79   async def reply
-000124b0: 5f6c 6f63 6174 696f 6e28 0d0a 2020 2020  _location(..    
-000124c0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-000124d0: 2020 206c 6174 6974 7564 653a 2066 6c6f     latitude: flo
-000124e0: 6174 2c0d 0a20 2020 2020 2020 206c 6f6e  at,..        lon
-000124f0: 6769 7475 6465 3a20 666c 6f61 742c 0d0a  gitude: float,..
-00012500: 2020 2020 2020 2020 7175 6f74 653a 2062          quote: b
-00012510: 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20 2020  ool = None,..   
-00012520: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
-00012530: 6966 6963 6174 696f 6e3a 2062 6f6f 6c20  ification: bool 
-00012540: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-00012550: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
-00012560: 655f 6964 3a20 696e 7420 3d20 4e6f 6e65  e_id: int = None
-00012570: 2c0d 0a20 2020 2020 2020 2072 6570 6c79  ,..        reply
-00012580: 5f6d 6172 6b75 703a 2055 6e69 6f6e 5b0d  _markup: Union[.
-00012590: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-000125a0: 7065 732e 496e 6c69 6e65 4b65 7962 6f61  pes.InlineKeyboa
-000125b0: 7264 4d61 726b 7570 222c 0d0a 2020 2020  rdMarkup",..    
-000125c0: 2020 2020 2020 2020 2274 7970 6573 2e52          "types.R
-000125d0: 6570 6c79 4b65 7962 6f61 7264 4d61 726b  eplyKeyboardMark
-000125e0: 7570 222c 0d0a 2020 2020 2020 2020 2020  up",..          
-000125f0: 2020 2274 7970 6573 2e52 6570 6c79 4b65    "types.ReplyKe
-00012600: 7962 6f61 7264 5265 6d6f 7665 222c 0d0a  yboardRemove",..
-00012610: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00012620: 6573 2e46 6f72 6365 5265 706c 7922 0d0a  es.ForceReply"..
-00012630: 2020 2020 2020 2020 5d20 3d20 4e6f 6e65          ] = None
-00012640: 0d0a 2020 2020 2920 2d3e 2022 4d65 7373  ..    ) -> "Mess
-00012650: 6167 6522 3a0d 0a20 2020 2020 2020 2022  age":..        "
-00012660: 2222 426f 756e 6420 6d65 7468 6f64 202a  ""Bound method *
-00012670: 7265 706c 795f 6c6f 6361 7469 6f6e 2a20  reply_location* 
-00012680: 6f66 203a 6f62 6a3a 607e 6669 7070 6572  of :obj:`~fipper
-00012690: 2e74 7970 6573 2e4d 6573 7361 6765 602e  .types.Message`.
-000126a0: 0d0a 0d0a 2020 2020 2020 2020 5573 6520  ....        Use 
-000126b0: 6173 2061 2073 686f 7274 6375 7420 666f  as a shortcut fo
-000126c0: 723a 0d0a 0d0a 2020 2020 2020 2020 2e2e  r:....        ..
-000126d0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-000126e0: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
-000126f0: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
-00012700: 2e73 656e 645f 6c6f 6361 7469 6f6e 280d  .send_location(.
-00012710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012720: 2063 6861 745f 6964 3d6d 6573 7361 6765   chat_id=message
-00012730: 2e63 6861 742e 6964 2c0d 0a20 2020 2020  .chat.id,..     
-00012740: 2020 2020 2020 2020 2020 206c 6174 6974             latit
-00012750: 7564 653d 6c61 7469 7475 6465 2c0d 0a20  ude=latitude,.. 
-00012760: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00012770: 6f6e 6769 7475 6465 3d6c 6f6e 6769 7475  ongitude=longitu
-00012780: 6465 0d0a 2020 2020 2020 2020 2020 2020  de..            
-00012790: 290d 0a0d 0a20 2020 2020 2020 2045 7861  )....        Exa
-000127a0: 6d70 6c65 3a0d 0a20 2020 2020 2020 2020  mple:..         
-000127b0: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-000127c0: 3a3a 2070 7974 686f 6e0d 0a0d 0a20 2020  :: python....   
-000127d0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-000127e0: 6974 206d 6573 7361 6765 2e72 6570 6c79  it message.reply
-000127f0: 5f6c 6f63 6174 696f 6e28 6c61 7469 7475  _location(latitu
-00012800: 6465 2c20 6c6f 6e67 6974 7564 6529 0d0a  de, longitude)..
-00012810: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00012820: 7465 7273 3a0d 0a20 2020 2020 2020 2020  ters:..         
-00012830: 2020 206c 6174 6974 7564 6520 2860 6066     latitude (``f
-00012840: 6c6f 6174 6060 293a 0d0a 2020 2020 2020  loat``):..      
-00012850: 2020 2020 2020 2020 2020 4c61 7469 7475            Latitu
-00012860: 6465 206f 6620 7468 6520 6c6f 6361 7469  de of the locati
-00012870: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 2020  on.....         
-00012880: 2020 206c 6f6e 6769 7475 6465 2028 6060     longitude (``
-00012890: 666c 6f61 7460 6029 3a0d 0a20 2020 2020  float``):..     
-000128a0: 2020 2020 2020 2020 2020 204c 6f6e 6769             Longi
-000128b0: 7475 6465 206f 6620 7468 6520 6c6f 6361  tude of the loca
-000128c0: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
-000128d0: 2020 2020 2071 756f 7465 2028 6060 626f       quote (``bo
-000128e0: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
-000128f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00012900: 2020 2020 4966 2060 6054 7275 6560 602c      If ``True``,
-00012910: 2074 6865 206d 6573 7361 6765 2077 696c   the message wil
-00012920: 6c20 6265 2073 656e 7420 6173 2061 2072  l be sent as a r
-00012930: 6570 6c79 2074 6f20 7468 6973 206d 6573  eply to this mes
-00012940: 7361 6765 2e0d 0a20 2020 2020 2020 2020  sage...         
-00012950: 2020 2020 2020 2049 6620 2a72 6570 6c79         If *reply
-00012960: 5f74 6f5f 6d65 7373 6167 655f 6964 2a20  _to_message_id* 
-00012970: 6973 2070 6173 7365 642c 2074 6869 7320  is passed, this 
-00012980: 7061 7261 6d65 7465 7220 7769 6c6c 2062  parameter will b
-00012990: 6520 6967 6e6f 7265 642e 0d0a 2020 2020  e ignored...    
-000129a0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-000129b0: 756c 7473 2074 6f20 6060 5472 7565 6060  ults to ``True``
-000129c0: 2069 6e20 6772 6f75 7020 6368 6174 7320   in group chats 
-000129d0: 616e 6420 6060 4661 6c73 6560 6020 696e  and ``False`` in
-000129e0: 2070 7269 7661 7465 2063 6861 7473 2e0d   private chats..
-000129f0: 0a0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
-00012a00: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-00012a10: 696f 6e20 2860 6062 6f6f 6c60 602c 202a  ion (``bool``, *
-00012a20: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
-00012a30: 2020 2020 2020 2020 2020 2020 2053 656e               Sen
-00012a40: 6473 2074 6865 206d 6573 7361 6765 2073  ds the message s
-00012a50: 696c 656e 746c 792e 0d0a 2020 2020 2020  ilently...      
-00012a60: 2020 2020 2020 2020 2020 5573 6572 7320            Users 
-00012a70: 7769 6c6c 2072 6563 6569 7665 2061 206e  will receive a n
-00012a80: 6f74 6966 6963 6174 696f 6e20 7769 7468  otification with
-00012a90: 206e 6f20 736f 756e 642e 0d0a 0d0a 2020   no sound.....  
-00012aa0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00012ab0: 746f 5f6d 6573 7361 6765 5f69 6420 2860  to_message_id (`
-00012ac0: 6069 6e74 6060 2c20 2a6f 7074 696f 6e61  `int``, *optiona
-00012ad0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-00012ae0: 2020 2020 2020 4966 2074 6865 206d 6573        If the mes
-00012af0: 7361 6765 2069 7320 6120 7265 706c 792c  sage is a reply,
-00012b00: 2049 4420 6f66 2074 6865 206f 7269 6769   ID of the origi
-00012b10: 6e61 6c20 6d65 7373 6167 650d 0a0d 0a20  nal message.... 
-00012b20: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-00012b30: 5f6d 6172 6b75 7020 283a 6f62 6a3a 607e  _markup (:obj:`~
-00012b40: 6669 7070 6572 2e74 7970 6573 2e49 6e6c  fipper.types.Inl
-00012b50: 696e 654b 6579 626f 6172 644d 6172 6b75  ineKeyboardMarku
-00012b60: 7060 207c 203a 6f62 6a3a 607e 6669 7070  p` | :obj:`~fipp
-00012b70: 6572 2e74 7970 6573 2e52 6570 6c79 4b65  er.types.ReplyKe
-00012b80: 7962 6f61 7264 4d61 726b 7570 6020 7c20  yboardMarkup` | 
-00012b90: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
-00012ba0: 7065 732e 5265 706c 794b 6579 626f 6172  pes.ReplyKeyboar
-00012bb0: 6452 656d 6f76 6560 207c 203a 6f62 6a3a  dRemove` | :obj:
-00012bc0: 607e 6669 7070 6572 2e74 7970 6573 2e46  `~fipper.types.F
-00012bd0: 6f72 6365 5265 706c 7960 2c20 2a6f 7074  orceReply`, *opt
-00012be0: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
-00012bf0: 2020 2020 2020 2020 2020 4164 6469 7469            Additi
-00012c00: 6f6e 616c 2069 6e74 6572 6661 6365 206f  onal interface o
-00012c10: 7074 696f 6e73 2e20 416e 206f 626a 6563  ptions. An objec
-00012c20: 7420 666f 7220 616e 2069 6e6c 696e 6520  t for an inline 
-00012c30: 6b65 7962 6f61 7264 2c20 6375 7374 6f6d  keyboard, custom
-00012c40: 2072 6570 6c79 206b 6579 626f 6172 642c   reply keyboard,
-00012c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012c60: 2020 696e 7374 7275 6374 696f 6e73 2074    instructions t
-00012c70: 6f20 7265 6d6f 7665 2072 6570 6c79 206b  o remove reply k
-00012c80: 6579 626f 6172 6420 6f72 2074 6f20 666f  eyboard or to fo
-00012c90: 7263 6520 6120 7265 706c 7920 6672 6f6d  rce a reply from
-00012ca0: 2074 6865 2075 7365 722e 0d0a 0d0a 2020   the user.....  
-00012cb0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00012cc0: 2020 2020 2020 2020 2020 2020 4f6e 2073              On s
-00012cd0: 7563 6365 7373 2c20 7468 6520 7365 6e74  uccess, the sent
-00012ce0: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
-00012cf0: 7970 6573 2e4d 6573 7361 6765 6020 6973  ypes.Message` is
-00012d00: 2072 6574 7572 6e65 642e 0d0a 0d0a 2020   returned.....  
-00012d10: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
-00012d20: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
-00012d30: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
-00012d40: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
-00012d50: 7272 6f72 2e0d 0a20 2020 2020 2020 2022  rror...        "
-00012d60: 2222 0d0a 2020 2020 2020 2020 6966 2071  ""..        if q
-00012d70: 756f 7465 2069 7320 4e6f 6e65 3a0d 0a20  uote is None:.. 
-00012d80: 2020 2020 2020 2020 2020 2071 756f 7465             quote
-00012d90: 203d 2073 656c 662e 6368 6174 2e74 7970   = self.chat.typ
-00012da0: 6520 213d 2065 6e75 6d73 2e43 6861 7454  e != enums.ChatT
-00012db0: 7970 652e 5052 4956 4154 450d 0a0d 0a20  ype.PRIVATE.... 
-00012dc0: 2020 2020 2020 2069 6620 7265 706c 795f         if reply_
-00012dd0: 746f 5f6d 6573 7361 6765 5f69 6420 6973  to_message_id is
-00012de0: 204e 6f6e 6520 616e 6420 7175 6f74 653a   None and quote:
-00012df0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00012e00: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00012e10: 6420 3d20 7365 6c66 2e69 640d 0a0d 0a20  d = self.id.... 
-00012e20: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-00012e30: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
-00012e40: 2e73 656e 645f 6c6f 6361 7469 6f6e 280d  .send_location(.
-00012e50: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
-00012e60: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
-00012e70: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-00012e80: 6c61 7469 7475 6465 3d6c 6174 6974 7564  latitude=latitud
-00012e90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00012ea0: 6c6f 6e67 6974 7564 653d 6c6f 6e67 6974  longitude=longit
-00012eb0: 7564 652c 0d0a 2020 2020 2020 2020 2020  ude,..          
-00012ec0: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
-00012ed0: 6361 7469 6f6e 3d64 6973 6162 6c65 5f6e  cation=disable_n
-00012ee0: 6f74 6966 6963 6174 696f 6e2c 0d0a 2020  otification,..  
-00012ef0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00012f00: 746f 5f6d 6573 7361 6765 5f69 643d 7265  to_message_id=re
-00012f10: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00012f20: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-00012f30: 7265 706c 795f 6d61 726b 7570 3d72 6570  reply_markup=rep
-00012f40: 6c79 5f6d 6172 6b75 700d 0a20 2020 2020  ly_markup..     
-00012f50: 2020 2029 0d0a 0d0a 2020 2020 6173 796e     )....    asyn
-00012f60: 6320 6465 6620 7265 706c 795f 6d65 6469  c def reply_medi
-00012f70: 615f 6772 6f75 7028 0d0a 2020 2020 2020  a_group(..      
-00012f80: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00012f90: 206d 6564 6961 3a20 4c69 7374 5b55 6e69   media: List[Uni
-00012fa0: 6f6e 5b22 7479 7065 732e 496e 7075 744d  on["types.InputM
-00012fb0: 6564 6961 5068 6f74 6f22 2c20 2274 7970  ediaPhoto", "typ
-00012fc0: 6573 2e49 6e70 7574 4d65 6469 6156 6964  es.InputMediaVid
-00012fd0: 656f 225d 5d2c 0d0a 2020 2020 2020 2020  eo"]],..        
-00012fe0: 7175 6f74 653a 2062 6f6f 6c20 3d20 4e6f  quote: bool = No
-00012ff0: 6e65 2c0d 0a20 2020 2020 2020 2064 6973  ne,..        dis
-00013000: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00013010: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d  n: bool = None,.
-00013020: 0a20 2020 2020 2020 2072 6570 6c79 5f74  .        reply_t
-00013030: 6f5f 6d65 7373 6167 655f 6964 3a20 696e  o_message_id: in
-00013040: 7420 3d20 4e6f 6e65 0d0a 2020 2020 2920  t = None..    ) 
-00013050: 2d3e 204c 6973 745b 2274 7970 6573 2e4d  -> List["types.M
-00013060: 6573 7361 6765 225d 3a0d 0a20 2020 2020  essage"]:..     
-00013070: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
-00013080: 6f64 202a 7265 706c 795f 6d65 6469 615f  od *reply_media_
-00013090: 6772 6f75 702a 206f 6620 3a6f 626a 3a60  group* of :obj:`
-000130a0: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
-000130b0: 7373 6167 6560 2e0d 0a0d 0a20 2020 2020  ssage`.....     
-000130c0: 2020 2055 7365 2061 7320 6120 7368 6f72     Use as a shor
-000130d0: 7463 7574 2066 6f72 3a0d 0a0d 0a20 2020  tcut for:....   
-000130e0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-000130f0: 636b 3a3a 2070 7974 686f 6e0d 0a0d 0a20  ck:: python.... 
-00013100: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00013110: 2063 6c69 656e 742e 7365 6e64 5f6d 6564   client.send_med
-00013120: 6961 5f67 726f 7570 280d 0a20 2020 2020  ia_group(..     
-00013130: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00013140: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
-00013150: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-00013160: 2020 2020 206d 6564 6961 3d6c 6973 745f       media=list_
-00013170: 6f66 5f6d 6564 6961 0d0a 2020 2020 2020  of_media..      
-00013180: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
-00013190: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
-000131a0: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
-000131b0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
-000131c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000131d0: 2020 2061 7761 6974 206d 6573 7361 6765     await message
-000131e0: 2e72 6570 6c79 5f6d 6564 6961 5f67 726f  .reply_media_gro
-000131f0: 7570 286c 6973 745f 6f66 5f6d 6564 6961  up(list_of_media
-00013200: 290d 0a0d 0a20 2020 2020 2020 2050 6172  )....        Par
-00013210: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
-00013220: 2020 2020 2020 6d65 6469 6120 2860 606c        media (``l
-00013230: 6973 7460 6029 3a0d 0a20 2020 2020 2020  ist``):..       
-00013240: 2020 2020 2020 2020 2041 206c 6973 7420           A list 
-00013250: 636f 6e74 6169 6e69 6e67 2065 6974 6865  containing eithe
-00013260: 7220 3a6f 626a 3a60 7e66 6970 7065 722e  r :obj:`~fipper.
-00013270: 7479 7065 732e 496e 7075 744d 6564 6961  types.InputMedia
-00013280: 5068 6f74 6f60 206f 720d 0a20 2020 2020  Photo` or..     
-00013290: 2020 2020 2020 2020 2020 203a 6f62 6a3a             :obj:
-000132a0: 607e 6669 7070 6572 2e74 7970 6573 2e49  `~fipper.types.I
-000132b0: 6e70 7574 4d65 6469 6156 6964 656f 6020  nputMediaVideo` 
-000132c0: 6f62 6a65 6374 730d 0a20 2020 2020 2020  objects..       
-000132d0: 2020 2020 2020 2020 2064 6573 6372 6962           describ
-000132e0: 696e 6720 7068 6f74 6f73 2061 6e64 2076  ing photos and v
-000132f0: 6964 656f 7320 746f 2062 6520 7365 6e74  ideos to be sent
-00013300: 2c20 6d75 7374 2069 6e63 6c75 6465 2032  , must include 2
-00013310: e280 9331 3020 6974 656d 732e 0d0a 0d0a  ...10 items.....
-00013320: 2020 2020 2020 2020 2020 2020 7175 6f74              quot
-00013330: 6520 2860 6062 6f6f 6c60 602c 202a 6f70  e (``bool``, *op
-00013340: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-00013350: 2020 2020 2020 2020 2020 2049 6620 6060             If ``
-00013360: 5472 7565 6060 2c20 7468 6520 6d65 7373  True``, the mess
-00013370: 6167 6520 7769 6c6c 2062 6520 7365 6e74  age will be sent
-00013380: 2061 7320 6120 7265 706c 7920 746f 2074   as a reply to t
-00013390: 6869 7320 6d65 7373 6167 652e 0d0a 2020  his message...  
-000133a0: 2020 2020 2020 2020 2020 2020 2020 4966                If
-000133b0: 202a 7265 706c 795f 746f 5f6d 6573 7361   *reply_to_messa
-000133c0: 6765 5f69 642a 2069 7320 7061 7373 6564  ge_id* is passed
-000133d0: 2c20 7468 6973 2070 6172 616d 6574 6572  , this parameter
-000133e0: 2077 696c 6c20 6265 2069 676e 6f72 6564   will be ignored
-000133f0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00013400: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
-00013410: 6054 7275 6560 6020 696e 2067 726f 7570  `True`` in group
-00013420: 2063 6861 7473 2061 6e64 2060 6046 616c   chats and ``Fal
-00013430: 7365 6060 2069 6e20 7072 6976 6174 6520  se`` in private 
-00013440: 6368 6174 732e 0d0a 0d0a 2020 2020 2020  chats.....      
-00013450: 2020 2020 2020 6469 7361 626c 655f 6e6f        disable_no
-00013460: 7469 6669 6361 7469 6f6e 2028 6060 626f  tification (``bo
-00013470: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
-00013480: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00013490: 2020 2020 5365 6e64 7320 7468 6520 6d65      Sends the me
-000134a0: 7373 6167 6520 7369 6c65 6e74 6c79 2e0d  ssage silently..
-000134b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000134c0: 2055 7365 7273 2077 696c 6c20 7265 6365   Users will rece
-000134d0: 6976 6520 6120 6e6f 7469 6669 6361 7469  ive a notificati
-000134e0: 6f6e 2077 6974 6820 6e6f 2073 6f75 6e64  on with no sound
+00011d00: 7420 3d20 4e6f 6e65 2c0d 0a20 2020 2020  t = None,..     
+00011d10: 2020 2068 6964 655f 7669 613a 2062 6f6f     hide_via: boo
+00011d20: 6c20 3d20 4e6f 6e65 0d0a 2020 2020 2920  l = None..    ) 
+00011d30: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
+00011d40: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
+00011d50: 6d65 7468 6f64 202a 7265 706c 795f 696e  method *reply_in
+00011d60: 6c69 6e65 5f62 6f74 5f72 6573 756c 742a  line_bot_result*
+00011d70: 206f 6620 3a6f 626a 3a60 7e66 6970 7065   of :obj:`~fippe
+00011d80: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
+00011d90: 2e0d 0a0d 0a20 2020 2020 2020 2055 7365  .....        Use
+00011da0: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
+00011db0: 6f72 3a0d 0a0d 0a20 2020 2020 2020 202e  or:....        .
+00011dc0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+00011dd0: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
+00011de0: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
+00011df0: 742e 7365 6e64 5f69 6e6c 696e 655f 626f  t.send_inline_bo
+00011e00: 745f 7265 7375 6c74 280d 0a20 2020 2020  t_result(..     
+00011e10: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00011e20: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
+00011e30: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+00011e40: 2020 2020 2071 7565 7279 5f69 643d 7175       query_id=qu
+00011e50: 6572 795f 6964 2c0d 0a20 2020 2020 2020  ery_id,..       
+00011e60: 2020 2020 2020 2020 2072 6573 756c 745f           result_
+00011e70: 6964 3d72 6573 756c 745f 6964 0d0a 2020  id=result_id..  
+00011e80: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+00011e90: 2020 2020 2020 2045 7861 6d70 6c65 3a0d         Example:.
+00011ea0: 0a20 2020 2020 2020 2020 2020 202e 2e20  .            .. 
+00011eb0: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00011ec0: 686f 6e0d 0a0d 0a20 2020 2020 2020 2020  hon....         
+00011ed0: 2020 2020 2020 2061 7761 6974 206d 6573         await mes
+00011ee0: 7361 6765 2e72 6570 6c79 5f69 6e6c 696e  sage.reply_inlin
+00011ef0: 655f 626f 745f 7265 7375 6c74 2871 7565  e_bot_result(que
+00011f00: 7279 5f69 642c 2072 6573 756c 745f 6964  ry_id, result_id
+00011f10: 290d 0a0d 0a20 2020 2020 2020 2050 6172  )....        Par
+00011f20: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+00011f30: 2020 2020 2020 7175 6572 795f 6964 2028        query_id (
+00011f40: 6060 696e 7460 6029 3a0d 0a20 2020 2020  ``int``):..     
+00011f50: 2020 2020 2020 2020 2020 2055 6e69 7175             Uniqu
+00011f60: 6520 6964 656e 7469 6669 6572 2066 6f72  e identifier for
+00011f70: 2074 6865 2061 6e73 7765 7265 6420 7175   the answered qu
+00011f80: 6572 792e 0d0a 0d0a 2020 2020 2020 2020  ery.....        
+00011f90: 2020 2020 7265 7375 6c74 5f69 6420 2860      result_id (`
+00011fa0: 6073 7472 6060 293a 0d0a 2020 2020 2020  `str``):..      
+00011fb0: 2020 2020 2020 2020 2020 556e 6971 7565            Unique
+00011fc0: 2069 6465 6e74 6966 6965 7220 666f 7220   identifier for 
+00011fd0: 7468 6520 7265 7375 6c74 2074 6861 7420  the result that 
+00011fe0: 7761 7320 6368 6f73 656e 2e0d 0a0d 0a20  was chosen..... 
+00011ff0: 2020 2020 2020 2020 2020 2071 756f 7465             quote
+00012000: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+00012010: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+00012020: 2020 2020 2020 2020 2020 4966 2060 6054            If ``T
+00012030: 7275 6560 602c 2074 6865 206d 6573 7361  rue``, the messa
+00012040: 6765 2077 696c 6c20 6265 2073 656e 7420  ge will be sent 
+00012050: 6173 2061 2072 6570 6c79 2074 6f20 7468  as a reply to th
+00012060: 6973 206d 6573 7361 6765 2e0d 0a20 2020  is message...   
+00012070: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+00012080: 2a72 6570 6c79 5f74 6f5f 6d65 7373 6167  *reply_to_messag
+00012090: 655f 6964 2a20 6973 2070 6173 7365 642c  e_id* is passed,
+000120a0: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
+000120b0: 7769 6c6c 2062 6520 6967 6e6f 7265 642e  will be ignored.
+000120c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000120d0: 2020 4465 6661 756c 7473 2074 6f20 6060    Defaults to ``
+000120e0: 5472 7565 6060 2069 6e20 6772 6f75 7020  True`` in group 
+000120f0: 6368 6174 7320 616e 6420 6060 4661 6c73  chats and ``Fals
+00012100: 6560 6020 696e 2070 7269 7661 7465 2063  e`` in private c
+00012110: 6861 7473 2e0d 0a0d 0a20 2020 2020 2020  hats.....       
+00012120: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+00012130: 6966 6963 6174 696f 6e20 2860 6062 6f6f  ification (``boo
+00012140: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
+00012150: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012160: 2020 2053 656e 6473 2074 6865 206d 6573     Sends the mes
+00012170: 7361 6765 2073 696c 656e 746c 792e 0d0a  sage silently...
+00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 5573 6572 7320 7769 6c6c 2072 6563 6569  Users will recei
+000121a0: 7665 2061 206e 6f74 6966 6963 6174 696f  ve a notificatio
+000121b0: 6e20 7769 7468 206e 6f20 736f 756e 642e  n with no sound.
+000121c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000121d0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+000121e0: 5f69 6420 2860 6062 6f6f 6c60 602c 202a  _id (``bool``, *
+000121f0: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
+00012200: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+00012210: 7468 6520 6d65 7373 6167 6520 6973 2061  the message is a
+00012220: 2072 6570 6c79 2c20 4944 206f 6620 7468   reply, ID of th
+00012230: 6520 6f72 6967 696e 616c 206d 6573 7361  e original messa
+00012240: 6765 2e0d 0a20 2020 2020 2020 2020 2020  ge...           
+00012250: 200d 0a20 2020 2020 2020 2020 2020 2068   ..            h
+00012260: 6964 655f 7669 6120 2860 6062 6f6f 6c60  ide_via (``bool`
+00012270: 6029 3a0d 0a20 2020 2020 2020 2020 2020  `):..           
+00012280: 2020 2020 2053 656e 6473 2074 6865 206d       Sends the m
+00012290: 6573 7361 6765 2077 6974 6820 2a76 6961  essage with *via
+000122a0: 2040 626f 742a 2068 6964 6465 6e2e 0d0a   @bot* hidden...
+000122b0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000122c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000122d0: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
+000122e0: 7365 6e74 204d 6573 7361 6765 2069 7320  sent Message is 
+000122f0: 7265 7475 726e 6564 2e0d 0a0d 0a20 2020  returned.....   
+00012300: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
+00012310: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
+00012320: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
+00012330: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
+00012340: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
+00012350: 220d 0a20 2020 2020 2020 2069 6620 7175  "..        if qu
+00012360: 6f74 6520 6973 204e 6f6e 653a 0d0a 2020  ote is None:..  
+00012370: 2020 2020 2020 2020 2020 7175 6f74 6520            quote 
+00012380: 3d20 7365 6c66 2e63 6861 742e 7479 7065  = self.chat.type
+00012390: 2021 3d20 656e 756d 732e 4368 6174 5479   != enums.ChatTy
+000123a0: 7065 2e50 5249 5641 5445 0d0a 0d0a 2020  pe.PRIVATE....  
+000123b0: 2020 2020 2020 6966 2072 6570 6c79 5f74        if reply_t
+000123c0: 6f5f 6d65 7373 6167 655f 6964 2069 7320  o_message_id is 
+000123d0: 4e6f 6e65 2061 6e64 2071 756f 7465 3a0d  None and quote:.
+000123e0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+000123f0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+00012400: 203d 2073 656c 662e 6964 0d0a 0d0a 2020   = self.id....  
+00012410: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00012420: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+00012430: 7365 6e64 5f69 6e6c 696e 655f 626f 745f  send_inline_bot_
+00012440: 7265 7375 6c74 280d 0a20 2020 2020 2020  result(..       
+00012450: 2020 2020 2063 6861 745f 6964 3d73 656c       chat_id=sel
+00012460: 662e 6368 6174 2e69 642c 0d0a 2020 2020  f.chat.id,..    
+00012470: 2020 2020 2020 2020 7175 6572 795f 6964          query_id
+00012480: 3d71 7565 7279 5f69 642c 0d0a 2020 2020  =query_id,..    
+00012490: 2020 2020 2020 2020 7265 7375 6c74 5f69          result_i
+000124a0: 643d 7265 7375 6c74 5f69 642c 0d0a 2020  d=result_id,..  
+000124b0: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+000124c0: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
+000124d0: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+000124e0: 696f 6e2c 0d0a 2020 2020 2020 2020 2020  ion,..          
+000124f0: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
+00012500: 6765 5f69 643d 7265 706c 795f 746f 5f6d  ge_id=reply_to_m
+00012510: 6573 7361 6765 5f69 642c 0d0a 2020 2020  essage_id,..    
+00012520: 2020 2020 2020 2020 6869 6465 5f76 6961          hide_via
+00012530: 3d68 6964 655f 7669 610d 0a20 2020 2020  =hide_via..     
+00012540: 2020 2029 0d0a 0d0a 2020 2020 6173 796e     )....    asyn
+00012550: 6320 6465 6620 7265 706c 795f 6c6f 6361  c def reply_loca
+00012560: 7469 6f6e 280d 0a20 2020 2020 2020 2073  tion(..        s
+00012570: 656c 662c 0d0a 2020 2020 2020 2020 6c61  elf,..        la
+00012580: 7469 7475 6465 3a20 666c 6f61 742c 0d0a  titude: float,..
+00012590: 2020 2020 2020 2020 6c6f 6e67 6974 7564          longitud
+000125a0: 653a 2066 6c6f 6174 2c0d 0a20 2020 2020  e: float,..     
+000125b0: 2020 2071 756f 7465 3a20 626f 6f6c 203d     quote: bool =
+000125c0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000125d0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+000125e0: 7469 6f6e 3a20 626f 6f6c 203d 204e 6f6e  tion: bool = Non
+000125f0: 652c 0d0a 2020 2020 2020 2020 7265 706c  e,..        repl
+00012600: 795f 746f 5f6d 6573 7361 6765 5f69 643a  y_to_message_id:
+00012610: 2069 6e74 203d 204e 6f6e 652c 0d0a 2020   int = None,..  
+00012620: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+00012630: 7570 3a20 556e 696f 6e5b 0d0a 2020 2020  up: Union[..    
+00012640: 2020 2020 2020 2020 2274 7970 6573 2e49          "types.I
+00012650: 6e6c 696e 654b 6579 626f 6172 644d 6172  nlineKeyboardMar
+00012660: 6b75 7022 2c0d 0a20 2020 2020 2020 2020  kup",..         
+00012670: 2020 2022 7479 7065 732e 5265 706c 794b     "types.ReplyK
+00012680: 6579 626f 6172 644d 6172 6b75 7022 2c0d  eyboardMarkup",.
+00012690: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+000126a0: 7065 732e 5265 706c 794b 6579 626f 6172  pes.ReplyKeyboar
+000126b0: 6452 656d 6f76 6522 2c0d 0a20 2020 2020  dRemove",..     
+000126c0: 2020 2020 2020 2022 7479 7065 732e 466f         "types.Fo
+000126d0: 7263 6552 6570 6c79 220d 0a20 2020 2020  rceReply"..     
+000126e0: 2020 205d 203d 204e 6f6e 650d 0a20 2020     ] = None..   
+000126f0: 2029 202d 3e20 224d 6573 7361 6765 223a   ) -> "Message":
+00012700: 0d0a 2020 2020 2020 2020 2222 2242 6f75  ..        """Bou
+00012710: 6e64 206d 6574 686f 6420 2a72 6570 6c79  nd method *reply
+00012720: 5f6c 6f63 6174 696f 6e2a 206f 6620 3a6f  _location* of :o
+00012730: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
+00012740: 732e 4d65 7373 6167 6560 2e0d 0a0d 0a20  s.Message`..... 
+00012750: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
+00012760: 7368 6f72 7463 7574 2066 6f72 3a0d 0a0d  shortcut for:...
+00012770: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
+00012780: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
+00012790: 0a0d 0a20 2020 2020 2020 2020 2020 2061  ...            a
+000127a0: 7761 6974 2063 6c69 656e 742e 7365 6e64  wait client.send
+000127b0: 5f6c 6f63 6174 696f 6e28 0d0a 2020 2020  _location(..    
+000127c0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+000127d0: 5f69 643d 6d65 7373 6167 652e 6368 6174  _id=message.chat
+000127e0: 2e69 642c 0d0a 2020 2020 2020 2020 2020  .id,..          
+000127f0: 2020 2020 2020 6c61 7469 7475 6465 3d6c        latitude=l
+00012800: 6174 6974 7564 652c 0d0a 2020 2020 2020  atitude,..      
+00012810: 2020 2020 2020 2020 2020 6c6f 6e67 6974            longit
+00012820: 7564 653d 6c6f 6e67 6974 7564 650d 0a20  ude=longitude.. 
+00012830: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
+00012840: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+00012850: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
+00012860: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00012870: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
+00012880: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
+00012890: 7373 6167 652e 7265 706c 795f 6c6f 6361  ssage.reply_loca
+000128a0: 7469 6f6e 286c 6174 6974 7564 652c 206c  tion(latitude, l
+000128b0: 6f6e 6769 7475 6465 290d 0a0d 0a20 2020  ongitude)....   
+000128c0: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+000128d0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+000128e0: 7469 7475 6465 2028 6060 666c 6f61 7460  titude (``float`
+000128f0: 6029 3a0d 0a20 2020 2020 2020 2020 2020  `):..           
+00012900: 2020 2020 204c 6174 6974 7564 6520 6f66       Latitude of
+00012910: 2074 6865 206c 6f63 6174 696f 6e2e 0d0a   the location...
+00012920: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00012930: 6e67 6974 7564 6520 2860 6066 6c6f 6174  ngitude (``float
+00012940: 6060 293a 0d0a 2020 2020 2020 2020 2020  ``):..          
+00012950: 2020 2020 2020 4c6f 6e67 6974 7564 6520        Longitude 
+00012960: 6f66 2074 6865 206c 6f63 6174 696f 6e2e  of the location.
+00012970: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00012980: 7175 6f74 6520 2860 6062 6f6f 6c60 602c  quote (``bool``,
+00012990: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
+000129a0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+000129b0: 6620 6060 5472 7565 6060 2c20 7468 6520  f ``True``, the 
+000129c0: 6d65 7373 6167 6520 7769 6c6c 2062 6520  message will be 
+000129d0: 7365 6e74 2061 7320 6120 7265 706c 7920  sent as a reply 
+000129e0: 746f 2074 6869 7320 6d65 7373 6167 652e  to this message.
+000129f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012a00: 2020 4966 202a 7265 706c 795f 746f 5f6d    If *reply_to_m
+00012a10: 6573 7361 6765 5f69 642a 2069 7320 7061  essage_id* is pa
+00012a20: 7373 6564 2c20 7468 6973 2070 6172 616d  ssed, this param
+00012a30: 6574 6572 2077 696c 6c20 6265 2069 676e  eter will be ign
+00012a40: 6f72 6564 2e0d 0a20 2020 2020 2020 2020  ored...         
+00012a50: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00012a60: 746f 2060 6054 7275 6560 6020 696e 2067  to ``True`` in g
+00012a70: 726f 7570 2063 6861 7473 2061 6e64 2060  roup chats and `
+00012a80: 6046 616c 7365 6060 2069 6e20 7072 6976  `False`` in priv
+00012a90: 6174 6520 6368 6174 732e 0d0a 0d0a 2020  ate chats.....  
+00012aa0: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00012ab0: 655f 6e6f 7469 6669 6361 7469 6f6e 2028  e_notification (
+00012ac0: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
+00012ad0: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
+00012ae0: 2020 2020 2020 2020 5365 6e64 7320 7468          Sends th
+00012af0: 6520 6d65 7373 6167 6520 7369 6c65 6e74  e message silent
+00012b00: 6c79 2e0d 0a20 2020 2020 2020 2020 2020  ly...           
+00012b10: 2020 2020 2055 7365 7273 2077 696c 6c20       Users will 
+00012b20: 7265 6365 6976 6520 6120 6e6f 7469 6669  receive a notifi
+00012b30: 6361 7469 6f6e 2077 6974 6820 6e6f 2073  cation with no s
+00012b40: 6f75 6e64 2e0d 0a0d 0a20 2020 2020 2020  ound.....       
+00012b50: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
+00012b60: 7373 6167 655f 6964 2028 6060 696e 7460  ssage_id (``int`
+00012b70: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+00012b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b90: 2049 6620 7468 6520 6d65 7373 6167 6520   If the message 
+00012ba0: 6973 2061 2072 6570 6c79 2c20 4944 206f  is a reply, ID o
+00012bb0: 6620 7468 6520 6f72 6967 696e 616c 206d  f the original m
+00012bc0: 6573 7361 6765 0d0a 0d0a 2020 2020 2020  essage....      
+00012bd0: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+00012be0: 7570 2028 3a6f 626a 3a60 7e66 6970 7065  up (:obj:`~fippe
+00012bf0: 722e 7479 7065 732e 496e 6c69 6e65 4b65  r.types.InlineKe
+00012c00: 7962 6f61 7264 4d61 726b 7570 6020 7c20  yboardMarkup` | 
+00012c10: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
+00012c20: 7065 732e 5265 706c 794b 6579 626f 6172  pes.ReplyKeyboar
+00012c30: 644d 6172 6b75 7060 207c 203a 6f62 6a3a  dMarkup` | :obj:
+00012c40: 607e 6669 7070 6572 2e74 7970 6573 2e52  `~fipper.types.R
+00012c50: 6570 6c79 4b65 7962 6f61 7264 5265 6d6f  eplyKeyboardRemo
+00012c60: 7665 6020 7c20 3a6f 626a 3a60 7e66 6970  ve` | :obj:`~fip
+00012c70: 7065 722e 7479 7065 732e 466f 7263 6552  per.types.ForceR
+00012c80: 6570 6c79 602c 202a 6f70 7469 6f6e 616c  eply`, *optional
+00012c90: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
+00012ca0: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
+00012cb0: 696e 7465 7266 6163 6520 6f70 7469 6f6e  interface option
+00012cc0: 732e 2041 6e20 6f62 6a65 6374 2066 6f72  s. An object for
+00012cd0: 2061 6e20 696e 6c69 6e65 206b 6579 626f   an inline keybo
+00012ce0: 6172 642c 2063 7573 746f 6d20 7265 706c  ard, custom repl
+00012cf0: 7920 6b65 7962 6f61 7264 2c0d 0a20 2020  y keyboard,..   
+00012d00: 2020 2020 2020 2020 2020 2020 2069 6e73               ins
+00012d10: 7472 7563 7469 6f6e 7320 746f 2072 656d  tructions to rem
+00012d20: 6f76 6520 7265 706c 7920 6b65 7962 6f61  ove reply keyboa
+00012d30: 7264 206f 7220 746f 2066 6f72 6365 2061  rd or to force a
+00012d40: 2072 6570 6c79 2066 726f 6d20 7468 6520   reply from the 
+00012d50: 7573 6572 2e0d 0a0d 0a20 2020 2020 2020  user.....       
+00012d60: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00012d70: 2020 2020 2020 204f 6e20 7375 6363 6573         On succes
+00012d80: 732c 2074 6865 2073 656e 7420 3a6f 626a  s, the sent :obj
+00012d90: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
+00012da0: 4d65 7373 6167 6560 2069 7320 7265 7475  Message` is retu
+00012db0: 726e 6564 2e0d 0a0d 0a20 2020 2020 2020  rned.....       
+00012dc0: 2052 6169 7365 733a 0d0a 2020 2020 2020   Raises:..      
+00012dd0: 2020 2020 2020 5250 4345 7272 6f72 3a20        RPCError: 
+00012de0: 496e 2063 6173 6520 6f66 2061 2054 656c  In case of a Tel
+00012df0: 6567 7261 6d20 5250 4320 6572 726f 722e  egram RPC error.
+00012e00: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00012e10: 2020 2020 2020 2069 6620 7175 6f74 6520         if quote 
+00012e20: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00012e30: 2020 2020 2020 7175 6f74 6520 3d20 7365        quote = se
+00012e40: 6c66 2e63 6861 742e 7479 7065 2021 3d20  lf.chat.type != 
+00012e50: 656e 756d 732e 4368 6174 5479 7065 2e50  enums.ChatType.P
+00012e60: 5249 5641 5445 0d0a 0d0a 2020 2020 2020  RIVATE....      
+00012e70: 2020 6966 2072 6570 6c79 5f74 6f5f 6d65    if reply_to_me
+00012e80: 7373 6167 655f 6964 2069 7320 4e6f 6e65  ssage_id is None
+00012e90: 2061 6e64 2071 756f 7465 3a0d 0a20 2020   and quote:..   
+00012ea0: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
+00012eb0: 6f5f 6d65 7373 6167 655f 6964 203d 2073  o_message_id = s
+00012ec0: 656c 662e 6964 0d0a 0d0a 2020 2020 2020  elf.id....      
+00012ed0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+00012ee0: 656c 662e 5f63 6c69 656e 742e 7365 6e64  elf._client.send
+00012ef0: 5f6c 6f63 6174 696f 6e28 0d0a 2020 2020  _location(..    
+00012f00: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+00012f10: 7365 6c66 2e63 6861 742e 6964 2c0d 0a20  self.chat.id,.. 
+00012f20: 2020 2020 2020 2020 2020 206c 6174 6974             latit
+00012f30: 7564 653d 6c61 7469 7475 6465 2c0d 0a20  ude=latitude,.. 
+00012f40: 2020 2020 2020 2020 2020 206c 6f6e 6769             longi
+00012f50: 7475 6465 3d6c 6f6e 6769 7475 6465 2c0d  tude=longitude,.
+00012f60: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00012f70: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00012f80: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
+00012f90: 6361 7469 6f6e 2c0d 0a20 2020 2020 2020  cation,..       
+00012fa0: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
+00012fb0: 7373 6167 655f 6964 3d72 6570 6c79 5f74  ssage_id=reply_t
+00012fc0: 6f5f 6d65 7373 6167 655f 6964 2c0d 0a20  o_message_id,.. 
+00012fd0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+00012fe0: 5f6d 6172 6b75 703d 7265 706c 795f 6d61  _markup=reply_ma
+00012ff0: 726b 7570 0d0a 2020 2020 2020 2020 290d  rkup..        ).
+00013000: 0a0d 0a20 2020 2061 7379 6e63 2064 6566  ...    async def
+00013010: 2072 6570 6c79 5f6d 6564 6961 5f67 726f   reply_media_gro
+00013020: 7570 280d 0a20 2020 2020 2020 2073 656c  up(..        sel
+00013030: 662c 0d0a 2020 2020 2020 2020 6d65 6469  f,..        medi
+00013040: 613a 204c 6973 745b 556e 696f 6e5b 2274  a: List[Union["t
+00013050: 7970 6573 2e49 6e70 7574 4d65 6469 6150  ypes.InputMediaP
+00013060: 686f 746f 222c 2022 7479 7065 732e 496e  hoto", "types.In
+00013070: 7075 744d 6564 6961 5669 6465 6f22 5d5d  putMediaVideo"]]
+00013080: 2c0d 0a20 2020 2020 2020 2071 756f 7465  ,..        quote
+00013090: 3a20 626f 6f6c 203d 204e 6f6e 652c 0d0a  : bool = None,..
+000130a0: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+000130b0: 6e6f 7469 6669 6361 7469 6f6e 3a20 626f  notification: bo
+000130c0: 6f6c 203d 204e 6f6e 652c 0d0a 2020 2020  ol = None,..    
+000130d0: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
+000130e0: 7361 6765 5f69 643a 2069 6e74 203d 204e  sage_id: int = N
+000130f0: 6f6e 650d 0a20 2020 2029 202d 3e20 4c69  one..    ) -> Li
+00013100: 7374 5b22 7479 7065 732e 4d65 7373 6167  st["types.Messag
+00013110: 6522 5d3a 0d0a 2020 2020 2020 2020 2222  e"]:..        ""
+00013120: 2242 6f75 6e64 206d 6574 686f 6420 2a72  "Bound method *r
+00013130: 6570 6c79 5f6d 6564 6961 5f67 726f 7570  eply_media_group
+00013140: 2a20 6f66 203a 6f62 6a3a 607e 6669 7070  * of :obj:`~fipp
+00013150: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
+00013160: 602e 0d0a 0d0a 2020 2020 2020 2020 5573  `.....        Us
+00013170: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
+00013180: 666f 723a 0d0a 0d0a 2020 2020 2020 2020  for:....        
+00013190: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000131a0: 7079 7468 6f6e 0d0a 0d0a 2020 2020 2020  python....      
+000131b0: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
+000131c0: 6e74 2e73 656e 645f 6d65 6469 615f 6772  nt.send_media_gr
+000131d0: 6f75 7028 0d0a 2020 2020 2020 2020 2020  oup(..          
+000131e0: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
+000131f0: 7373 6167 652e 6368 6174 2e69 642c 0d0a  ssage.chat.id,..
+00013200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013210: 6d65 6469 613d 6c69 7374 5f6f 665f 6d65  media=list_of_me
+00013220: 6469 610d 0a20 2020 2020 2020 2020 2020  dia..           
+00013230: 2029 0d0a 0d0a 2020 2020 2020 2020 4578   )....        Ex
+00013240: 616d 706c 653a 0d0a 2020 2020 2020 2020  ample:..        
+00013250: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+00013260: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
+00013270: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+00013280: 6169 7420 6d65 7373 6167 652e 7265 706c  ait message.repl
+00013290: 795f 6d65 6469 615f 6772 6f75 7028 6c69  y_media_group(li
+000132a0: 7374 5f6f 665f 6d65 6469 6129 0d0a 0d0a  st_of_media)....
+000132b0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+000132c0: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
+000132d0: 206d 6564 6961 2028 6060 6c69 7374 6060   media (``list``
+000132e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000132f0: 2020 2020 4120 6c69 7374 2063 6f6e 7461      A list conta
+00013300: 696e 696e 6720 6569 7468 6572 203a 6f62  ining either :ob
+00013310: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+00013320: 2e49 6e70 7574 4d65 6469 6150 686f 746f  .InputMediaPhoto
+00013330: 6020 6f72 0d0a 2020 2020 2020 2020 2020  ` or..          
+00013340: 2020 2020 2020 3a6f 626a 3a60 7e66 6970        :obj:`~fip
+00013350: 7065 722e 7479 7065 732e 496e 7075 744d  per.types.InputM
+00013360: 6564 6961 5669 6465 6f60 206f 626a 6563  ediaVideo` objec
+00013370: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
+00013380: 2020 2020 6465 7363 7269 6269 6e67 2070      describing p
+00013390: 686f 746f 7320 616e 6420 7669 6465 6f73  hotos and videos
+000133a0: 2074 6f20 6265 2073 656e 742c 206d 7573   to be sent, mus
+000133b0: 7420 696e 636c 7564 6520 32e2 8093 3130  t include 2...10
+000133c0: 2069 7465 6d73 2e0d 0a0d 0a20 2020 2020   items.....     
+000133d0: 2020 2020 2020 2071 756f 7465 2028 6060         quote (``
+000133e0: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
+000133f0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+00013400: 2020 2020 2020 4966 2060 6054 7275 6560        If ``True`
+00013410: 602c 2074 6865 206d 6573 7361 6765 2077  `, the message w
+00013420: 696c 6c20 6265 2073 656e 7420 6173 2061  ill be sent as a
+00013430: 2072 6570 6c79 2074 6f20 7468 6973 206d   reply to this m
+00013440: 6573 7361 6765 2e0d 0a20 2020 2020 2020  essage...       
+00013450: 2020 2020 2020 2020 2049 6620 2a72 6570           If *rep
+00013460: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+00013470: 2a20 6973 2070 6173 7365 642c 2074 6869  * is passed, thi
+00013480: 7320 7061 7261 6d65 7465 7220 7769 6c6c  s parameter will
+00013490: 2062 6520 6967 6e6f 7265 642e 0d0a 2020   be ignored...  
+000134a0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+000134b0: 6661 756c 7473 2074 6f20 6060 5472 7565  faults to ``True
+000134c0: 6060 2069 6e20 6772 6f75 7020 6368 6174  `` in group chat
+000134d0: 7320 616e 6420 6060 4661 6c73 6560 6020  s and ``False`` 
+000134e0: 696e 2070 7269 7661 7465 2063 6861 7473  in private chats
 000134f0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00013500: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
-00013510: 655f 6964 2028 6060 696e 7460 602c 202a  e_id (``int``, *
-00013520: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
-00013530: 2020 2020 2020 2020 2020 2020 2049 6620               If 
-00013540: 7468 6520 6d65 7373 6167 6520 6973 2061  the message is a
-00013550: 2072 6570 6c79 2c20 4944 206f 6620 7468   reply, ID of th
-00013560: 6520 6f72 6967 696e 616c 206d 6573 7361  e original messa
-00013570: 6765 2e0d 0a0d 0a20 2020 2020 2020 2052  ge.....        R
-00013580: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00013590: 2020 2020 204f 6e20 7375 6363 6573 732c       On success,
-000135a0: 2061 203a 6f62 6a3a 607e 6669 7070 6572   a :obj:`~fipper
-000135b0: 2e74 7970 6573 2e4d 6573 7361 6765 7360  .types.Messages`
-000135c0: 206f 626a 6563 7420 6973 2072 6574 7572   object is retur
-000135d0: 6e65 6420 636f 6e74 6169 6e69 6e67 2061  ned containing a
-000135e0: 6c6c 2074 6865 0d0a 2020 2020 2020 2020  ll the..        
-000135f0: 2020 2020 7369 6e67 6c65 206d 6573 7361      single messa
-00013600: 6765 7320 7365 6e74 2e0d 0a0d 0a20 2020  ges sent.....   
-00013610: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
-00013620: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
-00013630: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
-00013640: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
-00013650: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
-00013660: 220d 0a20 2020 2020 2020 2069 6620 7175  "..        if qu
-00013670: 6f74 6520 6973 204e 6f6e 653a 0d0a 2020  ote is None:..  
-00013680: 2020 2020 2020 2020 2020 7175 6f74 6520            quote 
-00013690: 3d20 7365 6c66 2e63 6861 742e 7479 7065  = self.chat.type
-000136a0: 2021 3d20 656e 756d 732e 4368 6174 5479   != enums.ChatTy
-000136b0: 7065 2e50 5249 5641 5445 0d0a 0d0a 2020  pe.PRIVATE....  
-000136c0: 2020 2020 2020 6966 2072 6570 6c79 5f74        if reply_t
-000136d0: 6f5f 6d65 7373 6167 655f 6964 2069 7320  o_message_id is 
-000136e0: 4e6f 6e65 2061 6e64 2071 756f 7465 3a0d  None and quote:.
-000136f0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00013700: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-00013710: 203d 2073 656c 662e 6964 0d0a 0d0a 2020   = self.id....  
-00013720: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-00013730: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-00013740: 7365 6e64 5f6d 6564 6961 5f67 726f 7570  send_media_group
-00013750: 280d 0a20 2020 2020 2020 2020 2020 2063  (..            c
-00013760: 6861 745f 6964 3d73 656c 662e 6368 6174  hat_id=self.chat
-00013770: 2e69 642c 0d0a 2020 2020 2020 2020 2020  .id,..          
-00013780: 2020 6d65 6469 613d 6d65 6469 612c 0d0a    media=media,..
-00013790: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-000137a0: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-000137b0: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-000137c0: 6174 696f 6e2c 0d0a 2020 2020 2020 2020  ation,..        
-000137d0: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
-000137e0: 7361 6765 5f69 643d 7265 706c 795f 746f  sage_id=reply_to
-000137f0: 5f6d 6573 7361 6765 5f69 640d 0a20 2020  _message_id..   
-00013800: 2020 2020 2029 0d0a 0d0a 2020 2020 6173       )....    as
-00013810: 796e 6320 6465 6620 7265 706c 795f 7068  ync def reply_ph
-00013820: 6f74 6f28 0d0a 2020 2020 2020 2020 7365  oto(..        se
-00013830: 6c66 2c0d 0a20 2020 2020 2020 2070 686f  lf,..        pho
-00013840: 746f 3a20 556e 696f 6e5b 7374 722c 2042  to: Union[str, B
-00013850: 696e 6172 7949 4f5d 2c0d 0a20 2020 2020  inaryIO],..     
-00013860: 2020 2071 756f 7465 3a20 626f 6f6c 203d     quote: bool =
-00013870: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00013880: 6361 7074 696f 6e3a 2073 7472 203d 2022  caption: str = "
-00013890: 222c 0d0a 2020 2020 2020 2020 7061 7273  ",..        pars
-000138a0: 655f 6d6f 6465 3a20 4f70 7469 6f6e 616c  e_mode: Optional
-000138b0: 5b22 656e 756d 732e 5061 7273 654d 6f64  ["enums.ParseMod
-000138c0: 6522 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  e"] = None,..   
-000138d0: 2020 2020 2063 6170 7469 6f6e 5f65 6e74       caption_ent
-000138e0: 6974 6965 733a 204c 6973 745b 2274 7970  ities: List["typ
-000138f0: 6573 2e4d 6573 7361 6765 456e 7469 7479  es.MessageEntity
-00013900: 225d 203d 204e 6f6e 652c 0d0a 2020 2020  "] = None,..    
-00013910: 2020 2020 7474 6c5f 7365 636f 6e64 733a      ttl_seconds:
-00013920: 2069 6e74 203d 204e 6f6e 652c 0d0a 2020   int = None,..  
-00013930: 2020 2020 2020 6469 7361 626c 655f 6e6f        disable_no
-00013940: 7469 6669 6361 7469 6f6e 3a20 626f 6f6c  tification: bool
-00013950: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00013960: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00013970: 6765 5f69 643a 2069 6e74 203d 204e 6f6e  ge_id: int = Non
-00013980: 652c 0d0a 2020 2020 2020 2020 7265 706c  e,..        repl
-00013990: 795f 6d61 726b 7570 3a20 556e 696f 6e5b  y_markup: Union[
-000139a0: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-000139b0: 7970 6573 2e49 6e6c 696e 654b 6579 626f  ypes.InlineKeybo
-000139c0: 6172 644d 6172 6b75 7022 2c0d 0a20 2020  ardMarkup",..   
-000139d0: 2020 2020 2020 2020 2022 7479 7065 732e           "types.
-000139e0: 5265 706c 794b 6579 626f 6172 644d 6172  ReplyKeyboardMar
-000139f0: 6b75 7022 2c0d 0a20 2020 2020 2020 2020  kup",..         
-00013a00: 2020 2022 7479 7065 732e 5265 706c 794b     "types.ReplyK
-00013a10: 6579 626f 6172 6452 656d 6f76 6522 2c0d  eyboardRemove",.
-00013a20: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00013a30: 7065 732e 466f 7263 6552 6570 6c79 220d  pes.ForceReply".
-00013a40: 0a20 2020 2020 2020 205d 203d 204e 6f6e  .        ] = Non
-00013a50: 652c 0d0a 2020 2020 2020 2020 7072 6f67  e,..        prog
-00013a60: 7265 7373 3a20 4361 6c6c 6162 6c65 203d  ress: Callable =
-00013a70: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00013a80: 7072 6f67 7265 7373 5f61 7267 733a 2074  progress_args: t
-00013a90: 7570 6c65 203d 2028 290d 0a20 2020 2029  uple = ()..    )
-00013aa0: 202d 3e20 224d 6573 7361 6765 223a 0d0a   -> "Message":..
-00013ab0: 2020 2020 2020 2020 2222 2242 6f75 6e64          """Bound
-00013ac0: 206d 6574 686f 6420 2a72 6570 6c79 5f70   method *reply_p
-00013ad0: 686f 746f 2a20 6f66 203a 6f62 6a3a 607e  hoto* of :obj:`~
-00013ae0: 6669 7070 6572 2e74 7970 6573 2e4d 6573  fipper.types.Mes
-00013af0: 7361 6765 602e 0d0a 0d0a 2020 2020 2020  sage`.....      
-00013b00: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
-00013b10: 6375 7420 666f 723a 0d0a 0d0a 2020 2020  cut for:....    
-00013b20: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00013b30: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
-00013b40: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00013b50: 636c 6965 6e74 2e73 656e 645f 7068 6f74  client.send_phot
-00013b60: 6f28 0d0a 2020 2020 2020 2020 2020 2020  o(..            
-00013b70: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
-00013b80: 6167 652e 6368 6174 2e69 642c 0d0a 2020  age.chat.id,..  
-00013b90: 2020 2020 2020 2020 2020 2020 2020 7068                ph
-00013ba0: 6f74 6f3d 7068 6f74 6f0d 0a20 2020 2020  oto=photo..     
-00013bb0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00013bc0: 2020 2020 4578 616d 706c 653a 0d0a 2020      Example:..  
-00013bd0: 2020 2020 2020 2020 2020 2e2e 2063 6f64            .. cod
-00013be0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-00013bf0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00013c00: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-00013c10: 652e 7265 706c 795f 7068 6f74 6f28 7068  e.reply_photo(ph
-00013c20: 6f74 6f29 0d0a 0d0a 2020 2020 2020 2020  oto)....        
-00013c30: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-00013c40: 2020 2020 2020 2020 2070 686f 746f 2028           photo (
-00013c50: 6060 7374 7260 6029 3a0d 0a20 2020 2020  ``str``):..     
-00013c60: 2020 2020 2020 2020 2020 2050 686f 746f             Photo
-00013c70: 2074 6f20 7365 6e64 2e0d 0a20 2020 2020   to send...     
-00013c80: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-00013c90: 6120 6669 6c65 5f69 6420 6173 2073 7472  a file_id as str
-00013ca0: 696e 6720 746f 2073 656e 6420 6120 7068  ing to send a ph
-00013cb0: 6f74 6f20 7468 6174 2065 7869 7374 7320  oto that exists 
-00013cc0: 6f6e 2074 6865 2054 656c 6567 7261 6d20  on the Telegram 
-00013cd0: 7365 7276 6572 732c 0d0a 2020 2020 2020  servers,..      
-00013ce0: 2020 2020 2020 2020 2020 7061 7373 2061            pass a
-00013cf0: 6e20 4854 5450 2055 524c 2061 7320 6120  n HTTP URL as a 
-00013d00: 7374 7269 6e67 2066 6f72 2054 656c 6567  string for Teleg
-00013d10: 7261 6d20 746f 2067 6574 2061 2070 686f  ram to get a pho
-00013d20: 746f 2066 726f 6d20 7468 6520 496e 7465  to from the Inte
-00013d30: 726e 6574 2c20 6f72 0d0a 2020 2020 2020  rnet, or..      
-00013d40: 2020 2020 2020 2020 2020 7061 7373 2061            pass a
-00013d50: 2066 696c 6520 7061 7468 2061 7320 7374   file path as st
-00013d60: 7269 6e67 2074 6f20 7570 6c6f 6164 2061  ring to upload a
-00013d70: 206e 6577 2070 686f 746f 2074 6861 7420   new photo that 
-00013d80: 6578 6973 7473 206f 6e20 796f 7572 206c  exists on your l
-00013d90: 6f63 616c 206d 6163 6869 6e65 2e0d 0a0d  ocal machine....
-00013da0: 0a20 2020 2020 2020 2020 2020 2071 756f  .            quo
-00013db0: 7465 2028 6060 626f 6f6c 6060 2c20 2a6f  te (``bool``, *o
-00013dc0: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-00013dd0: 2020 2020 2020 2020 2020 2020 4966 2060              If `
-00013de0: 6054 7275 6560 602c 2074 6865 206d 6573  `True``, the mes
-00013df0: 7361 6765 2077 696c 6c20 6265 2073 656e  sage will be sen
-00013e00: 7420 6173 2061 2072 6570 6c79 2074 6f20  t as a reply to 
-00013e10: 7468 6973 206d 6573 7361 6765 2e0d 0a20  this message... 
-00013e20: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-00013e30: 6620 2a72 6570 6c79 5f74 6f5f 6d65 7373  f *reply_to_mess
-00013e40: 6167 655f 6964 2a20 6973 2070 6173 7365  age_id* is passe
-00013e50: 642c 2074 6869 7320 7061 7261 6d65 7465  d, this paramete
-00013e60: 7220 7769 6c6c 2062 6520 6967 6e6f 7265  r will be ignore
-00013e70: 642e 0d0a 2020 2020 2020 2020 2020 2020  d...            
-00013e80: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00013e90: 6060 5472 7565 6060 2069 6e20 6772 6f75  ``True`` in grou
-00013ea0: 7020 6368 6174 7320 616e 6420 6060 4661  p chats and ``Fa
-00013eb0: 6c73 6560 6020 696e 2070 7269 7661 7465  lse`` in private
-00013ec0: 2063 6861 7473 2e0d 0a0d 0a20 2020 2020   chats.....     
-00013ed0: 2020 2020 2020 2063 6170 7469 6f6e 2028         caption (
-00013ee0: 6060 7374 7260 602c 202a 6f70 7469 6f6e  ``str``, *option
-00013ef0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
-00013f00: 2020 2020 2020 2050 686f 746f 2063 6170         Photo cap
-00013f10: 7469 6f6e 2c20 302d 3130 3234 2063 6861  tion, 0-1024 cha
-00013f20: 7261 6374 6572 732e 0d0a 0d0a 2020 2020  racters.....    
-00013f30: 2020 2020 2020 2020 7061 7273 655f 6d6f          parse_mo
-00013f40: 6465 2028 3a6f 626a 3a60 7e66 6970 7065  de (:obj:`~fippe
-00013f50: 722e 656e 756d 732e 5061 7273 654d 6f64  r.enums.ParseMod
-00013f60: 6560 2c20 2a6f 7074 696f 6e61 6c2a 293a  e`, *optional*):
-00013f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013f80: 2020 4279 2064 6566 6175 6c74 2c20 7465    By default, te
-00013f90: 7874 7320 6172 6520 7061 7273 6564 2075  xts are parsed u
-00013fa0: 7369 6e67 2062 6f74 6820 4d61 726b 646f  sing both Markdo
-00013fb0: 776e 2061 6e64 2048 544d 4c20 7374 796c  wn and HTML styl
-00013fc0: 6573 2e0d 0a20 2020 2020 2020 2020 2020  es...           
-00013fd0: 2020 2020 2059 6f75 2063 616e 2063 6f6d       You can com
-00013fe0: 6269 6e65 2062 6f74 6820 7379 6e74 6178  bine both syntax
-00013ff0: 6573 2074 6f67 6574 6865 722e 0d0a 0d0a  es together.....
-00014000: 2020 2020 2020 2020 2020 2020 6361 7074              capt
-00014010: 696f 6e5f 656e 7469 7469 6573 2028 4c69  ion_entities (Li
-00014020: 7374 206f 6620 3a6f 626a 3a60 7e66 6970  st of :obj:`~fip
-00014030: 7065 722e 7479 7065 732e 4d65 7373 6167  per.types.Messag
-00014040: 6545 6e74 6974 7960 293a 0d0a 2020 2020  eEntity`):..    
-00014050: 2020 2020 2020 2020 2020 2020 4c69 7374              List
-00014060: 206f 6620 7370 6563 6961 6c20 656e 7469   of special enti
-00014070: 7469 6573 2074 6861 7420 6170 7065 6172  ties that appear
-00014080: 2069 6e20 7468 6520 6361 7074 696f 6e2c   in the caption,
-00014090: 2077 6869 6368 2063 616e 2062 6520 7370   which can be sp
-000140a0: 6563 6966 6965 6420 696e 7374 6561 6420  ecified instead 
-000140b0: 6f66 202a 7061 7273 655f 6d6f 6465 2a2e  of *parse_mode*.
-000140c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000140d0: 7474 6c5f 7365 636f 6e64 7320 2860 6069  ttl_seconds (``i
-000140e0: 6e74 6060 2c20 2a6f 7074 696f 6e61 6c2a  nt``, *optional*
-000140f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00014100: 2020 2020 5365 6c66 2d44 6573 7472 7563      Self-Destruc
-00014110: 7420 5469 6d65 722e 0d0a 2020 2020 2020  t Timer...      
-00014120: 2020 2020 2020 2020 2020 4966 2079 6f75            If you
-00014130: 2073 6574 2061 2074 696d 6572 2c20 7468   set a timer, th
-00014140: 6520 7068 6f74 6f20 7769 6c6c 2073 656c  e photo will sel
-00014150: 662d 6465 7374 7275 6374 2069 6e20 2a74  f-destruct in *t
-00014160: 746c 5f73 6563 6f6e 6473 2a0d 0a20 2020  tl_seconds*..   
-00014170: 2020 2020 2020 2020 2020 2020 2073 6563               sec
-00014180: 6f6e 6473 2061 6674 6572 2069 7420 7761  onds after it wa
-00014190: 7320 7669 6577 6564 2e0d 0a0d 0a20 2020  s viewed.....   
-000141a0: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-000141b0: 5f6e 6f74 6966 6963 6174 696f 6e20 2860  _notification (`
-000141c0: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
-000141d0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
-000141e0: 2020 2020 2020 2053 656e 6473 2074 6865         Sends the
-000141f0: 206d 6573 7361 6765 2073 696c 656e 746c   message silentl
-00014200: 792e 0d0a 2020 2020 2020 2020 2020 2020  y...            
-00014210: 2020 2020 5573 6572 7320 7769 6c6c 2072      Users will r
-00014220: 6563 6569 7665 2061 206e 6f74 6966 6963  eceive a notific
-00014230: 6174 696f 6e20 7769 7468 206e 6f20 736f  ation with no so
-00014240: 756e 642e 0d0a 0d0a 2020 2020 2020 2020  und.....        
-00014250: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
-00014260: 7361 6765 5f69 6420 2860 6069 6e74 6060  sage_id (``int``
-00014270: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014290: 4966 2074 6865 206d 6573 7361 6765 2069  If the message i
-000142a0: 7320 6120 7265 706c 792c 2049 4420 6f66  s a reply, ID of
-000142b0: 2074 6865 206f 7269 6769 6e61 6c20 6d65   the original me
-000142c0: 7373 6167 652e 0d0a 0d0a 2020 2020 2020  ssage.....      
-000142d0: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
-000142e0: 7570 2028 3a6f 626a 3a60 7e66 6970 7065  up (:obj:`~fippe
-000142f0: 722e 7479 7065 732e 496e 6c69 6e65 4b65  r.types.InlineKe
-00014300: 7962 6f61 7264 4d61 726b 7570 6020 7c20  yboardMarkup` | 
-00014310: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
-00014320: 7065 732e 5265 706c 794b 6579 626f 6172  pes.ReplyKeyboar
-00014330: 644d 6172 6b75 7060 207c 203a 6f62 6a3a  dMarkup` | :obj:
-00014340: 607e 6669 7070 6572 2e74 7970 6573 2e52  `~fipper.types.R
-00014350: 6570 6c79 4b65 7962 6f61 7264 5265 6d6f  eplyKeyboardRemo
-00014360: 7665 6020 7c20 3a6f 626a 3a60 7e66 6970  ve` | :obj:`~fip
-00014370: 7065 722e 7479 7065 732e 466f 7263 6552  per.types.ForceR
-00014380: 6570 6c79 602c 202a 6f70 7469 6f6e 616c  eply`, *optional
-00014390: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-000143a0: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
-000143b0: 696e 7465 7266 6163 6520 6f70 7469 6f6e  interface option
-000143c0: 732e 2041 6e20 6f62 6a65 6374 2066 6f72  s. An object for
-000143d0: 2061 6e20 696e 6c69 6e65 206b 6579 626f   an inline keybo
-000143e0: 6172 642c 2063 7573 746f 6d20 7265 706c  ard, custom repl
-000143f0: 7920 6b65 7962 6f61 7264 2c0d 0a20 2020  y keyboard,..   
-00014400: 2020 2020 2020 2020 2020 2020 2069 6e73               ins
-00014410: 7472 7563 7469 6f6e 7320 746f 2072 656d  tructions to rem
-00014420: 6f76 6520 7265 706c 7920 6b65 7962 6f61  ove reply keyboa
-00014430: 7264 206f 7220 746f 2066 6f72 6365 2061  rd or to force a
-00014440: 2072 6570 6c79 2066 726f 6d20 7468 6520   reply from the 
-00014450: 7573 6572 2e0d 0a0d 0a20 2020 2020 2020  user.....       
-00014460: 2020 2020 2070 726f 6772 6573 7320 2860       progress (`
-00014470: 6043 616c 6c61 626c 6560 602c 202a 6f70  `Callable``, *op
-00014480: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-00014490: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-000144a0: 6120 6361 6c6c 6261 636b 2066 756e 6374  a callback funct
-000144b0: 696f 6e20 746f 2076 6965 7720 7468 6520  ion to view the 
-000144c0: 6669 6c65 2074 7261 6e73 6d69 7373 696f  file transmissio
-000144d0: 6e20 7072 6f67 7265 7373 2e0d 0a20 2020  n progress...   
-000144e0: 2020 2020 2020 2020 2020 2020 2054 6865               The
-000144f0: 2066 756e 6374 696f 6e20 6d75 7374 2074   function must t
-00014500: 616b 6520 2a28 6375 7272 656e 742c 2074  ake *(current, t
-00014510: 6f74 616c 292a 2061 7320 706f 7369 7469  otal)* as positi
-00014520: 6f6e 616c 2061 7267 756d 656e 7473 2028  onal arguments (
-00014530: 6c6f 6f6b 2061 7420 4f74 6865 7220 5061  look at Other Pa
-00014540: 7261 6d65 7465 7273 2062 656c 6f77 2066  rameters below f
-00014550: 6f72 2061 0d0a 2020 2020 2020 2020 2020  or a..          
-00014560: 2020 2020 2020 6465 7461 696c 6564 2064        detailed d
-00014570: 6573 6372 6970 7469 6f6e 2920 616e 6420  escription) and 
-00014580: 7769 6c6c 2062 6520 6361 6c6c 6564 2062  will be called b
-00014590: 6163 6b20 6561 6368 2074 696d 6520 6120  ack each time a 
-000145a0: 6e65 7720 6669 6c65 2063 6875 6e6b 2068  new file chunk h
-000145b0: 6173 2062 6565 6e20 7375 6363 6573 7366  as been successf
-000145c0: 756c 6c79 0d0a 2020 2020 2020 2020 2020  ully..          
-000145d0: 2020 2020 2020 7472 616e 736d 6974 7465        transmitte
-000145e0: 642e 0d0a 0d0a 2020 2020 2020 2020 2020  d.....          
-000145f0: 2020 7072 6f67 7265 7373 5f61 7267 7320    progress_args 
-00014600: 2860 6074 7570 6c65 6060 2c20 2a6f 7074  (``tuple``, *opt
-00014610: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
-00014620: 2020 2020 2020 2020 2020 4578 7472 6120            Extra 
-00014630: 6375 7374 6f6d 2061 7267 756d 656e 7473  custom arguments
-00014640: 2066 6f72 2074 6865 2070 726f 6772 6573   for the progres
-00014650: 7320 6361 6c6c 6261 636b 2066 756e 6374  s callback funct
-00014660: 696f 6e2e 0d0a 2020 2020 2020 2020 2020  ion...          
-00014670: 2020 2020 2020 596f 7520 6361 6e20 7061        You can pa
-00014680: 7373 2061 6e79 7468 696e 6720 796f 7520  ss anything you 
-00014690: 6e65 6564 2074 6f20 6265 2061 7661 696c  need to be avail
-000146a0: 6162 6c65 2069 6e20 7468 6520 7072 6f67  able in the prog
-000146b0: 7265 7373 2063 616c 6c62 6163 6b20 7363  ress callback sc
-000146c0: 6f70 653b 2066 6f72 2065 7861 6d70 6c65  ope; for example
-000146d0: 2c20 6120 4d65 7373 6167 650d 0a20 2020  , a Message..   
-000146e0: 2020 2020 2020 2020 2020 2020 206f 626a               obj
-000146f0: 6563 7420 6f72 2061 2043 6c69 656e 7420  ect or a Client 
-00014700: 696e 7374 616e 6365 2069 6e20 6f72 6465  instance in orde
-00014710: 7220 746f 2065 6469 7420 7468 6520 6d65  r to edit the me
-00014720: 7373 6167 6520 7769 7468 2074 6865 2075  ssage with the u
-00014730: 7064 6174 6564 2070 726f 6772 6573 7320  pdated progress 
-00014740: 7374 6174 7573 2e0d 0a0d 0a20 2020 2020  status.....     
-00014750: 2020 204f 7468 6572 2050 6172 616d 6574     Other Paramet
-00014760: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
-00014770: 2020 6375 7272 656e 7420 2860 6069 6e74    current (``int
-00014780: 6060 293a 0d0a 2020 2020 2020 2020 2020  ``):..          
-00014790: 2020 2020 2020 5468 6520 616d 6f75 6e74        The amount
-000147a0: 206f 6620 6279 7465 7320 7472 616e 736d   of bytes transm
-000147b0: 6974 7465 6420 736f 2066 6172 2e0d 0a0d  itted so far....
-000147c0: 0a20 2020 2020 2020 2020 2020 2074 6f74  .            tot
-000147d0: 616c 2028 6060 696e 7460 6029 3a0d 0a20  al (``int``):.. 
-000147e0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000147f0: 6865 2074 6f74 616c 2073 697a 6520 6f66  he total size of
-00014800: 2074 6865 2066 696c 652e 0d0a 0d0a 2020   the file.....  
-00014810: 2020 2020 2020 2020 2020 2a61 7267 7320            *args 
-00014820: 2860 6074 7570 6c65 6060 2c20 2a6f 7074  (``tuple``, *opt
-00014830: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
-00014840: 2020 2020 2020 2020 2020 4578 7472 6120            Extra 
-00014850: 6375 7374 6f6d 2061 7267 756d 656e 7473  custom arguments
-00014860: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
-00014870: 6865 2060 6070 726f 6772 6573 735f 6172  he ``progress_ar
-00014880: 6773 6060 2070 6172 616d 6574 6572 2e0d  gs`` parameter..
-00014890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000148a0: 2059 6f75 2063 616e 2065 6974 6865 7220   You can either 
-000148b0: 6b65 6570 2060 602a 6172 6773 6060 206f  keep ``*args`` o
-000148c0: 7220 6164 6420 6576 6572 7920 7369 6e67  r add every sing
-000148d0: 6c65 2065 7874 7261 2061 7267 756d 656e  le extra argumen
-000148e0: 7420 696e 2079 6f75 7220 6675 6e63 7469  t in your functi
-000148f0: 6f6e 2073 6967 6e61 7475 7265 2e0d 0a0d  on signature....
-00014900: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00014910: 3a0d 0a20 2020 2020 2020 2020 2020 204f  :..            O
-00014920: 6e20 7375 6363 6573 732c 2074 6865 2073  n success, the s
-00014930: 656e 7420 3a6f 626a 3a60 7e66 6970 7065  ent :obj:`~fippe
-00014940: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
-00014950: 2069 7320 7265 7475 726e 6564 2e0d 0a20   is returned... 
-00014960: 2020 2020 2020 2020 2020 2049 6e20 6361             In ca
-00014970: 7365 2074 6865 2075 706c 6f61 6420 6973  se the upload is
-00014980: 2064 656c 6962 6572 6174 656c 7920 7374   deliberately st
-00014990: 6f70 7065 6420 7769 7468 203a 6d65 7468  opped with :meth
-000149a0: 3a60 7e66 6970 7065 722e 436c 6965 6e74  :`~fipper.Client
-000149b0: 2e73 746f 705f 7472 616e 736d 6973 7369  .stop_transmissi
-000149c0: 6f6e 602c 204e 6f6e 6520 6973 2072 6574  on`, None is ret
-000149d0: 7572 6e65 640d 0a20 2020 2020 2020 2020  urned..         
-000149e0: 2020 2069 6e73 7465 6164 2e0d 0a0d 0a20     instead..... 
-000149f0: 2020 2020 2020 2052 6169 7365 733a 0d0a         Raises:..
-00014a00: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
-00014a10: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
-00014a20: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
-00014a30: 6572 726f 722e 0d0a 2020 2020 2020 2020  error...        
-00014a40: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-00014a50: 7175 6f74 6520 6973 204e 6f6e 653a 0d0a  quote is None:..
-00014a60: 2020 2020 2020 2020 2020 2020 7175 6f74              quot
-00014a70: 6520 3d20 7365 6c66 2e63 6861 742e 7479  e = self.chat.ty
-00014a80: 7065 2021 3d20 656e 756d 732e 4368 6174  pe != enums.Chat
-00014a90: 5479 7065 2e50 5249 5641 5445 0d0a 0d0a  Type.PRIVATE....
-00014aa0: 2020 2020 2020 2020 6966 2072 6570 6c79          if reply
-00014ab0: 5f74 6f5f 6d65 7373 6167 655f 6964 2069  _to_message_id i
-00014ac0: 7320 4e6f 6e65 2061 6e64 2071 756f 7465  s None and quote
-00014ad0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00014ae0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00014af0: 6964 203d 2073 656c 662e 6964 0d0a 0d0a  id = self.id....
-00014b00: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00014b10: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-00014b20: 742e 7365 6e64 5f70 686f 746f 280d 0a20  t.send_photo(.. 
-00014b30: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00014b40: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
-00014b50: 0d0a 2020 2020 2020 2020 2020 2020 7068  ..            ph
-00014b60: 6f74 6f3d 7068 6f74 6f2c 0d0a 2020 2020  oto=photo,..    
-00014b70: 2020 2020 2020 2020 6361 7074 696f 6e3d          caption=
-00014b80: 6361 7074 696f 6e2c 0d0a 2020 2020 2020  caption,..      
-00014b90: 2020 2020 2020 7061 7273 655f 6d6f 6465        parse_mode
-00014ba0: 3d70 6172 7365 5f6d 6f64 652c 0d0a 2020  =parse_mode,..  
-00014bb0: 2020 2020 2020 2020 2020 6361 7074 696f            captio
-00014bc0: 6e5f 656e 7469 7469 6573 3d63 6170 7469  n_entities=capti
-00014bd0: 6f6e 5f65 6e74 6974 6965 732c 0d0a 2020  on_entities,..  
-00014be0: 2020 2020 2020 2020 2020 7474 6c5f 7365            ttl_se
-00014bf0: 636f 6e64 733d 7474 6c5f 7365 636f 6e64  conds=ttl_second
-00014c00: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00014c10: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00014c20: 7469 6f6e 3d64 6973 6162 6c65 5f6e 6f74  tion=disable_not
-00014c30: 6966 6963 6174 696f 6e2c 0d0a 2020 2020  ification,..    
-00014c40: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
-00014c50: 5f6d 6573 7361 6765 5f69 643d 7265 706c  _message_id=repl
-00014c60: 795f 746f 5f6d 6573 7361 6765 5f69 642c  y_to_message_id,
-00014c70: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00014c80: 706c 795f 6d61 726b 7570 3d72 6570 6c79  ply_markup=reply
-00014c90: 5f6d 6172 6b75 702c 0d0a 2020 2020 2020  _markup,..      
-00014ca0: 2020 2020 2020 7072 6f67 7265 7373 3d70        progress=p
-00014cb0: 726f 6772 6573 732c 0d0a 2020 2020 2020  rogress,..      
-00014cc0: 2020 2020 2020 7072 6f67 7265 7373 5f61        progress_a
-00014cd0: 7267 733d 7072 6f67 7265 7373 5f61 7267  rgs=progress_arg
-00014ce0: 730d 0a20 2020 2020 2020 2029 0d0a 0d0a  s..        )....
-00014cf0: 2020 2020 6173 796e 6320 6465 6620 7265      async def re
-00014d00: 706c 795f 706f 6c6c 280d 0a20 2020 2020  ply_poll(..     
-00014d10: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-00014d20: 2020 7175 6573 7469 6f6e 3a20 7374 722c    question: str,
-00014d30: 0d0a 2020 2020 2020 2020 6f70 7469 6f6e  ..        option
-00014d40: 733a 204c 6973 745b 7374 725d 2c0d 0a20  s: List[str],.. 
-00014d50: 2020 2020 2020 2069 735f 616e 6f6e 796d         is_anonym
-00014d60: 6f75 733a 2062 6f6f 6c20 3d20 5472 7565  ous: bool = True
-00014d70: 2c0d 0a20 2020 2020 2020 2074 7970 653a  ,..        type:
-00014d80: 2022 656e 756d 732e 506f 6c6c 5479 7065   "enums.PollType
-00014d90: 2220 3d20 656e 756d 732e 506f 6c6c 5479  " = enums.PollTy
-00014da0: 7065 2e52 4547 554c 4152 2c0d 0a20 2020  pe.REGULAR,..   
-00014db0: 2020 2020 2061 6c6c 6f77 735f 6d75 6c74       allows_mult
-00014dc0: 6970 6c65 5f61 6e73 7765 7273 3a20 626f  iple_answers: bo
-00014dd0: 6f6c 203d 204e 6f6e 652c 0d0a 2020 2020  ol = None,..    
-00014de0: 2020 2020 636f 7272 6563 745f 6f70 7469      correct_opti
-00014df0: 6f6e 5f69 643a 2069 6e74 203d 204e 6f6e  on_id: int = Non
-00014e00: 652c 0d0a 2020 2020 2020 2020 6578 706c  e,..        expl
-00014e10: 616e 6174 696f 6e3a 2073 7472 203d 204e  anation: str = N
-00014e20: 6f6e 652c 0d0a 2020 2020 2020 2020 6578  one,..        ex
-00014e30: 706c 616e 6174 696f 6e5f 7061 7273 655f  planation_parse_
-00014e40: 6d6f 6465 3a20 2265 6e75 6d73 2e50 6172  mode: "enums.Par
-00014e50: 7365 4d6f 6465 2220 3d20 4e6f 6e65 2c0d  seMode" = None,.
-00014e60: 0a20 2020 2020 2020 2065 7870 6c61 6e61  .        explana
-00014e70: 7469 6f6e 5f65 6e74 6974 6965 733a 204c  tion_entities: L
-00014e80: 6973 745b 2274 7970 6573 2e4d 6573 7361  ist["types.Messa
-00014e90: 6765 456e 7469 7479 225d 203d 204e 6f6e  geEntity"] = Non
-00014ea0: 652c 0d0a 2020 2020 2020 2020 6f70 656e  e,..        open
-00014eb0: 5f70 6572 696f 643a 2069 6e74 203d 204e  _period: int = N
-00014ec0: 6f6e 652c 0d0a 2020 2020 2020 2020 636c  one,..        cl
-00014ed0: 6f73 655f 6461 7465 3a20 6461 7465 7469  ose_date: dateti
-00014ee0: 6d65 203d 204e 6f6e 652c 0d0a 2020 2020  me = None,..    
-00014ef0: 2020 2020 6973 5f63 6c6f 7365 643a 2062      is_closed: b
-00014f00: 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20 2020  ool = None,..   
-00014f10: 2020 2020 2071 756f 7465 3a20 626f 6f6c       quote: bool
-00014f20: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00014f30: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
-00014f40: 6361 7469 6f6e 3a20 626f 6f6c 203d 204e  cation: bool = N
-00014f50: 6f6e 652c 0d0a 2020 2020 2020 2020 7072  one,..        pr
-00014f60: 6f74 6563 745f 636f 6e74 656e 743a 2062  otect_content: b
-00014f70: 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20 2020  ool = None,..   
-00014f80: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
-00014f90: 7373 6167 655f 6964 3a20 696e 7420 3d20  ssage_id: int = 
-00014fa0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2073  None,..        s
-00014fb0: 6368 6564 756c 655f 6461 7465 3a20 6461  chedule_date: da
-00014fc0: 7465 7469 6d65 203d 204e 6f6e 652c 0d0a  tetime = None,..
-00014fd0: 2020 2020 2020 2020 7265 706c 795f 6d61          reply_ma
-00014fe0: 726b 7570 3a20 556e 696f 6e5b 0d0a 2020  rkup: Union[..  
-00014ff0: 2020 2020 2020 2020 2020 2274 7970 6573            "types
-00015000: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
-00015010: 6172 6b75 7022 2c0d 0a20 2020 2020 2020  arkup",..       
-00015020: 2020 2020 2022 7479 7065 732e 5265 706c       "types.Repl
-00015030: 794b 6579 626f 6172 644d 6172 6b75 7022  yKeyboardMarkup"
-00015040: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00015050: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
-00015060: 6172 6452 656d 6f76 6522 2c0d 0a20 2020  ardRemove",..   
-00015070: 2020 2020 2020 2020 2022 7479 7065 732e           "types.
-00015080: 466f 7263 6552 6570 6c79 220d 0a20 2020  ForceReply"..   
-00015090: 2020 2020 205d 203d 204e 6f6e 650d 0a20       ] = None.. 
-000150a0: 2020 2029 202d 3e20 224d 6573 7361 6765     ) -> "Message
-000150b0: 223a 0d0a 2020 2020 2020 2020 2222 2242  ":..        """B
-000150c0: 6f75 6e64 206d 6574 686f 6420 2a72 6570  ound method *rep
-000150d0: 6c79 5f70 6f6c 6c2a 206f 6620 3a6f 626a  ly_poll* of :obj
-000150e0: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
-000150f0: 4d65 7373 6167 6560 2e0d 0a0d 0a20 2020  Message`.....   
-00015100: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
-00015110: 6f72 7463 7574 2066 6f72 3a0d 0a0d 0a20  ortcut for:.... 
-00015120: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-00015130: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
-00015140: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-00015150: 6974 2063 6c69 656e 742e 7365 6e64 5f70  it client.send_p
-00015160: 6f6c 6c28 0d0a 2020 2020 2020 2020 2020  oll(..          
-00015170: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
-00015180: 7373 6167 652e 6368 6174 2e69 642c 0d0a  ssage.chat.id,..
-00015190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151a0: 7175 6573 7469 6f6e 3d22 5468 6973 2069  question="This i
-000151b0: 7320 6120 706f 6c6c 222c 0d0a 2020 2020  s a poll",..    
-000151c0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-000151d0: 6f6e 733d 5b22 4122 2c20 2242 222c 2022  ons=["A", "B", "
-000151e0: 435d 0d0a 2020 2020 2020 2020 2020 2020  C]..            
-000151f0: 290d 0a0d 0a20 2020 2020 2020 2045 7861  )....        Exa
-00015200: 6d70 6c65 3a0d 0a20 2020 2020 2020 2020  mple:..         
-00015210: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-00015220: 3a3a 2070 7974 686f 6e0d 0a0d 0a20 2020  :: python....   
-00015230: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-00015240: 6974 206d 6573 7361 6765 2e72 6570 6c79  it message.reply
-00015250: 5f70 6f6c 6c28 2254 6869 7320 6973 2061  _poll("This is a
-00015260: 2070 6f6c 6c22 2c20 5b22 4122 2c20 2242   poll", ["A", "B
-00015270: 222c 2022 4322 5d29 0d0a 0d0a 2020 2020  ", "C"])....    
-00015280: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
-00015290: 0a20 2020 2020 2020 2020 2020 2071 7565  .            que
-000152a0: 7374 696f 6e20 2860 6073 7472 6060 293a  stion (``str``):
-000152b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000152c0: 2020 506f 6c6c 2071 7565 7374 696f 6e2c    Poll question,
-000152d0: 2031 2d32 3535 2063 6861 7261 6374 6572   1-255 character
-000152e0: 732e 0d0a 0d0a 2020 2020 2020 2020 2020  s.....          
-000152f0: 2020 6f70 7469 6f6e 7320 284c 6973 7420    options (List 
-00015300: 6f66 2060 6073 7472 6060 293a 0d0a 2020  of ``str``):..  
-00015310: 2020 2020 2020 2020 2020 2020 2020 4c69                Li
-00015320: 7374 206f 6620 616e 7377 6572 206f 7074  st of answer opt
-00015330: 696f 6e73 2c20 322d 3130 2073 7472 696e  ions, 2-10 strin
-00015340: 6773 2031 2d31 3030 2063 6861 7261 6374  gs 1-100 charact
-00015350: 6572 7320 6561 6368 2e0d 0a0d 0a20 2020  ers each.....   
-00015360: 2020 2020 2020 2020 2069 735f 616e 6f6e           is_anon
-00015370: 796d 6f75 7320 2860 6062 6f6f 6c60 602c  ymous (``bool``,
-00015380: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
-00015390: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000153a0: 7275 652c 2069 6620 7468 6520 706f 6c6c  rue, if the poll
-000153b0: 206e 6565 6473 2074 6f20 6265 2061 6e6f   needs to be ano
-000153c0: 6e79 6d6f 7573 2e0d 0a20 2020 2020 2020  nymous...       
-000153d0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-000153e0: 7320 746f 2054 7275 652e 0d0a 0d0a 2020  s to True.....  
-000153f0: 2020 2020 2020 2020 2020 7479 7065 2028            type (
-00015400: 3a6f 626a 607e 6669 7070 6572 2e65 6e75  :obj`~fipper.enu
-00015410: 6d73 2e50 6f6c 6c54 7970 6560 2c20 2a6f  ms.PollType`, *o
-00015420: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-00015430: 2020 2020 2020 2020 2020 2020 506f 6c6c              Poll
-00015440: 2074 7970 652c 203a 6f62 6a3a 607e 6669   type, :obj:`~fi
-00015450: 7070 6572 2e65 6e75 6d73 2e50 6f6c 6c54  pper.enums.PollT
-00015460: 7970 652e 5155 495a 6020 6f72 203a 6f62  ype.QUIZ` or :ob
-00015470: 6a3a 607e 6669 7070 6572 2e65 6e75 6d73  j:`~fipper.enums
-00015480: 2e50 6f6c 6c54 7970 652e 5245 4755 4c41  .PollType.REGULA
-00015490: 5260 2e0d 0a20 2020 2020 2020 2020 2020  R`...           
-000154a0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-000154b0: 203a 6f62 6a3a 607e 6669 7070 6572 2e65   :obj:`~fipper.e
-000154c0: 6e75 6d73 2e50 6f6c 6c54 7970 652e 5245  nums.PollType.RE
-000154d0: 4755 4c41 5260 2e0d 0a0d 0a20 2020 2020  GULAR`.....     
-000154e0: 2020 2020 2020 2061 6c6c 6f77 735f 6d75         allows_mu
-000154f0: 6c74 6970 6c65 5f61 6e73 7765 7273 2028  ltiple_answers (
-00015500: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
-00015510: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-00015520: 2020 2020 2020 2020 5472 7565 2c20 6966          True, if
-00015530: 2074 6865 2070 6f6c 6c20 616c 6c6f 7773   the poll allows
-00015540: 206d 756c 7469 706c 6520 616e 7377 6572   multiple answer
-00015550: 732c 2069 676e 6f72 6564 2066 6f72 2070  s, ignored for p
-00015560: 6f6c 6c73 2069 6e20 7175 697a 206d 6f64  olls in quiz mod
-00015570: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-00015580: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00015590: 4661 6c73 652e 0d0a 0d0a 2020 2020 2020  False.....      
-000155a0: 2020 2020 2020 636f 7272 6563 745f 6f70        correct_op
-000155b0: 7469 6f6e 5f69 6420 2860 6069 6e74 6060  tion_id (``int``
-000155c0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155e0: 302d 6261 7365 6420 6964 656e 7469 6669  0-based identifi
-000155f0: 6572 206f 6620 7468 6520 636f 7272 6563  er of the correc
-00015600: 7420 616e 7377 6572 206f 7074 696f 6e2c  t answer option,
-00015610: 2072 6571 7569 7265 6420 666f 7220 706f   required for po
-00015620: 6c6c 7320 696e 2071 7569 7a20 6d6f 6465  lls in quiz mode
-00015630: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00015640: 2065 7870 6c61 6e61 7469 6f6e 2028 6060   explanation (``
-00015650: 7374 7260 602c 202a 6f70 7469 6f6e 616c  str``, *optional
-00015660: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-00015670: 2020 2020 2054 6578 7420 7468 6174 2069       Text that i
-00015680: 7320 7368 6f77 6e20 7768 656e 2061 2075  s shown when a u
-00015690: 7365 7220 6368 6f6f 7365 7320 616e 2069  ser chooses an i
-000156a0: 6e63 6f72 7265 6374 2061 6e73 7765 7220  ncorrect answer 
-000156b0: 6f72 2074 6170 7320 6f6e 2074 6865 206c  or taps on the l
-000156c0: 616d 7020 6963 6f6e 2069 6e20 6120 7175  amp icon in a qu
-000156d0: 697a 2d73 7479 6c65 0d0a 2020 2020 2020  iz-style..      
-000156e0: 2020 2020 2020 2020 2020 706f 6c6c 2c20            poll, 
-000156f0: 302d 3230 3020 6368 6172 6163 7465 7273  0-200 characters
-00015700: 2077 6974 6820 6174 206d 6f73 7420 3220   with at most 2 
-00015710: 6c69 6e65 2066 6565 6473 2061 6674 6572  line feeds after
-00015720: 2065 6e74 6974 6965 7320 7061 7273 696e   entities parsin
-00015730: 672e 0d0a 0d0a 2020 2020 2020 2020 2020  g.....          
-00015740: 2020 6578 706c 616e 6174 696f 6e5f 7061    explanation_pa
-00015750: 7273 655f 6d6f 6465 2028 3a6f 626a 3a60  rse_mode (:obj:`
-00015760: 7e66 6970 7065 722e 656e 756d 732e 5061  ~fipper.enums.Pa
-00015770: 7273 654d 6f64 6560 2c20 2a6f 7074 696f  rseMode`, *optio
-00015780: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-00015790: 2020 2020 2020 2020 4279 2064 6566 6175          By defau
-000157a0: 6c74 2c20 7465 7874 7320 6172 6520 7061  lt, texts are pa
-000157b0: 7273 6564 2075 7369 6e67 2062 6f74 6820  rsed using both 
-000157c0: 4d61 726b 646f 776e 2061 6e64 2048 544d  Markdown and HTM
-000157d0: 4c20 7374 796c 6573 2e0d 0a20 2020 2020  L styles...     
-000157e0: 2020 2020 2020 2020 2020 2059 6f75 2063             You c
-000157f0: 616e 2063 6f6d 6269 6e65 2062 6f74 6820  an combine both 
-00015800: 7379 6e74 6178 6573 2074 6f67 6574 6865  syntaxes togethe
-00015810: 722e 0d0a 0d0a 2020 2020 2020 2020 2020  r.....          
-00015820: 2020 6578 706c 616e 6174 696f 6e5f 656e    explanation_en
-00015830: 7469 7469 6573 2028 4c69 7374 206f 6620  tities (List of 
-00015840: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
-00015850: 7065 732e 4d65 7373 6167 6545 6e74 6974  pes.MessageEntit
-00015860: 7960 293a 0d0a 2020 2020 2020 2020 2020  y`):..          
-00015870: 2020 2020 2020 4c69 7374 206f 6620 7370        List of sp
-00015880: 6563 6961 6c20 656e 7469 7469 6573 2074  ecial entities t
-00015890: 6861 7420 6170 7065 6172 2069 6e20 7468  hat appear in th
-000158a0: 6520 706f 6c6c 2065 7870 6c61 6e61 7469  e poll explanati
-000158b0: 6f6e 2c20 7768 6963 6820 6361 6e20 6265  on, which can be
-000158c0: 2073 7065 6369 6669 6564 2069 6e73 7465   specified inste
-000158d0: 6164 206f 660d 0a20 2020 2020 2020 2020  ad of..         
-000158e0: 2020 2020 2020 202a 7061 7273 655f 6d6f         *parse_mo
-000158f0: 6465 2a2e 0d0a 0d0a 2020 2020 2020 2020  de*.....        
-00015900: 2020 2020 6f70 656e 5f70 6572 696f 6420      open_period 
-00015910: 2860 6069 6e74 6060 2c20 2a6f 7074 696f  (``int``, *optio
-00015920: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-00015930: 2020 2020 2020 2020 416d 6f75 6e74 206f          Amount o
-00015940: 6620 7469 6d65 2069 6e20 7365 636f 6e64  f time in second
-00015950: 7320 7468 6520 706f 6c6c 2077 696c 6c20  s the poll will 
-00015960: 6265 2061 6374 6976 6520 6166 7465 7220  be active after 
-00015970: 6372 6561 7469 6f6e 2c20 352d 3630 302e  creation, 5-600.
+00013500: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
+00013510: 6174 696f 6e20 2860 6062 6f6f 6c60 602c  ation (``bool``,
+00013520: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
+00013530: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00013540: 656e 6473 2074 6865 206d 6573 7361 6765  ends the message
+00013550: 2073 696c 656e 746c 792e 0d0a 2020 2020   silently...    
+00013560: 2020 2020 2020 2020 2020 2020 5573 6572              User
+00013570: 7320 7769 6c6c 2072 6563 6569 7665 2061  s will receive a
+00013580: 206e 6f74 6966 6963 6174 696f 6e20 7769   notification wi
+00013590: 7468 206e 6f20 736f 756e 642e 0d0a 0d0a  th no sound.....
+000135a0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+000135b0: 795f 746f 5f6d 6573 7361 6765 5f69 6420  y_to_message_id 
+000135c0: 2860 6069 6e74 6060 2c20 2a6f 7074 696f  (``int``, *optio
+000135d0: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
+000135e0: 2020 2020 2020 2020 4966 2074 6865 206d          If the m
+000135f0: 6573 7361 6765 2069 7320 6120 7265 706c  essage is a repl
+00013600: 792c 2049 4420 6f66 2074 6865 206f 7269  y, ID of the ori
+00013610: 6769 6e61 6c20 6d65 7373 6167 652e 0d0a  ginal message...
+00013620: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00013630: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00013640: 4f6e 2073 7563 6365 7373 2c20 6120 3a6f  On success, a :o
+00013650: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
+00013660: 732e 4d65 7373 6167 6573 6020 6f62 6a65  s.Messages` obje
+00013670: 6374 2069 7320 7265 7475 726e 6564 2063  ct is returned c
+00013680: 6f6e 7461 696e 696e 6720 616c 6c20 7468  ontaining all th
+00013690: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
+000136a0: 696e 676c 6520 6d65 7373 6167 6573 2073  ingle messages s
+000136b0: 656e 742e 0d0a 0d0a 2020 2020 2020 2020  ent.....        
+000136c0: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+000136d0: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+000136e0: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+000136f0: 6772 616d 2052 5043 2065 7272 6f72 2e0d  gram RPC error..
+00013700: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00013710: 2020 2020 2020 6966 2071 756f 7465 2069        if quote i
+00013720: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00013730: 2020 2020 2071 756f 7465 203d 2073 656c       quote = sel
+00013740: 662e 6368 6174 2e74 7970 6520 213d 2065  f.chat.type != e
+00013750: 6e75 6d73 2e43 6861 7454 7970 652e 5052  nums.ChatType.PR
+00013760: 4956 4154 450d 0a0d 0a20 2020 2020 2020  IVATE....       
+00013770: 2069 6620 7265 706c 795f 746f 5f6d 6573   if reply_to_mes
+00013780: 7361 6765 5f69 6420 6973 204e 6f6e 6520  sage_id is None 
+00013790: 616e 6420 7175 6f74 653a 0d0a 2020 2020  and quote:..    
+000137a0: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
+000137b0: 5f6d 6573 7361 6765 5f69 6420 3d20 7365  _message_id = se
+000137c0: 6c66 2e69 640d 0a0d 0a20 2020 2020 2020  lf.id....       
+000137d0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+000137e0: 6c66 2e5f 636c 6965 6e74 2e73 656e 645f  lf._client.send_
+000137f0: 6d65 6469 615f 6772 6f75 7028 0d0a 2020  media_group(..  
+00013800: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
+00013810: 643d 7365 6c66 2e63 6861 742e 6964 2c0d  d=self.chat.id,.
+00013820: 0a20 2020 2020 2020 2020 2020 206d 6564  .            med
+00013830: 6961 3d6d 6564 6961 2c0d 0a20 2020 2020  ia=media,..     
+00013840: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
+00013850: 6f74 6966 6963 6174 696f 6e3d 6469 7361  otification=disa
+00013860: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00013870: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00013880: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+00013890: 6964 3d72 6570 6c79 5f74 6f5f 6d65 7373  id=reply_to_mess
+000138a0: 6167 655f 6964 0d0a 2020 2020 2020 2020  age_id..        
+000138b0: 290d 0a0d 0a20 2020 2061 7379 6e63 2064  )....    async d
+000138c0: 6566 2072 6570 6c79 5f70 686f 746f 280d  ef reply_photo(.
+000138d0: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
+000138e0: 2020 2020 2020 2020 7068 6f74 6f3a 2055          photo: U
+000138f0: 6e69 6f6e 5b73 7472 2c20 4269 6e61 7279  nion[str, Binary
+00013900: 494f 5d2c 0d0a 2020 2020 2020 2020 7175  IO],..        qu
+00013910: 6f74 653a 2062 6f6f 6c20 3d20 4e6f 6e65  ote: bool = None
+00013920: 2c0d 0a20 2020 2020 2020 2063 6170 7469  ,..        capti
+00013930: 6f6e 3a20 7374 7220 3d20 2222 2c0d 0a20  on: str = "",.. 
+00013940: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
+00013950: 653a 204f 7074 696f 6e61 6c5b 2265 6e75  e: Optional["enu
+00013960: 6d73 2e50 6172 7365 4d6f 6465 225d 203d  ms.ParseMode"] =
+00013970: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00013980: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
+00013990: 3a20 4c69 7374 5b22 7479 7065 732e 4d65  : List["types.Me
+000139a0: 7373 6167 6545 6e74 6974 7922 5d20 3d20  ssageEntity"] = 
+000139b0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2074  None,..        t
+000139c0: 746c 5f73 6563 6f6e 6473 3a20 696e 7420  tl_seconds: int 
+000139d0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+000139e0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
+000139f0: 6174 696f 6e3a 2062 6f6f 6c20 3d20 4e6f  ation: bool = No
+00013a00: 6e65 2c0d 0a20 2020 2020 2020 2072 6570  ne,..        rep
+00013a10: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+00013a20: 3a20 696e 7420 3d20 4e6f 6e65 2c0d 0a20  : int = None,.. 
+00013a30: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
+00013a40: 6b75 703a 2055 6e69 6f6e 5b0d 0a20 2020  kup: Union[..   
+00013a50: 2020 2020 2020 2020 2022 7479 7065 732e           "types.
+00013a60: 496e 6c69 6e65 4b65 7962 6f61 7264 4d61  InlineKeyboardMa
+00013a70: 726b 7570 222c 0d0a 2020 2020 2020 2020  rkup",..        
+00013a80: 2020 2020 2274 7970 6573 2e52 6570 6c79      "types.Reply
+00013a90: 4b65 7962 6f61 7264 4d61 726b 7570 222c  KeyboardMarkup",
+00013aa0: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
+00013ab0: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
+00013ac0: 7264 5265 6d6f 7665 222c 0d0a 2020 2020  rdRemove",..    
+00013ad0: 2020 2020 2020 2020 2274 7970 6573 2e46          "types.F
+00013ae0: 6f72 6365 5265 706c 7922 0d0a 2020 2020  orceReply"..    
+00013af0: 2020 2020 5d20 3d20 4e6f 6e65 2c0d 0a20      ] = None,.. 
+00013b00: 2020 2020 2020 2070 726f 6772 6573 733a         progress:
+00013b10: 2043 616c 6c61 626c 6520 3d20 4e6f 6e65   Callable = None
+00013b20: 2c0d 0a20 2020 2020 2020 2070 726f 6772  ,..        progr
+00013b30: 6573 735f 6172 6773 3a20 7475 706c 6520  ess_args: tuple 
+00013b40: 3d20 2829 0d0a 2020 2020 2920 2d3e 2022  = ()..    ) -> "
+00013b50: 4d65 7373 6167 6522 3a0d 0a20 2020 2020  Message":..     
+00013b60: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+00013b70: 6f64 202a 7265 706c 795f 7068 6f74 6f2a  od *reply_photo*
+00013b80: 206f 6620 3a6f 626a 3a60 7e66 6970 7065   of :obj:`~fippe
+00013b90: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
+00013ba0: 2e0d 0a0d 0a20 2020 2020 2020 2055 7365  .....        Use
+00013bb0: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
+00013bc0: 6f72 3a0d 0a0d 0a20 2020 2020 2020 202e  or:....        .
+00013bd0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+00013be0: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
+00013bf0: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
+00013c00: 742e 7365 6e64 5f70 686f 746f 280d 0a20  t.send_photo(.. 
+00013c10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013c20: 6861 745f 6964 3d6d 6573 7361 6765 2e63  hat_id=message.c
+00013c30: 6861 742e 6964 2c0d 0a20 2020 2020 2020  hat.id,..       
+00013c40: 2020 2020 2020 2020 2070 686f 746f 3d70           photo=p
+00013c50: 686f 746f 0d0a 2020 2020 2020 2020 2020  hoto..          
+00013c60: 2020 290d 0a0d 0a20 2020 2020 2020 2045    )....        E
+00013c70: 7861 6d70 6c65 3a0d 0a20 2020 2020 2020  xample:..       
+00013c80: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
+00013c90: 636b 3a3a 2070 7974 686f 6e0d 0a0d 0a20  ck:: python.... 
+00013ca0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00013cb0: 7761 6974 206d 6573 7361 6765 2e72 6570  wait message.rep
+00013cc0: 6c79 5f70 686f 746f 2870 686f 746f 290d  ly_photo(photo).
+00013cd0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00013ce0: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
+00013cf0: 2020 2020 7068 6f74 6f20 2860 6073 7472      photo (``str
+00013d00: 6060 293a 0d0a 2020 2020 2020 2020 2020  ``):..          
+00013d10: 2020 2020 2020 5068 6f74 6f20 746f 2073        Photo to s
+00013d20: 656e 642e 0d0a 2020 2020 2020 2020 2020  end...          
+00013d30: 2020 2020 2020 5061 7373 2061 2066 696c        Pass a fil
+00013d40: 655f 6964 2061 7320 7374 7269 6e67 2074  e_id as string t
+00013d50: 6f20 7365 6e64 2061 2070 686f 746f 2074  o send a photo t
+00013d60: 6861 7420 6578 6973 7473 206f 6e20 7468  hat exists on th
+00013d70: 6520 5465 6c65 6772 616d 2073 6572 7665  e Telegram serve
+00013d80: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+00013d90: 2020 2020 2070 6173 7320 616e 2048 5454       pass an HTT
+00013da0: 5020 5552 4c20 6173 2061 2073 7472 696e  P URL as a strin
+00013db0: 6720 666f 7220 5465 6c65 6772 616d 2074  g for Telegram t
+00013dc0: 6f20 6765 7420 6120 7068 6f74 6f20 6672  o get a photo fr
+00013dd0: 6f6d 2074 6865 2049 6e74 6572 6e65 742c  om the Internet,
+00013de0: 206f 720d 0a20 2020 2020 2020 2020 2020   or..           
+00013df0: 2020 2020 2070 6173 7320 6120 6669 6c65       pass a file
+00013e00: 2070 6174 6820 6173 2073 7472 696e 6720   path as string 
+00013e10: 746f 2075 706c 6f61 6420 6120 6e65 7720  to upload a new 
+00013e20: 7068 6f74 6f20 7468 6174 2065 7869 7374  photo that exist
+00013e30: 7320 6f6e 2079 6f75 7220 6c6f 6361 6c20  s on your local 
+00013e40: 6d61 6368 696e 652e 0d0a 0d0a 2020 2020  machine.....    
+00013e50: 2020 2020 2020 2020 7175 6f74 6520 2860          quote (`
+00013e60: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
+00013e70: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+00013e80: 2020 2020 2020 2049 6620 6060 5472 7565         If ``True
+00013e90: 6060 2c20 7468 6520 6d65 7373 6167 6520  ``, the message 
+00013ea0: 7769 6c6c 2062 6520 7365 6e74 2061 7320  will be sent as 
+00013eb0: 6120 7265 706c 7920 746f 2074 6869 7320  a reply to this 
+00013ec0: 6d65 7373 6167 652e 0d0a 2020 2020 2020  message...      
+00013ed0: 2020 2020 2020 2020 2020 4966 202a 7265            If *re
+00013ee0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00013ef0: 642a 2069 7320 7061 7373 6564 2c20 7468  d* is passed, th
+00013f00: 6973 2070 6172 616d 6574 6572 2077 696c  is parameter wil
+00013f10: 6c20 6265 2069 676e 6f72 6564 2e0d 0a20  l be ignored... 
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00013f30: 6566 6175 6c74 7320 746f 2060 6054 7275  efaults to ``Tru
+00013f40: 6560 6020 696e 2067 726f 7570 2063 6861  e`` in group cha
+00013f50: 7473 2061 6e64 2060 6046 616c 7365 6060  ts and ``False``
+00013f60: 2069 6e20 7072 6976 6174 6520 6368 6174   in private chat
+00013f70: 732e 0d0a 0d0a 2020 2020 2020 2020 2020  s.....          
+00013f80: 2020 6361 7074 696f 6e20 2860 6073 7472    caption (``str
+00013f90: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+00013fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013fb0: 2020 5068 6f74 6f20 6361 7074 696f 6e2c    Photo caption,
+00013fc0: 2030 2d31 3032 3420 6368 6172 6163 7465   0-1024 characte
+00013fd0: 7273 2e0d 0a0d 0a20 2020 2020 2020 2020  rs.....         
+00013fe0: 2020 2070 6172 7365 5f6d 6f64 6520 283a     parse_mode (:
+00013ff0: 6f62 6a3a 607e 6669 7070 6572 2e65 6e75  obj:`~fipper.enu
+00014000: 6d73 2e50 6172 7365 4d6f 6465 602c 202a  ms.ParseMode`, *
+00014010: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
+00014020: 2020 2020 2020 2020 2020 2020 2042 7920               By 
+00014030: 6465 6661 756c 742c 2074 6578 7473 2061  default, texts a
+00014040: 7265 2070 6172 7365 6420 7573 696e 6720  re parsed using 
+00014050: 626f 7468 204d 6172 6b64 6f77 6e20 616e  both Markdown an
+00014060: 6420 4854 4d4c 2073 7479 6c65 732e 0d0a  d HTML styles...
+00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014080: 596f 7520 6361 6e20 636f 6d62 696e 6520  You can combine 
+00014090: 626f 7468 2073 796e 7461 7865 7320 746f  both syntaxes to
+000140a0: 6765 7468 6572 2e0d 0a0d 0a20 2020 2020  gether.....     
+000140b0: 2020 2020 2020 2063 6170 7469 6f6e 5f65         caption_e
+000140c0: 6e74 6974 6965 7320 284c 6973 7420 6f66  ntities (List of
+000140d0: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
+000140e0: 7970 6573 2e4d 6573 7361 6765 456e 7469  ypes.MessageEnti
+000140f0: 7479 6029 3a0d 0a20 2020 2020 2020 2020  ty`):..         
+00014100: 2020 2020 2020 204c 6973 7420 6f66 2073         List of s
+00014110: 7065 6369 616c 2065 6e74 6974 6965 7320  pecial entities 
+00014120: 7468 6174 2061 7070 6561 7220 696e 2074  that appear in t
+00014130: 6865 2063 6170 7469 6f6e 2c20 7768 6963  he caption, whic
+00014140: 6820 6361 6e20 6265 2073 7065 6369 6669  h can be specifi
+00014150: 6564 2069 6e73 7465 6164 206f 6620 2a70  ed instead of *p
+00014160: 6172 7365 5f6d 6f64 652a 2e0d 0a0d 0a20  arse_mode*..... 
+00014170: 2020 2020 2020 2020 2020 2074 746c 5f73             ttl_s
+00014180: 6563 6f6e 6473 2028 6060 696e 7460 602c  econds (``int``,
+00014190: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
+000141a0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+000141b0: 656c 662d 4465 7374 7275 6374 2054 696d  elf-Destruct Tim
+000141c0: 6572 2e0d 0a20 2020 2020 2020 2020 2020  er...           
+000141d0: 2020 2020 2049 6620 796f 7520 7365 7420       If you set 
+000141e0: 6120 7469 6d65 722c 2074 6865 2070 686f  a timer, the pho
+000141f0: 746f 2077 696c 6c20 7365 6c66 2d64 6573  to will self-des
+00014200: 7472 7563 7420 696e 202a 7474 6c5f 7365  truct in *ttl_se
+00014210: 636f 6e64 732a 0d0a 2020 2020 2020 2020  conds*..        
+00014220: 2020 2020 2020 2020 7365 636f 6e64 7320          seconds 
+00014230: 6166 7465 7220 6974 2077 6173 2076 6965  after it was vie
+00014240: 7765 642e 0d0a 0d0a 2020 2020 2020 2020  wed.....        
+00014250: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
+00014260: 6669 6361 7469 6f6e 2028 6060 626f 6f6c  fication (``bool
+00014270: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+00014280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014290: 2020 5365 6e64 7320 7468 6520 6d65 7373    Sends the mess
+000142a0: 6167 6520 7369 6c65 6e74 6c79 2e0d 0a20  age silently... 
+000142b0: 2020 2020 2020 2020 2020 2020 2020 2055                 U
+000142c0: 7365 7273 2077 696c 6c20 7265 6365 6976  sers will receiv
+000142d0: 6520 6120 6e6f 7469 6669 6361 7469 6f6e  e a notification
+000142e0: 2077 6974 6820 6e6f 2073 6f75 6e64 2e0d   with no sound..
+000142f0: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+00014300: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+00014310: 6964 2028 6060 696e 7460 602c 202a 6f70  id (``int``, *op
+00014320: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00014330: 2020 2020 2020 2020 2020 2049 6620 7468             If th
+00014340: 6520 6d65 7373 6167 6520 6973 2061 2072  e message is a r
+00014350: 6570 6c79 2c20 4944 206f 6620 7468 6520  eply, ID of the 
+00014360: 6f72 6967 696e 616c 206d 6573 7361 6765  original message
+00014370: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00014380: 2072 6570 6c79 5f6d 6172 6b75 7020 283a   reply_markup (:
+00014390: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+000143a0: 6573 2e49 6e6c 696e 654b 6579 626f 6172  es.InlineKeyboar
+000143b0: 644d 6172 6b75 7060 207c 203a 6f62 6a3a  dMarkup` | :obj:
+000143c0: 607e 6669 7070 6572 2e74 7970 6573 2e52  `~fipper.types.R
+000143d0: 6570 6c79 4b65 7962 6f61 7264 4d61 726b  eplyKeyboardMark
+000143e0: 7570 6020 7c20 3a6f 626a 3a60 7e66 6970  up` | :obj:`~fip
+000143f0: 7065 722e 7479 7065 732e 5265 706c 794b  per.types.ReplyK
+00014400: 6579 626f 6172 6452 656d 6f76 6560 207c  eyboardRemove` |
+00014410: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
+00014420: 7970 6573 2e46 6f72 6365 5265 706c 7960  ypes.ForceReply`
+00014430: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014450: 4164 6469 7469 6f6e 616c 2069 6e74 6572  Additional inter
+00014460: 6661 6365 206f 7074 696f 6e73 2e20 416e  face options. An
+00014470: 206f 626a 6563 7420 666f 7220 616e 2069   object for an i
+00014480: 6e6c 696e 6520 6b65 7962 6f61 7264 2c20  nline keyboard, 
+00014490: 6375 7374 6f6d 2072 6570 6c79 206b 6579  custom reply key
+000144a0: 626f 6172 642c 0d0a 2020 2020 2020 2020  board,..        
+000144b0: 2020 2020 2020 2020 696e 7374 7275 6374          instruct
+000144c0: 696f 6e73 2074 6f20 7265 6d6f 7665 2072  ions to remove r
+000144d0: 6570 6c79 206b 6579 626f 6172 6420 6f72  eply keyboard or
+000144e0: 2074 6f20 666f 7263 6520 6120 7265 706c   to force a repl
+000144f0: 7920 6672 6f6d 2074 6865 2075 7365 722e  y from the user.
+00014500: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00014510: 7072 6f67 7265 7373 2028 6060 4361 6c6c  progress (``Call
+00014520: 6162 6c65 6060 2c20 2a6f 7074 696f 6e61  able``, *optiona
+00014530: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+00014540: 2020 2020 2020 5061 7373 2061 2063 616c        Pass a cal
+00014550: 6c62 6163 6b20 6675 6e63 7469 6f6e 2074  lback function t
+00014560: 6f20 7669 6577 2074 6865 2066 696c 6520  o view the file 
+00014570: 7472 616e 736d 6973 7369 6f6e 2070 726f  transmission pro
+00014580: 6772 6573 732e 0d0a 2020 2020 2020 2020  gress...        
+00014590: 2020 2020 2020 2020 5468 6520 6675 6e63          The func
+000145a0: 7469 6f6e 206d 7573 7420 7461 6b65 202a  tion must take *
+000145b0: 2863 7572 7265 6e74 2c20 746f 7461 6c29  (current, total)
+000145c0: 2a20 6173 2070 6f73 6974 696f 6e61 6c20  * as positional 
+000145d0: 6172 6775 6d65 6e74 7320 286c 6f6f 6b20  arguments (look 
+000145e0: 6174 204f 7468 6572 2050 6172 616d 6574  at Other Paramet
+000145f0: 6572 7320 6265 6c6f 7720 666f 7220 610d  ers below for a.
+00014600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014610: 2064 6574 6169 6c65 6420 6465 7363 7269   detailed descri
+00014620: 7074 696f 6e29 2061 6e64 2077 696c 6c20  ption) and will 
+00014630: 6265 2063 616c 6c65 6420 6261 636b 2065  be called back e
+00014640: 6163 6820 7469 6d65 2061 206e 6577 2066  ach time a new f
+00014650: 696c 6520 6368 756e 6b20 6861 7320 6265  ile chunk has be
+00014660: 656e 2073 7563 6365 7373 6675 6c6c 790d  en successfully.
+00014670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014680: 2074 7261 6e73 6d69 7474 6564 2e0d 0a0d   transmitted....
+00014690: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000146a0: 6772 6573 735f 6172 6773 2028 6060 7475  gress_args (``tu
+000146b0: 706c 6560 602c 202a 6f70 7469 6f6e 616c  ple``, *optional
+000146c0: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
+000146d0: 2020 2020 2045 7874 7261 2063 7573 746f       Extra custo
+000146e0: 6d20 6172 6775 6d65 6e74 7320 666f 7220  m arguments for 
+000146f0: 7468 6520 7072 6f67 7265 7373 2063 616c  the progress cal
+00014700: 6c62 6163 6b20 6675 6e63 7469 6f6e 2e0d  lback function..
+00014710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014720: 2059 6f75 2063 616e 2070 6173 7320 616e   You can pass an
+00014730: 7974 6869 6e67 2079 6f75 206e 6565 6420  ything you need 
+00014740: 746f 2062 6520 6176 6169 6c61 626c 6520  to be available 
+00014750: 696e 2074 6865 2070 726f 6772 6573 7320  in the progress 
+00014760: 6361 6c6c 6261 636b 2073 636f 7065 3b20  callback scope; 
+00014770: 666f 7220 6578 616d 706c 652c 2061 204d  for example, a M
+00014780: 6573 7361 6765 0d0a 2020 2020 2020 2020  essage..        
+00014790: 2020 2020 2020 2020 6f62 6a65 6374 206f          object o
+000147a0: 7220 6120 436c 6965 6e74 2069 6e73 7461  r a Client insta
+000147b0: 6e63 6520 696e 206f 7264 6572 2074 6f20  nce in order to 
+000147c0: 6564 6974 2074 6865 206d 6573 7361 6765  edit the message
+000147d0: 2077 6974 6820 7468 6520 7570 6461 7465   with the update
+000147e0: 6420 7072 6f67 7265 7373 2073 7461 7475  d progress statu
+000147f0: 732e 0d0a 0d0a 2020 2020 2020 2020 4f74  s.....        Ot
+00014800: 6865 7220 5061 7261 6d65 7465 7273 3a0d  her Parameters:.
+00014810: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
+00014820: 7265 6e74 2028 6060 696e 7460 6029 3a0d  rent (``int``):.
+00014830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014840: 2054 6865 2061 6d6f 756e 7420 6f66 2062   The amount of b
+00014850: 7974 6573 2074 7261 6e73 6d69 7474 6564  ytes transmitted
+00014860: 2073 6f20 6661 722e 0d0a 0d0a 2020 2020   so far.....    
+00014870: 2020 2020 2020 2020 746f 7461 6c20 2860          total (`
+00014880: 6069 6e74 6060 293a 0d0a 2020 2020 2020  `int``):..      
+00014890: 2020 2020 2020 2020 2020 5468 6520 746f            The to
+000148a0: 7461 6c20 7369 7a65 206f 6620 7468 6520  tal size of the 
+000148b0: 6669 6c65 2e0d 0a0d 0a20 2020 2020 2020  file.....       
+000148c0: 2020 2020 202a 6172 6773 2028 6060 7475       *args (``tu
+000148d0: 706c 6560 602c 202a 6f70 7469 6f6e 616c  ple``, *optional
+000148e0: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
+000148f0: 2020 2020 2045 7874 7261 2063 7573 746f       Extra custo
+00014900: 6d20 6172 6775 6d65 6e74 7320 6173 2064  m arguments as d
+00014910: 6566 696e 6564 2069 6e20 7468 6520 6060  efined in the ``
+00014920: 7072 6f67 7265 7373 5f61 7267 7360 6020  progress_args`` 
+00014930: 7061 7261 6d65 7465 722e 0d0a 2020 2020  parameter...    
+00014940: 2020 2020 2020 2020 2020 2020 596f 7520              You 
+00014950: 6361 6e20 6569 7468 6572 206b 6565 7020  can either keep 
+00014960: 6060 2a61 7267 7360 6020 6f72 2061 6464  ``*args`` or add
+00014970: 2065 7665 7279 2073 696e 676c 6520 6578   every single ex
+00014980: 7472 6120 6172 6775 6d65 6e74 2069 6e20  tra argument in 
+00014990: 796f 7572 2066 756e 6374 696f 6e20 7369  your function si
+000149a0: 676e 6174 7572 652e 0d0a 0d0a 2020 2020  gnature.....    
+000149b0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+000149c0: 2020 2020 2020 2020 2020 4f6e 2073 7563            On suc
+000149d0: 6365 7373 2c20 7468 6520 7365 6e74 203a  cess, the sent :
+000149e0: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+000149f0: 6573 2e4d 6573 7361 6765 6020 6973 2072  es.Message` is r
+00014a00: 6574 7572 6e65 642e 0d0a 2020 2020 2020  eturned...      
+00014a10: 2020 2020 2020 496e 2063 6173 6520 7468        In case th
+00014a20: 6520 7570 6c6f 6164 2069 7320 6465 6c69  e upload is deli
+00014a30: 6265 7261 7465 6c79 2073 746f 7070 6564  berately stopped
+00014a40: 2077 6974 6820 3a6d 6574 683a 607e 6669   with :meth:`~fi
+00014a50: 7070 6572 2e43 6c69 656e 742e 7374 6f70  pper.Client.stop
+00014a60: 5f74 7261 6e73 6d69 7373 696f 6e60 2c20  _transmission`, 
+00014a70: 4e6f 6e65 2069 7320 7265 7475 726e 6564  None is returned
+00014a80: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00014a90: 7374 6561 642e 0d0a 0d0a 2020 2020 2020  stead.....      
+00014aa0: 2020 5261 6973 6573 3a0d 0a20 2020 2020    Raises:..     
+00014ab0: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
+00014ac0: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
+00014ad0: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
+00014ae0: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00014af0: 2020 2020 2020 2020 6966 2071 756f 7465          if quote
+00014b00: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00014b10: 2020 2020 2020 2071 756f 7465 203d 2073         quote = s
+00014b20: 656c 662e 6368 6174 2e74 7970 6520 213d  elf.chat.type !=
+00014b30: 2065 6e75 6d73 2e43 6861 7454 7970 652e   enums.ChatType.
+00014b40: 5052 4956 4154 450d 0a0d 0a20 2020 2020  PRIVATE....     
+00014b50: 2020 2069 6620 7265 706c 795f 746f 5f6d     if reply_to_m
+00014b60: 6573 7361 6765 5f69 6420 6973 204e 6f6e  essage_id is Non
+00014b70: 6520 616e 6420 7175 6f74 653a 0d0a 2020  e and quote:..  
+00014b80: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00014b90: 746f 5f6d 6573 7361 6765 5f69 6420 3d20  to_message_id = 
+00014ba0: 7365 6c66 2e69 640d 0a0d 0a20 2020 2020  self.id....     
+00014bb0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00014bc0: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
+00014bd0: 645f 7068 6f74 6f28 0d0a 2020 2020 2020  d_photo(..      
+00014be0: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
+00014bf0: 6c66 2e63 6861 742e 6964 2c0d 0a20 2020  lf.chat.id,..   
+00014c00: 2020 2020 2020 2020 2070 686f 746f 3d70           photo=p
+00014c10: 686f 746f 2c0d 0a20 2020 2020 2020 2020  hoto,..         
+00014c20: 2020 2063 6170 7469 6f6e 3d63 6170 7469     caption=capti
+00014c30: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
+00014c40: 2070 6172 7365 5f6d 6f64 653d 7061 7273   parse_mode=pars
+00014c50: 655f 6d6f 6465 2c0d 0a20 2020 2020 2020  e_mode,..       
+00014c60: 2020 2020 2063 6170 7469 6f6e 5f65 6e74       caption_ent
+00014c70: 6974 6965 733d 6361 7074 696f 6e5f 656e  ities=caption_en
+00014c80: 7469 7469 6573 2c0d 0a20 2020 2020 2020  tities,..       
+00014c90: 2020 2020 2074 746c 5f73 6563 6f6e 6473       ttl_seconds
+00014ca0: 3d74 746c 5f73 6563 6f6e 6473 2c0d 0a20  =ttl_seconds,.. 
+00014cb0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
+00014cc0: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
+00014cd0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00014ce0: 7469 6f6e 2c0d 0a20 2020 2020 2020 2020  tion,..         
+00014cf0: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
+00014d00: 6167 655f 6964 3d72 6570 6c79 5f74 6f5f  age_id=reply_to_
+00014d10: 6d65 7373 6167 655f 6964 2c0d 0a20 2020  message_id,..   
+00014d20: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+00014d30: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
+00014d40: 7570 2c0d 0a20 2020 2020 2020 2020 2020  up,..           
+00014d50: 2070 726f 6772 6573 733d 7072 6f67 7265   progress=progre
+00014d60: 7373 2c0d 0a20 2020 2020 2020 2020 2020  ss,..           
+00014d70: 2070 726f 6772 6573 735f 6172 6773 3d70   progress_args=p
+00014d80: 726f 6772 6573 735f 6172 6773 0d0a 2020  rogress_args..  
+00014d90: 2020 2020 2020 290d 0a0d 0a20 2020 2061        )....    a
+00014da0: 7379 6e63 2064 6566 2072 6570 6c79 5f70  sync def reply_p
+00014db0: 6f6c 6c28 0d0a 2020 2020 2020 2020 7365  oll(..        se
+00014dc0: 6c66 2c0d 0a20 2020 2020 2020 2071 7565  lf,..        que
+00014dd0: 7374 696f 6e3a 2073 7472 2c0d 0a20 2020  stion: str,..   
+00014de0: 2020 2020 206f 7074 696f 6e73 3a20 4c69       options: Li
+00014df0: 7374 5b73 7472 5d2c 0d0a 2020 2020 2020  st[str],..      
+00014e00: 2020 6973 5f61 6e6f 6e79 6d6f 7573 3a20    is_anonymous: 
+00014e10: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
+00014e20: 2020 2020 2020 7479 7065 3a20 2265 6e75        type: "enu
+00014e30: 6d73 2e50 6f6c 6c54 7970 6522 203d 2065  ms.PollType" = e
+00014e40: 6e75 6d73 2e50 6f6c 6c54 7970 652e 5245  nums.PollType.RE
+00014e50: 4755 4c41 522c 0d0a 2020 2020 2020 2020  GULAR,..        
+00014e60: 616c 6c6f 7773 5f6d 756c 7469 706c 655f  allows_multiple_
+00014e70: 616e 7377 6572 733a 2062 6f6f 6c20 3d20  answers: bool = 
+00014e80: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2063  None,..        c
+00014e90: 6f72 7265 6374 5f6f 7074 696f 6e5f 6964  orrect_option_id
+00014ea0: 3a20 696e 7420 3d20 4e6f 6e65 2c0d 0a20  : int = None,.. 
+00014eb0: 2020 2020 2020 2065 7870 6c61 6e61 7469         explanati
+00014ec0: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0d  on: str = None,.
+00014ed0: 0a20 2020 2020 2020 2065 7870 6c61 6e61  .        explana
+00014ee0: 7469 6f6e 5f70 6172 7365 5f6d 6f64 653a  tion_parse_mode:
+00014ef0: 2022 656e 756d 732e 5061 7273 654d 6f64   "enums.ParseMod
+00014f00: 6522 203d 204e 6f6e 652c 0d0a 2020 2020  e" = None,..    
+00014f10: 2020 2020 6578 706c 616e 6174 696f 6e5f      explanation_
+00014f20: 656e 7469 7469 6573 3a20 4c69 7374 5b22  entities: List["
+00014f30: 7479 7065 732e 4d65 7373 6167 6545 6e74  types.MessageEnt
+00014f40: 6974 7922 5d20 3d20 4e6f 6e65 2c0d 0a20  ity"] = None,.. 
+00014f50: 2020 2020 2020 206f 7065 6e5f 7065 7269         open_peri
+00014f60: 6f64 3a20 696e 7420 3d20 4e6f 6e65 2c0d  od: int = None,.
+00014f70: 0a20 2020 2020 2020 2063 6c6f 7365 5f64  .        close_d
+00014f80: 6174 653a 2064 6174 6574 696d 6520 3d20  ate: datetime = 
+00014f90: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2069  None,..        i
+00014fa0: 735f 636c 6f73 6564 3a20 626f 6f6c 203d  s_closed: bool =
+00014fb0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00014fc0: 7175 6f74 653a 2062 6f6f 6c20 3d20 4e6f  quote: bool = No
+00014fd0: 6e65 2c0d 0a20 2020 2020 2020 2064 6973  ne,..        dis
+00014fe0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00014ff0: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d  n: bool = None,.
+00015000: 0a20 2020 2020 2020 2070 726f 7465 6374  .        protect
+00015010: 5f63 6f6e 7465 6e74 3a20 626f 6f6c 203d  _content: bool =
+00015020: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00015030: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00015040: 5f69 643a 2069 6e74 203d 204e 6f6e 652c  _id: int = None,
+00015050: 0d0a 2020 2020 2020 2020 7363 6865 6475  ..        schedu
+00015060: 6c65 5f64 6174 653a 2064 6174 6574 696d  le_date: datetim
+00015070: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
+00015080: 2020 2072 6570 6c79 5f6d 6172 6b75 703a     reply_markup:
+00015090: 2055 6e69 6f6e 5b0d 0a20 2020 2020 2020   Union[..       
+000150a0: 2020 2020 2022 7479 7065 732e 496e 6c69       "types.Inli
+000150b0: 6e65 4b65 7962 6f61 7264 4d61 726b 7570  neKeyboardMarkup
+000150c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000150d0: 2274 7970 6573 2e52 6570 6c79 4b65 7962  "types.ReplyKeyb
+000150e0: 6f61 7264 4d61 726b 7570 222c 0d0a 2020  oardMarkup",..  
+000150f0: 2020 2020 2020 2020 2020 2274 7970 6573            "types
+00015100: 2e52 6570 6c79 4b65 7962 6f61 7264 5265  .ReplyKeyboardRe
+00015110: 6d6f 7665 222c 0d0a 2020 2020 2020 2020  move",..        
+00015120: 2020 2020 2274 7970 6573 2e46 6f72 6365      "types.Force
+00015130: 5265 706c 7922 0d0a 2020 2020 2020 2020  Reply"..        
+00015140: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 2920  ] = None..    ) 
+00015150: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
+00015160: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
+00015170: 6d65 7468 6f64 202a 7265 706c 795f 706f  method *reply_po
+00015180: 6c6c 2a20 6f66 203a 6f62 6a3a 607e 6669  ll* of :obj:`~fi
+00015190: 7070 6572 2e74 7970 6573 2e4d 6573 7361  pper.types.Messa
+000151a0: 6765 602e 0d0a 0d0a 2020 2020 2020 2020  ge`.....        
+000151b0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
+000151c0: 7420 666f 723a 0d0a 0d0a 2020 2020 2020  t for:....      
+000151d0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+000151e0: 3a20 7079 7468 6f6e 0d0a 0d0a 2020 2020  : python....    
+000151f0: 2020 2020 2020 2020 6177 6169 7420 636c          await cl
+00015200: 6965 6e74 2e73 656e 645f 706f 6c6c 280d  ient.send_poll(.
+00015210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015220: 2063 6861 745f 6964 3d6d 6573 7361 6765   chat_id=message
+00015230: 2e63 6861 742e 6964 2c0d 0a20 2020 2020  .chat.id,..     
+00015240: 2020 2020 2020 2020 2020 2071 7565 7374             quest
+00015250: 696f 6e3d 2254 6869 7320 6973 2061 2070  ion="This is a p
+00015260: 6f6c 6c22 2c0d 0a20 2020 2020 2020 2020  oll",..         
+00015270: 2020 2020 2020 206f 7074 696f 6e73 3d5b         options=[
+00015280: 2241 222c 2022 4222 2c20 2243 5d0d 0a20  "A", "B", "C].. 
+00015290: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
+000152a0: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+000152b0: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
+000152c0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+000152d0: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
+000152e0: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
+000152f0: 7373 6167 652e 7265 706c 795f 706f 6c6c  ssage.reply_poll
+00015300: 2822 5468 6973 2069 7320 6120 706f 6c6c  ("This is a poll
+00015310: 222c 205b 2241 222c 2022 4222 2c20 2243  ", ["A", "B", "C
+00015320: 225d 290d 0a0d 0a20 2020 2020 2020 2050  "])....        P
+00015330: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+00015340: 2020 2020 2020 2020 7175 6573 7469 6f6e          question
+00015350: 2028 6060 7374 7260 6029 3a0d 0a20 2020   (``str``):..   
+00015360: 2020 2020 2020 2020 2020 2020 2050 6f6c               Pol
+00015370: 6c20 7175 6573 7469 6f6e 2c20 312d 3235  l question, 1-25
+00015380: 3520 6368 6172 6163 7465 7273 2e0d 0a0d  5 characters....
+00015390: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+000153a0: 696f 6e73 2028 4c69 7374 206f 6620 6060  ions (List of ``
+000153b0: 7374 7260 6029 3a0d 0a20 2020 2020 2020  str``):..       
+000153c0: 2020 2020 2020 2020 204c 6973 7420 6f66           List of
+000153d0: 2061 6e73 7765 7220 6f70 7469 6f6e 732c   answer options,
+000153e0: 2032 2d31 3020 7374 7269 6e67 7320 312d   2-10 strings 1-
+000153f0: 3130 3020 6368 6172 6163 7465 7273 2065  100 characters e
+00015400: 6163 682e 0d0a 0d0a 2020 2020 2020 2020  ach.....        
+00015410: 2020 2020 6973 5f61 6e6f 6e79 6d6f 7573      is_anonymous
+00015420: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+00015430: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+00015440: 2020 2020 2020 2020 2020 5472 7565 2c20            True, 
+00015450: 6966 2074 6865 2070 6f6c 6c20 6e65 6564  if the poll need
+00015460: 7320 746f 2062 6520 616e 6f6e 796d 6f75  s to be anonymou
+00015470: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
+00015480: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00015490: 5472 7565 2e0d 0a0d 0a20 2020 2020 2020  True.....       
+000154a0: 2020 2020 2074 7970 6520 283a 6f62 6a60       type (:obj`
+000154b0: 7e66 6970 7065 722e 656e 756d 732e 506f  ~fipper.enums.Po
+000154c0: 6c6c 5479 7065 602c 202a 6f70 7469 6f6e  llType`, *option
+000154d0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+000154e0: 2020 2020 2020 2050 6f6c 6c20 7479 7065         Poll type
+000154f0: 2c20 3a6f 626a 3a60 7e66 6970 7065 722e  , :obj:`~fipper.
+00015500: 656e 756d 732e 506f 6c6c 5479 7065 2e51  enums.PollType.Q
+00015510: 5549 5a60 206f 7220 3a6f 626a 3a60 7e66  UIZ` or :obj:`~f
+00015520: 6970 7065 722e 656e 756d 732e 506f 6c6c  ipper.enums.Poll
+00015530: 5479 7065 2e52 4547 554c 4152 602e 0d0a  Type.REGULAR`...
+00015540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015550: 4465 6661 756c 7473 2074 6f20 3a6f 626a  Defaults to :obj
+00015560: 3a60 7e66 6970 7065 722e 656e 756d 732e  :`~fipper.enums.
+00015570: 506f 6c6c 5479 7065 2e52 4547 554c 4152  PollType.REGULAR
+00015580: 602e 0d0a 0d0a 2020 2020 2020 2020 2020  `.....          
+00015590: 2020 616c 6c6f 7773 5f6d 756c 7469 706c    allows_multipl
+000155a0: 655f 616e 7377 6572 7320 2860 6062 6f6f  e_answers (``boo
+000155b0: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
+000155c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000155d0: 2020 2054 7275 652c 2069 6620 7468 6520     True, if the 
+000155e0: 706f 6c6c 2061 6c6c 6f77 7320 6d75 6c74  poll allows mult
+000155f0: 6970 6c65 2061 6e73 7765 7273 2c20 6967  iple answers, ig
+00015600: 6e6f 7265 6420 666f 7220 706f 6c6c 7320  nored for polls 
+00015610: 696e 2071 7569 7a20 6d6f 6465 2e0d 0a20  in quiz mode... 
+00015620: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00015630: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00015640: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00015650: 2063 6f72 7265 6374 5f6f 7074 696f 6e5f   correct_option_
+00015660: 6964 2028 6060 696e 7460 602c 202a 6f70  id (``int``, *op
+00015670: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00015680: 2020 2020 2020 2020 2020 2030 2d62 6173             0-bas
+00015690: 6564 2069 6465 6e74 6966 6965 7220 6f66  ed identifier of
+000156a0: 2074 6865 2063 6f72 7265 6374 2061 6e73   the correct ans
+000156b0: 7765 7220 6f70 7469 6f6e 2c20 7265 7175  wer option, requ
+000156c0: 6972 6564 2066 6f72 2070 6f6c 6c73 2069  ired for polls i
+000156d0: 6e20 7175 697a 206d 6f64 652e 0d0a 0d0a  n quiz mode.....
+000156e0: 2020 2020 2020 2020 2020 2020 6578 706c              expl
+000156f0: 616e 6174 696f 6e20 2860 6073 7472 6060  anation (``str``
+00015700: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015720: 5465 7874 2074 6861 7420 6973 2073 686f  Text that is sho
+00015730: 776e 2077 6865 6e20 6120 7573 6572 2063  wn when a user c
+00015740: 686f 6f73 6573 2061 6e20 696e 636f 7272  hooses an incorr
+00015750: 6563 7420 616e 7377 6572 206f 7220 7461  ect answer or ta
+00015760: 7073 206f 6e20 7468 6520 6c61 6d70 2069  ps on the lamp i
+00015770: 636f 6e20 696e 2061 2071 7569 7a2d 7374  con in a quiz-st
+00015780: 796c 650d 0a20 2020 2020 2020 2020 2020  yle..           
+00015790: 2020 2020 2070 6f6c 6c2c 2030 2d32 3030       poll, 0-200
+000157a0: 2063 6861 7261 6374 6572 7320 7769 7468   characters with
+000157b0: 2061 7420 6d6f 7374 2032 206c 696e 6520   at most 2 line 
+000157c0: 6665 6564 7320 6166 7465 7220 656e 7469  feeds after enti
+000157d0: 7469 6573 2070 6172 7369 6e67 2e0d 0a0d  ties parsing....
+000157e0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+000157f0: 6c61 6e61 7469 6f6e 5f70 6172 7365 5f6d  lanation_parse_m
+00015800: 6f64 6520 283a 6f62 6a3a 607e 6669 7070  ode (:obj:`~fipp
+00015810: 6572 2e65 6e75 6d73 2e50 6172 7365 4d6f  er.enums.ParseMo
+00015820: 6465 602c 202a 6f70 7469 6f6e 616c 2a29  de`, *optional*)
+00015830: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00015840: 2020 2042 7920 6465 6661 756c 742c 2074     By default, t
+00015850: 6578 7473 2061 7265 2070 6172 7365 6420  exts are parsed 
+00015860: 7573 696e 6720 626f 7468 204d 6172 6b64  using both Markd
+00015870: 6f77 6e20 616e 6420 4854 4d4c 2073 7479  own and HTML sty
+00015880: 6c65 732e 0d0a 2020 2020 2020 2020 2020  les...          
+00015890: 2020 2020 2020 596f 7520 6361 6e20 636f        You can co
+000158a0: 6d62 696e 6520 626f 7468 2073 796e 7461  mbine both synta
+000158b0: 7865 7320 746f 6765 7468 6572 2e0d 0a0d  xes together....
+000158c0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+000158d0: 6c61 6e61 7469 6f6e 5f65 6e74 6974 6965  lanation_entitie
+000158e0: 7320 284c 6973 7420 6f66 203a 6f62 6a3a  s (List of :obj:
+000158f0: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
+00015900: 6573 7361 6765 456e 7469 7479 6029 3a0d  essageEntity`):.
+00015910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015920: 204c 6973 7420 6f66 2073 7065 6369 616c   List of special
+00015930: 2065 6e74 6974 6965 7320 7468 6174 2061   entities that a
+00015940: 7070 6561 7220 696e 2074 6865 2070 6f6c  ppear in the pol
+00015950: 6c20 6578 706c 616e 6174 696f 6e2c 2077  l explanation, w
+00015960: 6869 6368 2063 616e 2062 6520 7370 6563  hich can be spec
+00015970: 6966 6965 6420 696e 7374 6561 6420 6f66  ified instead of
 00015980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015990: 2020 4361 6e27 7420 6265 2075 7365 6420    Can't be used 
-000159a0: 746f 6765 7468 6572 2077 6974 6820 2a63  together with *c
-000159b0: 6c6f 7365 5f64 6174 652a 2e0d 0a0d 0a20  lose_date*..... 
-000159c0: 2020 2020 2020 2020 2020 2063 6c6f 7365             close
-000159d0: 5f64 6174 6520 283a 7079 3a6f 626a 3a60  _date (:py:obj:`
-000159e0: 7e64 6174 6574 696d 652e 6461 7465 7469  ~datetime.dateti
-000159f0: 6d65 602c 202a 6f70 7469 6f6e 616c 2a29  me`, *optional*)
-00015a00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015a10: 2020 2050 6f69 6e74 2069 6e20 7469 6d65     Point in time
-00015a20: 2077 6865 6e20 7468 6520 706f 6c6c 2077   when the poll w
-00015a30: 696c 6c20 6265 2061 7574 6f6d 6174 6963  ill be automatic
-00015a40: 616c 6c79 2063 6c6f 7365 642e 0d0a 2020  ally closed...  
-00015a50: 2020 2020 2020 2020 2020 2020 2020 4d75                Mu
-00015a60: 7374 2062 6520 6174 206c 6561 7374 2035  st be at least 5
-00015a70: 2061 6e64 206e 6f20 6d6f 7265 2074 6861   and no more tha
-00015a80: 6e20 3630 3020 7365 636f 6e64 7320 696e  n 600 seconds in
-00015a90: 2074 6865 2066 7574 7572 652e 0d0a 2020   the future...  
-00015aa0: 2020 2020 2020 2020 2020 2020 2020 4361                Ca
-00015ab0: 6e27 7420 6265 2075 7365 6420 746f 6765  n't be used toge
-00015ac0: 7468 6572 2077 6974 6820 2a6f 7065 6e5f  ther with *open_
-00015ad0: 7065 7269 6f64 2a2e 0d0a 0d0a 2020 2020  period*.....    
-00015ae0: 2020 2020 2020 2020 6973 5f63 6c6f 7365          is_close
-00015af0: 6420 2860 6062 6f6f 6c60 602c 202a 6f70  d (``bool``, *op
-00015b00: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-00015b10: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-00015b20: 5472 7565 2c20 6966 2074 6865 2070 6f6c  True, if the pol
-00015b30: 6c20 6e65 6564 7320 746f 2062 6520 696d  l needs to be im
-00015b40: 6d65 6469 6174 656c 7920 636c 6f73 6564  mediately closed
-00015b50: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015b60: 2020 2054 6869 7320 6361 6e20 6265 2075     This can be u
-00015b70: 7365 6675 6c20 666f 7220 706f 6c6c 2070  seful for poll p
-00015b80: 7265 7669 6577 2e0d 0a0d 0a20 2020 2020  review.....     
-00015b90: 2020 2020 2020 2071 756f 7465 2028 6060         quote (``
+00015990: 2020 2a70 6172 7365 5f6d 6f64 652a 2e0d    *parse_mode*..
+000159a0: 0a0d 0a20 2020 2020 2020 2020 2020 206f  ...            o
+000159b0: 7065 6e5f 7065 7269 6f64 2028 6060 696e  pen_period (``in
+000159c0: 7460 602c 202a 6f70 7469 6f6e 616c 2a29  t``, *optional*)
+000159d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000159e0: 2020 2041 6d6f 756e 7420 6f66 2074 696d     Amount of tim
+000159f0: 6520 696e 2073 6563 6f6e 6473 2074 6865  e in seconds the
+00015a00: 2070 6f6c 6c20 7769 6c6c 2062 6520 6163   poll will be ac
+00015a10: 7469 7665 2061 6674 6572 2063 7265 6174  tive after creat
+00015a20: 696f 6e2c 2035 2d36 3030 2e0d 0a20 2020  ion, 5-600...   
+00015a30: 2020 2020 2020 2020 2020 2020 2043 616e               Can
+00015a40: 2774 2062 6520 7573 6564 2074 6f67 6574  't be used toget
+00015a50: 6865 7220 7769 7468 202a 636c 6f73 655f  her with *close_
+00015a60: 6461 7465 2a2e 0d0a 0d0a 2020 2020 2020  date*.....      
+00015a70: 2020 2020 2020 636c 6f73 655f 6461 7465        close_date
+00015a80: 2028 3a70 793a 6f62 6a3a 607e 6461 7465   (:py:obj:`~date
+00015a90: 7469 6d65 2e64 6174 6574 696d 6560 2c20  time.datetime`, 
+00015aa0: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+00015ab0: 2020 2020 2020 2020 2020 2020 2020 506f                Po
+00015ac0: 696e 7420 696e 2074 696d 6520 7768 656e  int in time when
+00015ad0: 2074 6865 2070 6f6c 6c20 7769 6c6c 2062   the poll will b
+00015ae0: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
+00015af0: 636c 6f73 6564 2e0d 0a20 2020 2020 2020  closed...       
+00015b00: 2020 2020 2020 2020 204d 7573 7420 6265           Must be
+00015b10: 2061 7420 6c65 6173 7420 3520 616e 6420   at least 5 and 
+00015b20: 6e6f 206d 6f72 6520 7468 616e 2036 3030  no more than 600
+00015b30: 2073 6563 6f6e 6473 2069 6e20 7468 6520   seconds in the 
+00015b40: 6675 7475 7265 2e0d 0a20 2020 2020 2020  future...       
+00015b50: 2020 2020 2020 2020 2043 616e 2774 2062           Can't b
+00015b60: 6520 7573 6564 2074 6f67 6574 6865 7220  e used together 
+00015b70: 7769 7468 202a 6f70 656e 5f70 6572 696f  with *open_perio
+00015b80: 642a 2e0d 0a0d 0a20 2020 2020 2020 2020  d*.....         
+00015b90: 2020 2069 735f 636c 6f73 6564 2028 6060     is_closed (``
 00015ba0: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
 00015bb0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-00015bc0: 2020 2020 2020 4966 2060 6054 7275 6560        If ``True`
-00015bd0: 602c 2074 6865 206d 6573 7361 6765 2077  `, the message w
-00015be0: 696c 6c20 6265 2073 656e 7420 6173 2061  ill be sent as a
-00015bf0: 2072 6570 6c79 2074 6f20 7468 6973 206d   reply to this m
-00015c00: 6573 7361 6765 2e0d 0a20 2020 2020 2020  essage...       
-00015c10: 2020 2020 2020 2020 2049 6620 2a72 6570           If *rep
-00015c20: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-00015c30: 2a20 6973 2070 6173 7365 642c 2074 6869  * is passed, thi
-00015c40: 7320 7061 7261 6d65 7465 7220 7769 6c6c  s parameter will
-00015c50: 2062 6520 6967 6e6f 7265 642e 0d0a 2020   be ignored...  
-00015c60: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00015c70: 6661 756c 7473 2074 6f20 6060 5472 7565  faults to ``True
-00015c80: 6060 2069 6e20 6772 6f75 7020 6368 6174  `` in group chat
-00015c90: 7320 616e 6420 6060 4661 6c73 6560 6020  s and ``False`` 
-00015ca0: 696e 2070 7269 7661 7465 2063 6861 7473  in private chats
-00015cb0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00015cc0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-00015cd0: 6174 696f 6e20 2860 6062 6f6f 6c60 602c  ation (``bool``,
-00015ce0: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
-00015cf0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00015d00: 656e 6473 2074 6865 206d 6573 7361 6765  ends the message
-00015d10: 2073 696c 656e 746c 792e 0d0a 2020 2020   silently...    
-00015d20: 2020 2020 2020 2020 2020 2020 5573 6572              User
-00015d30: 7320 7769 6c6c 2072 6563 6569 7665 2061  s will receive a
-00015d40: 206e 6f74 6966 6963 6174 696f 6e20 7769   notification wi
-00015d50: 7468 206e 6f20 736f 756e 642e 0d0a 0d0a  th no sound.....
-00015d60: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-00015d70: 6563 745f 636f 6e74 656e 7420 2860 6062  ect_content (``b
-00015d80: 6f6f 6c60 602c 202a 6f70 7469 6f6e 616c  ool``, *optional
-00015d90: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-00015da0: 2020 2020 2050 726f 7465 6374 7320 7468       Protects th
-00015db0: 6520 636f 6e74 656e 7473 206f 6620 7468  e contents of th
-00015dc0: 6520 7365 6e74 206d 6573 7361 6765 2066  e sent message f
-00015dd0: 726f 6d20 666f 7277 6172 6469 6e67 2061  rom forwarding a
-00015de0: 6e64 2073 6176 696e 672e 0d0a 0d0a 2020  nd saving.....  
-00015df0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-00015e00: 746f 5f6d 6573 7361 6765 5f69 6420 2860  to_message_id (`
-00015e10: 6069 6e74 6060 2c20 2a6f 7074 696f 6e61  `int``, *optiona
-00015e20: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-00015e30: 2020 2020 2020 4966 2074 6865 206d 6573        If the mes
-00015e40: 7361 6765 2069 7320 6120 7265 706c 792c  sage is a reply,
-00015e50: 2049 4420 6f66 2074 6865 206f 7269 6769   ID of the origi
-00015e60: 6e61 6c20 6d65 7373 6167 652e 0d0a 0d0a  nal message.....
-00015e70: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-00015e80: 6475 6c65 5f64 6174 6520 283a 7079 3a6f  dule_date (:py:o
-00015e90: 626a 3a60 7e64 6174 6574 696d 652e 6461  bj:`~datetime.da
-00015ea0: 7465 7469 6d65 602c 202a 6f70 7469 6f6e  tetime`, *option
-00015eb0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
-00015ec0: 2020 2020 2020 2044 6174 6520 7768 656e         Date when
-00015ed0: 2074 6865 206d 6573 7361 6765 2077 696c   the message wil
-00015ee0: 6c20 6265 2061 7574 6f6d 6174 6963 616c  l be automatical
-00015ef0: 6c79 2073 656e 742e 0d0a 0d0a 2020 2020  ly sent.....    
-00015f00: 2020 2020 2020 2020 7265 706c 795f 6d61          reply_ma
-00015f10: 726b 7570 2028 3a6f 626a 3a60 7e66 6970  rkup (:obj:`~fip
-00015f20: 7065 722e 7479 7065 732e 496e 6c69 6e65  per.types.Inline
-00015f30: 4b65 7962 6f61 7264 4d61 726b 7570 6020  KeyboardMarkup` 
-00015f40: 7c20 3a6f 626a 3a60 7e66 6970 7065 722e  | :obj:`~fipper.
-00015f50: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
-00015f60: 6172 644d 6172 6b75 7060 207c 203a 6f62  ardMarkup` | :ob
-00015f70: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
-00015f80: 2e52 6570 6c79 4b65 7962 6f61 7264 5265  .ReplyKeyboardRe
-00015f90: 6d6f 7665 6020 7c20 3a6f 626a 3a60 7e66  move` | :obj:`~f
-00015fa0: 6970 7065 722e 7479 7065 732e 466f 7263  ipper.types.Forc
-00015fb0: 6552 6570 6c79 602c 202a 6f70 7469 6f6e  eReply`, *option
-00015fc0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
-00015fd0: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
-00015fe0: 6c20 696e 7465 7266 6163 6520 6f70 7469  l interface opti
-00015ff0: 6f6e 732e 2041 6e20 6f62 6a65 6374 2066  ons. An object f
-00016000: 6f72 2061 6e20 696e 6c69 6e65 206b 6579  or an inline key
-00016010: 626f 6172 642c 2063 7573 746f 6d20 7265  board, custom re
-00016020: 706c 7920 6b65 7962 6f61 7264 2c0d 0a20  ply keyboard,.. 
-00016030: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016040: 6e73 7472 7563 7469 6f6e 7320 746f 2072  nstructions to r
-00016050: 656d 6f76 6520 7265 706c 7920 6b65 7962  emove reply keyb
-00016060: 6f61 7264 206f 7220 746f 2066 6f72 6365  oard or to force
-00016070: 2061 2072 6570 6c79 2066 726f 6d20 7468   a reply from th
-00016080: 6520 7573 6572 2e0d 0a0d 0a20 2020 2020  e user.....     
-00016090: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-000160a0: 2020 2020 2020 2020 204f 6e20 7375 6363           On succ
-000160b0: 6573 732c 2074 6865 2073 656e 7420 3a6f  ess, the sent :o
-000160c0: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
-000160d0: 732e 4d65 7373 6167 6560 2069 7320 7265  s.Message` is re
-000160e0: 7475 726e 6564 2e0d 0a0d 0a20 2020 2020  turned.....     
-000160f0: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
-00016100: 2020 2020 2020 2020 5250 4345 7272 6f72          RPCError
-00016110: 3a20 496e 2063 6173 6520 6f66 2061 2054  : In case of a T
-00016120: 656c 6567 7261 6d20 5250 4320 6572 726f  elegram RPC erro
-00016130: 722e 0d0a 2020 2020 2020 2020 2222 220d  r...        """.
-00016140: 0a20 2020 2020 2020 2069 6620 7175 6f74  .        if quot
-00016150: 6520 6973 204e 6f6e 653a 0d0a 2020 2020  e is None:..    
-00016160: 2020 2020 2020 2020 7175 6f74 6520 3d20          quote = 
-00016170: 7365 6c66 2e63 6861 742e 7479 7065 2021  self.chat.type !
-00016180: 3d20 656e 756d 732e 4368 6174 5479 7065  = enums.ChatType
-00016190: 2e50 5249 5641 5445 0d0a 0d0a 2020 2020  .PRIVATE....    
-000161a0: 2020 2020 6966 2072 6570 6c79 5f74 6f5f      if reply_to_
-000161b0: 6d65 7373 6167 655f 6964 2069 7320 4e6f  message_id is No
-000161c0: 6e65 2061 6e64 2071 756f 7465 3a0d 0a20  ne and quote:.. 
-000161d0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-000161e0: 5f74 6f5f 6d65 7373 6167 655f 6964 203d  _to_message_id =
-000161f0: 2073 656c 662e 6964 0d0a 0d0a 2020 2020   self.id....    
-00016200: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00016210: 2073 656c 662e 5f63 6c69 656e 742e 7365   self._client.se
-00016220: 6e64 5f70 6f6c 6c28 0d0a 2020 2020 2020  nd_poll(..      
-00016230: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
-00016240: 6c66 2e63 6861 742e 6964 2c0d 0a20 2020  lf.chat.id,..   
-00016250: 2020 2020 2020 2020 2071 7565 7374 696f           questio
-00016260: 6e3d 7175 6573 7469 6f6e 2c0d 0a20 2020  n=question,..   
-00016270: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-00016280: 3d6f 7074 696f 6e73 2c0d 0a20 2020 2020  =options,..     
-00016290: 2020 2020 2020 2069 735f 616e 6f6e 796d         is_anonym
-000162a0: 6f75 733d 6973 5f61 6e6f 6e79 6d6f 7573  ous=is_anonymous
-000162b0: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-000162c0: 7970 653d 7479 7065 2c0d 0a20 2020 2020  ype=type,..     
-000162d0: 2020 2020 2020 2061 6c6c 6f77 735f 6d75         allows_mu
-000162e0: 6c74 6970 6c65 5f61 6e73 7765 7273 3d61  ltiple_answers=a
-000162f0: 6c6c 6f77 735f 6d75 6c74 6970 6c65 5f61  llows_multiple_a
-00016300: 6e73 7765 7273 2c0d 0a20 2020 2020 2020  nswers,..       
-00016310: 2020 2020 2063 6f72 7265 6374 5f6f 7074       correct_opt
-00016320: 696f 6e5f 6964 3d63 6f72 7265 6374 5f6f  ion_id=correct_o
-00016330: 7074 696f 6e5f 6964 2c0d 0a20 2020 2020  ption_id,..     
-00016340: 2020 2020 2020 2065 7870 6c61 6e61 7469         explanati
-00016350: 6f6e 3d65 7870 6c61 6e61 7469 6f6e 2c0d  on=explanation,.
-00016360: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-00016370: 6c61 6e61 7469 6f6e 5f70 6172 7365 5f6d  lanation_parse_m
-00016380: 6f64 653d 6578 706c 616e 6174 696f 6e5f  ode=explanation_
-00016390: 7061 7273 655f 6d6f 6465 2c0d 0a20 2020  parse_mode,..   
-000163a0: 2020 2020 2020 2020 2065 7870 6c61 6e61           explana
-000163b0: 7469 6f6e 5f65 6e74 6974 6965 733d 6578  tion_entities=ex
-000163c0: 706c 616e 6174 696f 6e5f 656e 7469 7469  planation_entiti
-000163d0: 6573 2c0d 0a20 2020 2020 2020 2020 2020  es,..           
-000163e0: 206f 7065 6e5f 7065 7269 6f64 3d6f 7065   open_period=ope
-000163f0: 6e5f 7065 7269 6f64 2c0d 0a20 2020 2020  n_period,..     
-00016400: 2020 2020 2020 2063 6c6f 7365 5f64 6174         close_dat
-00016410: 653d 636c 6f73 655f 6461 7465 2c0d 0a20  e=close_date,.. 
-00016420: 2020 2020 2020 2020 2020 2069 735f 636c             is_cl
-00016430: 6f73 6564 3d69 735f 636c 6f73 6564 2c0d  osed=is_closed,.
-00016440: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00016450: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00016460: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
-00016470: 6361 7469 6f6e 2c0d 0a20 2020 2020 2020  cation,..       
-00016480: 2020 2020 2070 726f 7465 6374 5f63 6f6e       protect_con
-00016490: 7465 6e74 3d70 726f 7465 6374 5f63 6f6e  tent=protect_con
-000164a0: 7465 6e74 2c0d 0a20 2020 2020 2020 2020  tent,..         
-000164b0: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
-000164c0: 6167 655f 6964 3d72 6570 6c79 5f74 6f5f  age_id=reply_to_
-000164d0: 6d65 7373 6167 655f 6964 2c0d 0a20 2020  message_id,..   
-000164e0: 2020 2020 2020 2020 2073 6368 6564 756c           schedul
-000164f0: 655f 6461 7465 3d73 6368 6564 756c 655f  e_date=schedule_
-00016500: 6461 7465 2c0d 0a20 2020 2020 2020 2020  date,..         
-00016510: 2020 2072 6570 6c79 5f6d 6172 6b75 703d     reply_markup=
-00016520: 7265 706c 795f 6d61 726b 7570 0d0a 2020  reply_markup..  
-00016530: 2020 2020 2020 290d 0a0d 0a20 2020 2061        )....    a
-00016540: 7379 6e63 2064 6566 2072 6570 6c79 5f73  sync def reply_s
-00016550: 7469 636b 6572 280d 0a20 2020 2020 2020  ticker(..       
-00016560: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-00016570: 7374 6963 6b65 723a 2055 6e69 6f6e 5b73  sticker: Union[s
-00016580: 7472 2c20 4269 6e61 7279 494f 5d2c 0d0a  tr, BinaryIO],..
-00016590: 2020 2020 2020 2020 7175 6f74 653a 2062          quote: b
-000165a0: 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20 2020  ool = None,..   
-000165b0: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
-000165c0: 6966 6963 6174 696f 6e3a 2062 6f6f 6c20  ification: bool 
-000165d0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-000165e0: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
-000165f0: 655f 6964 3a20 696e 7420 3d20 4e6f 6e65  e_id: int = None
-00016600: 2c0d 0a20 2020 2020 2020 2072 6570 6c79  ,..        reply
-00016610: 5f6d 6172 6b75 703a 2055 6e69 6f6e 5b0d  _markup: Union[.
-00016620: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00016630: 7065 732e 496e 6c69 6e65 4b65 7962 6f61  pes.InlineKeyboa
-00016640: 7264 4d61 726b 7570 222c 0d0a 2020 2020  rdMarkup",..    
-00016650: 2020 2020 2020 2020 2274 7970 6573 2e52          "types.R
-00016660: 6570 6c79 4b65 7962 6f61 7264 4d61 726b  eplyKeyboardMark
-00016670: 7570 222c 0d0a 2020 2020 2020 2020 2020  up",..          
-00016680: 2020 2274 7970 6573 2e52 6570 6c79 4b65    "types.ReplyKe
-00016690: 7962 6f61 7264 5265 6d6f 7665 222c 0d0a  yboardRemove",..
-000166a0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000166b0: 6573 2e46 6f72 6365 5265 706c 7922 0d0a  es.ForceReply"..
-000166c0: 2020 2020 2020 2020 5d20 3d20 4e6f 6e65          ] = None
-000166d0: 2c0d 0a20 2020 2020 2020 2070 726f 6772  ,..        progr
-000166e0: 6573 733a 2043 616c 6c61 626c 6520 3d20  ess: Callable = 
-000166f0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2070  None,..        p
-00016700: 726f 6772 6573 735f 6172 6773 3a20 7475  rogress_args: tu
-00016710: 706c 6520 3d20 2829 0d0a 2020 2020 2920  ple = ()..    ) 
-00016720: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
-00016730: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
-00016740: 6d65 7468 6f64 202a 7265 706c 795f 7374  method *reply_st
-00016750: 6963 6b65 722a 206f 6620 3a6f 626a 3a60  icker* of :obj:`
-00016760: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
-00016770: 7373 6167 6560 2e0d 0a0d 0a20 2020 2020  ssage`.....     
-00016780: 2020 2055 7365 2061 7320 6120 7368 6f72     Use as a shor
-00016790: 7463 7574 2066 6f72 3a0d 0a0d 0a20 2020  tcut for:....   
-000167a0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-000167b0: 636b 3a3a 2070 7974 686f 6e0d 0a0d 0a20  ck:: python.... 
-000167c0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-000167d0: 2063 6c69 656e 742e 7365 6e64 5f73 7469   client.send_sti
-000167e0: 636b 6572 280d 0a20 2020 2020 2020 2020  cker(..         
-000167f0: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
-00016800: 6573 7361 6765 2e63 6861 742e 6964 2c0d  essage.chat.id,.
-00016810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016820: 2073 7469 636b 6572 3d73 7469 636b 6572   sticker=sticker
-00016830: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00016840: 0a0d 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-00016850: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
-00016860: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
-00016870: 2070 7974 686f 6e0d 0a0d 0a20 2020 2020   python....     
-00016880: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00016890: 206d 6573 7361 6765 2e72 6570 6c79 5f73   message.reply_s
-000168a0: 7469 636b 6572 2873 7469 636b 6572 290d  ticker(sticker).
-000168b0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-000168c0: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
-000168d0: 2020 2020 7374 6963 6b65 7220 2860 6073      sticker (``s
-000168e0: 7472 6060 293a 0d0a 2020 2020 2020 2020  tr``):..        
-000168f0: 2020 2020 2020 2020 5374 6963 6b65 7220          Sticker 
-00016900: 746f 2073 656e 642e 0d0a 2020 2020 2020  to send...      
-00016910: 2020 2020 2020 2020 2020 5061 7373 2061            Pass a
-00016920: 2066 696c 655f 6964 2061 7320 7374 7269   file_id as stri
-00016930: 6e67 2074 6f20 7365 6e64 2061 2073 7469  ng to send a sti
-00016940: 636b 6572 2074 6861 7420 6578 6973 7473  cker that exists
-00016950: 206f 6e20 7468 6520 5465 6c65 6772 616d   on the Telegram
-00016960: 2073 6572 7665 7273 2c0d 0a20 2020 2020   servers,..     
-00016970: 2020 2020 2020 2020 2020 2070 6173 7320             pass 
-00016980: 616e 2048 5454 5020 5552 4c20 6173 2061  an HTTP URL as a
-00016990: 2073 7472 696e 6720 666f 7220 5465 6c65   string for Tele
-000169a0: 6772 616d 2074 6f20 6765 7420 6120 2e77  gram to get a .w
-000169b0: 6562 7020 7374 6963 6b65 7220 6669 6c65  ebp sticker file
-000169c0: 2066 726f 6d20 7468 6520 496e 7465 726e   from the Intern
-000169d0: 6574 2c20 6f72 0d0a 2020 2020 2020 2020  et, or..        
-000169e0: 2020 2020 2020 2020 7061 7373 2061 2066          pass a f
-000169f0: 696c 6520 7061 7468 2061 7320 7374 7269  ile path as stri
-00016a00: 6e67 2074 6f20 7570 6c6f 6164 2061 206e  ng to upload a n
-00016a10: 6577 2073 7469 636b 6572 2074 6861 7420  ew sticker that 
-00016a20: 6578 6973 7473 206f 6e20 796f 7572 206c  exists on your l
-00016a30: 6f63 616c 206d 6163 6869 6e65 2e0d 0a0d  ocal machine....
-00016a40: 0a20 2020 2020 2020 2020 2020 2071 756f  .            quo
-00016a50: 7465 2028 6060 626f 6f6c 6060 2c20 2a6f  te (``bool``, *o
-00016a60: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-00016a70: 2020 2020 2020 2020 2020 2020 4966 2060              If `
-00016a80: 6054 7275 6560 602c 2074 6865 206d 6573  `True``, the mes
-00016a90: 7361 6765 2077 696c 6c20 6265 2073 656e  sage will be sen
-00016aa0: 7420 6173 2061 2072 6570 6c79 2074 6f20  t as a reply to 
-00016ab0: 7468 6973 206d 6573 7361 6765 2e0d 0a20  this message... 
-00016ac0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-00016ad0: 6620 2a72 6570 6c79 5f74 6f5f 6d65 7373  f *reply_to_mess
-00016ae0: 6167 655f 6964 2a20 6973 2070 6173 7365  age_id* is passe
-00016af0: 642c 2074 6869 7320 7061 7261 6d65 7465  d, this paramete
-00016b00: 7220 7769 6c6c 2062 6520 6967 6e6f 7265  r will be ignore
-00016b10: 642e 0d0a 2020 2020 2020 2020 2020 2020  d...            
-00016b20: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00016b30: 6060 5472 7565 6060 2069 6e20 6772 6f75  ``True`` in grou
-00016b40: 7020 6368 6174 7320 616e 6420 6060 4661  p chats and ``Fa
-00016b50: 6c73 6560 6020 696e 2070 7269 7661 7465  lse`` in private
-00016b60: 2063 6861 7473 2e0d 0a0d 0a20 2020 2020   chats.....     
-00016b70: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
-00016b80: 6f74 6966 6963 6174 696f 6e20 2860 6062  otification (``b
-00016b90: 6f6f 6c60 602c 202a 6f70 7469 6f6e 616c  ool``, *optional
-00016ba0: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-00016bb0: 2020 2020 2053 656e 6473 2074 6865 206d       Sends the m
-00016bc0: 6573 7361 6765 2073 696c 656e 746c 792e  essage silently.
-00016bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016be0: 2020 5573 6572 7320 7769 6c6c 2072 6563    Users will rec
-00016bf0: 6569 7665 2061 206e 6f74 6966 6963 6174  eive a notificat
-00016c00: 696f 6e20 7769 7468 206e 6f20 736f 756e  ion with no soun
-00016c10: 642e 0d0a 0d0a 2020 2020 2020 2020 2020  d.....          
-00016c20: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00016c30: 6765 5f69 6420 2860 6069 6e74 6060 2c20  ge_id (``int``, 
-00016c40: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
-00016c50: 2020 2020 2020 2020 2020 2020 2020 4966                If
-00016c60: 2074 6865 206d 6573 7361 6765 2069 7320   the message is 
-00016c70: 6120 7265 706c 792c 2049 4420 6f66 2074  a reply, ID of t
-00016c80: 6865 206f 7269 6769 6e61 6c20 6d65 7373  he original mess
-00016c90: 6167 652e 0d0a 0d0a 2020 2020 2020 2020  age.....        
-00016ca0: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
-00016cb0: 2028 3a6f 626a 3a60 7e66 6970 7065 722e   (:obj:`~fipper.
-00016cc0: 7479 7065 732e 496e 6c69 6e65 4b65 7962  types.InlineKeyb
-00016cd0: 6f61 7264 4d61 726b 7570 6020 7c20 3a6f  oardMarkup` | :o
-00016ce0: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
-00016cf0: 732e 5265 706c 794b 6579 626f 6172 644d  s.ReplyKeyboardM
-00016d00: 6172 6b75 7060 207c 203a 6f62 6a3a 607e  arkup` | :obj:`~
-00016d10: 6669 7070 6572 2e74 7970 6573 2e52 6570  fipper.types.Rep
-00016d20: 6c79 4b65 7962 6f61 7264 5265 6d6f 7665  lyKeyboardRemove
-00016d30: 6020 7c20 3a6f 626a 3a60 7e66 6970 7065  ` | :obj:`~fippe
-00016d40: 722e 7479 7065 732e 466f 7263 6552 6570  r.types.ForceRep
-00016d50: 6c79 602c 202a 6f70 7469 6f6e 616c 2a29  ly`, *optional*)
-00016d60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016d70: 2020 2041 6464 6974 696f 6e61 6c20 696e     Additional in
-00016d80: 7465 7266 6163 6520 6f70 7469 6f6e 732e  terface options.
-00016d90: 2041 6e20 6f62 6a65 6374 2066 6f72 2061   An object for a
-00016da0: 6e20 696e 6c69 6e65 206b 6579 626f 6172  n inline keyboar
-00016db0: 642c 2063 7573 746f 6d20 7265 706c 7920  d, custom reply 
-00016dc0: 6b65 7962 6f61 7264 2c0d 0a20 2020 2020  keyboard,..     
-00016dd0: 2020 2020 2020 2020 2020 2069 6e73 7472             instr
-00016de0: 7563 7469 6f6e 7320 746f 2072 656d 6f76  uctions to remov
-00016df0: 6520 7265 706c 7920 6b65 7962 6f61 7264  e reply keyboard
-00016e00: 206f 7220 746f 2066 6f72 6365 2061 2072   or to force a r
-00016e10: 6570 6c79 2066 726f 6d20 7468 6520 7573  eply from the us
-00016e20: 6572 2e0d 0a0d 0a20 2020 2020 2020 2020  er.....         
-00016e30: 2020 2070 726f 6772 6573 7320 2860 6043     progress (``C
-00016e40: 616c 6c61 626c 6560 602c 202a 6f70 7469  allable``, *opti
-00016e50: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
-00016e60: 2020 2020 2020 2020 2050 6173 7320 6120           Pass a 
-00016e70: 6361 6c6c 6261 636b 2066 756e 6374 696f  callback functio
-00016e80: 6e20 746f 2076 6965 7720 7468 6520 6669  n to view the fi
-00016e90: 6c65 2074 7261 6e73 6d69 7373 696f 6e20  le transmission 
-00016ea0: 7072 6f67 7265 7373 2e0d 0a20 2020 2020  progress...     
-00016eb0: 2020 2020 2020 2020 2020 2054 6865 2066             The f
-00016ec0: 756e 6374 696f 6e20 6d75 7374 2074 616b  unction must tak
-00016ed0: 6520 2a28 6375 7272 656e 742c 2074 6f74  e *(current, tot
-00016ee0: 616c 292a 2061 7320 706f 7369 7469 6f6e  al)* as position
-00016ef0: 616c 2061 7267 756d 656e 7473 2028 6c6f  al arguments (lo
-00016f00: 6f6b 2061 7420 4f74 6865 7220 5061 7261  ok at Other Para
-00016f10: 6d65 7465 7273 2062 656c 6f77 2066 6f72  meters below for
-00016f20: 2061 0d0a 2020 2020 2020 2020 2020 2020   a..            
-00016f30: 2020 2020 6465 7461 696c 6564 2064 6573      detailed des
-00016f40: 6372 6970 7469 6f6e 2920 616e 6420 7769  cription) and wi
-00016f50: 6c6c 2062 6520 6361 6c6c 6564 2062 6163  ll be called bac
-00016f60: 6b20 6561 6368 2074 696d 6520 6120 6e65  k each time a ne
-00016f70: 7720 6669 6c65 2063 6875 6e6b 2068 6173  w file chunk has
-00016f80: 2062 6565 6e20 7375 6363 6573 7366 756c   been successful
-00016f90: 6c79 0d0a 2020 2020 2020 2020 2020 2020  ly..            
-00016fa0: 2020 2020 7472 616e 736d 6974 7465 642e      transmitted.
-00016fb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016fc0: 7072 6f67 7265 7373 5f61 7267 7320 2860  progress_args (`
-00016fd0: 6074 7570 6c65 6060 2c20 2a6f 7074 696f  `tuple``, *optio
-00016fe0: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-00016ff0: 2020 2020 2020 2020 4578 7472 6120 6375          Extra cu
-00017000: 7374 6f6d 2061 7267 756d 656e 7473 2066  stom arguments f
-00017010: 6f72 2074 6865 2070 726f 6772 6573 7320  or the progress 
-00017020: 6361 6c6c 6261 636b 2066 756e 6374 696f  callback functio
-00017030: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
-00017040: 2020 2020 596f 7520 6361 6e20 7061 7373      You can pass
-00017050: 2061 6e79 7468 696e 6720 796f 7520 6e65   anything you ne
-00017060: 6564 2074 6f20 6265 2061 7661 696c 6162  ed to be availab
-00017070: 6c65 2069 6e20 7468 6520 7072 6f67 7265  le in the progre
-00017080: 7373 2063 616c 6c62 6163 6b20 7363 6f70  ss callback scop
-00017090: 653b 2066 6f72 2065 7861 6d70 6c65 2c20  e; for example, 
-000170a0: 6120 4d65 7373 6167 650d 0a20 2020 2020  a Message..     
-000170b0: 2020 2020 2020 2020 2020 206f 626a 6563             objec
-000170c0: 7420 6f72 2061 2043 6c69 656e 7420 696e  t or a Client in
-000170d0: 7374 616e 6365 2069 6e20 6f72 6465 7220  stance in order 
-000170e0: 746f 2065 6469 7420 7468 6520 6d65 7373  to edit the mess
-000170f0: 6167 6520 7769 7468 2074 6865 2075 7064  age with the upd
-00017100: 6174 6564 2070 726f 6772 6573 7320 7374  ated progress st
-00017110: 6174 7573 2e0d 0a0d 0a20 2020 2020 2020  atus.....       
-00017120: 204f 7468 6572 2050 6172 616d 6574 6572   Other Parameter
-00017130: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00017140: 6375 7272 656e 7420 2860 6069 6e74 6060  current (``int``
-00017150: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00017160: 2020 2020 5468 6520 616d 6f75 6e74 206f      The amount o
-00017170: 6620 6279 7465 7320 7472 616e 736d 6974  f bytes transmit
-00017180: 7465 6420 736f 2066 6172 2e0d 0a0d 0a20  ted so far..... 
-00017190: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-000171a0: 2028 6060 696e 7460 6029 3a0d 0a20 2020   (``int``):..   
-000171b0: 2020 2020 2020 2020 2020 2020 2054 6865               The
-000171c0: 2074 6f74 616c 2073 697a 6520 6f66 2074   total size of t
-000171d0: 6865 2066 696c 652e 0d0a 0d0a 2020 2020  he file.....    
-000171e0: 2020 2020 2020 2020 2a61 7267 7320 2860          *args (`
-000171f0: 6074 7570 6c65 6060 2c20 2a6f 7074 696f  `tuple``, *optio
-00017200: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-00017210: 2020 2020 2020 2020 4578 7472 6120 6375          Extra cu
-00017220: 7374 6f6d 2061 7267 756d 656e 7473 2061  stom arguments a
-00017230: 7320 6465 6669 6e65 6420 696e 2074 6865  s defined in the
-00017240: 2060 6070 726f 6772 6573 735f 6172 6773   ``progress_args
-00017250: 6060 2070 6172 616d 6574 6572 2e0d 0a20  `` parameter... 
-00017260: 2020 2020 2020 2020 2020 2020 2020 2059                 Y
-00017270: 6f75 2063 616e 2065 6974 6865 7220 6b65  ou can either ke
-00017280: 6570 2060 602a 6172 6773 6060 206f 7220  ep ``*args`` or 
-00017290: 6164 6420 6576 6572 7920 7369 6e67 6c65  add every single
-000172a0: 2065 7874 7261 2061 7267 756d 656e 7420   extra argument 
-000172b0: 696e 2079 6f75 7220 6675 6e63 7469 6f6e  in your function
-000172c0: 2073 6967 6e61 7475 7265 2e0d 0a0d 0a20   signature..... 
-000172d0: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
-000172e0: 0a20 2020 2020 2020 2020 2020 204f 6e20  .            On 
-000172f0: 7375 6363 6573 732c 2074 6865 2073 656e  success, the sen
-00017300: 7420 3a6f 626a 3a60 7e66 6970 7065 722e  t :obj:`~fipper.
-00017310: 7479 7065 732e 4d65 7373 6167 6560 2069  types.Message` i
-00017320: 7320 7265 7475 726e 6564 2e0d 0a20 2020  s returned...   
-00017330: 2020 2020 2020 2020 2049 6e20 6361 7365           In case
-00017340: 2074 6865 2075 706c 6f61 6420 6973 2064   the upload is d
-00017350: 656c 6962 6572 6174 656c 7920 7374 6f70  eliberately stop
-00017360: 7065 6420 7769 7468 203a 6d65 7468 3a60  ped with :meth:`
-00017370: 7e66 6970 7065 722e 436c 6965 6e74 2e73  ~fipper.Client.s
-00017380: 746f 705f 7472 616e 736d 6973 7369 6f6e  top_transmission
-00017390: 602c 204e 6f6e 6520 6973 2072 6574 7572  `, None is retur
-000173a0: 6e65 640d 0a20 2020 2020 2020 2020 2020  ned..           
-000173b0: 2069 6e73 7465 6164 2e0d 0a0d 0a20 2020   instead.....   
-000173c0: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
-000173d0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
-000173e0: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
-000173f0: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
-00017400: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
-00017410: 220d 0a20 2020 2020 2020 2069 6620 7175  "..        if qu
-00017420: 6f74 6520 6973 204e 6f6e 653a 0d0a 2020  ote is None:..  
-00017430: 2020 2020 2020 2020 2020 7175 6f74 6520            quote 
-00017440: 3d20 7365 6c66 2e63 6861 742e 7479 7065  = self.chat.type
-00017450: 2021 3d20 656e 756d 732e 4368 6174 5479   != enums.ChatTy
-00017460: 7065 2e50 5249 5641 5445 0d0a 0d0a 2020  pe.PRIVATE....  
-00017470: 2020 2020 2020 6966 2072 6570 6c79 5f74        if reply_t
-00017480: 6f5f 6d65 7373 6167 655f 6964 2069 7320  o_message_id is 
-00017490: 4e6f 6e65 2061 6e64 2071 756f 7465 3a0d  None and quote:.
-000174a0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-000174b0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-000174c0: 203d 2073 656c 662e 6964 0d0a 0d0a 2020   = self.id....  
-000174d0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-000174e0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-000174f0: 7365 6e64 5f73 7469 636b 6572 280d 0a20  send_sticker(.. 
-00017500: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00017510: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
-00017520: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00017530: 6963 6b65 723d 7374 6963 6b65 722c 0d0a  icker=sticker,..
-00017540: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-00017550: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00017560: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-00017570: 6174 696f 6e2c 0d0a 2020 2020 2020 2020  ation,..        
-00017580: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
-00017590: 7361 6765 5f69 643d 7265 706c 795f 746f  sage_id=reply_to
-000175a0: 5f6d 6573 7361 6765 5f69 642c 0d0a 2020  _message_id,..  
-000175b0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-000175c0: 6d61 726b 7570 3d72 6570 6c79 5f6d 6172  markup=reply_mar
-000175d0: 6b75 702c 0d0a 2020 2020 2020 2020 2020  kup,..          
-000175e0: 2020 7072 6f67 7265 7373 3d70 726f 6772    progress=progr
-000175f0: 6573 732c 0d0a 2020 2020 2020 2020 2020  ess,..          
-00017600: 2020 7072 6f67 7265 7373 5f61 7267 733d    progress_args=
-00017610: 7072 6f67 7265 7373 5f61 7267 730d 0a20  progress_args.. 
-00017620: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00017630: 6173 796e 6320 6465 6620 7265 706c 795f  async def reply_
-00017640: 7665 6e75 6528 0d0a 2020 2020 2020 2020  venue(..        
-00017650: 7365 6c66 2c0d 0a20 2020 2020 2020 206c  self,..        l
-00017660: 6174 6974 7564 653a 2066 6c6f 6174 2c0d  atitude: float,.
-00017670: 0a20 2020 2020 2020 206c 6f6e 6769 7475  .        longitu
-00017680: 6465 3a20 666c 6f61 742c 0d0a 2020 2020  de: float,..    
-00017690: 2020 2020 7469 746c 653a 2073 7472 2c0d      title: str,.
-000176a0: 0a20 2020 2020 2020 2061 6464 7265 7373  .        address
-000176b0: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
-000176c0: 7175 6f74 653a 2062 6f6f 6c20 3d20 4e6f  quote: bool = No
-000176d0: 6e65 2c0d 0a20 2020 2020 2020 2066 6f75  ne,..        fou
-000176e0: 7273 7175 6172 655f 6964 3a20 7374 7220  rsquare_id: str 
-000176f0: 3d20 2222 2c0d 0a20 2020 2020 2020 2066  = "",..        f
-00017700: 6f75 7273 7175 6172 655f 7479 7065 3a20  oursquare_type: 
-00017710: 7374 7220 3d20 2222 2c0d 0a20 2020 2020  str = "",..     
-00017720: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
-00017730: 6963 6174 696f 6e3a 2062 6f6f 6c20 3d20  ication: bool = 
-00017740: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2072  None,..        r
-00017750: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00017760: 6964 3a20 696e 7420 3d20 4e6f 6e65 2c0d  id: int = None,.
-00017770: 0a20 2020 2020 2020 2072 6570 6c79 5f6d  .        reply_m
-00017780: 6172 6b75 703a 2055 6e69 6f6e 5b0d 0a20  arkup: Union[.. 
-00017790: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-000177a0: 732e 496e 6c69 6e65 4b65 7962 6f61 7264  s.InlineKeyboard
-000177b0: 4d61 726b 7570 222c 0d0a 2020 2020 2020  Markup",..      
-000177c0: 2020 2020 2020 2274 7970 6573 2e52 6570        "types.Rep
-000177d0: 6c79 4b65 7962 6f61 7264 4d61 726b 7570  lyKeyboardMarkup
-000177e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000177f0: 2274 7970 6573 2e52 6570 6c79 4b65 7962  "types.ReplyKeyb
-00017800: 6f61 7264 5265 6d6f 7665 222c 0d0a 2020  oardRemove",..  
-00017810: 2020 2020 2020 2020 2020 2274 7970 6573            "types
-00017820: 2e46 6f72 6365 5265 706c 7922 0d0a 2020  .ForceReply"..  
-00017830: 2020 2020 2020 5d20 3d20 4e6f 6e65 0d0a        ] = None..
-00017840: 2020 2020 2920 2d3e 2022 4d65 7373 6167      ) -> "Messag
-00017850: 6522 3a0d 0a20 2020 2020 2020 2022 2222  e":..        """
-00017860: 426f 756e 6420 6d65 7468 6f64 202a 7265  Bound method *re
-00017870: 706c 795f 7665 6e75 652a 206f 6620 3a6f  ply_venue* of :o
-00017880: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
-00017890: 732e 4d65 7373 6167 6560 2e0d 0a0d 0a20  s.Message`..... 
-000178a0: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
-000178b0: 7368 6f72 7463 7574 2066 6f72 3a0d 0a0d  shortcut for:...
-000178c0: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-000178d0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
-000178e0: 0a0d 0a20 2020 2020 2020 2020 2020 2061  ...            a
-000178f0: 7761 6974 2063 6c69 656e 742e 7365 6e64  wait client.send
-00017900: 5f76 656e 7565 280d 0a20 2020 2020 2020  _venue(..       
-00017910: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00017920: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
-00017930: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00017940: 2020 206c 6174 6974 7564 653d 6c61 7469     latitude=lati
-00017950: 7475 6465 2c0d 0a20 2020 2020 2020 2020  tude,..         
-00017960: 2020 2020 2020 206c 6f6e 6769 7475 6465         longitude
-00017970: 3d6c 6f6e 6769 7475 6465 2c0d 0a20 2020  =longitude,..   
-00017980: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-00017990: 6c65 3d22 5665 6e75 6520 7469 746c 6522  le="Venue title"
-000179a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000179b0: 2020 2061 6464 7265 7373 3d22 5665 6e75     address="Venu
-000179c0: 6520 6164 6472 6573 7322 0d0a 2020 2020  e address"..    
-000179d0: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-000179e0: 2020 2020 2045 7861 6d70 6c65 3a0d 0a20       Example:.. 
-000179f0: 2020 2020 2020 2020 2020 202e 2e20 636f             .. co
-00017a00: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-00017a10: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
-00017a20: 2020 2020 2061 7761 6974 206d 6573 7361       await messa
-00017a30: 6765 2e72 6570 6c79 5f76 656e 7565 286c  ge.reply_venue(l
-00017a40: 6174 6974 7564 652c 206c 6f6e 6769 7475  atitude, longitu
-00017a50: 6465 2c20 2256 656e 7565 2074 6974 6c65  de, "Venue title
-00017a60: 222c 2022 5665 6e75 6520 6164 6472 6573  ", "Venue addres
-00017a70: 7322 290d 0a0d 0a20 2020 2020 2020 2050  s")....        P
-00017a80: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
-00017a90: 2020 2020 2020 2020 6c61 7469 7475 6465          latitude
-00017aa0: 2028 6060 666c 6f61 7460 6029 3a0d 0a20   (``float``):.. 
-00017ab0: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-00017ac0: 6174 6974 7564 6520 6f66 2074 6865 2076  atitude of the v
-00017ad0: 656e 7565 2e0d 0a0d 0a20 2020 2020 2020  enue.....       
-00017ae0: 2020 2020 206c 6f6e 6769 7475 6465 2028       longitude (
-00017af0: 6060 666c 6f61 7460 6029 3a0d 0a20 2020  ``float``):..   
-00017b00: 2020 2020 2020 2020 2020 2020 204c 6f6e               Lon
-00017b10: 6769 7475 6465 206f 6620 7468 6520 7665  gitude of the ve
-00017b20: 6e75 652e 0d0a 0d0a 2020 2020 2020 2020  nue.....        
-00017b30: 2020 2020 7469 746c 6520 2860 6073 7472      title (``str
-00017b40: 6060 293a 0d0a 2020 2020 2020 2020 2020  ``):..          
-00017b50: 2020 2020 2020 4e61 6d65 206f 6620 7468        Name of th
-00017b60: 6520 7665 6e75 652e 0d0a 0d0a 2020 2020  e venue.....    
-00017b70: 2020 2020 2020 2020 6164 6472 6573 7320          address 
-00017b80: 2860 6073 7472 6060 293a 0d0a 2020 2020  (``str``):..    
-00017b90: 2020 2020 2020 2020 2020 2020 4164 6472              Addr
-00017ba0: 6573 7320 6f66 2074 6865 2076 656e 7565  ess of the venue
-00017bb0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00017bc0: 2071 756f 7465 2028 6060 626f 6f6c 6060   quote (``bool``
-00017bd0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bf0: 4966 2060 6054 7275 6560 602c 2074 6865  If ``True``, the
-00017c00: 206d 6573 7361 6765 2077 696c 6c20 6265   message will be
-00017c10: 2073 656e 7420 6173 2061 2072 6570 6c79   sent as a reply
-00017c20: 2074 6f20 7468 6973 206d 6573 7361 6765   to this message
-00017c30: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017c40: 2020 2049 6620 2a72 6570 6c79 5f74 6f5f     If *reply_to_
-00017c50: 6d65 7373 6167 655f 6964 2a20 6973 2070  message_id* is p
-00017c60: 6173 7365 642c 2074 6869 7320 7061 7261  assed, this para
-00017c70: 6d65 7465 7220 7769 6c6c 2062 6520 6967  meter will be ig
-00017c80: 6e6f 7265 642e 0d0a 2020 2020 2020 2020  nored...        
-00017c90: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00017ca0: 2074 6f20 6060 5472 7565 6060 2069 6e20   to ``True`` in 
-00017cb0: 6772 6f75 7020 6368 6174 7320 616e 6420  group chats and 
-00017cc0: 6060 4661 6c73 6560 6020 696e 2070 7269  ``False`` in pri
-00017cd0: 7661 7465 2063 6861 7473 2e0d 0a0d 0a20  vate chats..... 
-00017ce0: 2020 2020 2020 2020 2020 2066 6f75 7273             fours
-00017cf0: 7175 6172 655f 6964 2028 6060 7374 7260  quare_id (``str`
-00017d00: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-00017d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d20: 2046 6f75 7273 7175 6172 6520 6964 656e   Foursquare iden
-00017d30: 7469 6669 6572 206f 6620 7468 6520 7665  tifier of the ve
-00017d40: 6e75 652e 0d0a 0d0a 2020 2020 2020 2020  nue.....        
-00017d50: 2020 2020 666f 7572 7371 7561 7265 5f74      foursquare_t
-00017d60: 7970 6520 2860 6073 7472 6060 2c20 2a6f  ype (``str``, *o
-00017d70: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-00017d80: 2020 2020 2020 2020 2020 2020 466f 7572              Four
-00017d90: 7371 7561 7265 2074 7970 6520 6f66 2074  square type of t
-00017da0: 6865 2076 656e 7565 2c20 6966 206b 6e6f  he venue, if kno
-00017db0: 776e 2e0d 0a20 2020 2020 2020 2020 2020  wn...           
-00017dc0: 2020 2020 2028 466f 7220 6578 616d 706c       (For exampl
-00017dd0: 652c 2022 6172 7473 5f65 6e74 6572 7461  e, "arts_enterta
-00017de0: 696e 6d65 6e74 2f64 6566 6175 6c74 222c  inment/default",
-00017df0: 2022 6172 7473 5f65 6e74 6572 7461 696e   "arts_entertain
-00017e00: 6d65 6e74 2f61 7175 6172 6975 6d22 206f  ment/aquarium" o
-00017e10: 7220 2266 6f6f 642f 6963 6563 7265 616d  r "food/icecream
-00017e20: 222e 290d 0a0d 0a20 2020 2020 2020 2020  ".)....         
-00017e30: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
-00017e40: 6963 6174 696f 6e20 2860 6062 6f6f 6c60  ication (``bool`
-00017e50: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-00017e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017e70: 2053 656e 6473 2074 6865 206d 6573 7361   Sends the messa
-00017e80: 6765 2073 696c 656e 746c 792e 0d0a 2020  ge silently...  
-00017e90: 2020 2020 2020 2020 2020 2020 2020 5573                Us
-00017ea0: 6572 7320 7769 6c6c 2072 6563 6569 7665  ers will receive
-00017eb0: 2061 206e 6f74 6966 6963 6174 696f 6e20   a notification 
-00017ec0: 7769 7468 206e 6f20 736f 756e 642e 0d0a  with no sound...
-00017ed0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00017ee0: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00017ef0: 6420 2860 6069 6e74 6060 2c20 2a6f 7074  d (``int``, *opt
-00017f00: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
-00017f10: 2020 2020 2020 2020 2020 4966 2074 6865            If the
-00017f20: 206d 6573 7361 6765 2069 7320 6120 7265   message is a re
-00017f30: 706c 792c 2049 4420 6f66 2074 6865 206f  ply, ID of the o
-00017f40: 7269 6769 6e61 6c20 6d65 7373 6167 650d  riginal message.
-00017f50: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-00017f60: 6570 6c79 5f6d 6172 6b75 7020 283a 6f62  eply_markup (:ob
-00017f70: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
-00017f80: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
-00017f90: 6172 6b75 7060 207c 203a 6f62 6a3a 607e  arkup` | :obj:`~
-00017fa0: 6669 7070 6572 2e74 7970 6573 2e52 6570  fipper.types.Rep
-00017fb0: 6c79 4b65 7962 6f61 7264 4d61 726b 7570  lyKeyboardMarkup
-00017fc0: 6020 7c20 3a6f 626a 3a60 7e66 6970 7065  ` | :obj:`~fippe
-00017fd0: 722e 7479 7065 732e 5265 706c 794b 6579  r.types.ReplyKey
-00017fe0: 626f 6172 6452 656d 6f76 6560 207c 203a  boardRemove` | :
-00017ff0: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
-00018000: 6573 2e46 6f72 6365 5265 706c 7960 2c20  es.ForceReply`, 
-00018010: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
-00018020: 2020 2020 2020 2020 2020 2020 2020 4164                Ad
-00018030: 6469 7469 6f6e 616c 2069 6e74 6572 6661  ditional interfa
-00018040: 6365 206f 7074 696f 6e73 2e20 416e 206f  ce options. An o
-00018050: 626a 6563 7420 666f 7220 616e 2069 6e6c  bject for an inl
-00018060: 696e 6520 6b65 7962 6f61 7264 2c20 6375  ine keyboard, cu
-00018070: 7374 6f6d 2072 6570 6c79 206b 6579 626f  stom reply keybo
-00018080: 6172 642c 0d0a 2020 2020 2020 2020 2020  ard,..          
-00018090: 2020 2020 2020 696e 7374 7275 6374 696f        instructio
-000180a0: 6e73 2074 6f20 7265 6d6f 7665 2072 6570  ns to remove rep
-000180b0: 6c79 206b 6579 626f 6172 6420 6f72 2074  ly keyboard or t
-000180c0: 6f20 666f 7263 6520 6120 7265 706c 7920  o force a reply 
-000180d0: 6672 6f6d 2074 6865 2075 7365 722e 0d0a  from the user...
-000180e0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000180f0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00018100: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
-00018110: 7365 6e74 203a 6f62 6a3a 607e 6669 7070  sent :obj:`~fipp
-00018120: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
-00018130: 6020 6973 2072 6574 7572 6e65 642e 0d0a  ` is returned...
-00018140: 0d0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00018150: 3a0d 0a20 2020 2020 2020 2020 2020 2052  :..            R
-00018160: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
-00018170: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
-00018180: 5043 2065 7272 6f72 2e0d 0a20 2020 2020  PC error...     
-00018190: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000181a0: 6966 2071 756f 7465 2069 7320 4e6f 6e65  if quote is None
-000181b0: 3a0d 0a20 2020 2020 2020 2020 2020 2071  :..            q
-000181c0: 756f 7465 203d 2073 656c 662e 6368 6174  uote = self.chat
-000181d0: 2e74 7970 6520 213d 2065 6e75 6d73 2e43  .type != enums.C
-000181e0: 6861 7454 7970 652e 5052 4956 4154 450d  hatType.PRIVATE.
-000181f0: 0a0d 0a20 2020 2020 2020 2069 6620 7265  ...        if re
-00018200: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
-00018210: 6420 6973 204e 6f6e 6520 616e 6420 7175  d is None and qu
-00018220: 6f74 653a 0d0a 2020 2020 2020 2020 2020  ote:..          
-00018230: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00018240: 6765 5f69 6420 3d20 7365 6c66 2e69 640d  ge_id = self.id.
-00018250: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00018260: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-00018270: 6965 6e74 2e73 656e 645f 7665 6e75 6528  ient.send_venue(
-00018280: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-00018290: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
-000182a0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-000182b0: 206c 6174 6974 7564 653d 6c61 7469 7475   latitude=latitu
-000182c0: 6465 2c0d 0a20 2020 2020 2020 2020 2020  de,..           
-000182d0: 206c 6f6e 6769 7475 6465 3d6c 6f6e 6769   longitude=longi
-000182e0: 7475 6465 2c0d 0a20 2020 2020 2020 2020  tude,..         
-000182f0: 2020 2074 6974 6c65 3d74 6974 6c65 2c0d     title=title,.
-00018300: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-00018310: 7265 7373 3d61 6464 7265 7373 2c0d 0a20  ress=address,.. 
-00018320: 2020 2020 2020 2020 2020 2066 6f75 7273             fours
-00018330: 7175 6172 655f 6964 3d66 6f75 7273 7175  quare_id=foursqu
-00018340: 6172 655f 6964 2c0d 0a20 2020 2020 2020  are_id,..       
-00018350: 2020 2020 2066 6f75 7273 7175 6172 655f       foursquare_
-00018360: 7479 7065 3d66 6f75 7273 7175 6172 655f  type=foursquare_
-00018370: 7479 7065 2c0d 0a20 2020 2020 2020 2020  type,..         
-00018380: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
-00018390: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
-000183a0: 6e6f 7469 6669 6361 7469 6f6e 2c0d 0a20  notification,.. 
-000183b0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-000183c0: 5f74 6f5f 6d65 7373 6167 655f 6964 3d72  _to_message_id=r
-000183d0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-000183e0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-000183f0: 2072 6570 6c79 5f6d 6172 6b75 703d 7265   reply_markup=re
-00018400: 706c 795f 6d61 726b 7570 0d0a 2020 2020  ply_markup..    
-00018410: 2020 2020 290d 0a0d 0a20 2020 2061 7379      )....    asy
-00018420: 6e63 2064 6566 2072 6570 6c79 5f76 6964  nc def reply_vid
-00018430: 656f 280d 0a20 2020 2020 2020 2073 656c  eo(..        sel
-00018440: 662c 0d0a 2020 2020 2020 2020 7669 6465  f,..        vide
-00018450: 6f3a 2055 6e69 6f6e 5b73 7472 2c20 4269  o: Union[str, Bi
-00018460: 6e61 7279 494f 5d2c 0d0a 2020 2020 2020  naryIO],..      
-00018470: 2020 7175 6f74 653a 2062 6f6f 6c20 3d20    quote: bool = 
-00018480: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2063  None,..        c
-00018490: 6170 7469 6f6e 3a20 7374 7220 3d20 2222  aption: str = ""
-000184a0: 2c0d 0a20 2020 2020 2020 2070 6172 7365  ,..        parse
-000184b0: 5f6d 6f64 653a 204f 7074 696f 6e61 6c5b  _mode: Optional[
-000184c0: 2265 6e75 6d73 2e50 6172 7365 4d6f 6465  "enums.ParseMode
-000184d0: 225d 203d 204e 6f6e 652c 0d0a 2020 2020  "] = None,..    
-000184e0: 2020 2020 6361 7074 696f 6e5f 656e 7469      caption_enti
-000184f0: 7469 6573 3a20 4c69 7374 5b22 7479 7065  ties: List["type
-00018500: 732e 4d65 7373 6167 6545 6e74 6974 7922  s.MessageEntity"
-00018510: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-00018520: 2020 2074 746c 5f73 6563 6f6e 6473 3a20     ttl_seconds: 
-00018530: 696e 7420 3d20 4e6f 6e65 2c0d 0a20 2020  int = None,..   
-00018540: 2020 2020 2064 7572 6174 696f 6e3a 2069       duration: i
-00018550: 6e74 203d 2030 2c0d 0a20 2020 2020 2020  nt = 0,..       
-00018560: 2077 6964 7468 3a20 696e 7420 3d20 302c   width: int = 0,
-00018570: 0d0a 2020 2020 2020 2020 6865 6967 6874  ..        height
-00018580: 3a20 696e 7420 3d20 302c 0d0a 2020 2020  : int = 0,..    
-00018590: 2020 2020 7468 756d 623a 2073 7472 203d      thumb: str =
-000185a0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-000185b0: 7375 7070 6f72 7473 5f73 7472 6561 6d69  supports_streami
-000185c0: 6e67 3a20 626f 6f6c 203d 2054 7275 652c  ng: bool = True,
-000185d0: 0d0a 2020 2020 2020 2020 6469 7361 626c  ..        disabl
-000185e0: 655f 6e6f 7469 6669 6361 7469 6f6e 3a20  e_notification: 
-000185f0: 626f 6f6c 203d 204e 6f6e 652c 0d0a 2020  bool = None,..  
-00018600: 2020 2020 2020 7265 706c 795f 746f 5f6d        reply_to_m
-00018610: 6573 7361 6765 5f69 643a 2069 6e74 203d  essage_id: int =
-00018620: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00018630: 7265 706c 795f 6d61 726b 7570 3a20 556e  reply_markup: Un
-00018640: 696f 6e5b 0d0a 2020 2020 2020 2020 2020  ion[..          
-00018650: 2020 2274 7970 6573 2e49 6e6c 696e 654b    "types.InlineK
-00018660: 6579 626f 6172 644d 6172 6b75 7022 2c0d  eyboardMarkup",.
-00018670: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00018680: 7065 732e 5265 706c 794b 6579 626f 6172  pes.ReplyKeyboar
-00018690: 644d 6172 6b75 7022 2c0d 0a20 2020 2020  dMarkup",..     
-000186a0: 2020 2020 2020 2022 7479 7065 732e 5265         "types.Re
-000186b0: 706c 794b 6579 626f 6172 6452 656d 6f76  plyKeyboardRemov
-000186c0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-000186d0: 2022 7479 7065 732e 466f 7263 6552 6570   "types.ForceRep
-000186e0: 6c79 220d 0a20 2020 2020 2020 205d 203d  ly"..        ] =
-000186f0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00018700: 7072 6f67 7265 7373 3a20 4361 6c6c 6162  progress: Callab
-00018710: 6c65 203d 204e 6f6e 652c 0d0a 2020 2020  le = None,..    
-00018720: 2020 2020 7072 6f67 7265 7373 5f61 7267      progress_arg
-00018730: 733a 2074 7570 6c65 203d 2028 290d 0a20  s: tuple = ().. 
-00018740: 2020 2029 202d 3e20 224d 6573 7361 6765     ) -> "Message
-00018750: 223a 0d0a 2020 2020 2020 2020 2222 2242  ":..        """B
-00018760: 6f75 6e64 206d 6574 686f 6420 2a72 6570  ound method *rep
-00018770: 6c79 5f76 6964 656f 2a20 6f66 203a 6f62  ly_video* of :ob
-00018780: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
-00018790: 2e4d 6573 7361 6765 602e 0d0a 0d0a 2020  .Message`.....  
-000187a0: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
-000187b0: 686f 7274 6375 7420 666f 723a 0d0a 0d0a  hortcut for:....
-000187c0: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
-000187d0: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0d0a  block:: python..
-000187e0: 0d0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
-000187f0: 6169 7420 636c 6965 6e74 2e73 656e 645f  ait client.send_
-00018800: 7669 6465 6f28 0d0a 2020 2020 2020 2020  video(..        
-00018810: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-00018820: 6d65 7373 6167 652e 6368 6174 2e69 642c  message.chat.id,
-00018830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018840: 2020 7669 6465 6f3d 7669 6465 6f0d 0a20    video=video.. 
-00018850: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
-00018860: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-00018870: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-00018880: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00018890: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
-000188a0: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
-000188b0: 7373 6167 652e 7265 706c 795f 7669 6465  ssage.reply_vide
-000188c0: 6f28 7669 6465 6f29 0d0a 0d0a 2020 2020  o(video)....    
-000188d0: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
-000188e0: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
-000188f0: 656f 2028 6060 7374 7260 6029 3a0d 0a20  eo (``str``):.. 
-00018900: 2020 2020 2020 2020 2020 2020 2020 2056                 V
-00018910: 6964 656f 2074 6f20 7365 6e64 2e0d 0a20  ideo to send... 
-00018920: 2020 2020 2020 2020 2020 2020 2020 2050                 P
-00018930: 6173 7320 6120 6669 6c65 5f69 6420 6173  ass a file_id as
-00018940: 2073 7472 696e 6720 746f 2073 656e 6420   string to send 
-00018950: 6120 7669 6465 6f20 7468 6174 2065 7869  a video that exi
-00018960: 7374 7320 6f6e 2074 6865 2054 656c 6567  sts on the Teleg
-00018970: 7261 6d20 7365 7276 6572 732c 0d0a 2020  ram servers,..  
-00018980: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00018990: 7373 2061 6e20 4854 5450 2055 524c 2061  ss an HTTP URL a
-000189a0: 7320 6120 7374 7269 6e67 2066 6f72 2054  s a string for T
-000189b0: 656c 6567 7261 6d20 746f 2067 6574 2061  elegram to get a
-000189c0: 2076 6964 656f 2066 726f 6d20 7468 6520   video from the 
-000189d0: 496e 7465 726e 6574 2c20 6f72 0d0a 2020  Internet, or..  
-000189e0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000189f0: 7373 2061 2066 696c 6520 7061 7468 2061  ss a file path a
-00018a00: 7320 7374 7269 6e67 2074 6f20 7570 6c6f  s string to uplo
-00018a10: 6164 2061 206e 6577 2076 6964 656f 2074  ad a new video t
-00018a20: 6861 7420 6578 6973 7473 206f 6e20 796f  hat exists on yo
-00018a30: 7572 206c 6f63 616c 206d 6163 6869 6e65  ur local machine
-00018a40: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00018a50: 2071 756f 7465 2028 6060 626f 6f6c 6060   quote (``bool``
-00018a60: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-00018a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a80: 4966 2060 6054 7275 6560 602c 2074 6865  If ``True``, the
-00018a90: 206d 6573 7361 6765 2077 696c 6c20 6265   message will be
-00018aa0: 2073 656e 7420 6173 2061 2072 6570 6c79   sent as a reply
-00018ab0: 2074 6f20 7468 6973 206d 6573 7361 6765   to this message
-00018ac0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018ad0: 2020 2049 6620 2a72 6570 6c79 5f74 6f5f     If *reply_to_
-00018ae0: 6d65 7373 6167 655f 6964 2a20 6973 2070  message_id* is p
-00018af0: 6173 7365 642c 2074 6869 7320 7061 7261  assed, this para
-00018b00: 6d65 7465 7220 7769 6c6c 2062 6520 6967  meter will be ig
-00018b10: 6e6f 7265 642e 0d0a 2020 2020 2020 2020  nored...        
-00018b20: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00018b30: 2074 6f20 6060 5472 7565 6060 2069 6e20   to ``True`` in 
-00018b40: 6772 6f75 7020 6368 6174 7320 616e 6420  group chats and 
-00018b50: 6060 4661 6c73 6560 6020 696e 2070 7269  ``False`` in pri
-00018b60: 7661 7465 2063 6861 7473 2e0d 0a0d 0a20  vate chats..... 
-00018b70: 2020 2020 2020 2020 2020 2063 6170 7469             capti
-00018b80: 6f6e 2028 6060 7374 7260 602c 202a 6f70  on (``str``, *op
-00018b90: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-00018ba0: 2020 2020 2020 2020 2020 2056 6964 656f             Video
-00018bb0: 2063 6170 7469 6f6e 2c20 302d 3130 3234   caption, 0-1024
-00018bc0: 2063 6861 7261 6374 6572 732e 0d0a 0d0a   characters.....
-00018bd0: 2020 2020 2020 2020 2020 2020 7061 7273              pars
-00018be0: 655f 6d6f 6465 2028 3a6f 626a 3a60 7e66  e_mode (:obj:`~f
-00018bf0: 6970 7065 722e 656e 756d 732e 5061 7273  ipper.enums.Pars
-00018c00: 654d 6f64 6560 2c20 2a6f 7074 696f 6e61  eMode`, *optiona
-00018c10: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-00018c20: 2020 2020 2020 4279 2064 6566 6175 6c74        By default
-00018c30: 2c20 7465 7874 7320 6172 6520 7061 7273  , texts are pars
-00018c40: 6564 2075 7369 6e67 2062 6f74 6820 4d61  ed using both Ma
-00018c50: 726b 646f 776e 2061 6e64 2048 544d 4c20  rkdown and HTML 
-00018c60: 7374 796c 6573 2e0d 0a20 2020 2020 2020  styles...       
-00018c70: 2020 2020 2020 2020 2059 6f75 2063 616e           You can
-00018c80: 2063 6f6d 6269 6e65 2062 6f74 6820 7379   combine both sy
-00018c90: 6e74 6178 6573 2074 6f67 6574 6865 722e  ntaxes together.
-00018ca0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018cb0: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
-00018cc0: 2028 4c69 7374 206f 6620 3a6f 626a 3a60   (List of :obj:`
-00018cd0: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
-00018ce0: 7373 6167 6545 6e74 6974 7960 293a 0d0a  ssageEntity`):..
-00018cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d00: 4c69 7374 206f 6620 7370 6563 6961 6c20  List of special 
-00018d10: 656e 7469 7469 6573 2074 6861 7420 6170  entities that ap
-00018d20: 7065 6172 2069 6e20 7468 6520 6361 7074  pear in the capt
-00018d30: 696f 6e2c 2077 6869 6368 2063 616e 2062  ion, which can b
-00018d40: 6520 7370 6563 6966 6965 6420 696e 7374  e specified inst
-00018d50: 6561 6420 6f66 202a 7061 7273 655f 6d6f  ead of *parse_mo
-00018d60: 6465 2a2e 0d0a 0d0a 2020 2020 2020 2020  de*.....        
-00018d70: 2020 2020 7474 6c5f 7365 636f 6e64 7320      ttl_seconds 
-00018d80: 2860 6069 6e74 6060 2c20 2a6f 7074 696f  (``int``, *optio
-00018d90: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-00018da0: 2020 2020 2020 2020 5365 6c66 2d44 6573          Self-Des
-00018db0: 7472 7563 7420 5469 6d65 722e 0d0a 2020  truct Timer...  
-00018dc0: 2020 2020 2020 2020 2020 2020 2020 4966                If
-00018dd0: 2079 6f75 2073 6574 2061 2074 696d 6572   you set a timer
-00018de0: 2c20 7468 6520 7669 6465 6f20 7769 6c6c  , the video will
-00018df0: 2073 656c 662d 6465 7374 7275 6374 2069   self-destruct i
-00018e00: 6e20 2a74 746c 5f73 6563 6f6e 6473 2a0d  n *ttl_seconds*.
-00018e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e20: 2073 6563 6f6e 6473 2061 6674 6572 2069   seconds after i
-00018e30: 7420 7761 7320 7669 6577 6564 2e0d 0a0d  t was viewed....
-00018e40: 0a20 2020 2020 2020 2020 2020 2064 7572  .            dur
-00018e50: 6174 696f 6e20 2860 6069 6e74 6060 2c20  ation (``int``, 
-00018e60: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
-00018e70: 2020 2020 2020 2020 2020 2020 2020 4475                Du
-00018e80: 7261 7469 6f6e 206f 6620 7365 6e74 2076  ration of sent v
-00018e90: 6964 656f 2069 6e20 7365 636f 6e64 732e  ideo in seconds.
-00018ea0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018eb0: 7769 6474 6820 2860 6069 6e74 6060 2c20  width (``int``, 
-00018ec0: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
-00018ed0: 2020 2020 2020 2020 2020 2020 2020 5669                Vi
-00018ee0: 6465 6f20 7769 6474 682e 0d0a 0d0a 2020  deo width.....  
-00018ef0: 2020 2020 2020 2020 2020 6865 6967 6874            height
+00015bc0: 2020 2020 2020 5061 7373 2054 7275 652c        Pass True,
+00015bd0: 2069 6620 7468 6520 706f 6c6c 206e 6565   if the poll nee
+00015be0: 6473 2074 6f20 6265 2069 6d6d 6564 6961  ds to be immedia
+00015bf0: 7465 6c79 2063 6c6f 7365 642e 0d0a 2020  tely closed...  
+00015c00: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00015c10: 6973 2063 616e 2062 6520 7573 6566 756c  is can be useful
+00015c20: 2066 6f72 2070 6f6c 6c20 7072 6576 6965   for poll previe
+00015c30: 772e 0d0a 0d0a 2020 2020 2020 2020 2020  w.....          
+00015c40: 2020 7175 6f74 6520 2860 6062 6f6f 6c60    quote (``bool`
+00015c50: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+00015c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015c70: 2049 6620 6060 5472 7565 6060 2c20 7468   If ``True``, th
+00015c80: 6520 6d65 7373 6167 6520 7769 6c6c 2062  e message will b
+00015c90: 6520 7365 6e74 2061 7320 6120 7265 706c  e sent as a repl
+00015ca0: 7920 746f 2074 6869 7320 6d65 7373 6167  y to this messag
+00015cb0: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
+00015cc0: 2020 2020 4966 202a 7265 706c 795f 746f      If *reply_to
+00015cd0: 5f6d 6573 7361 6765 5f69 642a 2069 7320  _message_id* is 
+00015ce0: 7061 7373 6564 2c20 7468 6973 2070 6172  passed, this par
+00015cf0: 616d 6574 6572 2077 696c 6c20 6265 2069  ameter will be i
+00015d00: 676e 6f72 6564 2e0d 0a20 2020 2020 2020  gnored...       
+00015d10: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00015d20: 7320 746f 2060 6054 7275 6560 6020 696e  s to ``True`` in
+00015d30: 2067 726f 7570 2063 6861 7473 2061 6e64   group chats and
+00015d40: 2060 6046 616c 7365 6060 2069 6e20 7072   ``False`` in pr
+00015d50: 6976 6174 6520 6368 6174 732e 0d0a 0d0a  ivate chats.....
+00015d60: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+00015d70: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00015d80: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+00015d90: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+00015da0: 2020 2020 2020 2020 2020 5365 6e64 7320            Sends 
+00015db0: 7468 6520 6d65 7373 6167 6520 7369 6c65  the message sile
+00015dc0: 6e74 6c79 2e0d 0a20 2020 2020 2020 2020  ntly...         
+00015dd0: 2020 2020 2020 2055 7365 7273 2077 696c         Users wil
+00015de0: 6c20 7265 6365 6976 6520 6120 6e6f 7469  l receive a noti
+00015df0: 6669 6361 7469 6f6e 2077 6974 6820 6e6f  fication with no
+00015e00: 2073 6f75 6e64 2e0d 0a0d 0a20 2020 2020   sound.....     
+00015e10: 2020 2020 2020 2070 726f 7465 6374 5f63         protect_c
+00015e20: 6f6e 7465 6e74 2028 6060 626f 6f6c 6060  ontent (``bool``
+00015e30: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+00015e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e50: 5072 6f74 6563 7473 2074 6865 2063 6f6e  Protects the con
+00015e60: 7465 6e74 7320 6f66 2074 6865 2073 656e  tents of the sen
+00015e70: 7420 6d65 7373 6167 6520 6672 6f6d 2066  t message from f
+00015e80: 6f72 7761 7264 696e 6720 616e 6420 7361  orwarding and sa
+00015e90: 7669 6e67 2e0d 0a0d 0a20 2020 2020 2020  ving.....       
+00015ea0: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
+00015eb0: 7373 6167 655f 6964 2028 6060 696e 7460  ssage_id (``int`
+00015ec0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+00015ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ee0: 2049 6620 7468 6520 6d65 7373 6167 6520   If the message 
+00015ef0: 6973 2061 2072 6570 6c79 2c20 4944 206f  is a reply, ID o
+00015f00: 6620 7468 6520 6f72 6967 696e 616c 206d  f the original m
+00015f10: 6573 7361 6765 2e0d 0a0d 0a20 2020 2020  essage.....     
+00015f20: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
+00015f30: 6461 7465 2028 3a70 793a 6f62 6a3a 607e  date (:py:obj:`~
+00015f40: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
+00015f50: 6560 2c20 2a6f 7074 696f 6e61 6c2a 293a  e`, *optional*):
+00015f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015f70: 2020 4461 7465 2077 6865 6e20 7468 6520    Date when the 
+00015f80: 6d65 7373 6167 6520 7769 6c6c 2062 6520  message will be 
+00015f90: 6175 746f 6d61 7469 6361 6c6c 7920 7365  automatically se
+00015fa0: 6e74 2e0d 0a0d 0a20 2020 2020 2020 2020  nt.....         
+00015fb0: 2020 2072 6570 6c79 5f6d 6172 6b75 7020     reply_markup 
+00015fc0: 283a 6f62 6a3a 607e 6669 7070 6572 2e74  (:obj:`~fipper.t
+00015fd0: 7970 6573 2e49 6e6c 696e 654b 6579 626f  ypes.InlineKeybo
+00015fe0: 6172 644d 6172 6b75 7060 207c 203a 6f62  ardMarkup` | :ob
+00015ff0: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+00016000: 2e52 6570 6c79 4b65 7962 6f61 7264 4d61  .ReplyKeyboardMa
+00016010: 726b 7570 6020 7c20 3a6f 626a 3a60 7e66  rkup` | :obj:`~f
+00016020: 6970 7065 722e 7479 7065 732e 5265 706c  ipper.types.Repl
+00016030: 794b 6579 626f 6172 6452 656d 6f76 6560  yKeyboardRemove`
+00016040: 207c 203a 6f62 6a3a 607e 6669 7070 6572   | :obj:`~fipper
+00016050: 2e74 7970 6573 2e46 6f72 6365 5265 706c  .types.ForceRepl
+00016060: 7960 2c20 2a6f 7074 696f 6e61 6c2a 293a  y`, *optional*):
+00016070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016080: 2020 4164 6469 7469 6f6e 616c 2069 6e74    Additional int
+00016090: 6572 6661 6365 206f 7074 696f 6e73 2e20  erface options. 
+000160a0: 416e 206f 626a 6563 7420 666f 7220 616e  An object for an
+000160b0: 2069 6e6c 696e 6520 6b65 7962 6f61 7264   inline keyboard
+000160c0: 2c20 6375 7374 6f6d 2072 6570 6c79 206b  , custom reply k
+000160d0: 6579 626f 6172 642c 0d0a 2020 2020 2020  eyboard,..      
+000160e0: 2020 2020 2020 2020 2020 696e 7374 7275            instru
+000160f0: 6374 696f 6e73 2074 6f20 7265 6d6f 7665  ctions to remove
+00016100: 2072 6570 6c79 206b 6579 626f 6172 6420   reply keyboard 
+00016110: 6f72 2074 6f20 666f 7263 6520 6120 7265  or to force a re
+00016120: 706c 7920 6672 6f6d 2074 6865 2075 7365  ply from the use
+00016130: 722e 0d0a 0d0a 2020 2020 2020 2020 5265  r.....        Re
+00016140: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00016150: 2020 2020 4f6e 2073 7563 6365 7373 2c20      On success, 
+00016160: 7468 6520 7365 6e74 203a 6f62 6a3a 607e  the sent :obj:`~
+00016170: 6669 7070 6572 2e74 7970 6573 2e4d 6573  fipper.types.Mes
+00016180: 7361 6765 6020 6973 2072 6574 7572 6e65  sage` is returne
+00016190: 642e 0d0a 0d0a 2020 2020 2020 2020 5261  d.....        Ra
+000161a0: 6973 6573 3a0d 0a20 2020 2020 2020 2020  ises:..         
+000161b0: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
+000161c0: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
+000161d0: 616d 2052 5043 2065 7272 6f72 2e0d 0a20  am RPC error... 
+000161e0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000161f0: 2020 2020 6966 2071 756f 7465 2069 7320      if quote is 
+00016200: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00016210: 2020 2071 756f 7465 203d 2073 656c 662e     quote = self.
+00016220: 6368 6174 2e74 7970 6520 213d 2065 6e75  chat.type != enu
+00016230: 6d73 2e43 6861 7454 7970 652e 5052 4956  ms.ChatType.PRIV
+00016240: 4154 450d 0a0d 0a20 2020 2020 2020 2069  ATE....        i
+00016250: 6620 7265 706c 795f 746f 5f6d 6573 7361  f reply_to_messa
+00016260: 6765 5f69 6420 6973 204e 6f6e 6520 616e  ge_id is None an
+00016270: 6420 7175 6f74 653a 0d0a 2020 2020 2020  d quote:..      
+00016280: 2020 2020 2020 7265 706c 795f 746f 5f6d        reply_to_m
+00016290: 6573 7361 6765 5f69 6420 3d20 7365 6c66  essage_id = self
+000162a0: 2e69 640d 0a0d 0a20 2020 2020 2020 2072  .id....        r
+000162b0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+000162c0: 2e5f 636c 6965 6e74 2e73 656e 645f 706f  ._client.send_po
+000162d0: 6c6c 280d 0a20 2020 2020 2020 2020 2020  ll(..           
+000162e0: 2063 6861 745f 6964 3d73 656c 662e 6368   chat_id=self.ch
+000162f0: 6174 2e69 642c 0d0a 2020 2020 2020 2020  at.id,..        
+00016300: 2020 2020 7175 6573 7469 6f6e 3d71 7565      question=que
+00016310: 7374 696f 6e2c 0d0a 2020 2020 2020 2020  stion,..        
+00016320: 2020 2020 6f70 7469 6f6e 733d 6f70 7469      options=opti
+00016330: 6f6e 732c 0d0a 2020 2020 2020 2020 2020  ons,..          
+00016340: 2020 6973 5f61 6e6f 6e79 6d6f 7573 3d69    is_anonymous=i
+00016350: 735f 616e 6f6e 796d 6f75 732c 0d0a 2020  s_anonymous,..  
+00016360: 2020 2020 2020 2020 2020 7479 7065 3d74            type=t
+00016370: 7970 652c 0d0a 2020 2020 2020 2020 2020  ype,..          
+00016380: 2020 616c 6c6f 7773 5f6d 756c 7469 706c    allows_multipl
+00016390: 655f 616e 7377 6572 733d 616c 6c6f 7773  e_answers=allows
+000163a0: 5f6d 756c 7469 706c 655f 616e 7377 6572  _multiple_answer
+000163b0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+000163c0: 636f 7272 6563 745f 6f70 7469 6f6e 5f69  correct_option_i
+000163d0: 643d 636f 7272 6563 745f 6f70 7469 6f6e  d=correct_option
+000163e0: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
+000163f0: 2020 6578 706c 616e 6174 696f 6e3d 6578    explanation=ex
+00016400: 706c 616e 6174 696f 6e2c 0d0a 2020 2020  planation,..    
+00016410: 2020 2020 2020 2020 6578 706c 616e 6174          explanat
+00016420: 696f 6e5f 7061 7273 655f 6d6f 6465 3d65  ion_parse_mode=e
+00016430: 7870 6c61 6e61 7469 6f6e 5f70 6172 7365  xplanation_parse
+00016440: 5f6d 6f64 652c 0d0a 2020 2020 2020 2020  _mode,..        
+00016450: 2020 2020 6578 706c 616e 6174 696f 6e5f      explanation_
+00016460: 656e 7469 7469 6573 3d65 7870 6c61 6e61  entities=explana
+00016470: 7469 6f6e 5f65 6e74 6974 6965 732c 0d0a  tion_entities,..
+00016480: 2020 2020 2020 2020 2020 2020 6f70 656e              open
+00016490: 5f70 6572 696f 643d 6f70 656e 5f70 6572  _period=open_per
+000164a0: 696f 642c 0d0a 2020 2020 2020 2020 2020  iod,..          
+000164b0: 2020 636c 6f73 655f 6461 7465 3d63 6c6f    close_date=clo
+000164c0: 7365 5f64 6174 652c 0d0a 2020 2020 2020  se_date,..      
+000164d0: 2020 2020 2020 6973 5f63 6c6f 7365 643d        is_closed=
+000164e0: 6973 5f63 6c6f 7365 642c 0d0a 2020 2020  is_closed,..    
+000164f0: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+00016500: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
+00016510: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00016520: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
+00016530: 7072 6f74 6563 745f 636f 6e74 656e 743d  protect_content=
+00016540: 7072 6f74 6563 745f 636f 6e74 656e 742c  protect_content,
+00016550: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00016560: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00016570: 643d 7265 706c 795f 746f 5f6d 6573 7361  d=reply_to_messa
+00016580: 6765 5f69 642c 0d0a 2020 2020 2020 2020  ge_id,..        
+00016590: 2020 2020 7363 6865 6475 6c65 5f64 6174      schedule_dat
+000165a0: 653d 7363 6865 6475 6c65 5f64 6174 652c  e=schedule_date,
+000165b0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000165c0: 706c 795f 6d61 726b 7570 3d72 6570 6c79  ply_markup=reply
+000165d0: 5f6d 6172 6b75 700d 0a20 2020 2020 2020  _markup..       
+000165e0: 2029 0d0a 0d0a 2020 2020 6173 796e 6320   )....    async 
+000165f0: 6465 6620 7265 706c 795f 7374 6963 6b65  def reply_sticke
+00016600: 7228 0d0a 2020 2020 2020 2020 7365 6c66  r(..        self
+00016610: 2c0d 0a20 2020 2020 2020 2073 7469 636b  ,..        stick
+00016620: 6572 3a20 556e 696f 6e5b 7374 722c 2042  er: Union[str, B
+00016630: 696e 6172 7949 4f5d 2c0d 0a20 2020 2020  inaryIO],..     
+00016640: 2020 2071 756f 7465 3a20 626f 6f6c 203d     quote: bool =
+00016650: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00016660: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00016670: 7469 6f6e 3a20 626f 6f6c 203d 204e 6f6e  tion: bool = Non
+00016680: 652c 0d0a 2020 2020 2020 2020 7265 706c  e,..        repl
+00016690: 795f 746f 5f6d 6573 7361 6765 5f69 643a  y_to_message_id:
+000166a0: 2069 6e74 203d 204e 6f6e 652c 0d0a 2020   int = None,..  
+000166b0: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+000166c0: 7570 3a20 556e 696f 6e5b 0d0a 2020 2020  up: Union[..    
+000166d0: 2020 2020 2020 2020 2274 7970 6573 2e49          "types.I
+000166e0: 6e6c 696e 654b 6579 626f 6172 644d 6172  nlineKeyboardMar
+000166f0: 6b75 7022 2c0d 0a20 2020 2020 2020 2020  kup",..         
+00016700: 2020 2022 7479 7065 732e 5265 706c 794b     "types.ReplyK
+00016710: 6579 626f 6172 644d 6172 6b75 7022 2c0d  eyboardMarkup",.
+00016720: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+00016730: 7065 732e 5265 706c 794b 6579 626f 6172  pes.ReplyKeyboar
+00016740: 6452 656d 6f76 6522 2c0d 0a20 2020 2020  dRemove",..     
+00016750: 2020 2020 2020 2022 7479 7065 732e 466f         "types.Fo
+00016760: 7263 6552 6570 6c79 220d 0a20 2020 2020  rceReply"..     
+00016770: 2020 205d 203d 204e 6f6e 652c 0d0a 2020     ] = None,..  
+00016780: 2020 2020 2020 7072 6f67 7265 7373 3a20        progress: 
+00016790: 4361 6c6c 6162 6c65 203d 204e 6f6e 652c  Callable = None,
+000167a0: 0d0a 2020 2020 2020 2020 7072 6f67 7265  ..        progre
+000167b0: 7373 5f61 7267 733a 2074 7570 6c65 203d  ss_args: tuple =
+000167c0: 2028 290d 0a20 2020 2029 202d 3e20 224d   ()..    ) -> "M
+000167d0: 6573 7361 6765 223a 0d0a 2020 2020 2020  essage":..      
+000167e0: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
+000167f0: 6420 2a72 6570 6c79 5f73 7469 636b 6572  d *reply_sticker
+00016800: 2a20 6f66 203a 6f62 6a3a 607e 6669 7070  * of :obj:`~fipp
+00016810: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
+00016820: 602e 0d0a 0d0a 2020 2020 2020 2020 5573  `.....        Us
+00016830: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
+00016840: 666f 723a 0d0a 0d0a 2020 2020 2020 2020  for:....        
+00016850: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00016860: 7079 7468 6f6e 0d0a 0d0a 2020 2020 2020  python....      
+00016870: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
+00016880: 6e74 2e73 656e 645f 7374 6963 6b65 7228  nt.send_sticker(
+00016890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000168a0: 2020 6368 6174 5f69 643d 6d65 7373 6167    chat_id=messag
+000168b0: 652e 6368 6174 2e69 642c 0d0a 2020 2020  e.chat.id,..    
+000168c0: 2020 2020 2020 2020 2020 2020 7374 6963              stic
+000168d0: 6b65 723d 7374 6963 6b65 720d 0a20 2020  ker=sticker..   
+000168e0: 2020 2020 2020 2020 2029 0d0a 0d0a 2020           )....  
+000168f0: 2020 2020 2020 4578 616d 706c 653a 0d0a        Example:..
+00016900: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
+00016910: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00016920: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
+00016930: 2020 2020 2020 6177 6169 7420 6d65 7373        await mess
+00016940: 6167 652e 7265 706c 795f 7374 6963 6b65  age.reply_sticke
+00016950: 7228 7374 6963 6b65 7229 0d0a 0d0a 2020  r(sticker)....  
+00016960: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00016970: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00016980: 7469 636b 6572 2028 6060 7374 7260 6029  ticker (``str``)
+00016990: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000169a0: 2020 2053 7469 636b 6572 2074 6f20 7365     Sticker to se
+000169b0: 6e64 2e0d 0a20 2020 2020 2020 2020 2020  nd...           
+000169c0: 2020 2020 2050 6173 7320 6120 6669 6c65       Pass a file
+000169d0: 5f69 6420 6173 2073 7472 696e 6720 746f  _id as string to
+000169e0: 2073 656e 6420 6120 7374 6963 6b65 7220   send a sticker 
+000169f0: 7468 6174 2065 7869 7374 7320 6f6e 2074  that exists on t
+00016a00: 6865 2054 656c 6567 7261 6d20 7365 7276  he Telegram serv
+00016a10: 6572 732c 0d0a 2020 2020 2020 2020 2020  ers,..          
+00016a20: 2020 2020 2020 7061 7373 2061 6e20 4854        pass an HT
+00016a30: 5450 2055 524c 2061 7320 6120 7374 7269  TP URL as a stri
+00016a40: 6e67 2066 6f72 2054 656c 6567 7261 6d20  ng for Telegram 
+00016a50: 746f 2067 6574 2061 202e 7765 6270 2073  to get a .webp s
+00016a60: 7469 636b 6572 2066 696c 6520 6672 6f6d  ticker file from
+00016a70: 2074 6865 2049 6e74 6572 6e65 742c 206f   the Internet, o
+00016a80: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00016a90: 2020 2070 6173 7320 6120 6669 6c65 2070     pass a file p
+00016aa0: 6174 6820 6173 2073 7472 696e 6720 746f  ath as string to
+00016ab0: 2075 706c 6f61 6420 6120 6e65 7720 7374   upload a new st
+00016ac0: 6963 6b65 7220 7468 6174 2065 7869 7374  icker that exist
+00016ad0: 7320 6f6e 2079 6f75 7220 6c6f 6361 6c20  s on your local 
+00016ae0: 6d61 6368 696e 652e 0d0a 0d0a 2020 2020  machine.....    
+00016af0: 2020 2020 2020 2020 7175 6f74 6520 2860          quote (`
+00016b00: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
+00016b10: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+00016b20: 2020 2020 2020 2049 6620 6060 5472 7565         If ``True
+00016b30: 6060 2c20 7468 6520 6d65 7373 6167 6520  ``, the message 
+00016b40: 7769 6c6c 2062 6520 7365 6e74 2061 7320  will be sent as 
+00016b50: 6120 7265 706c 7920 746f 2074 6869 7320  a reply to this 
+00016b60: 6d65 7373 6167 652e 0d0a 2020 2020 2020  message...      
+00016b70: 2020 2020 2020 2020 2020 4966 202a 7265            If *re
+00016b80: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00016b90: 642a 2069 7320 7061 7373 6564 2c20 7468  d* is passed, th
+00016ba0: 6973 2070 6172 616d 6574 6572 2077 696c  is parameter wil
+00016bb0: 6c20 6265 2069 676e 6f72 6564 2e0d 0a20  l be ignored... 
+00016bc0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00016bd0: 6566 6175 6c74 7320 746f 2060 6054 7275  efaults to ``Tru
+00016be0: 6560 6020 696e 2067 726f 7570 2063 6861  e`` in group cha
+00016bf0: 7473 2061 6e64 2060 6046 616c 7365 6060  ts and ``False``
+00016c00: 2069 6e20 7072 6976 6174 6520 6368 6174   in private chat
+00016c10: 732e 0d0a 0d0a 2020 2020 2020 2020 2020  s.....          
+00016c20: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
+00016c30: 6361 7469 6f6e 2028 6060 626f 6f6c 6060  cation (``bool``
+00016c40: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c60: 5365 6e64 7320 7468 6520 6d65 7373 6167  Sends the messag
+00016c70: 6520 7369 6c65 6e74 6c79 2e0d 0a20 2020  e silently...   
+00016c80: 2020 2020 2020 2020 2020 2020 2055 7365               Use
+00016c90: 7273 2077 696c 6c20 7265 6365 6976 6520  rs will receive 
+00016ca0: 6120 6e6f 7469 6669 6361 7469 6f6e 2077  a notification w
+00016cb0: 6974 6820 6e6f 2073 6f75 6e64 2e0d 0a0d  ith no sound....
+00016cc0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00016cd0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+00016ce0: 2028 6060 696e 7460 602c 202a 6f70 7469   (``int``, *opti
+00016cf0: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
+00016d00: 2020 2020 2020 2020 2049 6620 7468 6520           If the 
+00016d10: 6d65 7373 6167 6520 6973 2061 2072 6570  message is a rep
+00016d20: 6c79 2c20 4944 206f 6620 7468 6520 6f72  ly, ID of the or
+00016d30: 6967 696e 616c 206d 6573 7361 6765 2e0d  iginal message..
+00016d40: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+00016d50: 6570 6c79 5f6d 6172 6b75 7020 283a 6f62  eply_markup (:ob
+00016d60: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+00016d70: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
+00016d80: 6172 6b75 7060 207c 203a 6f62 6a3a 607e  arkup` | :obj:`~
+00016d90: 6669 7070 6572 2e74 7970 6573 2e52 6570  fipper.types.Rep
+00016da0: 6c79 4b65 7962 6f61 7264 4d61 726b 7570  lyKeyboardMarkup
+00016db0: 6020 7c20 3a6f 626a 3a60 7e66 6970 7065  ` | :obj:`~fippe
+00016dc0: 722e 7479 7065 732e 5265 706c 794b 6579  r.types.ReplyKey
+00016dd0: 626f 6172 6452 656d 6f76 6560 207c 203a  boardRemove` | :
+00016de0: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+00016df0: 6573 2e46 6f72 6365 5265 706c 7960 2c20  es.ForceReply`, 
+00016e00: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+00016e10: 2020 2020 2020 2020 2020 2020 2020 4164                Ad
+00016e20: 6469 7469 6f6e 616c 2069 6e74 6572 6661  ditional interfa
+00016e30: 6365 206f 7074 696f 6e73 2e20 416e 206f  ce options. An o
+00016e40: 626a 6563 7420 666f 7220 616e 2069 6e6c  bject for an inl
+00016e50: 696e 6520 6b65 7962 6f61 7264 2c20 6375  ine keyboard, cu
+00016e60: 7374 6f6d 2072 6570 6c79 206b 6579 626f  stom reply keybo
+00016e70: 6172 642c 0d0a 2020 2020 2020 2020 2020  ard,..          
+00016e80: 2020 2020 2020 696e 7374 7275 6374 696f        instructio
+00016e90: 6e73 2074 6f20 7265 6d6f 7665 2072 6570  ns to remove rep
+00016ea0: 6c79 206b 6579 626f 6172 6420 6f72 2074  ly keyboard or t
+00016eb0: 6f20 666f 7263 6520 6120 7265 706c 7920  o force a reply 
+00016ec0: 6672 6f6d 2074 6865 2075 7365 722e 0d0a  from the user...
+00016ed0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00016ee0: 6f67 7265 7373 2028 6060 4361 6c6c 6162  ogress (``Callab
+00016ef0: 6c65 6060 2c20 2a6f 7074 696f 6e61 6c2a  le``, *optional*
+00016f00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016f10: 2020 2020 5061 7373 2061 2063 616c 6c62      Pass a callb
+00016f20: 6163 6b20 6675 6e63 7469 6f6e 2074 6f20  ack function to 
+00016f30: 7669 6577 2074 6865 2066 696c 6520 7472  view the file tr
+00016f40: 616e 736d 6973 7369 6f6e 2070 726f 6772  ansmission progr
+00016f50: 6573 732e 0d0a 2020 2020 2020 2020 2020  ess...          
+00016f60: 2020 2020 2020 5468 6520 6675 6e63 7469        The functi
+00016f70: 6f6e 206d 7573 7420 7461 6b65 202a 2863  on must take *(c
+00016f80: 7572 7265 6e74 2c20 746f 7461 6c29 2a20  urrent, total)* 
+00016f90: 6173 2070 6f73 6974 696f 6e61 6c20 6172  as positional ar
+00016fa0: 6775 6d65 6e74 7320 286c 6f6f 6b20 6174  guments (look at
+00016fb0: 204f 7468 6572 2050 6172 616d 6574 6572   Other Parameter
+00016fc0: 7320 6265 6c6f 7720 666f 7220 610d 0a20  s below for a.. 
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00016fe0: 6574 6169 6c65 6420 6465 7363 7269 7074  etailed descript
+00016ff0: 696f 6e29 2061 6e64 2077 696c 6c20 6265  ion) and will be
+00017000: 2063 616c 6c65 6420 6261 636b 2065 6163   called back eac
+00017010: 6820 7469 6d65 2061 206e 6577 2066 696c  h time a new fil
+00017020: 6520 6368 756e 6b20 6861 7320 6265 656e  e chunk has been
+00017030: 2073 7563 6365 7373 6675 6c6c 790d 0a20   successfully.. 
+00017040: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00017050: 7261 6e73 6d69 7474 6564 2e0d 0a0d 0a20  ransmitted..... 
+00017060: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+00017070: 6573 735f 6172 6773 2028 6060 7475 706c  ess_args (``tupl
+00017080: 6560 602c 202a 6f70 7469 6f6e 616c 2a29  e``, *optional*)
+00017090: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000170a0: 2020 2045 7874 7261 2063 7573 746f 6d20     Extra custom 
+000170b0: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
+000170c0: 6520 7072 6f67 7265 7373 2063 616c 6c62  e progress callb
+000170d0: 6163 6b20 6675 6e63 7469 6f6e 2e0d 0a20  ack function... 
+000170e0: 2020 2020 2020 2020 2020 2020 2020 2059                 Y
+000170f0: 6f75 2063 616e 2070 6173 7320 616e 7974  ou can pass anyt
+00017100: 6869 6e67 2079 6f75 206e 6565 6420 746f  hing you need to
+00017110: 2062 6520 6176 6169 6c61 626c 6520 696e   be available in
+00017120: 2074 6865 2070 726f 6772 6573 7320 6361   the progress ca
+00017130: 6c6c 6261 636b 2073 636f 7065 3b20 666f  llback scope; fo
+00017140: 7220 6578 616d 706c 652c 2061 204d 6573  r example, a Mes
+00017150: 7361 6765 0d0a 2020 2020 2020 2020 2020  sage..          
+00017160: 2020 2020 2020 6f62 6a65 6374 206f 7220        object or 
+00017170: 6120 436c 6965 6e74 2069 6e73 7461 6e63  a Client instanc
+00017180: 6520 696e 206f 7264 6572 2074 6f20 6564  e in order to ed
+00017190: 6974 2074 6865 206d 6573 7361 6765 2077  it the message w
+000171a0: 6974 6820 7468 6520 7570 6461 7465 6420  ith the updated 
+000171b0: 7072 6f67 7265 7373 2073 7461 7475 732e  progress status.
+000171c0: 0d0a 0d0a 2020 2020 2020 2020 4f74 6865  ....        Othe
+000171d0: 7220 5061 7261 6d65 7465 7273 3a0d 0a20  r Parameters:.. 
+000171e0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+000171f0: 6e74 2028 6060 696e 7460 6029 3a0d 0a20  nt (``int``):.. 
+00017200: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00017210: 6865 2061 6d6f 756e 7420 6f66 2062 7974  he amount of byt
+00017220: 6573 2074 7261 6e73 6d69 7474 6564 2073  es transmitted s
+00017230: 6f20 6661 722e 0d0a 0d0a 2020 2020 2020  o far.....      
+00017240: 2020 2020 2020 746f 7461 6c20 2860 6069        total (``i
+00017250: 6e74 6060 293a 0d0a 2020 2020 2020 2020  nt``):..        
+00017260: 2020 2020 2020 2020 5468 6520 746f 7461          The tota
+00017270: 6c20 7369 7a65 206f 6620 7468 6520 6669  l size of the fi
+00017280: 6c65 2e0d 0a0d 0a20 2020 2020 2020 2020  le.....         
+00017290: 2020 202a 6172 6773 2028 6060 7475 706c     *args (``tupl
+000172a0: 6560 602c 202a 6f70 7469 6f6e 616c 2a29  e``, *optional*)
+000172b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000172c0: 2020 2045 7874 7261 2063 7573 746f 6d20     Extra custom 
+000172d0: 6172 6775 6d65 6e74 7320 6173 2064 6566  arguments as def
+000172e0: 696e 6564 2069 6e20 7468 6520 6060 7072  ined in the ``pr
+000172f0: 6f67 7265 7373 5f61 7267 7360 6020 7061  ogress_args`` pa
+00017300: 7261 6d65 7465 722e 0d0a 2020 2020 2020  rameter...      
+00017310: 2020 2020 2020 2020 2020 596f 7520 6361            You ca
+00017320: 6e20 6569 7468 6572 206b 6565 7020 6060  n either keep ``
+00017330: 2a61 7267 7360 6020 6f72 2061 6464 2065  *args`` or add e
+00017340: 7665 7279 2073 696e 676c 6520 6578 7472  very single extr
+00017350: 6120 6172 6775 6d65 6e74 2069 6e20 796f  a argument in yo
+00017360: 7572 2066 756e 6374 696f 6e20 7369 676e  ur function sign
+00017370: 6174 7572 652e 0d0a 0d0a 2020 2020 2020  ature.....      
+00017380: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00017390: 2020 2020 2020 2020 4f6e 2073 7563 6365          On succe
+000173a0: 7373 2c20 7468 6520 7365 6e74 203a 6f62  ss, the sent :ob
+000173b0: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+000173c0: 2e4d 6573 7361 6765 6020 6973 2072 6574  .Message` is ret
+000173d0: 7572 6e65 642e 0d0a 2020 2020 2020 2020  urned...        
+000173e0: 2020 2020 496e 2063 6173 6520 7468 6520      In case the 
+000173f0: 7570 6c6f 6164 2069 7320 6465 6c69 6265  upload is delibe
+00017400: 7261 7465 6c79 2073 746f 7070 6564 2077  rately stopped w
+00017410: 6974 6820 3a6d 6574 683a 607e 6669 7070  ith :meth:`~fipp
+00017420: 6572 2e43 6c69 656e 742e 7374 6f70 5f74  er.Client.stop_t
+00017430: 7261 6e73 6d69 7373 696f 6e60 2c20 4e6f  ransmission`, No
+00017440: 6e65 2069 7320 7265 7475 726e 6564 0d0a  ne is returned..
+00017450: 2020 2020 2020 2020 2020 2020 696e 7374              inst
+00017460: 6561 642e 0d0a 0d0a 2020 2020 2020 2020  ead.....        
+00017470: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+00017480: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+00017490: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+000174a0: 6772 616d 2052 5043 2065 7272 6f72 2e0d  gram RPC error..
+000174b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000174c0: 2020 2020 2020 6966 2071 756f 7465 2069        if quote i
+000174d0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+000174e0: 2020 2020 2071 756f 7465 203d 2073 656c       quote = sel
+000174f0: 662e 6368 6174 2e74 7970 6520 213d 2065  f.chat.type != e
+00017500: 6e75 6d73 2e43 6861 7454 7970 652e 5052  nums.ChatType.PR
+00017510: 4956 4154 450d 0a0d 0a20 2020 2020 2020  IVATE....       
+00017520: 2069 6620 7265 706c 795f 746f 5f6d 6573   if reply_to_mes
+00017530: 7361 6765 5f69 6420 6973 204e 6f6e 6520  sage_id is None 
+00017540: 616e 6420 7175 6f74 653a 0d0a 2020 2020  and quote:..    
+00017550: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
+00017560: 5f6d 6573 7361 6765 5f69 6420 3d20 7365  _message_id = se
+00017570: 6c66 2e69 640d 0a0d 0a20 2020 2020 2020  lf.id....       
+00017580: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00017590: 6c66 2e5f 636c 6965 6e74 2e73 656e 645f  lf._client.send_
+000175a0: 7374 6963 6b65 7228 0d0a 2020 2020 2020  sticker(..      
+000175b0: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
+000175c0: 6c66 2e63 6861 742e 6964 2c0d 0a20 2020  lf.chat.id,..   
+000175d0: 2020 2020 2020 2020 2073 7469 636b 6572           sticker
+000175e0: 3d73 7469 636b 6572 2c0d 0a20 2020 2020  =sticker,..     
+000175f0: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
+00017600: 6f74 6966 6963 6174 696f 6e3d 6469 7361  otification=disa
+00017610: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+00017620: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00017630: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+00017640: 6964 3d72 6570 6c79 5f74 6f5f 6d65 7373  id=reply_to_mess
+00017650: 6167 655f 6964 2c0d 0a20 2020 2020 2020  age_id,..       
+00017660: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
+00017670: 703d 7265 706c 795f 6d61 726b 7570 2c0d  p=reply_markup,.
+00017680: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00017690: 6772 6573 733d 7072 6f67 7265 7373 2c0d  gress=progress,.
+000176a0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000176b0: 6772 6573 735f 6172 6773 3d70 726f 6772  gress_args=progr
+000176c0: 6573 735f 6172 6773 0d0a 2020 2020 2020  ess_args..      
+000176d0: 2020 290d 0a0d 0a20 2020 2061 7379 6e63    )....    async
+000176e0: 2064 6566 2072 6570 6c79 5f76 656e 7565   def reply_venue
+000176f0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
+00017700: 0d0a 2020 2020 2020 2020 6c61 7469 7475  ..        latitu
+00017710: 6465 3a20 666c 6f61 742c 0d0a 2020 2020  de: float,..    
+00017720: 2020 2020 6c6f 6e67 6974 7564 653a 2066      longitude: f
+00017730: 6c6f 6174 2c0d 0a20 2020 2020 2020 2074  loat,..        t
+00017740: 6974 6c65 3a20 7374 722c 0d0a 2020 2020  itle: str,..    
+00017750: 2020 2020 6164 6472 6573 733a 2073 7472      address: str
+00017760: 2c0d 0a20 2020 2020 2020 2071 756f 7465  ,..        quote
+00017770: 3a20 626f 6f6c 203d 204e 6f6e 652c 0d0a  : bool = None,..
+00017780: 2020 2020 2020 2020 666f 7572 7371 7561          foursqua
+00017790: 7265 5f69 643a 2073 7472 203d 2022 222c  re_id: str = "",
+000177a0: 0d0a 2020 2020 2020 2020 666f 7572 7371  ..        foursq
+000177b0: 7561 7265 5f74 7970 653a 2073 7472 203d  uare_type: str =
+000177c0: 2022 222c 0d0a 2020 2020 2020 2020 6469   "",..        di
+000177d0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+000177e0: 6f6e 3a20 626f 6f6c 203d 204e 6f6e 652c  on: bool = None,
+000177f0: 0d0a 2020 2020 2020 2020 7265 706c 795f  ..        reply_
+00017800: 746f 5f6d 6573 7361 6765 5f69 643a 2069  to_message_id: i
+00017810: 6e74 203d 204e 6f6e 652c 0d0a 2020 2020  nt = None,..    
+00017820: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
+00017830: 3a20 556e 696f 6e5b 0d0a 2020 2020 2020  : Union[..      
+00017840: 2020 2020 2020 2274 7970 6573 2e49 6e6c        "types.Inl
+00017850: 696e 654b 6579 626f 6172 644d 6172 6b75  ineKeyboardMarku
+00017860: 7022 2c0d 0a20 2020 2020 2020 2020 2020  p",..           
+00017870: 2022 7479 7065 732e 5265 706c 794b 6579   "types.ReplyKey
+00017880: 626f 6172 644d 6172 6b75 7022 2c0d 0a20  boardMarkup",.. 
+00017890: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000178a0: 732e 5265 706c 794b 6579 626f 6172 6452  s.ReplyKeyboardR
+000178b0: 656d 6f76 6522 2c0d 0a20 2020 2020 2020  emove",..       
+000178c0: 2020 2020 2022 7479 7065 732e 466f 7263       "types.Forc
+000178d0: 6552 6570 6c79 220d 0a20 2020 2020 2020  eReply"..       
+000178e0: 205d 203d 204e 6f6e 650d 0a20 2020 2029   ] = None..    )
+000178f0: 202d 3e20 224d 6573 7361 6765 223a 0d0a   -> "Message":..
+00017900: 2020 2020 2020 2020 2222 2242 6f75 6e64          """Bound
+00017910: 206d 6574 686f 6420 2a72 6570 6c79 5f76   method *reply_v
+00017920: 656e 7565 2a20 6f66 203a 6f62 6a3a 607e  enue* of :obj:`~
+00017930: 6669 7070 6572 2e74 7970 6573 2e4d 6573  fipper.types.Mes
+00017940: 7361 6765 602e 0d0a 0d0a 2020 2020 2020  sage`.....      
+00017950: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
+00017960: 6375 7420 666f 723a 0d0a 0d0a 2020 2020  cut for:....    
+00017970: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+00017980: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
+00017990: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+000179a0: 636c 6965 6e74 2e73 656e 645f 7665 6e75  client.send_venu
+000179b0: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+000179c0: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
+000179d0: 6167 652e 6368 6174 2e69 642c 0d0a 2020  age.chat.id,..  
+000179e0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+000179f0: 7469 7475 6465 3d6c 6174 6974 7564 652c  titude=latitude,
+00017a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017a10: 2020 6c6f 6e67 6974 7564 653d 6c6f 6e67    longitude=long
+00017a20: 6974 7564 652c 0d0a 2020 2020 2020 2020  itude,..        
+00017a30: 2020 2020 2020 2020 7469 746c 653d 2256          title="V
+00017a40: 656e 7565 2074 6974 6c65 222c 0d0a 2020  enue title",..  
+00017a50: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00017a60: 6472 6573 733d 2256 656e 7565 2061 6464  dress="Venue add
+00017a70: 7265 7373 220d 0a20 2020 2020 2020 2020  ress"..         
+00017a80: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+00017a90: 4578 616d 706c 653a 0d0a 2020 2020 2020  Example:..      
+00017aa0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+00017ab0: 6f63 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a  ock:: python....
+00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ad0: 6177 6169 7420 6d65 7373 6167 652e 7265  await message.re
+00017ae0: 706c 795f 7665 6e75 6528 6c61 7469 7475  ply_venue(latitu
+00017af0: 6465 2c20 6c6f 6e67 6974 7564 652c 2022  de, longitude, "
+00017b00: 5665 6e75 6520 7469 746c 6522 2c20 2256  Venue title", "V
+00017b10: 656e 7565 2061 6464 7265 7373 2229 0d0a  enue address")..
+00017b20: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00017b30: 7465 7273 3a0d 0a20 2020 2020 2020 2020  ters:..         
+00017b40: 2020 206c 6174 6974 7564 6520 2860 6066     latitude (``f
+00017b50: 6c6f 6174 6060 293a 0d0a 2020 2020 2020  loat``):..      
+00017b60: 2020 2020 2020 2020 2020 4c61 7469 7475            Latitu
+00017b70: 6465 206f 6620 7468 6520 7665 6e75 652e  de of the venue.
+00017b80: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017b90: 6c6f 6e67 6974 7564 6520 2860 6066 6c6f  longitude (``flo
+00017ba0: 6174 6060 293a 0d0a 2020 2020 2020 2020  at``):..        
+00017bb0: 2020 2020 2020 2020 4c6f 6e67 6974 7564          Longitud
+00017bc0: 6520 6f66 2074 6865 2076 656e 7565 2e0d  e of the venue..
+00017bd0: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+00017be0: 6974 6c65 2028 6060 7374 7260 6029 3a0d  itle (``str``):.
+00017bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c00: 204e 616d 6520 6f66 2074 6865 2076 656e   Name of the ven
+00017c10: 7565 2e0d 0a0d 0a20 2020 2020 2020 2020  ue.....         
+00017c20: 2020 2061 6464 7265 7373 2028 6060 7374     address (``st
+00017c30: 7260 6029 3a0d 0a20 2020 2020 2020 2020  r``):..         
+00017c40: 2020 2020 2020 2041 6464 7265 7373 206f         Address o
+00017c50: 6620 7468 6520 7665 6e75 652e 0d0a 0d0a  f the venue.....
+00017c60: 2020 2020 2020 2020 2020 2020 7175 6f74              quot
+00017c70: 6520 2860 6062 6f6f 6c60 602c 202a 6f70  e (``bool``, *op
+00017c80: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00017c90: 2020 2020 2020 2020 2020 2049 6620 6060             If ``
+00017ca0: 5472 7565 6060 2c20 7468 6520 6d65 7373  True``, the mess
+00017cb0: 6167 6520 7769 6c6c 2062 6520 7365 6e74  age will be sent
+00017cc0: 2061 7320 6120 7265 706c 7920 746f 2074   as a reply to t
+00017cd0: 6869 7320 6d65 7373 6167 652e 0d0a 2020  his message...  
+00017ce0: 2020 2020 2020 2020 2020 2020 2020 4966                If
+00017cf0: 202a 7265 706c 795f 746f 5f6d 6573 7361   *reply_to_messa
+00017d00: 6765 5f69 642a 2069 7320 7061 7373 6564  ge_id* is passed
+00017d10: 2c20 7468 6973 2070 6172 616d 6574 6572  , this parameter
+00017d20: 2077 696c 6c20 6265 2069 676e 6f72 6564   will be ignored
+00017d30: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017d40: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
+00017d50: 6054 7275 6560 6020 696e 2067 726f 7570  `True`` in group
+00017d60: 2063 6861 7473 2061 6e64 2060 6046 616c   chats and ``Fal
+00017d70: 7365 6060 2069 6e20 7072 6976 6174 6520  se`` in private 
+00017d80: 6368 6174 732e 0d0a 0d0a 2020 2020 2020  chats.....      
+00017d90: 2020 2020 2020 666f 7572 7371 7561 7265        foursquare
+00017da0: 5f69 6420 2860 6073 7472 6060 2c20 2a6f  _id (``str``, *o
+00017db0: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+00017dc0: 2020 2020 2020 2020 2020 2020 466f 7572              Four
+00017dd0: 7371 7561 7265 2069 6465 6e74 6966 6965  square identifie
+00017de0: 7220 6f66 2074 6865 2076 656e 7565 2e0d  r of the venue..
+00017df0: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
+00017e00: 6f75 7273 7175 6172 655f 7479 7065 2028  oursquare_type (
+00017e10: 6060 7374 7260 602c 202a 6f70 7469 6f6e  ``str``, *option
+00017e20: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+00017e30: 2020 2020 2020 2046 6f75 7273 7175 6172         Foursquar
+00017e40: 6520 7479 7065 206f 6620 7468 6520 7665  e type of the ve
+00017e50: 6e75 652c 2069 6620 6b6e 6f77 6e2e 0d0a  nue, if known...
+00017e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e70: 2846 6f72 2065 7861 6d70 6c65 2c20 2261  (For example, "a
+00017e80: 7274 735f 656e 7465 7274 6169 6e6d 656e  rts_entertainmen
+00017e90: 742f 6465 6661 756c 7422 2c20 2261 7274  t/default", "art
+00017ea0: 735f 656e 7465 7274 6169 6e6d 656e 742f  s_entertainment/
+00017eb0: 6171 7561 7269 756d 2220 6f72 2022 666f  aquarium" or "fo
+00017ec0: 6f64 2f69 6365 6372 6561 6d22 2e29 0d0a  od/icecream".)..
+00017ed0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+00017ee0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00017ef0: 6f6e 2028 6060 626f 6f6c 6060 2c20 2a6f  on (``bool``, *o
+00017f00: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+00017f10: 2020 2020 2020 2020 2020 2020 5365 6e64              Send
+00017f20: 7320 7468 6520 6d65 7373 6167 6520 7369  s the message si
+00017f30: 6c65 6e74 6c79 2e0d 0a20 2020 2020 2020  lently...       
+00017f40: 2020 2020 2020 2020 2055 7365 7273 2077           Users w
+00017f50: 696c 6c20 7265 6365 6976 6520 6120 6e6f  ill receive a no
+00017f60: 7469 6669 6361 7469 6f6e 2077 6974 6820  tification with 
+00017f70: 6e6f 2073 6f75 6e64 2e0d 0a0d 0a20 2020  no sound.....   
+00017f80: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
+00017f90: 6f5f 6d65 7373 6167 655f 6964 2028 6060  o_message_id (``
+00017fa0: 696e 7460 602c 202a 6f70 7469 6f6e 616c  int``, *optional
+00017fb0: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
+00017fc0: 2020 2020 2049 6620 7468 6520 6d65 7373       If the mess
+00017fd0: 6167 6520 6973 2061 2072 6570 6c79 2c20  age is a reply, 
+00017fe0: 4944 206f 6620 7468 6520 6f72 6967 696e  ID of the origin
+00017ff0: 616c 206d 6573 7361 6765 0d0a 0d0a 2020  al message....  
+00018000: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00018010: 6d61 726b 7570 2028 3a6f 626a 3a60 7e66  markup (:obj:`~f
+00018020: 6970 7065 722e 7479 7065 732e 496e 6c69  ipper.types.Inli
+00018030: 6e65 4b65 7962 6f61 7264 4d61 726b 7570  neKeyboardMarkup
+00018040: 6020 7c20 3a6f 626a 3a60 7e66 6970 7065  ` | :obj:`~fippe
+00018050: 722e 7479 7065 732e 5265 706c 794b 6579  r.types.ReplyKey
+00018060: 626f 6172 644d 6172 6b75 7060 207c 203a  boardMarkup` | :
+00018070: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+00018080: 6573 2e52 6570 6c79 4b65 7962 6f61 7264  es.ReplyKeyboard
+00018090: 5265 6d6f 7665 6020 7c20 3a6f 626a 3a60  Remove` | :obj:`
+000180a0: 7e66 6970 7065 722e 7479 7065 732e 466f  ~fipper.types.Fo
+000180b0: 7263 6552 6570 6c79 602c 202a 6f70 7469  rceReply`, *opti
+000180c0: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
+000180d0: 2020 2020 2020 2020 2041 6464 6974 696f           Additio
+000180e0: 6e61 6c20 696e 7465 7266 6163 6520 6f70  nal interface op
+000180f0: 7469 6f6e 732e 2041 6e20 6f62 6a65 6374  tions. An object
+00018100: 2066 6f72 2061 6e20 696e 6c69 6e65 206b   for an inline k
+00018110: 6579 626f 6172 642c 2063 7573 746f 6d20  eyboard, custom 
+00018120: 7265 706c 7920 6b65 7962 6f61 7264 2c0d  reply keyboard,.
+00018130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018140: 2069 6e73 7472 7563 7469 6f6e 7320 746f   instructions to
+00018150: 2072 656d 6f76 6520 7265 706c 7920 6b65   remove reply ke
+00018160: 7962 6f61 7264 206f 7220 746f 2066 6f72  yboard or to for
+00018170: 6365 2061 2072 6570 6c79 2066 726f 6d20  ce a reply from 
+00018180: 7468 6520 7573 6572 2e0d 0a0d 0a20 2020  the user.....   
+00018190: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+000181a0: 2020 2020 2020 2020 2020 204f 6e20 7375             On su
+000181b0: 6363 6573 732c 2074 6865 2073 656e 7420  ccess, the sent 
+000181c0: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
+000181d0: 7065 732e 4d65 7373 6167 6560 2069 7320  pes.Message` is 
+000181e0: 7265 7475 726e 6564 2e0d 0a0d 0a20 2020  returned.....   
+000181f0: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
+00018200: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
+00018210: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
+00018220: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
+00018230: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
+00018240: 220d 0a20 2020 2020 2020 2069 6620 7175  "..        if qu
+00018250: 6f74 6520 6973 204e 6f6e 653a 0d0a 2020  ote is None:..  
+00018260: 2020 2020 2020 2020 2020 7175 6f74 6520            quote 
+00018270: 3d20 7365 6c66 2e63 6861 742e 7479 7065  = self.chat.type
+00018280: 2021 3d20 656e 756d 732e 4368 6174 5479   != enums.ChatTy
+00018290: 7065 2e50 5249 5641 5445 0d0a 0d0a 2020  pe.PRIVATE....  
+000182a0: 2020 2020 2020 6966 2072 6570 6c79 5f74        if reply_t
+000182b0: 6f5f 6d65 7373 6167 655f 6964 2069 7320  o_message_id is 
+000182c0: 4e6f 6e65 2061 6e64 2071 756f 7465 3a0d  None and quote:.
+000182d0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+000182e0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+000182f0: 203d 2073 656c 662e 6964 0d0a 0d0a 2020   = self.id....  
+00018300: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00018310: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+00018320: 7365 6e64 5f76 656e 7565 280d 0a20 2020  send_venue(..   
+00018330: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+00018340: 3d73 656c 662e 6368 6174 2e69 642c 0d0a  =self.chat.id,..
+00018350: 2020 2020 2020 2020 2020 2020 6c61 7469              lati
+00018360: 7475 6465 3d6c 6174 6974 7564 652c 0d0a  tude=latitude,..
+00018370: 2020 2020 2020 2020 2020 2020 6c6f 6e67              long
+00018380: 6974 7564 653d 6c6f 6e67 6974 7564 652c  itude=longitude,
+00018390: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+000183a0: 746c 653d 7469 746c 652c 0d0a 2020 2020  tle=title,..    
+000183b0: 2020 2020 2020 2020 6164 6472 6573 733d          address=
+000183c0: 6164 6472 6573 732c 0d0a 2020 2020 2020  address,..      
+000183d0: 2020 2020 2020 666f 7572 7371 7561 7265        foursquare
+000183e0: 5f69 643d 666f 7572 7371 7561 7265 5f69  _id=foursquare_i
+000183f0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+00018400: 666f 7572 7371 7561 7265 5f74 7970 653d  foursquare_type=
+00018410: 666f 7572 7371 7561 7265 5f74 7970 652c  foursquare_type,
+00018420: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+00018430: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00018440: 6f6e 3d64 6973 6162 6c65 5f6e 6f74 6966  on=disable_notif
+00018450: 6963 6174 696f 6e2c 0d0a 2020 2020 2020  ication,..      
+00018460: 2020 2020 2020 7265 706c 795f 746f 5f6d        reply_to_m
+00018470: 6573 7361 6765 5f69 643d 7265 706c 795f  essage_id=reply_
+00018480: 746f 5f6d 6573 7361 6765 5f69 642c 0d0a  to_message_id,..
+00018490: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+000184a0: 795f 6d61 726b 7570 3d72 6570 6c79 5f6d  y_markup=reply_m
+000184b0: 6172 6b75 700d 0a20 2020 2020 2020 2029  arkup..        )
+000184c0: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
+000184d0: 6620 7265 706c 795f 7669 6465 6f28 0d0a  f reply_video(..
+000184e0: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
+000184f0: 2020 2020 2020 2076 6964 656f 3a20 556e         video: Un
+00018500: 696f 6e5b 7374 722c 2042 696e 6172 7949  ion[str, BinaryI
+00018510: 4f5d 2c0d 0a20 2020 2020 2020 2071 756f  O],..        quo
+00018520: 7465 3a20 626f 6f6c 203d 204e 6f6e 652c  te: bool = None,
+00018530: 0d0a 2020 2020 2020 2020 6361 7074 696f  ..        captio
+00018540: 6e3a 2073 7472 203d 2022 222c 0d0a 2020  n: str = "",..  
+00018550: 2020 2020 2020 7061 7273 655f 6d6f 6465        parse_mode
+00018560: 3a20 4f70 7469 6f6e 616c 5b22 656e 756d  : Optional["enum
+00018570: 732e 5061 7273 654d 6f64 6522 5d20 3d20  s.ParseMode"] = 
+00018580: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2063  None,..        c
+00018590: 6170 7469 6f6e 5f65 6e74 6974 6965 733a  aption_entities:
+000185a0: 204c 6973 745b 2274 7970 6573 2e4d 6573   List["types.Mes
+000185b0: 7361 6765 456e 7469 7479 225d 203d 204e  sageEntity"] = N
+000185c0: 6f6e 652c 0d0a 2020 2020 2020 2020 7474  one,..        tt
+000185d0: 6c5f 7365 636f 6e64 733a 2069 6e74 203d  l_seconds: int =
+000185e0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000185f0: 6475 7261 7469 6f6e 3a20 696e 7420 3d20  duration: int = 
+00018600: 302c 0d0a 2020 2020 2020 2020 7769 6474  0,..        widt
+00018610: 683a 2069 6e74 203d 2030 2c0d 0a20 2020  h: int = 0,..   
+00018620: 2020 2020 2068 6569 6768 743a 2069 6e74       height: int
+00018630: 203d 2030 2c0d 0a20 2020 2020 2020 2074   = 0,..        t
+00018640: 6875 6d62 3a20 7374 7220 3d20 4e6f 6e65  humb: str = None
+00018650: 2c0d 0a20 2020 2020 2020 2073 7570 706f  ,..        suppo
+00018660: 7274 735f 7374 7265 616d 696e 673a 2062  rts_streaming: b
+00018670: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
+00018680: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+00018690: 6966 6963 6174 696f 6e3a 2062 6f6f 6c20  ification: bool 
+000186a0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+000186b0: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+000186c0: 655f 6964 3a20 696e 7420 3d20 4e6f 6e65  e_id: int = None
+000186d0: 2c0d 0a20 2020 2020 2020 2072 6570 6c79  ,..        reply
+000186e0: 5f6d 6172 6b75 703a 2055 6e69 6f6e 5b0d  _markup: Union[.
+000186f0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+00018700: 7065 732e 496e 6c69 6e65 4b65 7962 6f61  pes.InlineKeyboa
+00018710: 7264 4d61 726b 7570 222c 0d0a 2020 2020  rdMarkup",..    
+00018720: 2020 2020 2020 2020 2274 7970 6573 2e52          "types.R
+00018730: 6570 6c79 4b65 7962 6f61 7264 4d61 726b  eplyKeyboardMark
+00018740: 7570 222c 0d0a 2020 2020 2020 2020 2020  up",..          
+00018750: 2020 2274 7970 6573 2e52 6570 6c79 4b65    "types.ReplyKe
+00018760: 7962 6f61 7264 5265 6d6f 7665 222c 0d0a  yboardRemove",..
+00018770: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00018780: 6573 2e46 6f72 6365 5265 706c 7922 0d0a  es.ForceReply"..
+00018790: 2020 2020 2020 2020 5d20 3d20 4e6f 6e65          ] = None
+000187a0: 2c0d 0a20 2020 2020 2020 2070 726f 6772  ,..        progr
+000187b0: 6573 733a 2043 616c 6c61 626c 6520 3d20  ess: Callable = 
+000187c0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2070  None,..        p
+000187d0: 726f 6772 6573 735f 6172 6773 3a20 7475  rogress_args: tu
+000187e0: 706c 6520 3d20 2829 0d0a 2020 2020 2920  ple = ()..    ) 
+000187f0: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
+00018800: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
+00018810: 6d65 7468 6f64 202a 7265 706c 795f 7669  method *reply_vi
+00018820: 6465 6f2a 206f 6620 3a6f 626a 3a60 7e66  deo* of :obj:`~f
+00018830: 6970 7065 722e 7479 7065 732e 4d65 7373  ipper.types.Mess
+00018840: 6167 6560 2e0d 0a0d 0a20 2020 2020 2020  age`.....       
+00018850: 2055 7365 2061 7320 6120 7368 6f72 7463   Use as a shortc
+00018860: 7574 2066 6f72 3a0d 0a0d 0a20 2020 2020  ut for:....     
+00018870: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+00018880: 3a3a 2070 7974 686f 6e0d 0a0d 0a20 2020  :: python....   
+00018890: 2020 2020 2020 2020 2061 7761 6974 2063           await c
+000188a0: 6c69 656e 742e 7365 6e64 5f76 6964 656f  lient.send_video
+000188b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000188c0: 2020 2063 6861 745f 6964 3d6d 6573 7361     chat_id=messa
+000188d0: 6765 2e63 6861 742e 6964 2c0d 0a20 2020  ge.chat.id,..   
+000188e0: 2020 2020 2020 2020 2020 2020 2076 6964               vid
+000188f0: 656f 3d76 6964 656f 0d0a 2020 2020 2020  eo=video..      
+00018900: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+00018910: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
+00018920: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
+00018930: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
+00018940: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018950: 2020 2061 7761 6974 206d 6573 7361 6765     await message
+00018960: 2e72 6570 6c79 5f76 6964 656f 2876 6964  .reply_video(vid
+00018970: 656f 290d 0a0d 0a20 2020 2020 2020 2050  eo)....        P
+00018980: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+00018990: 2020 2020 2020 2020 7669 6465 6f20 2860          video (`
+000189a0: 6073 7472 6060 293a 0d0a 2020 2020 2020  `str``):..      
+000189b0: 2020 2020 2020 2020 2020 5669 6465 6f20            Video 
+000189c0: 746f 2073 656e 642e 0d0a 2020 2020 2020  to send...      
+000189d0: 2020 2020 2020 2020 2020 5061 7373 2061            Pass a
+000189e0: 2066 696c 655f 6964 2061 7320 7374 7269   file_id as stri
+000189f0: 6e67 2074 6f20 7365 6e64 2061 2076 6964  ng to send a vid
+00018a00: 656f 2074 6861 7420 6578 6973 7473 206f  eo that exists o
+00018a10: 6e20 7468 6520 5465 6c65 6772 616d 2073  n the Telegram s
+00018a20: 6572 7665 7273 2c0d 0a20 2020 2020 2020  ervers,..       
+00018a30: 2020 2020 2020 2020 2070 6173 7320 616e           pass an
+00018a40: 2048 5454 5020 5552 4c20 6173 2061 2073   HTTP URL as a s
+00018a50: 7472 696e 6720 666f 7220 5465 6c65 6772  tring for Telegr
+00018a60: 616d 2074 6f20 6765 7420 6120 7669 6465  am to get a vide
+00018a70: 6f20 6672 6f6d 2074 6865 2049 6e74 6572  o from the Inter
+00018a80: 6e65 742c 206f 720d 0a20 2020 2020 2020  net, or..       
+00018a90: 2020 2020 2020 2020 2070 6173 7320 6120           pass a 
+00018aa0: 6669 6c65 2070 6174 6820 6173 2073 7472  file path as str
+00018ab0: 696e 6720 746f 2075 706c 6f61 6420 6120  ing to upload a 
+00018ac0: 6e65 7720 7669 6465 6f20 7468 6174 2065  new video that e
+00018ad0: 7869 7374 7320 6f6e 2079 6f75 7220 6c6f  xists on your lo
+00018ae0: 6361 6c20 6d61 6368 696e 652e 0d0a 0d0a  cal machine.....
+00018af0: 2020 2020 2020 2020 2020 2020 7175 6f74              quot
+00018b00: 6520 2860 6062 6f6f 6c60 602c 202a 6f70  e (``bool``, *op
+00018b10: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00018b20: 2020 2020 2020 2020 2020 2049 6620 6060             If ``
+00018b30: 5472 7565 6060 2c20 7468 6520 6d65 7373  True``, the mess
+00018b40: 6167 6520 7769 6c6c 2062 6520 7365 6e74  age will be sent
+00018b50: 2061 7320 6120 7265 706c 7920 746f 2074   as a reply to t
+00018b60: 6869 7320 6d65 7373 6167 652e 0d0a 2020  his message...  
+00018b70: 2020 2020 2020 2020 2020 2020 2020 4966                If
+00018b80: 202a 7265 706c 795f 746f 5f6d 6573 7361   *reply_to_messa
+00018b90: 6765 5f69 642a 2069 7320 7061 7373 6564  ge_id* is passed
+00018ba0: 2c20 7468 6973 2070 6172 616d 6574 6572  , this parameter
+00018bb0: 2077 696c 6c20 6265 2069 676e 6f72 6564   will be ignored
+00018bc0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018bd0: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
+00018be0: 6054 7275 6560 6020 696e 2067 726f 7570  `True`` in group
+00018bf0: 2063 6861 7473 2061 6e64 2060 6046 616c   chats and ``Fal
+00018c00: 7365 6060 2069 6e20 7072 6976 6174 6520  se`` in private 
+00018c10: 6368 6174 732e 0d0a 0d0a 2020 2020 2020  chats.....      
+00018c20: 2020 2020 2020 6361 7074 696f 6e20 2860        caption (`
+00018c30: 6073 7472 6060 2c20 2a6f 7074 696f 6e61  `str``, *optiona
+00018c40: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+00018c50: 2020 2020 2020 5669 6465 6f20 6361 7074        Video capt
+00018c60: 696f 6e2c 2030 2d31 3032 3420 6368 6172  ion, 0-1024 char
+00018c70: 6163 7465 7273 2e0d 0a0d 0a20 2020 2020  acters.....     
+00018c80: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
+00018c90: 6520 283a 6f62 6a3a 607e 6669 7070 6572  e (:obj:`~fipper
+00018ca0: 2e65 6e75 6d73 2e50 6172 7365 4d6f 6465  .enums.ParseMode
+00018cb0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+00018cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018cd0: 2042 7920 6465 6661 756c 742c 2074 6578   By default, tex
+00018ce0: 7473 2061 7265 2070 6172 7365 6420 7573  ts are parsed us
+00018cf0: 696e 6720 626f 7468 204d 6172 6b64 6f77  ing both Markdow
+00018d00: 6e20 616e 6420 4854 4d4c 2073 7479 6c65  n and HTML style
+00018d10: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
+00018d20: 2020 2020 596f 7520 6361 6e20 636f 6d62      You can comb
+00018d30: 696e 6520 626f 7468 2073 796e 7461 7865  ine both syntaxe
+00018d40: 7320 746f 6765 7468 6572 2e0d 0a0d 0a20  s together..... 
+00018d50: 2020 2020 2020 2020 2020 2063 6170 7469             capti
+00018d60: 6f6e 5f65 6e74 6974 6965 7320 284c 6973  on_entities (Lis
+00018d70: 7420 6f66 203a 6f62 6a3a 607e 6669 7070  t of :obj:`~fipp
+00018d80: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
+00018d90: 456e 7469 7479 6029 3a0d 0a20 2020 2020  Entity`):..     
+00018da0: 2020 2020 2020 2020 2020 204c 6973 7420             List 
+00018db0: 6f66 2073 7065 6369 616c 2065 6e74 6974  of special entit
+00018dc0: 6965 7320 7468 6174 2061 7070 6561 7220  ies that appear 
+00018dd0: 696e 2074 6865 2063 6170 7469 6f6e 2c20  in the caption, 
+00018de0: 7768 6963 6820 6361 6e20 6265 2073 7065  which can be spe
+00018df0: 6369 6669 6564 2069 6e73 7465 6164 206f  cified instead o
+00018e00: 6620 2a70 6172 7365 5f6d 6f64 652a 2e0d  f *parse_mode*..
+00018e10: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+00018e20: 746c 5f73 6563 6f6e 6473 2028 6060 696e  tl_seconds (``in
+00018e30: 7460 602c 202a 6f70 7469 6f6e 616c 2a29  t``, *optional*)
+00018e40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018e50: 2020 2053 656c 662d 4465 7374 7275 6374     Self-Destruct
+00018e60: 2054 696d 6572 2e0d 0a20 2020 2020 2020   Timer...       
+00018e70: 2020 2020 2020 2020 2049 6620 796f 7520           If you 
+00018e80: 7365 7420 6120 7469 6d65 722c 2074 6865  set a timer, the
+00018e90: 2076 6964 656f 2077 696c 6c20 7365 6c66   video will self
+00018ea0: 2d64 6573 7472 7563 7420 696e 202a 7474  -destruct in *tt
+00018eb0: 6c5f 7365 636f 6e64 732a 0d0a 2020 2020  l_seconds*..    
+00018ec0: 2020 2020 2020 2020 2020 2020 7365 636f              seco
+00018ed0: 6e64 7320 6166 7465 7220 6974 2077 6173  nds after it was
+00018ee0: 2076 6965 7765 642e 0d0a 0d0a 2020 2020   viewed.....    
+00018ef0: 2020 2020 2020 2020 6475 7261 7469 6f6e          duration
 00018f00: 2028 6060 696e 7460 602c 202a 6f70 7469   (``int``, *opti
 00018f10: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
-00018f20: 2020 2020 2020 2020 2056 6964 656f 2068           Video h
-00018f30: 6569 6768 742e 0d0a 0d0a 2020 2020 2020  eight.....      
-00018f40: 2020 2020 2020 7468 756d 6220 2860 6073        thumb (``s
-00018f50: 7472 6060 2c20 2a6f 7074 696f 6e61 6c2a  tr``, *optional*
-00018f60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00018f70: 2020 2020 5468 756d 626e 6169 6c20 6f66      Thumbnail of
-00018f80: 2074 6865 2076 6964 656f 2073 656e 742e   the video sent.
-00018f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018fa0: 2020 5468 6520 7468 756d 626e 6169 6c20    The thumbnail 
-00018fb0: 7368 6f75 6c64 2062 6520 696e 204a 5045  should be in JPE
-00018fc0: 4720 666f 726d 6174 2061 6e64 206c 6573  G format and les
-00018fd0: 7320 7468 616e 2032 3030 204b 4220 696e  s than 200 KB in
-00018fe0: 2073 697a 652e 0d0a 2020 2020 2020 2020   size...        
-00018ff0: 2020 2020 2020 2020 4120 7468 756d 626e          A thumbn
-00019000: 6169 6c27 7320 7769 6474 6820 616e 6420  ail's width and 
-00019010: 6865 6967 6874 2073 686f 756c 6420 6e6f  height should no
-00019020: 7420 6578 6365 6564 2033 3230 2070 6978  t exceed 320 pix
-00019030: 656c 732e 0d0a 2020 2020 2020 2020 2020  els...          
-00019040: 2020 2020 2020 5468 756d 626e 6169 6c73        Thumbnails
-00019050: 2063 616e 2774 2062 6520 7265 7573 6564   can't be reused
-00019060: 2061 6e64 2063 616e 2062 6520 6f6e 6c79   and can be only
-00019070: 2075 706c 6f61 6465 6420 6173 2061 206e   uploaded as a n
-00019080: 6577 2066 696c 652e 0d0a 0d0a 2020 2020  ew file.....    
-00019090: 2020 2020 2020 2020 7375 7070 6f72 7473          supports
-000190a0: 5f73 7472 6561 6d69 6e67 2028 6060 626f  _streaming (``bo
-000190b0: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
-000190c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000190d0: 2020 2020 5061 7373 2054 7275 652c 2069      Pass True, i
-000190e0: 6620 7468 6520 7570 6c6f 6164 6564 2076  f the uploaded v
-000190f0: 6964 656f 2069 7320 7375 6974 6162 6c65  ideo is suitable
-00019100: 2066 6f72 2073 7472 6561 6d69 6e67 2e0d   for streaming..
-00019110: 0a0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
-00019120: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-00019130: 696f 6e20 2860 6062 6f6f 6c60 602c 202a  ion (``bool``, *
-00019140: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
-00019150: 2020 2020 2020 2020 2020 2020 2053 656e               Sen
-00019160: 6473 2074 6865 206d 6573 7361 6765 2073  ds the message s
-00019170: 696c 656e 746c 792e 0d0a 2020 2020 2020  ilently...      
-00019180: 2020 2020 2020 2020 2020 5573 6572 7320            Users 
-00019190: 7769 6c6c 2072 6563 6569 7665 2061 206e  will receive a n
-000191a0: 6f74 6966 6963 6174 696f 6e20 7769 7468  otification with
-000191b0: 206e 6f20 736f 756e 642e 0d0a 0d0a 2020   no sound.....  
-000191c0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-000191d0: 746f 5f6d 6573 7361 6765 5f69 6420 2860  to_message_id (`
-000191e0: 6069 6e74 6060 2c20 2a6f 7074 696f 6e61  `int``, *optiona
-000191f0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-00019200: 2020 2020 2020 4966 2074 6865 206d 6573        If the mes
-00019210: 7361 6765 2069 7320 6120 7265 706c 792c  sage is a reply,
-00019220: 2049 4420 6f66 2074 6865 206f 7269 6769   ID of the origi
-00019230: 6e61 6c20 6d65 7373 6167 652e 0d0a 0d0a  nal message.....
-00019240: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-00019250: 795f 6d61 726b 7570 2028 3a6f 626a 3a60  y_markup (:obj:`
-00019260: 7e66 6970 7065 722e 7479 7065 732e 496e  ~fipper.types.In
-00019270: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
-00019280: 7570 6020 7c20 3a6f 626a 3a60 7e66 6970  up` | :obj:`~fip
-00019290: 7065 722e 7479 7065 732e 5265 706c 794b  per.types.ReplyK
-000192a0: 6579 626f 6172 644d 6172 6b75 7060 207c  eyboardMarkup` |
-000192b0: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
-000192c0: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
-000192d0: 7264 5265 6d6f 7665 6020 7c20 3a6f 626a  rdRemove` | :obj
-000192e0: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
-000192f0: 466f 7263 6552 6570 6c79 602c 202a 6f70  ForceReply`, *op
-00019300: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-00019310: 2020 2020 2020 2020 2020 2041 6464 6974             Addit
-00019320: 696f 6e61 6c20 696e 7465 7266 6163 6520  ional interface 
-00019330: 6f70 7469 6f6e 732e 2041 6e20 6f62 6a65  options. An obje
-00019340: 6374 2066 6f72 2061 6e20 696e 6c69 6e65  ct for an inline
-00019350: 206b 6579 626f 6172 642c 2063 7573 746f   keyboard, custo
-00019360: 6d20 7265 706c 7920 6b65 7962 6f61 7264  m reply keyboard
-00019370: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00019380: 2020 2069 6e73 7472 7563 7469 6f6e 7320     instructions 
-00019390: 746f 2072 656d 6f76 6520 7265 706c 7920  to remove reply 
-000193a0: 6b65 7962 6f61 7264 206f 7220 746f 2066  keyboard or to f
-000193b0: 6f72 6365 2061 2072 6570 6c79 2066 726f  orce a reply fro
-000193c0: 6d20 7468 6520 7573 6572 2e0d 0a0d 0a20  m the user..... 
-000193d0: 2020 2020 2020 2020 2020 2070 726f 6772             progr
-000193e0: 6573 7320 2860 6043 616c 6c61 626c 6560  ess (``Callable`
-000193f0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-00019400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019410: 2050 6173 7320 6120 6361 6c6c 6261 636b   Pass a callback
-00019420: 2066 756e 6374 696f 6e20 746f 2076 6965   function to vie
-00019430: 7720 7468 6520 6669 6c65 2074 7261 6e73  w the file trans
-00019440: 6d69 7373 696f 6e20 7072 6f67 7265 7373  mission progress
-00019450: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00019460: 2020 2054 6865 2066 756e 6374 696f 6e20     The function 
-00019470: 6d75 7374 2074 616b 6520 2a28 6375 7272  must take *(curr
-00019480: 656e 742c 2074 6f74 616c 292a 2061 7320  ent, total)* as 
-00019490: 706f 7369 7469 6f6e 616c 2061 7267 756d  positional argum
-000194a0: 656e 7473 2028 6c6f 6f6b 2061 7420 4f74  ents (look at Ot
-000194b0: 6865 7220 5061 7261 6d65 7465 7273 2062  her Parameters b
-000194c0: 656c 6f77 2066 6f72 2061 0d0a 2020 2020  elow for a..    
-000194d0: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-000194e0: 696c 6564 2064 6573 6372 6970 7469 6f6e  iled description
-000194f0: 2920 616e 6420 7769 6c6c 2062 6520 6361  ) and will be ca
-00019500: 6c6c 6564 2062 6163 6b20 6561 6368 2074  lled back each t
-00019510: 696d 6520 6120 6e65 7720 6669 6c65 2063  ime a new file c
-00019520: 6875 6e6b 2068 6173 2062 6565 6e20 7375  hunk has been su
-00019530: 6363 6573 7366 756c 6c79 0d0a 2020 2020  ccessfully..    
-00019540: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-00019550: 736d 6974 7465 642e 0d0a 0d0a 2020 2020  smitted.....    
-00019560: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-00019570: 5f61 7267 7320 2860 6074 7570 6c65 6060  _args (``tuple``
-00019580: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195a0: 4578 7472 6120 6375 7374 6f6d 2061 7267  Extra custom arg
-000195b0: 756d 656e 7473 2066 6f72 2074 6865 2070  uments for the p
-000195c0: 726f 6772 6573 7320 6361 6c6c 6261 636b  rogress callback
-000195d0: 2066 756e 6374 696f 6e2e 0d0a 2020 2020   function...    
-000195e0: 2020 2020 2020 2020 2020 2020 596f 7520              You 
-000195f0: 6361 6e20 7061 7373 2061 6e79 7468 696e  can pass anythin
-00019600: 6720 796f 7520 6e65 6564 2074 6f20 6265  g you need to be
-00019610: 2061 7661 696c 6162 6c65 2069 6e20 7468   available in th
-00019620: 6520 7072 6f67 7265 7373 2063 616c 6c62  e progress callb
-00019630: 6163 6b20 7363 6f70 653b 2066 6f72 2065  ack scope; for e
-00019640: 7861 6d70 6c65 2c20 6120 4d65 7373 6167  xample, a Messag
-00019650: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00019660: 2020 206f 626a 6563 7420 6f72 2061 2043     object or a C
-00019670: 6c69 656e 7420 696e 7374 616e 6365 2069  lient instance i
-00019680: 6e20 6f72 6465 7220 746f 2065 6469 7420  n order to edit 
-00019690: 7468 6520 6d65 7373 6167 6520 7769 7468  the message with
-000196a0: 2074 6865 2075 7064 6174 6564 2070 726f   the updated pro
-000196b0: 6772 6573 7320 7374 6174 7573 2e0d 0a0d  gress status....
-000196c0: 0a20 2020 2020 2020 204f 7468 6572 2050  .        Other P
-000196d0: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
-000196e0: 2020 2020 2020 2020 6375 7272 656e 7420          current 
-000196f0: 2860 6069 6e74 6060 293a 0d0a 2020 2020  (``int``):..    
-00019700: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00019710: 616d 6f75 6e74 206f 6620 6279 7465 7320  amount of bytes 
-00019720: 7472 616e 736d 6974 7465 6420 736f 2066  transmitted so f
-00019730: 6172 2e0d 0a0d 0a20 2020 2020 2020 2020  ar.....         
-00019740: 2020 2074 6f74 616c 2028 6060 696e 7460     total (``int`
-00019750: 6029 3a0d 0a20 2020 2020 2020 2020 2020  `):..           
-00019760: 2020 2020 2054 6865 2074 6f74 616c 2073       The total s
-00019770: 697a 6520 6f66 2074 6865 2066 696c 652e  ize of the file.
-00019780: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019790: 2a61 7267 7320 2860 6074 7570 6c65 6060  *args (``tuple``
-000197a0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197c0: 4578 7472 6120 6375 7374 6f6d 2061 7267  Extra custom arg
-000197d0: 756d 656e 7473 2061 7320 6465 6669 6e65  uments as define
-000197e0: 6420 696e 2074 6865 2060 6070 726f 6772  d in the ``progr
-000197f0: 6573 735f 6172 6773 6060 2070 6172 616d  ess_args`` param
-00019800: 6574 6572 2e0d 0a20 2020 2020 2020 2020  eter...         
-00019810: 2020 2020 2020 2059 6f75 2063 616e 2065         You can e
-00019820: 6974 6865 7220 6b65 6570 2060 602a 6172  ither keep ``*ar
-00019830: 6773 6060 206f 7220 6164 6420 6576 6572  gs`` or add ever
-00019840: 7920 7369 6e67 6c65 2065 7874 7261 2061  y single extra a
-00019850: 7267 756d 656e 7420 696e 2079 6f75 7220  rgument in your 
-00019860: 6675 6e63 7469 6f6e 2073 6967 6e61 7475  function signatu
-00019870: 7265 2e0d 0a0d 0a20 2020 2020 2020 2052  re.....        R
-00019880: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00019890: 2020 2020 204f 6e20 7375 6363 6573 732c       On success,
-000198a0: 2074 6865 2073 656e 7420 3a6f 626a 3a60   the sent :obj:`
-000198b0: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
-000198c0: 7373 6167 6560 2069 7320 7265 7475 726e  ssage` is return
-000198d0: 6564 2e0d 0a20 2020 2020 2020 2020 2020  ed...           
-000198e0: 2049 6e20 6361 7365 2074 6865 2075 706c   In case the upl
-000198f0: 6f61 6420 6973 2064 656c 6962 6572 6174  oad is deliberat
-00019900: 656c 7920 7374 6f70 7065 6420 7769 7468  ely stopped with
-00019910: 203a 6d65 7468 3a60 7e66 6970 7065 722e   :meth:`~fipper.
-00019920: 436c 6965 6e74 2e73 746f 705f 7472 616e  Client.stop_tran
-00019930: 736d 6973 7369 6f6e 602c 204e 6f6e 6520  smission`, None 
-00019940: 6973 2072 6574 7572 6e65 640d 0a20 2020  is returned..   
-00019950: 2020 2020 2020 2020 2069 6e73 7465 6164           instead
-00019960: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
-00019970: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
-00019980: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-00019990: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-000199a0: 6d20 5250 4320 6572 726f 722e 0d0a 2020  m RPC error...  
-000199b0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000199c0: 2020 2069 6620 7175 6f74 6520 6973 204e     if quote is N
-000199d0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000199e0: 2020 7175 6f74 6520 3d20 7365 6c66 2e63    quote = self.c
-000199f0: 6861 742e 7479 7065 2021 3d20 656e 756d  hat.type != enum
-00019a00: 732e 4368 6174 5479 7065 2e50 5249 5641  s.ChatType.PRIVA
-00019a10: 5445 0d0a 0d0a 2020 2020 2020 2020 6966  TE....        if
-00019a20: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
-00019a30: 655f 6964 2069 7320 4e6f 6e65 2061 6e64  e_id is None and
-00019a40: 2071 756f 7465 3a0d 0a20 2020 2020 2020   quote:..       
-00019a50: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
-00019a60: 7373 6167 655f 6964 203d 2073 656c 662e  ssage_id = self.
-00019a70: 6964 0d0a 0d0a 2020 2020 2020 2020 7265  id....        re
-00019a80: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00019a90: 5f63 6c69 656e 742e 7365 6e64 5f76 6964  _client.send_vid
-00019aa0: 656f 280d 0a20 2020 2020 2020 2020 2020  eo(..           
-00019ab0: 2063 6861 745f 6964 3d73 656c 662e 6368   chat_id=self.ch
-00019ac0: 6174 2e69 642c 0d0a 2020 2020 2020 2020  at.id,..        
-00019ad0: 2020 2020 7669 6465 6f3d 7669 6465 6f2c      video=video,
-00019ae0: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-00019af0: 7074 696f 6e3d 6361 7074 696f 6e2c 0d0a  ption=caption,..
-00019b00: 2020 2020 2020 2020 2020 2020 7061 7273              pars
-00019b10: 655f 6d6f 6465 3d70 6172 7365 5f6d 6f64  e_mode=parse_mod
-00019b20: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00019b30: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
-00019b40: 3d63 6170 7469 6f6e 5f65 6e74 6974 6965  =caption_entitie
-00019b50: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00019b60: 7474 6c5f 7365 636f 6e64 733d 7474 6c5f  ttl_seconds=ttl_
-00019b70: 7365 636f 6e64 732c 0d0a 2020 2020 2020  seconds,..      
-00019b80: 2020 2020 2020 6475 7261 7469 6f6e 3d64        duration=d
-00019b90: 7572 6174 696f 6e2c 0d0a 2020 2020 2020  uration,..      
-00019ba0: 2020 2020 2020 7769 6474 683d 7769 6474        width=widt
-00019bb0: 682c 0d0a 2020 2020 2020 2020 2020 2020  h,..            
-00019bc0: 6865 6967 6874 3d68 6569 6768 742c 0d0a  height=height,..
-00019bd0: 2020 2020 2020 2020 2020 2020 7468 756d              thum
-00019be0: 623d 7468 756d 622c 0d0a 2020 2020 2020  b=thumb,..      
-00019bf0: 2020 2020 2020 7375 7070 6f72 7473 5f73        supports_s
-00019c00: 7472 6561 6d69 6e67 3d73 7570 706f 7274  treaming=support
-00019c10: 735f 7374 7265 616d 696e 672c 0d0a 2020  s_streaming,..  
-00019c20: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
-00019c30: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
-00019c40: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-00019c50: 696f 6e2c 0d0a 2020 2020 2020 2020 2020  ion,..          
-00019c60: 2020 7265 706c 795f 746f 5f6d 6573 7361    reply_to_messa
-00019c70: 6765 5f69 643d 7265 706c 795f 746f 5f6d  ge_id=reply_to_m
-00019c80: 6573 7361 6765 5f69 642c 0d0a 2020 2020  essage_id,..    
-00019c90: 2020 2020 2020 2020 7265 706c 795f 6d61          reply_ma
-00019ca0: 726b 7570 3d72 6570 6c79 5f6d 6172 6b75  rkup=reply_marku
-00019cb0: 702c 0d0a 2020 2020 2020 2020 2020 2020  p,..            
-00019cc0: 7072 6f67 7265 7373 3d70 726f 6772 6573  progress=progres
-00019cd0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00019ce0: 7072 6f67 7265 7373 5f61 7267 733d 7072  progress_args=pr
-00019cf0: 6f67 7265 7373 5f61 7267 730d 0a20 2020  ogress_args..   
-00019d00: 2020 2020 2029 0d0a 0d0a 2020 2020 6173       )....    as
-00019d10: 796e 6320 6465 6620 7265 706c 795f 7669  ync def reply_vi
-00019d20: 6465 6f5f 6e6f 7465 280d 0a20 2020 2020  deo_note(..     
-00019d30: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-00019d40: 2020 7669 6465 6f5f 6e6f 7465 3a20 556e    video_note: Un
-00019d50: 696f 6e5b 7374 722c 2042 696e 6172 7949  ion[str, BinaryI
-00019d60: 4f5d 2c0d 0a20 2020 2020 2020 2071 756f  O],..        quo
-00019d70: 7465 3a20 626f 6f6c 203d 204e 6f6e 652c  te: bool = None,
-00019d80: 0d0a 2020 2020 2020 2020 6475 7261 7469  ..        durati
-00019d90: 6f6e 3a20 696e 7420 3d20 302c 0d0a 2020  on: int = 0,..  
-00019da0: 2020 2020 2020 6c65 6e67 7468 3a20 696e        length: in
-00019db0: 7420 3d20 312c 0d0a 2020 2020 2020 2020  t = 1,..        
-00019dc0: 7468 756d 623a 2073 7472 203d 204e 6f6e  thumb: str = Non
-00019dd0: 652c 0d0a 2020 2020 2020 2020 6469 7361  e,..        disa
-00019de0: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00019df0: 3a20 626f 6f6c 203d 204e 6f6e 652c 0d0a  : bool = None,..
-00019e00: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
-00019e10: 5f6d 6573 7361 6765 5f69 643a 2069 6e74  _message_id: int
-00019e20: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00019e30: 2020 7265 706c 795f 6d61 726b 7570 3a20    reply_markup: 
-00019e40: 556e 696f 6e5b 0d0a 2020 2020 2020 2020  Union[..        
-00019e50: 2020 2020 2274 7970 6573 2e49 6e6c 696e      "types.Inlin
-00019e60: 654b 6579 626f 6172 644d 6172 6b75 7022  eKeyboardMarkup"
-00019e70: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00019e80: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
-00019e90: 6172 644d 6172 6b75 7022 2c0d 0a20 2020  ardMarkup",..   
-00019ea0: 2020 2020 2020 2020 2022 7479 7065 732e           "types.
-00019eb0: 5265 706c 794b 6579 626f 6172 6452 656d  ReplyKeyboardRem
-00019ec0: 6f76 6522 2c0d 0a20 2020 2020 2020 2020  ove",..         
-00019ed0: 2020 2022 7479 7065 732e 466f 7263 6552     "types.ForceR
-00019ee0: 6570 6c79 220d 0a20 2020 2020 2020 205d  eply"..        ]
-00019ef0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00019f00: 2020 7072 6f67 7265 7373 3a20 4361 6c6c    progress: Call
-00019f10: 6162 6c65 203d 204e 6f6e 652c 0d0a 2020  able = None,..  
-00019f20: 2020 2020 2020 7072 6f67 7265 7373 5f61        progress_a
-00019f30: 7267 733a 2074 7570 6c65 203d 2028 290d  rgs: tuple = ().
-00019f40: 0a20 2020 2029 202d 3e20 224d 6573 7361  .    ) -> "Messa
-00019f50: 6765 223a 0d0a 2020 2020 2020 2020 2222  ge":..        ""
-00019f60: 2242 6f75 6e64 206d 6574 686f 6420 2a72  "Bound method *r
-00019f70: 6570 6c79 5f76 6964 656f 5f6e 6f74 652a  eply_video_note*
-00019f80: 206f 6620 3a6f 626a 3a60 7e66 6970 7065   of :obj:`~fippe
-00019f90: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
-00019fa0: 2e0d 0a0d 0a20 2020 2020 2020 2055 7365  .....        Use
-00019fb0: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
-00019fc0: 6f72 3a0d 0a0d 0a20 2020 2020 2020 202e  or:....        .
-00019fd0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00019fe0: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
-00019ff0: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
-0001a000: 742e 7365 6e64 5f76 6964 656f 5f6e 6f74  t.send_video_not
-0001a010: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
-0001a020: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
-0001a030: 6167 652e 6368 6174 2e69 642c 0d0a 2020  age.chat.id,..  
-0001a040: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-0001a050: 6465 6f5f 6e6f 7465 3d76 6964 656f 5f6e  deo_note=video_n
-0001a060: 6f74 650d 0a20 2020 2020 2020 2020 2020  ote..           
-0001a070: 2029 0d0a 0d0a 2020 2020 2020 2020 4578   )....        Ex
-0001a080: 616d 706c 653a 0d0a 2020 2020 2020 2020  ample:..        
-0001a090: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-0001a0a0: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
-0001a0b0: 2020 2020 2020 2020 2020 2020 2020 6177                aw
-0001a0c0: 6169 7420 6d65 7373 6167 652e 7265 706c  ait message.repl
-0001a0d0: 795f 7669 6465 6f5f 6e6f 7465 2876 6964  y_video_note(vid
-0001a0e0: 656f 5f6e 6f74 6529 0d0a 0d0a 2020 2020  eo_note)....    
-0001a0f0: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
-0001a100: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
-0001a110: 656f 5f6e 6f74 6520 2860 6073 7472 6060  eo_note (``str``
-0001a120: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001a130: 2020 2020 5669 6465 6f20 6e6f 7465 2074      Video note t
-0001a140: 6f20 7365 6e64 2e0d 0a20 2020 2020 2020  o send...       
-0001a150: 2020 2020 2020 2020 2050 6173 7320 6120           Pass a 
-0001a160: 6669 6c65 5f69 6420 6173 2073 7472 696e  file_id as strin
-0001a170: 6720 746f 2073 656e 6420 6120 7669 6465  g to send a vide
-0001a180: 6f20 6e6f 7465 2074 6861 7420 6578 6973  o note that exis
-0001a190: 7473 206f 6e20 7468 6520 5465 6c65 6772  ts on the Telegr
-0001a1a0: 616d 2073 6572 7665 7273 2c20 6f72 0d0a  am servers, or..
-0001a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1c0: 7061 7373 2061 2066 696c 6520 7061 7468  pass a file path
-0001a1d0: 2061 7320 7374 7269 6e67 2074 6f20 7570   as string to up
-0001a1e0: 6c6f 6164 2061 206e 6577 2076 6964 656f  load a new video
-0001a1f0: 206e 6f74 6520 7468 6174 2065 7869 7374   note that exist
-0001a200: 7320 6f6e 2079 6f75 7220 6c6f 6361 6c20  s on your local 
-0001a210: 6d61 6368 696e 652e 0d0a 2020 2020 2020  machine...      
-0001a220: 2020 2020 2020 2020 2020 5365 6e64 696e            Sendin
-0001a230: 6720 7669 6465 6f20 6e6f 7465 7320 6279  g video notes by
-0001a240: 2061 2055 524c 2069 7320 6375 7272 656e   a URL is curren
-0001a250: 746c 7920 756e 7375 7070 6f72 7465 642e  tly unsupported.
-0001a260: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a270: 7175 6f74 6520 2860 6062 6f6f 6c60 602c  quote (``bool``,
-0001a280: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
-0001a290: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-0001a2a0: 6620 6060 5472 7565 6060 2c20 7468 6520  f ``True``, the 
-0001a2b0: 6d65 7373 6167 6520 7769 6c6c 2062 6520  message will be 
-0001a2c0: 7365 6e74 2061 7320 6120 7265 706c 7920  sent as a reply 
-0001a2d0: 746f 2074 6869 7320 6d65 7373 6167 652e  to this message.
-0001a2e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a2f0: 2020 4966 202a 7265 706c 795f 746f 5f6d    If *reply_to_m
-0001a300: 6573 7361 6765 5f69 642a 2069 7320 7061  essage_id* is pa
-0001a310: 7373 6564 2c20 7468 6973 2070 6172 616d  ssed, this param
-0001a320: 6574 6572 2077 696c 6c20 6265 2069 676e  eter will be ign
-0001a330: 6f72 6564 2e0d 0a20 2020 2020 2020 2020  ored...         
-0001a340: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-0001a350: 746f 2060 6054 7275 6560 6020 696e 2067  to ``True`` in g
-0001a360: 726f 7570 2063 6861 7473 2061 6e64 2060  roup chats and `
-0001a370: 6046 616c 7365 6060 2069 6e20 7072 6976  `False`` in priv
-0001a380: 6174 6520 6368 6174 732e 0d0a 0d0a 2020  ate chats.....  
-0001a390: 2020 2020 2020 2020 2020 6475 7261 7469            durati
-0001a3a0: 6f6e 2028 6060 696e 7460 602c 202a 6f70  on (``int``, *op
-0001a3b0: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-0001a3c0: 2020 2020 2020 2020 2020 2044 7572 6174             Durat
-0001a3d0: 696f 6e20 6f66 2073 656e 7420 7669 6465  ion of sent vide
-0001a3e0: 6f20 696e 2073 6563 6f6e 6473 2e0d 0a0d  o in seconds....
-0001a3f0: 0a20 2020 2020 2020 2020 2020 206c 656e  .            len
-0001a400: 6774 6820 2860 6069 6e74 6060 2c20 2a6f  gth (``int``, *o
-0001a410: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-0001a420: 2020 2020 2020 2020 2020 2020 5669 6465              Vide
-0001a430: 6f20 7769 6474 6820 616e 6420 6865 6967  o width and heig
-0001a440: 6874 2e0d 0a0d 0a20 2020 2020 2020 2020  ht.....         
-0001a450: 2020 2074 6875 6d62 2028 6060 7374 7260     thumb (``str`
-0001a460: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-0001a470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a480: 2054 6875 6d62 6e61 696c 206f 6620 7468   Thumbnail of th
-0001a490: 6520 7669 6465 6f20 7365 6e74 2e0d 0a20  e video sent... 
-0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0001a4b0: 6865 2074 6875 6d62 6e61 696c 2073 686f  he thumbnail sho
-0001a4c0: 756c 6420 6265 2069 6e20 4a50 4547 2066  uld be in JPEG f
-0001a4d0: 6f72 6d61 7420 616e 6420 6c65 7373 2074  ormat and less t
-0001a4e0: 6861 6e20 3230 3020 4b42 2069 6e20 7369  han 200 KB in si
-0001a4f0: 7a65 2e0d 0a20 2020 2020 2020 2020 2020  ze...           
-0001a500: 2020 2020 2041 2074 6875 6d62 6e61 696c       A thumbnail
-0001a510: 2773 2077 6964 7468 2061 6e64 2068 6569  's width and hei
-0001a520: 6768 7420 7368 6f75 6c64 206e 6f74 2065  ght should not e
-0001a530: 7863 6565 6420 3332 3020 7069 7865 6c73  xceed 320 pixels
-0001a540: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a550: 2020 2054 6875 6d62 6e61 696c 7320 6361     Thumbnails ca
-0001a560: 6e27 7420 6265 2072 6575 7365 6420 616e  n't be reused an
-0001a570: 6420 6361 6e20 6265 206f 6e6c 7920 7570  d can be only up
-0001a580: 6c6f 6164 6564 2061 7320 6120 6e65 7720  loaded as a new 
-0001a590: 6669 6c65 2e0d 0a0d 0a20 2020 2020 2020  file.....       
-0001a5a0: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
-0001a5b0: 6966 6963 6174 696f 6e20 2860 6062 6f6f  ification (``boo
-0001a5c0: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
-0001a5d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a5e0: 2020 2053 656e 6473 2074 6865 206d 6573     Sends the mes
-0001a5f0: 7361 6765 2073 696c 656e 746c 792e 0d0a  sage silently...
-0001a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a610: 5573 6572 7320 7769 6c6c 2072 6563 6569  Users will recei
-0001a620: 7665 2061 206e 6f74 6966 6963 6174 696f  ve a notificatio
-0001a630: 6e20 7769 7468 206e 6f20 736f 756e 642e  n with no sound.
+00018f20: 2020 2020 2020 2020 2044 7572 6174 696f           Duratio
+00018f30: 6e20 6f66 2073 656e 7420 7669 6465 6f20  n of sent video 
+00018f40: 696e 2073 6563 6f6e 6473 2e0d 0a0d 0a20  in seconds..... 
+00018f50: 2020 2020 2020 2020 2020 2077 6964 7468             width
+00018f60: 2028 6060 696e 7460 602c 202a 6f70 7469   (``int``, *opti
+00018f70: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
+00018f80: 2020 2020 2020 2020 2056 6964 656f 2077           Video w
+00018f90: 6964 7468 2e0d 0a0d 0a20 2020 2020 2020  idth.....       
+00018fa0: 2020 2020 2068 6569 6768 7420 2860 6069       height (``i
+00018fb0: 6e74 6060 2c20 2a6f 7074 696f 6e61 6c2a  nt``, *optional*
+00018fc0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00018fd0: 2020 2020 5669 6465 6f20 6865 6967 6874      Video height
+00018fe0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00018ff0: 2074 6875 6d62 2028 6060 7374 7260 602c   thumb (``str``,
+00019000: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
+00019010: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00019020: 6875 6d62 6e61 696c 206f 6620 7468 6520  humbnail of the 
+00019030: 7669 6465 6f20 7365 6e74 2e0d 0a20 2020  video sent...   
+00019040: 2020 2020 2020 2020 2020 2020 2054 6865               The
+00019050: 2074 6875 6d62 6e61 696c 2073 686f 756c   thumbnail shoul
+00019060: 6420 6265 2069 6e20 4a50 4547 2066 6f72  d be in JPEG for
+00019070: 6d61 7420 616e 6420 6c65 7373 2074 6861  mat and less tha
+00019080: 6e20 3230 3020 4b42 2069 6e20 7369 7a65  n 200 KB in size
+00019090: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000190a0: 2020 2041 2074 6875 6d62 6e61 696c 2773     A thumbnail's
+000190b0: 2077 6964 7468 2061 6e64 2068 6569 6768   width and heigh
+000190c0: 7420 7368 6f75 6c64 206e 6f74 2065 7863  t should not exc
+000190d0: 6565 6420 3332 3020 7069 7865 6c73 2e0d  eed 320 pixels..
+000190e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000190f0: 2054 6875 6d62 6e61 696c 7320 6361 6e27   Thumbnails can'
+00019100: 7420 6265 2072 6575 7365 6420 616e 6420  t be reused and 
+00019110: 6361 6e20 6265 206f 6e6c 7920 7570 6c6f  can be only uplo
+00019120: 6164 6564 2061 7320 6120 6e65 7720 6669  aded as a new fi
+00019130: 6c65 2e0d 0a0d 0a20 2020 2020 2020 2020  le.....         
+00019140: 2020 2073 7570 706f 7274 735f 7374 7265     supports_stre
+00019150: 616d 696e 6720 2860 6062 6f6f 6c60 602c  aming (``bool``,
+00019160: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
+00019170: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+00019180: 6173 7320 5472 7565 2c20 6966 2074 6865  ass True, if the
+00019190: 2075 706c 6f61 6465 6420 7669 6465 6f20   uploaded video 
+000191a0: 6973 2073 7569 7461 626c 6520 666f 7220  is suitable for 
+000191b0: 7374 7265 616d 696e 672e 0d0a 0d0a 2020  streaming.....  
+000191c0: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+000191d0: 655f 6e6f 7469 6669 6361 7469 6f6e 2028  e_notification (
+000191e0: 6060 626f 6f6c 6060 2c20 2a6f 7074 696f  ``bool``, *optio
+000191f0: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
+00019200: 2020 2020 2020 2020 5365 6e64 7320 7468          Sends th
+00019210: 6520 6d65 7373 6167 6520 7369 6c65 6e74  e message silent
+00019220: 6c79 2e0d 0a20 2020 2020 2020 2020 2020  ly...           
+00019230: 2020 2020 2055 7365 7273 2077 696c 6c20       Users will 
+00019240: 7265 6365 6976 6520 6120 6e6f 7469 6669  receive a notifi
+00019250: 6361 7469 6f6e 2077 6974 6820 6e6f 2073  cation with no s
+00019260: 6f75 6e64 2e0d 0a0d 0a20 2020 2020 2020  ound.....       
+00019270: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
+00019280: 7373 6167 655f 6964 2028 6060 696e 7460  ssage_id (``int`
+00019290: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+000192a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000192b0: 2049 6620 7468 6520 6d65 7373 6167 6520   If the message 
+000192c0: 6973 2061 2072 6570 6c79 2c20 4944 206f  is a reply, ID o
+000192d0: 6620 7468 6520 6f72 6967 696e 616c 206d  f the original m
+000192e0: 6573 7361 6765 2e0d 0a0d 0a20 2020 2020  essage.....     
+000192f0: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
+00019300: 6b75 7020 283a 6f62 6a3a 607e 6669 7070  kup (:obj:`~fipp
+00019310: 6572 2e74 7970 6573 2e49 6e6c 696e 654b  er.types.InlineK
+00019320: 6579 626f 6172 644d 6172 6b75 7060 207c  eyboardMarkup` |
+00019330: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
+00019340: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
+00019350: 7264 4d61 726b 7570 6020 7c20 3a6f 626a  rdMarkup` | :obj
+00019360: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
+00019370: 5265 706c 794b 6579 626f 6172 6452 656d  ReplyKeyboardRem
+00019380: 6f76 6560 207c 203a 6f62 6a3a 607e 6669  ove` | :obj:`~fi
+00019390: 7070 6572 2e74 7970 6573 2e46 6f72 6365  pper.types.Force
+000193a0: 5265 706c 7960 2c20 2a6f 7074 696f 6e61  Reply`, *optiona
+000193b0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+000193c0: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+000193d0: 2069 6e74 6572 6661 6365 206f 7074 696f   interface optio
+000193e0: 6e73 2e20 416e 206f 626a 6563 7420 666f  ns. An object fo
+000193f0: 7220 616e 2069 6e6c 696e 6520 6b65 7962  r an inline keyb
+00019400: 6f61 7264 2c20 6375 7374 6f6d 2072 6570  oard, custom rep
+00019410: 6c79 206b 6579 626f 6172 642c 0d0a 2020  ly keyboard,..  
+00019420: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00019430: 7374 7275 6374 696f 6e73 2074 6f20 7265  structions to re
+00019440: 6d6f 7665 2072 6570 6c79 206b 6579 626f  move reply keybo
+00019450: 6172 6420 6f72 2074 6f20 666f 7263 6520  ard or to force 
+00019460: 6120 7265 706c 7920 6672 6f6d 2074 6865  a reply from the
+00019470: 2075 7365 722e 0d0a 0d0a 2020 2020 2020   user.....      
+00019480: 2020 2020 2020 7072 6f67 7265 7373 2028        progress (
+00019490: 6060 4361 6c6c 6162 6c65 6060 2c20 2a6f  ``Callable``, *o
+000194a0: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+000194b0: 2020 2020 2020 2020 2020 2020 5061 7373              Pass
+000194c0: 2061 2063 616c 6c62 6163 6b20 6675 6e63   a callback func
+000194d0: 7469 6f6e 2074 6f20 7669 6577 2074 6865  tion to view the
+000194e0: 2066 696c 6520 7472 616e 736d 6973 7369   file transmissi
+000194f0: 6f6e 2070 726f 6772 6573 732e 0d0a 2020  on progress...  
+00019500: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00019510: 6520 6675 6e63 7469 6f6e 206d 7573 7420  e function must 
+00019520: 7461 6b65 202a 2863 7572 7265 6e74 2c20  take *(current, 
+00019530: 746f 7461 6c29 2a20 6173 2070 6f73 6974  total)* as posit
+00019540: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
+00019550: 286c 6f6f 6b20 6174 204f 7468 6572 2050  (look at Other P
+00019560: 6172 616d 6574 6572 7320 6265 6c6f 7720  arameters below 
+00019570: 666f 7220 610d 0a20 2020 2020 2020 2020  for a..         
+00019580: 2020 2020 2020 2064 6574 6169 6c65 6420         detailed 
+00019590: 6465 7363 7269 7074 696f 6e29 2061 6e64  description) and
+000195a0: 2077 696c 6c20 6265 2063 616c 6c65 6420   will be called 
+000195b0: 6261 636b 2065 6163 6820 7469 6d65 2061  back each time a
+000195c0: 206e 6577 2066 696c 6520 6368 756e 6b20   new file chunk 
+000195d0: 6861 7320 6265 656e 2073 7563 6365 7373  has been success
+000195e0: 6675 6c6c 790d 0a20 2020 2020 2020 2020  fully..         
+000195f0: 2020 2020 2020 2074 7261 6e73 6d69 7474         transmitt
+00019600: 6564 2e0d 0a0d 0a20 2020 2020 2020 2020  ed.....         
+00019610: 2020 2070 726f 6772 6573 735f 6172 6773     progress_args
+00019620: 2028 6060 7475 706c 6560 602c 202a 6f70   (``tuple``, *op
+00019630: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00019640: 2020 2020 2020 2020 2020 2045 7874 7261             Extra
+00019650: 2063 7573 746f 6d20 6172 6775 6d65 6e74   custom argument
+00019660: 7320 666f 7220 7468 6520 7072 6f67 7265  s for the progre
+00019670: 7373 2063 616c 6c62 6163 6b20 6675 6e63  ss callback func
+00019680: 7469 6f6e 2e0d 0a20 2020 2020 2020 2020  tion...         
+00019690: 2020 2020 2020 2059 6f75 2063 616e 2070         You can p
+000196a0: 6173 7320 616e 7974 6869 6e67 2079 6f75  ass anything you
+000196b0: 206e 6565 6420 746f 2062 6520 6176 6169   need to be avai
+000196c0: 6c61 626c 6520 696e 2074 6865 2070 726f  lable in the pro
+000196d0: 6772 6573 7320 6361 6c6c 6261 636b 2073  gress callback s
+000196e0: 636f 7065 3b20 666f 7220 6578 616d 706c  cope; for exampl
+000196f0: 652c 2061 204d 6573 7361 6765 0d0a 2020  e, a Message..  
+00019700: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+00019710: 6a65 6374 206f 7220 6120 436c 6965 6e74  ject or a Client
+00019720: 2069 6e73 7461 6e63 6520 696e 206f 7264   instance in ord
+00019730: 6572 2074 6f20 6564 6974 2074 6865 206d  er to edit the m
+00019740: 6573 7361 6765 2077 6974 6820 7468 6520  essage with the 
+00019750: 7570 6461 7465 6420 7072 6f67 7265 7373  updated progress
+00019760: 2073 7461 7475 732e 0d0a 0d0a 2020 2020   status.....    
+00019770: 2020 2020 4f74 6865 7220 5061 7261 6d65      Other Parame
+00019780: 7465 7273 3a0d 0a20 2020 2020 2020 2020  ters:..         
+00019790: 2020 2063 7572 7265 6e74 2028 6060 696e     current (``in
+000197a0: 7460 6029 3a0d 0a20 2020 2020 2020 2020  t``):..         
+000197b0: 2020 2020 2020 2054 6865 2061 6d6f 756e         The amoun
+000197c0: 7420 6f66 2062 7974 6573 2074 7261 6e73  t of bytes trans
+000197d0: 6d69 7474 6564 2073 6f20 6661 722e 0d0a  mitted so far...
+000197e0: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
+000197f0: 7461 6c20 2860 6069 6e74 6060 293a 0d0a  tal (``int``):..
+00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019810: 5468 6520 746f 7461 6c20 7369 7a65 206f  The total size o
+00019820: 6620 7468 6520 6669 6c65 2e0d 0a0d 0a20  f the file..... 
+00019830: 2020 2020 2020 2020 2020 202a 6172 6773             *args
+00019840: 2028 6060 7475 706c 6560 602c 202a 6f70   (``tuple``, *op
+00019850: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00019860: 2020 2020 2020 2020 2020 2045 7874 7261             Extra
+00019870: 2063 7573 746f 6d20 6172 6775 6d65 6e74   custom argument
+00019880: 7320 6173 2064 6566 696e 6564 2069 6e20  s as defined in 
+00019890: 7468 6520 6060 7072 6f67 7265 7373 5f61  the ``progress_a
+000198a0: 7267 7360 6020 7061 7261 6d65 7465 722e  rgs`` parameter.
+000198b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000198c0: 2020 596f 7520 6361 6e20 6569 7468 6572    You can either
+000198d0: 206b 6565 7020 6060 2a61 7267 7360 6020   keep ``*args`` 
+000198e0: 6f72 2061 6464 2065 7665 7279 2073 696e  or add every sin
+000198f0: 676c 6520 6578 7472 6120 6172 6775 6d65  gle extra argume
+00019900: 6e74 2069 6e20 796f 7572 2066 756e 6374  nt in your funct
+00019910: 696f 6e20 7369 676e 6174 7572 652e 0d0a  ion signature...
+00019920: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00019930: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00019940: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
+00019950: 7365 6e74 203a 6f62 6a3a 607e 6669 7070  sent :obj:`~fipp
+00019960: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
+00019970: 6020 6973 2072 6574 7572 6e65 642e 0d0a  ` is returned...
+00019980: 2020 2020 2020 2020 2020 2020 496e 2063              In c
+00019990: 6173 6520 7468 6520 7570 6c6f 6164 2069  ase the upload i
+000199a0: 7320 6465 6c69 6265 7261 7465 6c79 2073  s deliberately s
+000199b0: 746f 7070 6564 2077 6974 6820 3a6d 6574  topped with :met
+000199c0: 683a 607e 6669 7070 6572 2e43 6c69 656e  h:`~fipper.Clien
+000199d0: 742e 7374 6f70 5f74 7261 6e73 6d69 7373  t.stop_transmiss
+000199e0: 696f 6e60 2c20 4e6f 6e65 2069 7320 7265  ion`, None is re
+000199f0: 7475 726e 6564 0d0a 2020 2020 2020 2020  turned..        
+00019a00: 2020 2020 696e 7374 6561 642e 0d0a 0d0a      instead.....
+00019a10: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
+00019a20: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
+00019a30: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
+00019a40: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
+00019a50: 2065 7272 6f72 2e0d 0a20 2020 2020 2020   error...       
+00019a60: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
+00019a70: 2071 756f 7465 2069 7320 4e6f 6e65 3a0d   quote is None:.
+00019a80: 0a20 2020 2020 2020 2020 2020 2071 756f  .            quo
+00019a90: 7465 203d 2073 656c 662e 6368 6174 2e74  te = self.chat.t
+00019aa0: 7970 6520 213d 2065 6e75 6d73 2e43 6861  ype != enums.Cha
+00019ab0: 7454 7970 652e 5052 4956 4154 450d 0a0d  tType.PRIVATE...
+00019ac0: 0a20 2020 2020 2020 2069 6620 7265 706c  .        if repl
+00019ad0: 795f 746f 5f6d 6573 7361 6765 5f69 6420  y_to_message_id 
+00019ae0: 6973 204e 6f6e 6520 616e 6420 7175 6f74  is None and quot
+00019af0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00019b00: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00019b10: 5f69 6420 3d20 7365 6c66 2e69 640d 0a0d  _id = self.id...
+00019b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019b30: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+00019b40: 6e74 2e73 656e 645f 7669 6465 6f28 0d0a  nt.send_video(..
+00019b50: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+00019b60: 5f69 643d 7365 6c66 2e63 6861 742e 6964  _id=self.chat.id
+00019b70: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00019b80: 6964 656f 3d76 6964 656f 2c0d 0a20 2020  ideo=video,..   
+00019b90: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
+00019ba0: 3d63 6170 7469 6f6e 2c0d 0a20 2020 2020  =caption,..     
+00019bb0: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
+00019bc0: 653d 7061 7273 655f 6d6f 6465 2c0d 0a20  e=parse_mode,.. 
+00019bd0: 2020 2020 2020 2020 2020 2063 6170 7469             capti
+00019be0: 6f6e 5f65 6e74 6974 6965 733d 6361 7074  on_entities=capt
+00019bf0: 696f 6e5f 656e 7469 7469 6573 2c0d 0a20  ion_entities,.. 
+00019c00: 2020 2020 2020 2020 2020 2074 746c 5f73             ttl_s
+00019c10: 6563 6f6e 6473 3d74 746c 5f73 6563 6f6e  econds=ttl_secon
+00019c20: 6473 2c0d 0a20 2020 2020 2020 2020 2020  ds,..           
+00019c30: 2064 7572 6174 696f 6e3d 6475 7261 7469   duration=durati
+00019c40: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
+00019c50: 2077 6964 7468 3d77 6964 7468 2c0d 0a20   width=width,.. 
+00019c60: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+00019c70: 743d 6865 6967 6874 2c0d 0a20 2020 2020  t=height,..     
+00019c80: 2020 2020 2020 2074 6875 6d62 3d74 6875         thumb=thu
+00019c90: 6d62 2c0d 0a20 2020 2020 2020 2020 2020  mb,..           
+00019ca0: 2073 7570 706f 7274 735f 7374 7265 616d   supports_stream
+00019cb0: 696e 673d 7375 7070 6f72 7473 5f73 7472  ing=supports_str
+00019cc0: 6561 6d69 6e67 2c0d 0a20 2020 2020 2020  eaming,..       
+00019cd0: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+00019ce0: 6966 6963 6174 696f 6e3d 6469 7361 626c  ification=disabl
+00019cf0: 655f 6e6f 7469 6669 6361 7469 6f6e 2c0d  e_notification,.
+00019d00: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00019d10: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+00019d20: 3d72 6570 6c79 5f74 6f5f 6d65 7373 6167  =reply_to_messag
+00019d30: 655f 6964 2c0d 0a20 2020 2020 2020 2020  e_id,..         
+00019d40: 2020 2072 6570 6c79 5f6d 6172 6b75 703d     reply_markup=
+00019d50: 7265 706c 795f 6d61 726b 7570 2c0d 0a20  reply_markup,.. 
+00019d60: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+00019d70: 6573 733d 7072 6f67 7265 7373 2c0d 0a20  ess=progress,.. 
+00019d80: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+00019d90: 6573 735f 6172 6773 3d70 726f 6772 6573  ess_args=progres
+00019da0: 735f 6172 6773 0d0a 2020 2020 2020 2020  s_args..        
+00019db0: 290d 0a0d 0a20 2020 2061 7379 6e63 2064  )....    async d
+00019dc0: 6566 2072 6570 6c79 5f76 6964 656f 5f6e  ef reply_video_n
+00019dd0: 6f74 6528 0d0a 2020 2020 2020 2020 7365  ote(..        se
+00019de0: 6c66 2c0d 0a20 2020 2020 2020 2076 6964  lf,..        vid
+00019df0: 656f 5f6e 6f74 653a 2055 6e69 6f6e 5b73  eo_note: Union[s
+00019e00: 7472 2c20 4269 6e61 7279 494f 5d2c 0d0a  tr, BinaryIO],..
+00019e10: 2020 2020 2020 2020 7175 6f74 653a 2062          quote: b
+00019e20: 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20 2020  ool = None,..   
+00019e30: 2020 2020 2064 7572 6174 696f 6e3a 2069       duration: i
+00019e40: 6e74 203d 2030 2c0d 0a20 2020 2020 2020  nt = 0,..       
+00019e50: 206c 656e 6774 683a 2069 6e74 203d 2031   length: int = 1
+00019e60: 2c0d 0a20 2020 2020 2020 2074 6875 6d62  ,..        thumb
+00019e70: 3a20 7374 7220 3d20 4e6f 6e65 2c0d 0a20  : str = None,.. 
+00019e80: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
+00019e90: 6f74 6966 6963 6174 696f 6e3a 2062 6f6f  otification: boo
+00019ea0: 6c20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  l = None,..     
+00019eb0: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
+00019ec0: 6167 655f 6964 3a20 696e 7420 3d20 4e6f  age_id: int = No
+00019ed0: 6e65 2c0d 0a20 2020 2020 2020 2072 6570  ne,..        rep
+00019ee0: 6c79 5f6d 6172 6b75 703a 2055 6e69 6f6e  ly_markup: Union
+00019ef0: 5b0d 0a20 2020 2020 2020 2020 2020 2022  [..            "
+00019f00: 7479 7065 732e 496e 6c69 6e65 4b65 7962  types.InlineKeyb
+00019f10: 6f61 7264 4d61 726b 7570 222c 0d0a 2020  oardMarkup",..  
+00019f20: 2020 2020 2020 2020 2020 2274 7970 6573            "types
+00019f30: 2e52 6570 6c79 4b65 7962 6f61 7264 4d61  .ReplyKeyboardMa
+00019f40: 726b 7570 222c 0d0a 2020 2020 2020 2020  rkup",..        
+00019f50: 2020 2020 2274 7970 6573 2e52 6570 6c79      "types.Reply
+00019f60: 4b65 7962 6f61 7264 5265 6d6f 7665 222c  KeyboardRemove",
+00019f70: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
+00019f80: 7970 6573 2e46 6f72 6365 5265 706c 7922  ypes.ForceReply"
+00019f90: 0d0a 2020 2020 2020 2020 5d20 3d20 4e6f  ..        ] = No
+00019fa0: 6e65 2c0d 0a20 2020 2020 2020 2070 726f  ne,..        pro
+00019fb0: 6772 6573 733a 2043 616c 6c61 626c 6520  gress: Callable 
+00019fc0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00019fd0: 2070 726f 6772 6573 735f 6172 6773 3a20   progress_args: 
+00019fe0: 7475 706c 6520 3d20 2829 0d0a 2020 2020  tuple = ()..    
+00019ff0: 2920 2d3e 2022 4d65 7373 6167 6522 3a0d  ) -> "Message":.
+0001a000: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
+0001a010: 6420 6d65 7468 6f64 202a 7265 706c 795f  d method *reply_
+0001a020: 7669 6465 6f5f 6e6f 7465 2a20 6f66 203a  video_note* of :
+0001a030: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+0001a040: 6573 2e4d 6573 7361 6765 602e 0d0a 0d0a  es.Message`.....
+0001a050: 2020 2020 2020 2020 5573 6520 6173 2061          Use as a
+0001a060: 2073 686f 7274 6375 7420 666f 723a 0d0a   shortcut for:..
+0001a070: 0d0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+0001a080: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+0001a090: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001a0a0: 6177 6169 7420 636c 6965 6e74 2e73 656e  await client.sen
+0001a0b0: 645f 7669 6465 6f5f 6e6f 7465 280d 0a20  d_video_note(.. 
+0001a0c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001a0d0: 6861 745f 6964 3d6d 6573 7361 6765 2e63  hat_id=message.c
+0001a0e0: 6861 742e 6964 2c0d 0a20 2020 2020 2020  hat.id,..       
+0001a0f0: 2020 2020 2020 2020 2076 6964 656f 5f6e           video_n
+0001a100: 6f74 653d 7669 6465 6f5f 6e6f 7465 0d0a  ote=video_note..
+0001a110: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
+0001a120: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+0001a130: 3a0d 0a20 2020 2020 2020 2020 2020 202e  :..            .
+0001a140: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+0001a150: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
+0001a160: 2020 2020 2020 2020 2061 7761 6974 206d           await m
+0001a170: 6573 7361 6765 2e72 6570 6c79 5f76 6964  essage.reply_vid
+0001a180: 656f 5f6e 6f74 6528 7669 6465 6f5f 6e6f  eo_note(video_no
+0001a190: 7465 290d 0a0d 0a20 2020 2020 2020 2050  te)....        P
+0001a1a0: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+0001a1b0: 2020 2020 2020 2020 7669 6465 6f5f 6e6f          video_no
+0001a1c0: 7465 2028 6060 7374 7260 6029 3a0d 0a20  te (``str``):.. 
+0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2056                 V
+0001a1e0: 6964 656f 206e 6f74 6520 746f 2073 656e  ideo note to sen
+0001a1f0: 642e 0d0a 2020 2020 2020 2020 2020 2020  d...            
+0001a200: 2020 2020 5061 7373 2061 2066 696c 655f      Pass a file_
+0001a210: 6964 2061 7320 7374 7269 6e67 2074 6f20  id as string to 
+0001a220: 7365 6e64 2061 2076 6964 656f 206e 6f74  send a video not
+0001a230: 6520 7468 6174 2065 7869 7374 7320 6f6e  e that exists on
+0001a240: 2074 6865 2054 656c 6567 7261 6d20 7365   the Telegram se
+0001a250: 7276 6572 732c 206f 720d 0a20 2020 2020  rvers, or..     
+0001a260: 2020 2020 2020 2020 2020 2070 6173 7320             pass 
+0001a270: 6120 6669 6c65 2070 6174 6820 6173 2073  a file path as s
+0001a280: 7472 696e 6720 746f 2075 706c 6f61 6420  tring to upload 
+0001a290: 6120 6e65 7720 7669 6465 6f20 6e6f 7465  a new video note
+0001a2a0: 2074 6861 7420 6578 6973 7473 206f 6e20   that exists on 
+0001a2b0: 796f 7572 206c 6f63 616c 206d 6163 6869  your local machi
+0001a2c0: 6e65 2e0d 0a20 2020 2020 2020 2020 2020  ne...           
+0001a2d0: 2020 2020 2053 656e 6469 6e67 2076 6964       Sending vid
+0001a2e0: 656f 206e 6f74 6573 2062 7920 6120 5552  eo notes by a UR
+0001a2f0: 4c20 6973 2063 7572 7265 6e74 6c79 2075  L is currently u
+0001a300: 6e73 7570 706f 7274 6564 2e0d 0a0d 0a20  nsupported..... 
+0001a310: 2020 2020 2020 2020 2020 2071 756f 7465             quote
+0001a320: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+0001a330: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+0001a340: 2020 2020 2020 2020 2020 4966 2060 6054            If ``T
+0001a350: 7275 6560 602c 2074 6865 206d 6573 7361  rue``, the messa
+0001a360: 6765 2077 696c 6c20 6265 2073 656e 7420  ge will be sent 
+0001a370: 6173 2061 2072 6570 6c79 2074 6f20 7468  as a reply to th
+0001a380: 6973 206d 6573 7361 6765 2e0d 0a20 2020  is message...   
+0001a390: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+0001a3a0: 2a72 6570 6c79 5f74 6f5f 6d65 7373 6167  *reply_to_messag
+0001a3b0: 655f 6964 2a20 6973 2070 6173 7365 642c  e_id* is passed,
+0001a3c0: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
+0001a3d0: 7769 6c6c 2062 6520 6967 6e6f 7265 642e  will be ignored.
+0001a3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a3f0: 2020 4465 6661 756c 7473 2074 6f20 6060    Defaults to ``
+0001a400: 5472 7565 6060 2069 6e20 6772 6f75 7020  True`` in group 
+0001a410: 6368 6174 7320 616e 6420 6060 4661 6c73  chats and ``Fals
+0001a420: 6560 6020 696e 2070 7269 7661 7465 2063  e`` in private c
+0001a430: 6861 7473 2e0d 0a0d 0a20 2020 2020 2020  hats.....       
+0001a440: 2020 2020 2064 7572 6174 696f 6e20 2860       duration (`
+0001a450: 6069 6e74 6060 2c20 2a6f 7074 696f 6e61  `int``, *optiona
+0001a460: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+0001a470: 2020 2020 2020 4475 7261 7469 6f6e 206f        Duration o
+0001a480: 6620 7365 6e74 2076 6964 656f 2069 6e20  f sent video in 
+0001a490: 7365 636f 6e64 732e 0d0a 0d0a 2020 2020  seconds.....    
+0001a4a0: 2020 2020 2020 2020 6c65 6e67 7468 2028          length (
+0001a4b0: 6060 696e 7460 602c 202a 6f70 7469 6f6e  ``int``, *option
+0001a4c0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+0001a4d0: 2020 2020 2020 2056 6964 656f 2077 6964         Video wid
+0001a4e0: 7468 2061 6e64 2068 6569 6768 742e 0d0a  th and height...
+0001a4f0: 0d0a 2020 2020 2020 2020 2020 2020 7468  ..            th
+0001a500: 756d 6220 2860 6073 7472 6060 2c20 2a6f  umb (``str``, *o
+0001a510: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+0001a520: 2020 2020 2020 2020 2020 2020 5468 756d              Thum
+0001a530: 626e 6169 6c20 6f66 2074 6865 2076 6964  bnail of the vid
+0001a540: 656f 2073 656e 742e 0d0a 2020 2020 2020  eo sent...      
+0001a550: 2020 2020 2020 2020 2020 5468 6520 7468            The th
+0001a560: 756d 626e 6169 6c20 7368 6f75 6c64 2062  umbnail should b
+0001a570: 6520 696e 204a 5045 4720 666f 726d 6174  e in JPEG format
+0001a580: 2061 6e64 206c 6573 7320 7468 616e 2032   and less than 2
+0001a590: 3030 204b 4220 696e 2073 697a 652e 0d0a  00 KB in size...
+0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5b0: 4120 7468 756d 626e 6169 6c27 7320 7769  A thumbnail's wi
+0001a5c0: 6474 6820 616e 6420 6865 6967 6874 2073  dth and height s
+0001a5d0: 686f 756c 6420 6e6f 7420 6578 6365 6564  hould not exceed
+0001a5e0: 2033 3230 2070 6978 656c 732e 0d0a 2020   320 pixels...  
+0001a5f0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+0001a600: 756d 626e 6169 6c73 2063 616e 2774 2062  umbnails can't b
+0001a610: 6520 7265 7573 6564 2061 6e64 2063 616e  e reused and can
+0001a620: 2062 6520 6f6e 6c79 2075 706c 6f61 6465   be only uploade
+0001a630: 6420 6173 2061 206e 6577 2066 696c 652e  d as a new file.
 0001a640: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a650: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-0001a660: 5f69 6420 2860 6069 6e74 6060 2c20 2a6f  _id (``int``, *o
-0001a670: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-0001a680: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-0001a690: 6865 206d 6573 7361 6765 2069 7320 6120  he message is a 
-0001a6a0: 7265 706c 792c 2049 4420 6f66 2074 6865  reply, ID of the
-0001a6b0: 206f 7269 6769 6e61 6c20 6d65 7373 6167   original messag
-0001a6c0: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-0001a6d0: 2072 6570 6c79 5f6d 6172 6b75 7020 283a   reply_markup (:
-0001a6e0: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
-0001a6f0: 6573 2e49 6e6c 696e 654b 6579 626f 6172  es.InlineKeyboar
-0001a700: 644d 6172 6b75 7060 207c 203a 6f62 6a3a  dMarkup` | :obj:
-0001a710: 607e 6669 7070 6572 2e74 7970 6573 2e52  `~fipper.types.R
-0001a720: 6570 6c79 4b65 7962 6f61 7264 4d61 726b  eplyKeyboardMark
-0001a730: 7570 6020 7c20 3a6f 626a 3a60 7e66 6970  up` | :obj:`~fip
-0001a740: 7065 722e 7479 7065 732e 5265 706c 794b  per.types.ReplyK
-0001a750: 6579 626f 6172 6452 656d 6f76 6560 207c  eyboardRemove` |
-0001a760: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
-0001a770: 7970 6573 2e46 6f72 6365 5265 706c 7960  ypes.ForceReply`
-0001a780: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-0001a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7a0: 4164 6469 7469 6f6e 616c 2069 6e74 6572  Additional inter
-0001a7b0: 6661 6365 206f 7074 696f 6e73 2e20 416e  face options. An
-0001a7c0: 206f 626a 6563 7420 666f 7220 616e 2069   object for an i
-0001a7d0: 6e6c 696e 6520 6b65 7962 6f61 7264 2c20  nline keyboard, 
-0001a7e0: 6375 7374 6f6d 2072 6570 6c79 206b 6579  custom reply key
-0001a7f0: 626f 6172 642c 0d0a 2020 2020 2020 2020  board,..        
-0001a800: 2020 2020 2020 2020 696e 7374 7275 6374          instruct
-0001a810: 696f 6e73 2074 6f20 7265 6d6f 7665 2072  ions to remove r
-0001a820: 6570 6c79 206b 6579 626f 6172 6420 6f72  eply keyboard or
-0001a830: 2074 6f20 666f 7263 6520 6120 7265 706c   to force a repl
-0001a840: 7920 6672 6f6d 2074 6865 2075 7365 722e  y from the user.
-0001a850: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a860: 7072 6f67 7265 7373 2028 6060 4361 6c6c  progress (``Call
-0001a870: 6162 6c65 6060 2c20 2a6f 7074 696f 6e61  able``, *optiona
-0001a880: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-0001a890: 2020 2020 2020 5061 7373 2061 2063 616c        Pass a cal
-0001a8a0: 6c62 6163 6b20 6675 6e63 7469 6f6e 2074  lback function t
-0001a8b0: 6f20 7669 6577 2074 6865 2066 696c 6520  o view the file 
-0001a8c0: 7472 616e 736d 6973 7369 6f6e 2070 726f  transmission pro
-0001a8d0: 6772 6573 732e 0d0a 2020 2020 2020 2020  gress...        
-0001a8e0: 2020 2020 2020 2020 5468 6520 6675 6e63          The func
-0001a8f0: 7469 6f6e 206d 7573 7420 7461 6b65 202a  tion must take *
-0001a900: 2863 7572 7265 6e74 2c20 746f 7461 6c29  (current, total)
-0001a910: 2a20 6173 2070 6f73 6974 696f 6e61 6c20  * as positional 
-0001a920: 6172 6775 6d65 6e74 7320 286c 6f6f 6b20  arguments (look 
-0001a930: 6174 204f 7468 6572 2050 6172 616d 6574  at Other Paramet
-0001a940: 6572 7320 6265 6c6f 7720 666f 7220 610d  ers below for a.
-0001a950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a960: 2064 6574 6169 6c65 6420 6465 7363 7269   detailed descri
-0001a970: 7074 696f 6e29 2061 6e64 2077 696c 6c20  ption) and will 
-0001a980: 6265 2063 616c 6c65 6420 6261 636b 2065  be called back e
-0001a990: 6163 6820 7469 6d65 2061 206e 6577 2066  ach time a new f
-0001a9a0: 696c 6520 6368 756e 6b20 6861 7320 6265  ile chunk has be
-0001a9b0: 656e 2073 7563 6365 7373 6675 6c6c 790d  en successfully.
-0001a9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a9d0: 2074 7261 6e73 6d69 7474 6564 2e0d 0a0d   transmitted....
-0001a9e0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0001a9f0: 6772 6573 735f 6172 6773 2028 6060 7475  gress_args (``tu
-0001aa00: 706c 6560 602c 202a 6f70 7469 6f6e 616c  ple``, *optional
-0001aa10: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-0001aa20: 2020 2020 2045 7874 7261 2063 7573 746f       Extra custo
-0001aa30: 6d20 6172 6775 6d65 6e74 7320 666f 7220  m arguments for 
-0001aa40: 7468 6520 7072 6f67 7265 7373 2063 616c  the progress cal
-0001aa50: 6c62 6163 6b20 6675 6e63 7469 6f6e 2e0d  lback function..
-0001aa60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001aa70: 2059 6f75 2063 616e 2070 6173 7320 616e   You can pass an
-0001aa80: 7974 6869 6e67 2079 6f75 206e 6565 6420  ything you need 
-0001aa90: 746f 2062 6520 6176 6169 6c61 626c 6520  to be available 
-0001aaa0: 696e 2074 6865 2070 726f 6772 6573 7320  in the progress 
-0001aab0: 6361 6c6c 6261 636b 2073 636f 7065 3b20  callback scope; 
-0001aac0: 666f 7220 6578 616d 706c 652c 2061 204d  for example, a M
-0001aad0: 6573 7361 6765 0d0a 2020 2020 2020 2020  essage..        
-0001aae0: 2020 2020 2020 2020 6f62 6a65 6374 206f          object o
-0001aaf0: 7220 6120 436c 6965 6e74 2069 6e73 7461  r a Client insta
-0001ab00: 6e63 6520 696e 206f 7264 6572 2074 6f20  nce in order to 
-0001ab10: 6564 6974 2074 6865 206d 6573 7361 6765  edit the message
-0001ab20: 2077 6974 6820 7468 6520 7570 6461 7465   with the update
-0001ab30: 6420 7072 6f67 7265 7373 2073 7461 7475  d progress statu
-0001ab40: 732e 0d0a 0d0a 2020 2020 2020 2020 4f74  s.....        Ot
-0001ab50: 6865 7220 5061 7261 6d65 7465 7273 3a0d  her Parameters:.
-0001ab60: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-0001ab70: 7265 6e74 2028 6060 696e 7460 6029 3a0d  rent (``int``):.
-0001ab80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ab90: 2054 6865 2061 6d6f 756e 7420 6f66 2062   The amount of b
-0001aba0: 7974 6573 2074 7261 6e73 6d69 7474 6564  ytes transmitted
-0001abb0: 2073 6f20 6661 722e 0d0a 0d0a 2020 2020   so far.....    
-0001abc0: 2020 2020 2020 2020 746f 7461 6c20 2860          total (`
-0001abd0: 6069 6e74 6060 293a 0d0a 2020 2020 2020  `int``):..      
-0001abe0: 2020 2020 2020 2020 2020 5468 6520 746f            The to
-0001abf0: 7461 6c20 7369 7a65 206f 6620 7468 6520  tal size of the 
-0001ac00: 6669 6c65 2e0d 0a0d 0a20 2020 2020 2020  file.....       
-0001ac10: 2020 2020 202a 6172 6773 2028 6060 7475       *args (``tu
-0001ac20: 706c 6560 602c 202a 6f70 7469 6f6e 616c  ple``, *optional
-0001ac30: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-0001ac40: 2020 2020 2045 7874 7261 2063 7573 746f       Extra custo
-0001ac50: 6d20 6172 6775 6d65 6e74 7320 6173 2064  m arguments as d
-0001ac60: 6566 696e 6564 2069 6e20 7468 6520 6060  efined in the ``
-0001ac70: 7072 6f67 7265 7373 5f61 7267 7360 6020  progress_args`` 
-0001ac80: 7061 7261 6d65 7465 722e 0d0a 2020 2020  parameter...    
-0001ac90: 2020 2020 2020 2020 2020 2020 596f 7520              You 
-0001aca0: 6361 6e20 6569 7468 6572 206b 6565 7020  can either keep 
-0001acb0: 6060 2a61 7267 7360 6020 6f72 2061 6464  ``*args`` or add
-0001acc0: 2065 7665 7279 2073 696e 676c 6520 6578   every single ex
-0001acd0: 7472 6120 6172 6775 6d65 6e74 2069 6e20  tra argument in 
-0001ace0: 796f 7572 2066 756e 6374 696f 6e20 7369  your function si
-0001acf0: 676e 6174 7572 652e 0d0a 0d0a 2020 2020  gnature.....    
-0001ad00: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-0001ad10: 2020 2020 2020 2020 2020 4f6e 2073 7563            On suc
-0001ad20: 6365 7373 2c20 7468 6520 7365 6e74 203a  cess, the sent :
-0001ad30: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
-0001ad40: 6573 2e4d 6573 7361 6765 6020 6973 2072  es.Message` is r
-0001ad50: 6574 7572 6e65 642e 0d0a 2020 2020 2020  eturned...      
-0001ad60: 2020 2020 2020 496e 2063 6173 6520 7468        In case th
-0001ad70: 6520 7570 6c6f 6164 2069 7320 6465 6c69  e upload is deli
-0001ad80: 6265 7261 7465 6c79 2073 746f 7070 6564  berately stopped
-0001ad90: 2077 6974 6820 3a6d 6574 683a 607e 6669   with :meth:`~fi
-0001ada0: 7070 6572 2e43 6c69 656e 742e 7374 6f70  pper.Client.stop
-0001adb0: 5f74 7261 6e73 6d69 7373 696f 6e60 2c20  _transmission`, 
-0001adc0: 4e6f 6e65 2069 7320 7265 7475 726e 6564  None is returned
-0001add0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-0001ade0: 7374 6561 642e 0d0a 0d0a 2020 2020 2020  stead.....      
-0001adf0: 2020 5261 6973 6573 3a0d 0a20 2020 2020    Raises:..     
-0001ae00: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
-0001ae10: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
-0001ae20: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
-0001ae30: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-0001ae40: 2020 2020 2020 2020 6966 2071 756f 7465          if quote
-0001ae50: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-0001ae60: 2020 2020 2020 2071 756f 7465 203d 2073         quote = s
-0001ae70: 656c 662e 6368 6174 2e74 7970 6520 213d  elf.chat.type !=
-0001ae80: 2065 6e75 6d73 2e43 6861 7454 7970 652e   enums.ChatType.
-0001ae90: 5052 4956 4154 450d 0a0d 0a20 2020 2020  PRIVATE....     
-0001aea0: 2020 2069 6620 7265 706c 795f 746f 5f6d     if reply_to_m
-0001aeb0: 6573 7361 6765 5f69 6420 6973 204e 6f6e  essage_id is Non
-0001aec0: 6520 616e 6420 7175 6f74 653a 0d0a 2020  e and quote:..  
-0001aed0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-0001aee0: 746f 5f6d 6573 7361 6765 5f69 6420 3d20  to_message_id = 
-0001aef0: 7365 6c66 2e69 640d 0a0d 0a20 2020 2020  self.id....     
-0001af00: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0001af10: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
-0001af20: 645f 7669 6465 6f5f 6e6f 7465 280d 0a20  d_video_note(.. 
-0001af30: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-0001af40: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
-0001af50: 0d0a 2020 2020 2020 2020 2020 2020 7669  ..            vi
-0001af60: 6465 6f5f 6e6f 7465 3d76 6964 656f 5f6e  deo_note=video_n
-0001af70: 6f74 652c 0d0a 2020 2020 2020 2020 2020  ote,..          
-0001af80: 2020 6475 7261 7469 6f6e 3d64 7572 6174    duration=durat
-0001af90: 696f 6e2c 0d0a 2020 2020 2020 2020 2020  ion,..          
-0001afa0: 2020 6c65 6e67 7468 3d6c 656e 6774 682c    length=length,
-0001afb0: 0d0a 2020 2020 2020 2020 2020 2020 7468  ..            th
-0001afc0: 756d 623d 7468 756d 622c 0d0a 2020 2020  umb=thumb,..    
-0001afd0: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-0001afe0: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
-0001aff0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-0001b000: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
-0001b010: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-0001b020: 5f69 643d 7265 706c 795f 746f 5f6d 6573  _id=reply_to_mes
-0001b030: 7361 6765 5f69 642c 0d0a 2020 2020 2020  sage_id,..      
-0001b040: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
-0001b050: 7570 3d72 6570 6c79 5f6d 6172 6b75 702c  up=reply_markup,
-0001b060: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-0001b070: 6f67 7265 7373 3d70 726f 6772 6573 732c  ogress=progress,
-0001b080: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-0001b090: 6f67 7265 7373 5f61 7267 733d 7072 6f67  ogress_args=prog
-0001b0a0: 7265 7373 5f61 7267 730d 0a20 2020 2020  ress_args..     
-0001b0b0: 2020 2029 0d0a 0d0a 2020 2020 6173 796e     )....    asyn
-0001b0c0: 6320 6465 6620 7265 706c 795f 766f 6963  c def reply_voic
-0001b0d0: 6528 0d0a 2020 2020 2020 2020 7365 6c66  e(..        self
-0001b0e0: 2c0d 0a20 2020 2020 2020 2076 6f69 6365  ,..        voice
-0001b0f0: 3a20 556e 696f 6e5b 7374 722c 2042 696e  : Union[str, Bin
-0001b100: 6172 7949 4f5d 2c0d 0a20 2020 2020 2020  aryIO],..       
-0001b110: 2071 756f 7465 3a20 626f 6f6c 203d 204e   quote: bool = N
-0001b120: 6f6e 652c 0d0a 2020 2020 2020 2020 6361  one,..        ca
-0001b130: 7074 696f 6e3a 2073 7472 203d 2022 222c  ption: str = "",
-0001b140: 0d0a 2020 2020 2020 2020 7061 7273 655f  ..        parse_
-0001b150: 6d6f 6465 3a20 4f70 7469 6f6e 616c 5b22  mode: Optional["
-0001b160: 656e 756d 732e 5061 7273 654d 6f64 6522  enums.ParseMode"
-0001b170: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-0001b180: 2020 2063 6170 7469 6f6e 5f65 6e74 6974     caption_entit
-0001b190: 6965 733a 204c 6973 745b 2274 7970 6573  ies: List["types
-0001b1a0: 2e4d 6573 7361 6765 456e 7469 7479 225d  .MessageEntity"]
-0001b1b0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-0001b1c0: 2020 6475 7261 7469 6f6e 3a20 696e 7420    duration: int 
-0001b1d0: 3d20 302c 0d0a 2020 2020 2020 2020 6469  = 0,..        di
-0001b1e0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-0001b1f0: 6f6e 3a20 626f 6f6c 203d 204e 6f6e 652c  on: bool = None,
-0001b200: 0d0a 2020 2020 2020 2020 7265 706c 795f  ..        reply_
-0001b210: 746f 5f6d 6573 7361 6765 5f69 643a 2069  to_message_id: i
-0001b220: 6e74 203d 204e 6f6e 652c 0d0a 2020 2020  nt = None,..    
-0001b230: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
-0001b240: 3a20 556e 696f 6e5b 0d0a 2020 2020 2020  : Union[..      
-0001b250: 2020 2020 2020 2274 7970 6573 2e49 6e6c        "types.Inl
-0001b260: 696e 654b 6579 626f 6172 644d 6172 6b75  ineKeyboardMarku
-0001b270: 7022 2c0d 0a20 2020 2020 2020 2020 2020  p",..           
-0001b280: 2022 7479 7065 732e 5265 706c 794b 6579   "types.ReplyKey
-0001b290: 626f 6172 644d 6172 6b75 7022 2c0d 0a20  boardMarkup",.. 
-0001b2a0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-0001b2b0: 732e 5265 706c 794b 6579 626f 6172 6452  s.ReplyKeyboardR
-0001b2c0: 656d 6f76 6522 2c0d 0a20 2020 2020 2020  emove",..       
-0001b2d0: 2020 2020 2022 7479 7065 732e 466f 7263       "types.Forc
-0001b2e0: 6552 6570 6c79 220d 0a20 2020 2020 2020  eReply"..       
-0001b2f0: 205d 203d 204e 6f6e 652c 0d0a 2020 2020   ] = None,..    
-0001b300: 2020 2020 7072 6f67 7265 7373 3a20 4361      progress: Ca
-0001b310: 6c6c 6162 6c65 203d 204e 6f6e 652c 0d0a  llable = None,..
-0001b320: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-0001b330: 5f61 7267 733a 2074 7570 6c65 203d 2028  _args: tuple = (
-0001b340: 290d 0a20 2020 2029 202d 3e20 224d 6573  )..    ) -> "Mes
-0001b350: 7361 6765 223a 0d0a 2020 2020 2020 2020  sage":..        
-0001b360: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
-0001b370: 2a72 6570 6c79 5f76 6f69 6365 2a20 6f66  *reply_voice* of
-0001b380: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
-0001b390: 7970 6573 2e4d 6573 7361 6765 602e 0d0a  ypes.Message`...
-0001b3a0: 0d0a 2020 2020 2020 2020 5573 6520 6173  ..        Use as
-0001b3b0: 2061 2073 686f 7274 6375 7420 666f 723a   a shortcut for:
-0001b3c0: 0d0a 0d0a 2020 2020 2020 2020 2e2e 2063  ....        .. c
-0001b3d0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0001b3e0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-0001b3f0: 2020 6177 6169 7420 636c 6965 6e74 2e73    await client.s
-0001b400: 656e 645f 766f 6963 6528 0d0a 2020 2020  end_voice(..    
-0001b410: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-0001b420: 5f69 643d 6d65 7373 6167 652e 6368 6174  _id=message.chat
-0001b430: 2e69 642c 0d0a 2020 2020 2020 2020 2020  .id,..          
-0001b440: 2020 2020 2020 766f 6963 653d 766f 6963        voice=voic
-0001b450: 650d 0a20 2020 2020 2020 2020 2020 2029  e..            )
-0001b460: 0d0a 0d0a 2020 2020 2020 2020 4578 616d  ....        Exam
-0001b470: 706c 653a 0d0a 2020 2020 2020 2020 2020  ple:..          
-0001b480: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-0001b490: 3a20 7079 7468 6f6e 0d0a 0d0a 2020 2020  : python....    
-0001b4a0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0001b4b0: 7420 6d65 7373 6167 652e 7265 706c 795f  t message.reply_
-0001b4c0: 766f 6963 6528 766f 6963 6529 0d0a 0d0a  voice(voice)....
-0001b4d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0001b4e0: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
-0001b4f0: 2076 6f69 6365 2028 6060 7374 7260 6029   voice (``str``)
-0001b500: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001b510: 2020 2041 7564 696f 2066 696c 6520 746f     Audio file to
-0001b520: 2073 656e 642e 0d0a 2020 2020 2020 2020   send...        
-0001b530: 2020 2020 2020 2020 5061 7373 2061 2066          Pass a f
-0001b540: 696c 655f 6964 2061 7320 7374 7269 6e67  ile_id as string
-0001b550: 2074 6f20 7365 6e64 2061 6e20 6175 6469   to send an audi
-0001b560: 6f20 7468 6174 2065 7869 7374 7320 6f6e  o that exists on
-0001b570: 2074 6865 2054 656c 6567 7261 6d20 7365   the Telegram se
-0001b580: 7276 6572 732c 0d0a 2020 2020 2020 2020  rvers,..        
-0001b590: 2020 2020 2020 2020 7061 7373 2061 6e20          pass an 
-0001b5a0: 4854 5450 2055 524c 2061 7320 6120 7374  HTTP URL as a st
-0001b5b0: 7269 6e67 2066 6f72 2054 656c 6567 7261  ring for Telegra
-0001b5c0: 6d20 746f 2067 6574 2061 6e20 6175 6469  m to get an audi
-0001b5d0: 6f20 6672 6f6d 2074 6865 2049 6e74 6572  o from the Inter
-0001b5e0: 6e65 742c 206f 720d 0a20 2020 2020 2020  net, or..       
-0001b5f0: 2020 2020 2020 2020 2070 6173 7320 6120           pass a 
-0001b600: 6669 6c65 2070 6174 6820 6173 2073 7472  file path as str
-0001b610: 696e 6720 746f 2075 706c 6f61 6420 6120  ing to upload a 
-0001b620: 6e65 7720 6175 6469 6f20 7468 6174 2065  new audio that e
-0001b630: 7869 7374 7320 6f6e 2079 6f75 7220 6c6f  xists on your lo
-0001b640: 6361 6c20 6d61 6368 696e 652e 0d0a 0d0a  cal machine.....
-0001b650: 2020 2020 2020 2020 2020 2020 7175 6f74              quot
-0001b660: 6520 2860 6062 6f6f 6c60 602c 202a 6f70  e (``bool``, *op
-0001b670: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-0001b680: 2020 2020 2020 2020 2020 2049 6620 6060             If ``
-0001b690: 5472 7565 6060 2c20 7468 6520 6d65 7373  True``, the mess
-0001b6a0: 6167 6520 7769 6c6c 2062 6520 7365 6e74  age will be sent
-0001b6b0: 2061 7320 6120 7265 706c 7920 746f 2074   as a reply to t
-0001b6c0: 6869 7320 6d65 7373 6167 652e 0d0a 2020  his message...  
-0001b6d0: 2020 2020 2020 2020 2020 2020 2020 4966                If
-0001b6e0: 202a 7265 706c 795f 746f 5f6d 6573 7361   *reply_to_messa
-0001b6f0: 6765 5f69 642a 2069 7320 7061 7373 6564  ge_id* is passed
-0001b700: 2c20 7468 6973 2070 6172 616d 6574 6572  , this parameter
-0001b710: 2077 696c 6c20 6265 2069 676e 6f72 6564   will be ignored
-0001b720: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001b730: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
-0001b740: 6054 7275 6560 6020 696e 2067 726f 7570  `True`` in group
-0001b750: 2063 6861 7473 2061 6e64 2060 6046 616c   chats and ``Fal
-0001b760: 7365 6060 2069 6e20 7072 6976 6174 6520  se`` in private 
-0001b770: 6368 6174 732e 0d0a 0d0a 2020 2020 2020  chats.....      
-0001b780: 2020 2020 2020 6361 7074 696f 6e20 2860        caption (`
-0001b790: 6073 7472 6060 2c20 2a6f 7074 696f 6e61  `str``, *optiona
-0001b7a0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-0001b7b0: 2020 2020 2020 566f 6963 6520 6d65 7373        Voice mess
-0001b7c0: 6167 6520 6361 7074 696f 6e2c 2030 2d31  age caption, 0-1
-0001b7d0: 3032 3420 6368 6172 6163 7465 7273 2e0d  024 characters..
-0001b7e0: 0a0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-0001b7f0: 6172 7365 5f6d 6f64 6520 283a 6f62 6a3a  arse_mode (:obj:
-0001b800: 607e 6669 7070 6572 2e65 6e75 6d73 2e50  `~fipper.enums.P
-0001b810: 6172 7365 4d6f 6465 602c 202a 6f70 7469  arseMode`, *opti
-0001b820: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
-0001b830: 2020 2020 2020 2020 2042 7920 6465 6661           By defa
-0001b840: 756c 742c 2074 6578 7473 2061 7265 2070  ult, texts are p
-0001b850: 6172 7365 6420 7573 696e 6720 626f 7468  arsed using both
-0001b860: 204d 6172 6b64 6f77 6e20 616e 6420 4854   Markdown and HT
-0001b870: 4d4c 2073 7479 6c65 732e 0d0a 2020 2020  ML styles...    
-0001b880: 2020 2020 2020 2020 2020 2020 596f 7520              You 
-0001b890: 6361 6e20 636f 6d62 696e 6520 626f 7468  can combine both
-0001b8a0: 2073 796e 7461 7865 7320 746f 6765 7468   syntaxes togeth
-0001b8b0: 6572 2e0d 0a0d 0a20 2020 2020 2020 2020  er.....         
-0001b8c0: 2020 2063 6170 7469 6f6e 5f65 6e74 6974     caption_entit
-0001b8d0: 6965 7320 284c 6973 7420 6f66 203a 6f62  ies (List of :ob
-0001b8e0: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
-0001b8f0: 2e4d 6573 7361 6765 456e 7469 7479 6029  .MessageEntity`)
-0001b900: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001b910: 2020 204c 6973 7420 6f66 2073 7065 6369     List of speci
-0001b920: 616c 2065 6e74 6974 6965 7320 7468 6174  al entities that
-0001b930: 2061 7070 6561 7220 696e 2074 6865 2063   appear in the c
-0001b940: 6170 7469 6f6e 2c20 7768 6963 6820 6361  aption, which ca
-0001b950: 6e20 6265 2073 7065 6369 6669 6564 2069  n be specified i
-0001b960: 6e73 7465 6164 206f 6620 2a70 6172 7365  nstead of *parse
-0001b970: 5f6d 6f64 652a 2e0d 0a0d 0a20 2020 2020  _mode*.....     
-0001b980: 2020 2020 2020 2064 7572 6174 696f 6e20         duration 
-0001b990: 2860 6069 6e74 6060 2c20 2a6f 7074 696f  (``int``, *optio
-0001b9a0: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-0001b9b0: 2020 2020 2020 2020 4475 7261 7469 6f6e          Duration
-0001b9c0: 206f 6620 7468 6520 766f 6963 6520 6d65   of the voice me
-0001b9d0: 7373 6167 6520 696e 2073 6563 6f6e 6473  ssage in seconds
-0001b9e0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-0001b9f0: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-0001ba00: 6174 696f 6e20 2860 6062 6f6f 6c60 602c  ation (``bool``,
-0001ba10: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
-0001ba20: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0001ba30: 656e 6473 2074 6865 206d 6573 7361 6765  ends the message
-0001ba40: 2073 696c 656e 746c 792e 0d0a 2020 2020   silently...    
-0001ba50: 2020 2020 2020 2020 2020 2020 5573 6572              User
-0001ba60: 7320 7769 6c6c 2072 6563 6569 7665 2061  s will receive a
-0001ba70: 206e 6f74 6966 6963 6174 696f 6e20 7769   notification wi
-0001ba80: 7468 206e 6f20 736f 756e 642e 0d0a 0d0a  th no sound.....
-0001ba90: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-0001baa0: 795f 746f 5f6d 6573 7361 6765 5f69 6420  y_to_message_id 
-0001bab0: 2860 6069 6e74 6060 2c20 2a6f 7074 696f  (``int``, *optio
-0001bac0: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-0001bad0: 2020 2020 2020 2020 4966 2074 6865 206d          If the m
-0001bae0: 6573 7361 6765 2069 7320 6120 7265 706c  essage is a repl
-0001baf0: 792c 2049 4420 6f66 2074 6865 206f 7269  y, ID of the ori
-0001bb00: 6769 6e61 6c20 6d65 7373 6167 650d 0a0d  ginal message...
-0001bb10: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-0001bb20: 6c79 5f6d 6172 6b75 7020 283a 6f62 6a3a  ly_markup (:obj:
-0001bb30: 607e 6669 7070 6572 2e74 7970 6573 2e49  `~fipper.types.I
-0001bb40: 6e6c 696e 654b 6579 626f 6172 644d 6172  nlineKeyboardMar
-0001bb50: 6b75 7060 207c 203a 6f62 6a3a 607e 6669  kup` | :obj:`~fi
-0001bb60: 7070 6572 2e74 7970 6573 2e52 6570 6c79  pper.types.Reply
-0001bb70: 4b65 7962 6f61 7264 4d61 726b 7570 6020  KeyboardMarkup` 
-0001bb80: 7c20 3a6f 626a 3a60 7e66 6970 7065 722e  | :obj:`~fipper.
-0001bb90: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
-0001bba0: 6172 6452 656d 6f76 6560 207c 203a 6f62  ardRemove` | :ob
-0001bbb0: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
-0001bbc0: 2e46 6f72 6365 5265 706c 7960 2c20 2a6f  .ForceReply`, *o
-0001bbd0: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-0001bbe0: 2020 2020 2020 2020 2020 2020 4164 6469              Addi
-0001bbf0: 7469 6f6e 616c 2069 6e74 6572 6661 6365  tional interface
-0001bc00: 206f 7074 696f 6e73 2e20 416e 206f 626a   options. An obj
-0001bc10: 6563 7420 666f 7220 616e 2069 6e6c 696e  ect for an inlin
-0001bc20: 6520 6b65 7962 6f61 7264 2c20 6375 7374  e keyboard, cust
-0001bc30: 6f6d 2072 6570 6c79 206b 6579 626f 6172  om reply keyboar
-0001bc40: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-0001bc50: 2020 2020 696e 7374 7275 6374 696f 6e73      instructions
-0001bc60: 2074 6f20 7265 6d6f 7665 2072 6570 6c79   to remove reply
-0001bc70: 206b 6579 626f 6172 6420 6f72 2074 6f20   keyboard or to 
-0001bc80: 666f 7263 6520 6120 7265 706c 7920 6672  force a reply fr
-0001bc90: 6f6d 2074 6865 2075 7365 722e 0d0a 0d0a  om the user.....
-0001bca0: 2020 2020 2020 2020 2020 2020 7072 6f67              prog
-0001bcb0: 7265 7373 2028 6060 4361 6c6c 6162 6c65  ress (``Callable
-0001bcc0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-0001bcd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bce0: 2020 5061 7373 2061 2063 616c 6c62 6163    Pass a callbac
-0001bcf0: 6b20 6675 6e63 7469 6f6e 2074 6f20 7669  k function to vi
-0001bd00: 6577 2074 6865 2066 696c 6520 7472 616e  ew the file tran
-0001bd10: 736d 6973 7369 6f6e 2070 726f 6772 6573  smission progres
-0001bd20: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
-0001bd30: 2020 2020 5468 6520 6675 6e63 7469 6f6e      The function
-0001bd40: 206d 7573 7420 7461 6b65 202a 2863 7572   must take *(cur
-0001bd50: 7265 6e74 2c20 746f 7461 6c29 2a20 6173  rent, total)* as
-0001bd60: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
-0001bd70: 6d65 6e74 7320 286c 6f6f 6b20 6174 204f  ments (look at O
-0001bd80: 7468 6572 2050 6172 616d 6574 6572 7320  ther Parameters 
-0001bd90: 6265 6c6f 7720 666f 7220 610d 0a20 2020  below for a..   
-0001bda0: 2020 2020 2020 2020 2020 2020 2064 6574               det
-0001bdb0: 6169 6c65 6420 6465 7363 7269 7074 696f  ailed descriptio
-0001bdc0: 6e29 2061 6e64 2077 696c 6c20 6265 2063  n) and will be c
-0001bdd0: 616c 6c65 6420 6261 636b 2065 6163 6820  alled back each 
-0001bde0: 7469 6d65 2061 206e 6577 2066 696c 6520  time a new file 
-0001bdf0: 6368 756e 6b20 6861 7320 6265 656e 2073  chunk has been s
-0001be00: 7563 6365 7373 6675 6c6c 790d 0a20 2020  uccessfully..   
-0001be10: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-0001be20: 6e73 6d69 7474 6564 2e0d 0a0d 0a20 2020  nsmitted.....   
-0001be30: 2020 2020 2020 2020 2070 726f 6772 6573           progres
-0001be40: 735f 6172 6773 2028 6060 7475 706c 6560  s_args (``tuple`
-0001be50: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-0001be60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001be70: 2045 7874 7261 2063 7573 746f 6d20 6172   Extra custom ar
-0001be80: 6775 6d65 6e74 7320 666f 7220 7468 6520  guments for the 
-0001be90: 7072 6f67 7265 7373 2063 616c 6c62 6163  progress callbac
-0001bea0: 6b20 6675 6e63 7469 6f6e 2e0d 0a20 2020  k function...   
-0001beb0: 2020 2020 2020 2020 2020 2020 2059 6f75               You
-0001bec0: 2063 616e 2070 6173 7320 616e 7974 6869   can pass anythi
-0001bed0: 6e67 2079 6f75 206e 6565 6420 746f 2062  ng you need to b
-0001bee0: 6520 6176 6169 6c61 626c 6520 696e 2074  e available in t
-0001bef0: 6865 2070 726f 6772 6573 7320 6361 6c6c  he progress call
-0001bf00: 6261 636b 2073 636f 7065 3b20 666f 7220  back scope; for 
-0001bf10: 6578 616d 706c 652c 2061 204d 6573 7361  example, a Messa
-0001bf20: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
-0001bf30: 2020 2020 6f62 6a65 6374 206f 7220 6120      object or a 
-0001bf40: 436c 6965 6e74 2069 6e73 7461 6e63 6520  Client instance 
-0001bf50: 696e 206f 7264 6572 2074 6f20 6564 6974  in order to edit
-0001bf60: 2074 6865 206d 6573 7361 6765 2077 6974   the message wit
-0001bf70: 6820 7468 6520 7570 6461 7465 6420 7072  h the updated pr
-0001bf80: 6f67 7265 7373 2073 7461 7475 732e 0d0a  ogress status...
-0001bf90: 0d0a 2020 2020 2020 2020 4f74 6865 7220  ..        Other 
-0001bfa0: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-0001bfb0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-0001bfc0: 2028 6060 696e 7460 6029 3a0d 0a20 2020   (``int``):..   
-0001bfd0: 2020 2020 2020 2020 2020 2020 2054 6865               The
-0001bfe0: 2061 6d6f 756e 7420 6f66 2062 7974 6573   amount of bytes
-0001bff0: 2074 7261 6e73 6d69 7474 6564 2073 6f20   transmitted so 
-0001c000: 6661 722e 0d0a 0d0a 2020 2020 2020 2020  far.....        
-0001c010: 2020 2020 746f 7461 6c20 2860 6069 6e74      total (``int
-0001c020: 6060 293a 0d0a 2020 2020 2020 2020 2020  ``):..          
-0001c030: 2020 2020 2020 5468 6520 746f 7461 6c20        The total 
-0001c040: 7369 7a65 206f 6620 7468 6520 6669 6c65  size of the file
-0001c050: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-0001c060: 202a 6172 6773 2028 6060 7475 706c 6560   *args (``tuple`
-0001c070: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-0001c080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c090: 2045 7874 7261 2063 7573 746f 6d20 6172   Extra custom ar
-0001c0a0: 6775 6d65 6e74 7320 6173 2064 6566 696e  guments as defin
-0001c0b0: 6564 2069 6e20 7468 6520 6060 7072 6f67  ed in the ``prog
-0001c0c0: 7265 7373 5f61 7267 7360 6020 7061 7261  ress_args`` para
-0001c0d0: 6d65 7465 722e 0d0a 2020 2020 2020 2020  meter...        
-0001c0e0: 2020 2020 2020 2020 596f 7520 6361 6e20          You can 
-0001c0f0: 6569 7468 6572 206b 6565 7020 6060 2a61  either keep ``*a
-0001c100: 7267 7360 6020 6f72 2061 6464 2065 7665  rgs`` or add eve
-0001c110: 7279 2073 696e 676c 6520 6578 7472 6120  ry single extra 
-0001c120: 6172 6775 6d65 6e74 2069 6e20 796f 7572  argument in your
-0001c130: 2066 756e 6374 696f 6e20 7369 676e 6174   function signat
-0001c140: 7572 652e 0d0a 0d0a 2020 2020 2020 2020  ure.....        
-0001c150: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
-0001c160: 2020 2020 2020 4f6e 2073 7563 6365 7373        On success
-0001c170: 2c20 7468 6520 7365 6e74 203a 6f62 6a3a  , the sent :obj:
-0001c180: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
-0001c190: 6573 7361 6765 6020 6973 2072 6574 7572  essage` is retur
-0001c1a0: 6e65 642e 0d0a 2020 2020 2020 2020 2020  ned...          
-0001c1b0: 2020 496e 2063 6173 6520 7468 6520 7570    In case the up
-0001c1c0: 6c6f 6164 2069 7320 6465 6c69 6265 7261  load is delibera
-0001c1d0: 7465 6c79 2073 746f 7070 6564 2077 6974  tely stopped wit
-0001c1e0: 6820 3a6d 6574 683a 607e 6669 7070 6572  h :meth:`~fipper
-0001c1f0: 2e43 6c69 656e 742e 7374 6f70 5f74 7261  .Client.stop_tra
-0001c200: 6e73 6d69 7373 696f 6e60 2c20 4e6f 6e65  nsmission`, None
-0001c210: 2069 7320 7265 7475 726e 6564 0d0a 2020   is returned..  
-0001c220: 2020 2020 2020 2020 2020 696e 7374 6561            instea
-0001c230: 642e 0d0a 0d0a 2020 2020 2020 2020 5261  d.....        Ra
-0001c240: 6973 6573 3a0d 0a20 2020 2020 2020 2020  ises:..         
-0001c250: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
-0001c260: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
-0001c270: 616d 2052 5043 2065 7272 6f72 2e0d 0a20  am RPC error... 
-0001c280: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0001c290: 2020 2020 6966 2071 756f 7465 2069 7320      if quote is 
-0001c2a0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0001c2b0: 2020 2071 756f 7465 203d 2073 656c 662e     quote = self.
-0001c2c0: 6368 6174 2e74 7970 6520 213d 2065 6e75  chat.type != enu
-0001c2d0: 6d73 2e43 6861 7454 7970 652e 5052 4956  ms.ChatType.PRIV
-0001c2e0: 4154 450d 0a0d 0a20 2020 2020 2020 2069  ATE....        i
-0001c2f0: 6620 7265 706c 795f 746f 5f6d 6573 7361  f reply_to_messa
-0001c300: 6765 5f69 6420 6973 204e 6f6e 6520 616e  ge_id is None an
-0001c310: 6420 7175 6f74 653a 0d0a 2020 2020 2020  d quote:..      
-0001c320: 2020 2020 2020 7265 706c 795f 746f 5f6d        reply_to_m
-0001c330: 6573 7361 6765 5f69 6420 3d20 7365 6c66  essage_id = self
-0001c340: 2e69 640d 0a0d 0a20 2020 2020 2020 2072  .id....        r
-0001c350: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-0001c360: 2e5f 636c 6965 6e74 2e73 656e 645f 766f  ._client.send_vo
-0001c370: 6963 6528 0d0a 2020 2020 2020 2020 2020  ice(..          
-0001c380: 2020 6368 6174 5f69 643d 7365 6c66 2e63    chat_id=self.c
-0001c390: 6861 742e 6964 2c0d 0a20 2020 2020 2020  hat.id,..       
-0001c3a0: 2020 2020 2076 6f69 6365 3d76 6f69 6365       voice=voice
-0001c3b0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-0001c3c0: 6170 7469 6f6e 3d63 6170 7469 6f6e 2c0d  aption=caption,.
-0001c3d0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-0001c3e0: 7365 5f6d 6f64 653d 7061 7273 655f 6d6f  se_mode=parse_mo
-0001c3f0: 6465 2c0d 0a20 2020 2020 2020 2020 2020  de,..           
-0001c400: 2063 6170 7469 6f6e 5f65 6e74 6974 6965   caption_entitie
-0001c410: 733d 6361 7074 696f 6e5f 656e 7469 7469  s=caption_entiti
-0001c420: 6573 2c0d 0a20 2020 2020 2020 2020 2020  es,..           
-0001c430: 2064 7572 6174 696f 6e3d 6475 7261 7469   duration=durati
-0001c440: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
-0001c450: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-0001c460: 6174 696f 6e3d 6469 7361 626c 655f 6e6f  ation=disable_no
-0001c470: 7469 6669 6361 7469 6f6e 2c0d 0a20 2020  tification,..   
-0001c480: 2020 2020 2020 2020 2072 6570 6c79 5f74           reply_t
-0001c490: 6f5f 6d65 7373 6167 655f 6964 3d72 6570  o_message_id=rep
-0001c4a0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-0001c4b0: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-0001c4c0: 6570 6c79 5f6d 6172 6b75 703d 7265 706c  eply_markup=repl
-0001c4d0: 795f 6d61 726b 7570 2c0d 0a20 2020 2020  y_markup,..     
-0001c4e0: 2020 2020 2020 2070 726f 6772 6573 733d         progress=
-0001c4f0: 7072 6f67 7265 7373 2c0d 0a20 2020 2020  progress,..     
-0001c500: 2020 2020 2020 2070 726f 6772 6573 735f         progress_
-0001c510: 6172 6773 3d70 726f 6772 6573 735f 6172  args=progress_ar
-0001c520: 6773 0d0a 2020 2020 2020 2020 290d 0a0d  gs..        )...
-0001c530: 0a20 2020 2061 7379 6e63 2064 6566 2065  .    async def e
-0001c540: 6469 745f 7465 7874 280d 0a20 2020 2020  dit_text(..     
-0001c550: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-0001c560: 2020 7465 7874 3a20 7374 722c 0d0a 2020    text: str,..  
-0001c570: 2020 2020 2020 7061 7273 655f 6d6f 6465        parse_mode
-0001c580: 3a20 4f70 7469 6f6e 616c 5b22 656e 756d  : Optional["enum
-0001c590: 732e 5061 7273 654d 6f64 6522 5d20 3d20  s.ParseMode"] = 
-0001c5a0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2065  None,..        e
-0001c5b0: 6e74 6974 6965 733a 204c 6973 745b 2274  ntities: List["t
-0001c5c0: 7970 6573 2e4d 6573 7361 6765 456e 7469  ypes.MessageEnti
-0001c5d0: 7479 225d 203d 204e 6f6e 652c 0d0a 2020  ty"] = None,..  
-0001c5e0: 2020 2020 2020 6469 7361 626c 655f 7765        disable_we
-0001c5f0: 625f 7061 6765 5f70 7265 7669 6577 3a20  b_page_preview: 
-0001c600: 626f 6f6c 203d 204e 6f6e 652c 0d0a 2020  bool = None,..  
-0001c610: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
-0001c620: 7570 3a20 2274 7970 6573 2e49 6e6c 696e  up: "types.Inlin
-0001c630: 654b 6579 626f 6172 644d 6172 6b75 7022  eKeyboardMarkup"
-0001c640: 203d 204e 6f6e 650d 0a20 2020 2029 202d   = None..    ) -
-0001c650: 3e20 224d 6573 7361 6765 223a 0d0a 2020  > "Message":..  
-0001c660: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
-0001c670: 6574 686f 6420 2a65 6469 745f 7465 7874  ethod *edit_text
-0001c680: 2a20 6f66 203a 6f62 6a3a 607e 6669 7070  * of :obj:`~fipp
-0001c690: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
-0001c6a0: 602e 0d0a 0d0a 2020 2020 2020 2020 416e  `.....        An
-0001c6b0: 2061 6c69 6173 2065 7869 7374 7320 6173   alias exists as
-0001c6c0: 202a 6564 6974 2a2e 0d0a 0d0a 2020 2020   *edit*.....    
-0001c6d0: 2020 2020 5573 6520 6173 2061 2073 686f      Use as a sho
-0001c6e0: 7274 6375 7420 666f 723a 0d0a 0d0a 2020  rtcut for:....  
-0001c6f0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-0001c700: 6f63 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a  ock:: python....
-0001c710: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0001c720: 7420 636c 6965 6e74 2e65 6469 745f 6d65  t client.edit_me
-0001c730: 7373 6167 655f 7465 7874 280d 0a20 2020  ssage_text(..   
-0001c740: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-0001c750: 745f 6964 3d6d 6573 7361 6765 2e63 6861  t_id=message.cha
-0001c760: 742e 6964 2c0d 0a20 2020 2020 2020 2020  t.id,..         
-0001c770: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-0001c780: 643d 6d65 7373 6167 652e 6964 2c0d 0a20  d=message.id,.. 
-0001c790: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001c7a0: 6578 743d 2268 656c 6c6f 220d 0a20 2020  ext="hello"..   
-0001c7b0: 2020 2020 2020 2020 2029 0d0a 0d0a 2020           )....  
-0001c7c0: 2020 2020 2020 4578 616d 706c 653a 0d0a        Example:..
-0001c7d0: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-0001c7e0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0001c7f0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-0001c800: 2020 2020 2020 6177 6169 7420 6d65 7373        await mess
-0001c810: 6167 652e 6564 6974 5f74 6578 7428 2268  age.edit_text("h
-0001c820: 656c 6c6f 2229 0d0a 0d0a 2020 2020 2020  ello")....      
-0001c830: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
-0001c840: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-0001c850: 2860 6073 7472 6060 293a 0d0a 2020 2020  (``str``):..    
-0001c860: 2020 2020 2020 2020 2020 2020 4e65 7720              New 
-0001c870: 7465 7874 206f 6620 7468 6520 6d65 7373  text of the mess
-0001c880: 6167 652e 0d0a 0d0a 2020 2020 2020 2020  age.....        
-0001c890: 2020 2020 7061 7273 655f 6d6f 6465 2028      parse_mode (
-0001c8a0: 3a6f 626a 3a60 7e66 6970 7065 722e 656e  :obj:`~fipper.en
-0001c8b0: 756d 732e 5061 7273 654d 6f64 6560 2c20  ums.ParseMode`, 
-0001c8c0: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
-0001c8d0: 2020 2020 2020 2020 2020 2020 2020 4279                By
-0001c8e0: 2064 6566 6175 6c74 2c20 7465 7874 7320   default, texts 
-0001c8f0: 6172 6520 7061 7273 6564 2075 7369 6e67  are parsed using
-0001c900: 2062 6f74 6820 4d61 726b 646f 776e 2061   both Markdown a
-0001c910: 6e64 2048 544d 4c20 7374 796c 6573 2e0d  nd HTML styles..
-0001c920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c930: 2059 6f75 2063 616e 2063 6f6d 6269 6e65   You can combine
-0001c940: 2062 6f74 6820 7379 6e74 6178 6573 2074   both syntaxes t
-0001c950: 6f67 6574 6865 722e 0d0a 0d0a 2020 2020  ogether.....    
-0001c960: 2020 2020 2020 2020 656e 7469 7469 6573          entities
-0001c970: 2028 4c69 7374 206f 6620 3a6f 626a 3a60   (List of :obj:`
-0001c980: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
-0001c990: 7373 6167 6545 6e74 6974 7960 293a 0d0a  ssageEntity`):..
-0001c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9b0: 4c69 7374 206f 6620 7370 6563 6961 6c20  List of special 
-0001c9c0: 656e 7469 7469 6573 2074 6861 7420 6170  entities that ap
-0001c9d0: 7065 6172 2069 6e20 6d65 7373 6167 6520  pear in message 
-0001c9e0: 7465 7874 2c20 7768 6963 6820 6361 6e20  text, which can 
-0001c9f0: 6265 2073 7065 6369 6669 6564 2069 6e73  be specified ins
-0001ca00: 7465 6164 206f 6620 2a70 6172 7365 5f6d  tead of *parse_m
-0001ca10: 6f64 652a 2e0d 0a0d 0a20 2020 2020 2020  ode*.....       
-0001ca20: 2020 2020 2064 6973 6162 6c65 5f77 6562       disable_web
-0001ca30: 5f70 6167 655f 7072 6576 6965 7720 2860  _page_preview (`
-0001ca40: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
-0001ca50: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
-0001ca60: 2020 2020 2020 2044 6973 6162 6c65 7320         Disables 
-0001ca70: 6c69 6e6b 2070 7265 7669 6577 7320 666f  link previews fo
-0001ca80: 7220 6c69 6e6b 7320 696e 2074 6869 7320  r links in this 
-0001ca90: 6d65 7373 6167 652e 0d0a 0d0a 2020 2020  message.....    
-0001caa0: 2020 2020 2020 2020 7265 706c 795f 6d61          reply_ma
-0001cab0: 726b 7570 2028 3a6f 626a 3a60 7e66 6970  rkup (:obj:`~fip
-0001cac0: 7065 722e 7479 7065 732e 496e 6c69 6e65  per.types.Inline
-0001cad0: 4b65 7962 6f61 7264 4d61 726b 7570 602c  KeyboardMarkup`,
-0001cae0: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
-0001caf0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0001cb00: 6e20 496e 6c69 6e65 4b65 7962 6f61 7264  n InlineKeyboard
-0001cb10: 4d61 726b 7570 206f 626a 6563 742e 0d0a  Markup object...
-0001cb20: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0001cb30: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-0001cb40: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
-0001cb50: 6564 6974 6564 203a 6f62 6a3a 607e 6669  edited :obj:`~fi
-0001cb60: 7070 6572 2e74 7970 6573 2e4d 6573 7361  pper.types.Messa
-0001cb70: 6765 6020 6973 2072 6574 7572 6e65 642e  ge` is returned.
-0001cb80: 0d0a 0d0a 2020 2020 2020 2020 5261 6973  ....        Rais
-0001cb90: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-0001cba0: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
-0001cbb0: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
-0001cbc0: 2052 5043 2065 7272 6f72 2e0d 0a20 2020   RPC error...   
-0001cbd0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0001cbe0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-0001cbf0: 656c 662e 5f63 6c69 656e 742e 6564 6974  elf._client.edit
-0001cc00: 5f6d 6573 7361 6765 5f74 6578 7428 0d0a  _message_text(..
-0001cc10: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-0001cc20: 5f69 643d 7365 6c66 2e63 6861 742e 6964  _id=self.chat.id
-0001cc30: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-0001cc40: 6573 7361 6765 5f69 643d 7365 6c66 2e69  essage_id=self.i
-0001cc50: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-0001cc60: 7465 7874 3d74 6578 742c 0d0a 2020 2020  text=text,..    
-0001cc70: 2020 2020 2020 2020 7061 7273 655f 6d6f          parse_mo
-0001cc80: 6465 3d70 6172 7365 5f6d 6f64 652c 0d0a  de=parse_mode,..
-0001cc90: 2020 2020 2020 2020 2020 2020 656e 7469              enti
-0001cca0: 7469 6573 3d65 6e74 6974 6965 732c 0d0a  ties=entities,..
-0001ccb0: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-0001ccc0: 626c 655f 7765 625f 7061 6765 5f70 7265  ble_web_page_pre
-0001ccd0: 7669 6577 3d64 6973 6162 6c65 5f77 6562  view=disable_web
-0001cce0: 5f70 6167 655f 7072 6576 6965 772c 0d0a  _page_preview,..
-0001ccf0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-0001cd00: 795f 6d61 726b 7570 3d72 6570 6c79 5f6d  y_markup=reply_m
-0001cd10: 6172 6b75 700d 0a20 2020 2020 2020 2029  arkup..        )
-0001cd20: 0d0a 0d0a 2020 2020 6564 6974 203d 2065  ....    edit = e
-0001cd30: 6469 745f 7465 7874 0d0a 0d0a 2020 2020  dit_text....    
-0001cd40: 6173 796e 6320 6465 6620 6564 6974 5f63  async def edit_c
-0001cd50: 6170 7469 6f6e 280d 0a20 2020 2020 2020  aption(..       
-0001cd60: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-0001cd70: 6361 7074 696f 6e3a 2073 7472 2c0d 0a20  caption: str,.. 
-0001cd80: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
-0001cd90: 653a 204f 7074 696f 6e61 6c5b 2265 6e75  e: Optional["enu
-0001cda0: 6d73 2e50 6172 7365 4d6f 6465 225d 203d  ms.ParseMode"] =
-0001cdb0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0001cdc0: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
-0001cdd0: 3a20 4c69 7374 5b22 7479 7065 732e 4d65  : List["types.Me
-0001cde0: 7373 6167 6545 6e74 6974 7922 5d20 3d20  ssageEntity"] = 
-0001cdf0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2072  None,..        r
-0001ce00: 6570 6c79 5f6d 6172 6b75 703a 2022 7479  eply_markup: "ty
-0001ce10: 7065 732e 496e 6c69 6e65 4b65 7962 6f61  pes.InlineKeyboa
-0001ce20: 7264 4d61 726b 7570 2220 3d20 4e6f 6e65  rdMarkup" = None
-0001ce30: 0d0a 2020 2020 2920 2d3e 2022 4d65 7373  ..    ) -> "Mess
-0001ce40: 6167 6522 3a0d 0a20 2020 2020 2020 2022  age":..        "
-0001ce50: 2222 426f 756e 6420 6d65 7468 6f64 202a  ""Bound method *
-0001ce60: 6564 6974 5f63 6170 7469 6f6e 2a20 6f66  edit_caption* of
-0001ce70: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
-0001ce80: 7970 6573 2e4d 6573 7361 6765 602e 0d0a  ypes.Message`...
-0001ce90: 0d0a 2020 2020 2020 2020 5573 6520 6173  ..        Use as
-0001cea0: 2061 2073 686f 7274 6375 7420 666f 723a   a shortcut for:
-0001ceb0: 0d0a 0d0a 2020 2020 2020 2020 2e2e 2063  ....        .. c
-0001cec0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-0001ced0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-0001cee0: 2020 6177 6169 7420 636c 6965 6e74 2e65    await client.e
-0001cef0: 6469 745f 6d65 7373 6167 655f 6361 7074  dit_message_capt
-0001cf00: 696f 6e28 0d0a 2020 2020 2020 2020 2020  ion(..          
-0001cf10: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
-0001cf20: 7373 6167 652e 6368 6174 2e69 642c 0d0a  ssage.chat.id,..
-0001cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf40: 6d65 7373 6167 655f 6964 3d6d 6573 7361  message_id=messa
-0001cf50: 6765 2e69 642c 0d0a 2020 2020 2020 2020  ge.id,..        
-0001cf60: 2020 2020 2020 2020 6361 7074 696f 6e3d          caption=
-0001cf70: 2268 656c 6c6f 220d 0a20 2020 2020 2020  "hello"..       
-0001cf80: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-0001cf90: 2020 4578 616d 706c 653a 0d0a 2020 2020    Example:..    
-0001cfa0: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
-0001cfb0: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0d0a  block:: python..
-0001cfc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001cfd0: 2020 6177 6169 7420 6d65 7373 6167 652e    await message.
-0001cfe0: 6564 6974 5f63 6170 7469 6f6e 2822 6865  edit_caption("he
-0001cff0: 6c6c 6f22 290d 0a0d 0a20 2020 2020 2020  llo")....       
-0001d000: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
-0001d010: 2020 2020 2020 2020 2020 6361 7074 696f            captio
-0001d020: 6e20 2860 6073 7472 6060 293a 0d0a 2020  n (``str``):..  
-0001d030: 2020 2020 2020 2020 2020 2020 2020 4e65                Ne
-0001d040: 7720 6361 7074 696f 6e20 6f66 2074 6865  w caption of the
-0001d050: 206d 6573 7361 6765 2e0d 0a0d 0a20 2020   message.....   
-0001d060: 2020 2020 2020 2020 2070 6172 7365 5f6d           parse_m
-0001d070: 6f64 6520 283a 6f62 6a3a 607e 6669 7070  ode (:obj:`~fipp
-0001d080: 6572 2e65 6e75 6d73 2e50 6172 7365 4d6f  er.enums.ParseMo
-0001d090: 6465 602c 202a 6f70 7469 6f6e 616c 2a29  de`, *optional*)
-0001d0a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001d0b0: 2020 2042 7920 6465 6661 756c 742c 2074     By default, t
-0001d0c0: 6578 7473 2061 7265 2070 6172 7365 6420  exts are parsed 
-0001d0d0: 7573 696e 6720 626f 7468 204d 6172 6b64  using both Markd
-0001d0e0: 6f77 6e20 616e 6420 4854 4d4c 2073 7479  own and HTML sty
-0001d0f0: 6c65 732e 0d0a 2020 2020 2020 2020 2020  les...          
-0001d100: 2020 2020 2020 596f 7520 6361 6e20 636f        You can co
-0001d110: 6d62 696e 6520 626f 7468 2073 796e 7461  mbine both synta
-0001d120: 7865 7320 746f 6765 7468 6572 2e0d 0a0d  xes together....
-0001d130: 0a20 2020 2020 2020 2020 2020 2063 6170  .            cap
-0001d140: 7469 6f6e 5f65 6e74 6974 6965 7320 284c  tion_entities (L
-0001d150: 6973 7420 6f66 203a 6f62 6a3a 607e 6669  ist of :obj:`~fi
-0001d160: 7070 6572 2e74 7970 6573 2e4d 6573 7361  pper.types.Messa
-0001d170: 6765 456e 7469 7479 6029 3a0d 0a20 2020  geEntity`):..   
-0001d180: 2020 2020 2020 2020 2020 2020 204c 6973               Lis
-0001d190: 7420 6f66 2073 7065 6369 616c 2065 6e74  t of special ent
-0001d1a0: 6974 6965 7320 7468 6174 2061 7070 6561  ities that appea
-0001d1b0: 7220 696e 2074 6865 2063 6170 7469 6f6e  r in the caption
-0001d1c0: 2c20 7768 6963 6820 6361 6e20 6265 2073  , which can be s
-0001d1d0: 7065 6369 6669 6564 2069 6e73 7465 6164  pecified instead
-0001d1e0: 206f 6620 2a70 6172 7365 5f6d 6f64 652a   of *parse_mode*
-0001d1f0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-0001d200: 2072 6570 6c79 5f6d 6172 6b75 7020 283a   reply_markup (:
-0001d210: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
-0001d220: 6573 2e49 6e6c 696e 654b 6579 626f 6172  es.InlineKeyboar
-0001d230: 644d 6172 6b75 7060 2c20 2a6f 7074 696f  dMarkup`, *optio
-0001d240: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-0001d250: 2020 2020 2020 2020 416e 2049 6e6c 696e          An Inlin
-0001d260: 654b 6579 626f 6172 644d 6172 6b75 7020  eKeyboardMarkup 
-0001d270: 6f62 6a65 6374 2e0d 0a0d 0a20 2020 2020  object.....     
-0001d280: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-0001d290: 2020 2020 2020 2020 204f 6e20 7375 6363           On succ
-0001d2a0: 6573 732c 2074 6865 2065 6469 7465 6420  ess, the edited 
-0001d2b0: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
-0001d2c0: 7065 732e 4d65 7373 6167 6560 2069 7320  pes.Message` is 
-0001d2d0: 7265 7475 726e 6564 2e0d 0a0d 0a20 2020  returned.....   
-0001d2e0: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
-0001d2f0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
-0001d300: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
-0001d310: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
-0001d320: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
-0001d330: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0001d340: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-0001d350: 6965 6e74 2e65 6469 745f 6d65 7373 6167  ient.edit_messag
-0001d360: 655f 6361 7074 696f 6e28 0d0a 2020 2020  e_caption(..    
-0001d370: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0001d380: 7365 6c66 2e63 6861 742e 6964 2c0d 0a20  self.chat.id,.. 
-0001d390: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0001d3a0: 6765 5f69 643d 7365 6c66 2e69 642c 0d0a  ge_id=self.id,..
-0001d3b0: 2020 2020 2020 2020 2020 2020 6361 7074              capt
-0001d3c0: 696f 6e3d 6361 7074 696f 6e2c 0d0a 2020  ion=caption,..  
-0001d3d0: 2020 2020 2020 2020 2020 7061 7273 655f            parse_
-0001d3e0: 6d6f 6465 3d70 6172 7365 5f6d 6f64 652c  mode=parse_mode,
-0001d3f0: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-0001d400: 7074 696f 6e5f 656e 7469 7469 6573 3d63  ption_entities=c
-0001d410: 6170 7469 6f6e 5f65 6e74 6974 6965 732c  aption_entities,
-0001d420: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001d430: 706c 795f 6d61 726b 7570 3d72 6570 6c79  ply_markup=reply
-0001d440: 5f6d 6172 6b75 700d 0a20 2020 2020 2020  _markup..       
-0001d450: 2029 0d0a 0d0a 2020 2020 6173 796e 6320   )....    async 
-0001d460: 6465 6620 6564 6974 5f6d 6564 6961 280d  def edit_media(.
-0001d470: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-0001d480: 2020 2020 2020 2020 6d65 6469 613a 2022          media: "
-0001d490: 7479 7065 732e 496e 7075 744d 6564 6961  types.InputMedia
-0001d4a0: 222c 0d0a 2020 2020 2020 2020 7265 706c  ",..        repl
-0001d4b0: 795f 6d61 726b 7570 3a20 2274 7970 6573  y_markup: "types
-0001d4c0: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
-0001d4d0: 6172 6b75 7022 203d 204e 6f6e 650d 0a20  arkup" = None.. 
-0001d4e0: 2020 2029 202d 3e20 224d 6573 7361 6765     ) -> "Message
-0001d4f0: 223a 0d0a 2020 2020 2020 2020 2222 2242  ":..        """B
-0001d500: 6f75 6e64 206d 6574 686f 6420 2a65 6469  ound method *edi
-0001d510: 745f 6d65 6469 612a 206f 6620 3a6f 626a  t_media* of :obj
-0001d520: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
-0001d530: 4d65 7373 6167 6560 2e0d 0a0d 0a20 2020  Message`.....   
-0001d540: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
-0001d550: 6f72 7463 7574 2066 6f72 3a0d 0a0d 0a20  ortcut for:.... 
-0001d560: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-0001d570: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
-0001d580: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-0001d590: 6974 2063 6c69 656e 742e 6564 6974 5f6d  it client.edit_m
-0001d5a0: 6573 7361 6765 5f6d 6564 6961 280d 0a20  essage_media(.. 
-0001d5b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001d5c0: 6861 745f 6964 3d6d 6573 7361 6765 2e63  hat_id=message.c
-0001d5d0: 6861 742e 6964 2c0d 0a20 2020 2020 2020  hat.id,..       
-0001d5e0: 2020 2020 2020 2020 206d 6573 7361 6765           message
-0001d5f0: 5f69 643d 6d65 7373 6167 652e 6964 2c0d  _id=message.id,.
-0001d600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d610: 206d 6564 6961 3d6d 6564 6961 0d0a 2020   media=media..  
-0001d620: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
-0001d630: 2020 2020 2020 2045 7861 6d70 6c65 3a0d         Example:.
-0001d640: 0a20 2020 2020 2020 2020 2020 202e 2e20  .            .. 
-0001d650: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-0001d660: 686f 6e0d 0a0d 0a20 2020 2020 2020 2020  hon....         
-0001d670: 2020 2020 2020 2061 7761 6974 206d 6573         await mes
-0001d680: 7361 6765 2e65 6469 745f 6d65 6469 6128  sage.edit_media(
-0001d690: 6d65 6469 6129 0d0a 0d0a 2020 2020 2020  media)....      
-0001d6a0: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
-0001d6b0: 2020 2020 2020 2020 2020 206d 6564 6961             media
-0001d6c0: 2028 3a6f 626a 3a60 7e66 6970 7065 722e   (:obj:`~fipper.
-0001d6d0: 7479 7065 732e 496e 7075 744d 6564 6961  types.InputMedia
-0001d6e0: 6029 3a0d 0a20 2020 2020 2020 2020 2020  `):..           
-0001d6f0: 2020 2020 204f 6e65 206f 6620 7468 6520       One of the 
-0001d700: 496e 7075 744d 6564 6961 206f 626a 6563  InputMedia objec
-0001d710: 7473 2064 6573 6372 6962 696e 6720 616e  ts describing an
-0001d720: 2061 6e69 6d61 7469 6f6e 2c20 6175 6469   animation, audi
-0001d730: 6f2c 2064 6f63 756d 656e 742c 2070 686f  o, document, pho
-0001d740: 746f 206f 7220 7669 6465 6f2e 0d0a 0d0a  to or video.....
-0001d750: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-0001d760: 795f 6d61 726b 7570 2028 3a6f 626a 3a60  y_markup (:obj:`
-0001d770: 7e66 6970 7065 722e 7479 7065 732e 496e  ~fipper.types.In
-0001d780: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
-0001d790: 7570 602c 202a 6f70 7469 6f6e 616c 2a29  up`, *optional*)
-0001d7a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001d7b0: 2020 2041 6e20 496e 6c69 6e65 4b65 7962     An InlineKeyb
-0001d7c0: 6f61 7264 4d61 726b 7570 206f 626a 6563  oardMarkup objec
-0001d7d0: 742e 0d0a 0d0a 2020 2020 2020 2020 5265  t.....        Re
-0001d7e0: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-0001d7f0: 2020 2020 4f6e 2073 7563 6365 7373 2c20      On success, 
-0001d800: 7468 6520 6564 6974 6564 203a 6f62 6a3a  the edited :obj:
-0001d810: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
-0001d820: 6573 7361 6765 6020 6973 2072 6574 7572  essage` is retur
-0001d830: 6e65 642e 0d0a 0d0a 2020 2020 2020 2020  ned.....        
-0001d840: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
-0001d850: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
-0001d860: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
-0001d870: 6772 616d 2052 5043 2065 7272 6f72 2e0d  gram RPC error..
-0001d880: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0001d890: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0001d8a0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-0001d8b0: 6564 6974 5f6d 6573 7361 6765 5f6d 6564  edit_message_med
-0001d8c0: 6961 280d 0a20 2020 2020 2020 2020 2020  ia(..           
-0001d8d0: 2063 6861 745f 6964 3d73 656c 662e 6368   chat_id=self.ch
-0001d8e0: 6174 2e69 642c 0d0a 2020 2020 2020 2020  at.id,..        
-0001d8f0: 2020 2020 6d65 7373 6167 655f 6964 3d73      message_id=s
-0001d900: 656c 662e 6964 2c0d 0a20 2020 2020 2020  elf.id,..       
-0001d910: 2020 2020 206d 6564 6961 3d6d 6564 6961       media=media
-0001d920: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-0001d930: 6570 6c79 5f6d 6172 6b75 703d 7265 706c  eply_markup=repl
-0001d940: 795f 6d61 726b 7570 0d0a 2020 2020 2020  y_markup..      
-0001d950: 2020 290d 0a0d 0a20 2020 2061 7379 6e63    )....    async
-0001d960: 2064 6566 2065 6469 745f 7265 706c 795f   def edit_reply_
-0001d970: 6d61 726b 7570 2873 656c 662c 2072 6570  markup(self, rep
-0001d980: 6c79 5f6d 6172 6b75 703a 2022 7479 7065  ly_markup: "type
-0001d990: 732e 496e 6c69 6e65 4b65 7962 6f61 7264  s.InlineKeyboard
-0001d9a0: 4d61 726b 7570 2220 3d20 4e6f 6e65 2920  Markup" = None) 
-0001d9b0: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
-0001d9c0: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
-0001d9d0: 6d65 7468 6f64 202a 6564 6974 5f72 6570  method *edit_rep
-0001d9e0: 6c79 5f6d 6172 6b75 702a 206f 6620 3a6f  ly_markup* of :o
-0001d9f0: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
-0001da00: 732e 4d65 7373 6167 6560 2e0d 0a0d 0a20  s.Message`..... 
-0001da10: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
-0001da20: 7368 6f72 7463 7574 2066 6f72 3a0d 0a0d  shortcut for:...
-0001da30: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-0001da40: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
-0001da50: 0a0d 0a20 2020 2020 2020 2020 2020 2061  ...            a
-0001da60: 7761 6974 2063 6c69 656e 742e 6564 6974  wait client.edit
-0001da70: 5f6d 6573 7361 6765 5f72 6570 6c79 5f6d  _message_reply_m
-0001da80: 6172 6b75 7028 0d0a 2020 2020 2020 2020  arkup(..        
-0001da90: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0001daa0: 6d65 7373 6167 652e 6368 6174 2e69 642c  message.chat.id,
-0001dab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dac0: 2020 6d65 7373 6167 655f 6964 3d6d 6573    message_id=mes
-0001dad0: 7361 6765 2e69 642c 0d0a 2020 2020 2020  sage.id,..      
-0001dae0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
-0001daf0: 6d61 726b 7570 3d69 6e6c 696e 655f 7265  markup=inline_re
-0001db00: 706c 795f 6d61 726b 7570 0d0a 2020 2020  ply_markup..    
-0001db10: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-0001db20: 2020 2020 2045 7861 6d70 6c65 3a0d 0a20       Example:.. 
-0001db30: 2020 2020 2020 2020 2020 202e 2e20 636f             .. co
-0001db40: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-0001db50: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
-0001db60: 2020 2020 2061 7761 6974 206d 6573 7361       await messa
-0001db70: 6765 2e65 6469 745f 7265 706c 795f 6d61  ge.edit_reply_ma
-0001db80: 726b 7570 2869 6e6c 696e 655f 7265 706c  rkup(inline_repl
-0001db90: 795f 6d61 726b 7570 290d 0a0d 0a20 2020  y_markup)....   
-0001dba0: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
-0001dbb0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001dbc0: 706c 795f 6d61 726b 7570 2028 3a6f 626a  ply_markup (:obj
-0001dbd0: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
-0001dbe0: 496e 6c69 6e65 4b65 7962 6f61 7264 4d61  InlineKeyboardMa
-0001dbf0: 726b 7570 6029 3a0d 0a20 2020 2020 2020  rkup`):..       
-0001dc00: 2020 2020 2020 2020 2041 6e20 496e 6c69           An Inli
-0001dc10: 6e65 4b65 7962 6f61 7264 4d61 726b 7570  neKeyboardMarkup
-0001dc20: 206f 626a 6563 742e 0d0a 0d0a 2020 2020   object.....    
-0001dc30: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-0001dc40: 2020 2020 2020 2020 2020 4f6e 2073 7563            On suc
-0001dc50: 6365 7373 2c20 6966 2065 6469 7465 6420  cess, if edited 
-0001dc60: 6d65 7373 6167 6520 6973 2073 656e 7420  message is sent 
-0001dc70: 6279 2074 6865 2062 6f74 2c20 7468 6520  by the bot, the 
-0001dc80: 6564 6974 6564 0d0a 2020 2020 2020 2020  edited..        
-0001dc90: 2020 2020 3a6f 626a 3a60 7e66 6970 7065      :obj:`~fippe
-0001dca0: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
-0001dcb0: 2069 7320 7265 7475 726e 6564 2c20 6f74   is returned, ot
-0001dcc0: 6865 7277 6973 6520 5472 7565 2069 7320  herwise True is 
-0001dcd0: 7265 7475 726e 6564 2e0d 0a0d 0a20 2020  returned.....   
-0001dce0: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
-0001dcf0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
-0001dd00: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
-0001dd10: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
-0001dd20: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
-0001dd30: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-0001dd40: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-0001dd50: 6965 6e74 2e65 6469 745f 6d65 7373 6167  ient.edit_messag
-0001dd60: 655f 7265 706c 795f 6d61 726b 7570 280d  e_reply_markup(.
-0001dd70: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
-0001dd80: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
-0001dd90: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-0001dda0: 6d65 7373 6167 655f 6964 3d73 656c 662e  message_id=self.
-0001ddb0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-0001ddc0: 2072 6570 6c79 5f6d 6172 6b75 703d 7265   reply_markup=re
-0001ddd0: 706c 795f 6d61 726b 7570 0d0a 2020 2020  ply_markup..    
-0001dde0: 2020 2020 290d 0a0d 0a20 2020 2061 7379      )....    asy
-0001ddf0: 6e63 2064 6566 2066 6f72 7761 7264 280d  nc def forward(.
-0001de00: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-0001de10: 2020 2020 2020 2020 6368 6174 5f69 643a          chat_id:
-0001de20: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
-0001de30: 2c0d 0a20 2020 2020 2020 2064 6973 6162  ,..        disab
-0001de40: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3a  le_notification:
-0001de50: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20   bool = None,.. 
-0001de60: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
-0001de70: 6461 7465 3a20 6461 7465 7469 6d65 203d  date: datetime =
-0001de80: 204e 6f6e 650d 0a20 2020 2029 202d 3e20   None..    ) -> 
-0001de90: 556e 696f 6e5b 2274 7970 6573 2e4d 6573  Union["types.Mes
-0001dea0: 7361 6765 222c 204c 6973 745b 2274 7970  sage", List["typ
-0001deb0: 6573 2e4d 6573 7361 6765 225d 5d3a 0d0a  es.Message"]]:..
-0001dec0: 2020 2020 2020 2020 2222 2242 6f75 6e64          """Bound
-0001ded0: 206d 6574 686f 6420 2a66 6f72 7761 7264   method *forward
-0001dee0: 2a20 6f66 203a 6f62 6a3a 607e 6669 7070  * of :obj:`~fipp
-0001def0: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
-0001df00: 602e 0d0a 0d0a 2020 2020 2020 2020 5573  `.....        Us
-0001df10: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-0001df20: 666f 723a 0d0a 0d0a 2020 2020 2020 2020  for:....        
-0001df30: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-0001df40: 7079 7468 6f6e 0d0a 0d0a 2020 2020 2020  python....      
-0001df50: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
-0001df60: 6e74 2e66 6f72 7761 7264 5f6d 6573 7361  nt.forward_messa
-0001df70: 6765 7328 0d0a 2020 2020 2020 2020 2020  ges(..          
-0001df80: 2020 2020 2020 6368 6174 5f69 643d 6368        chat_id=ch
-0001df90: 6174 5f69 642c 0d0a 2020 2020 2020 2020  at_id,..        
-0001dfa0: 2020 2020 2020 2020 6672 6f6d 5f63 6861          from_cha
-0001dfb0: 745f 6964 3d6d 6573 7361 6765 2e63 6861  t_id=message.cha
-0001dfc0: 742e 6964 2c0d 0a20 2020 2020 2020 2020  t.id,..         
-0001dfd0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-0001dfe0: 6473 3d6d 6573 7361 6765 2e69 640d 0a20  ds=message.id.. 
-0001dff0: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
-0001e000: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-0001e010: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-0001e020: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-0001e030: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
-0001e040: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
-0001e050: 7373 6167 652e 666f 7277 6172 6428 6368  ssage.forward(ch
-0001e060: 6174 5f69 6429 0d0a 0d0a 2020 2020 2020  at_id)....      
-0001e070: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
-0001e080: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-0001e090: 6964 2028 6060 696e 7460 6020 7c20 6060  id (``int`` | ``
-0001e0a0: 7374 7260 6029 3a0d 0a20 2020 2020 2020  str``):..       
-0001e0b0: 2020 2020 2020 2020 2055 6e69 7175 6520           Unique 
-0001e0c0: 6964 656e 7469 6669 6572 2028 696e 7429  identifier (int)
-0001e0d0: 206f 7220 7573 6572 6e61 6d65 2028 7374   or username (st
-0001e0e0: 7229 206f 6620 7468 6520 7461 7267 6574  r) of the target
-0001e0f0: 2063 6861 742e 0d0a 2020 2020 2020 2020   chat...        
-0001e100: 2020 2020 2020 2020 466f 7220 796f 7572          For your
-0001e110: 2070 6572 736f 6e61 6c20 636c 6f75 6420   personal cloud 
-0001e120: 2853 6176 6564 204d 6573 7361 6765 7329  (Saved Messages)
-0001e130: 2079 6f75 2063 616e 2073 696d 706c 7920   you can simply 
-0001e140: 7573 6520 226d 6522 206f 7220 2273 656c  use "me" or "sel
-0001e150: 6622 2e0d 0a20 2020 2020 2020 2020 2020  f"...           
-0001e160: 2020 2020 2046 6f72 2061 2063 6f6e 7461       For a conta
-0001e170: 6374 2074 6861 7420 6578 6973 7473 2069  ct that exists i
-0001e180: 6e20 796f 7572 2054 656c 6567 7261 6d20  n your Telegram 
-0001e190: 6164 6472 6573 7320 626f 6f6b 2079 6f75  address book you
-0001e1a0: 2063 616e 2075 7365 2068 6973 2070 686f   can use his pho
-0001e1b0: 6e65 206e 756d 6265 7220 2873 7472 292e  ne number (str).
-0001e1c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001e1d0: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-0001e1e0: 7469 6f6e 2028 6060 626f 6f6c 6060 2c20  tion (``bool``, 
-0001e1f0: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
-0001e200: 2020 2020 2020 2020 2020 2020 2020 5365                Se
-0001e210: 6e64 7320 7468 6520 6d65 7373 6167 6520  nds the message 
-0001e220: 7369 6c65 6e74 6c79 2e0d 0a20 2020 2020  silently...     
-0001e230: 2020 2020 2020 2020 2020 2055 7365 7273             Users
-0001e240: 2077 696c 6c20 7265 6365 6976 6520 6120   will receive a 
-0001e250: 6e6f 7469 6669 6361 7469 6f6e 2077 6974  notification wit
-0001e260: 6820 6e6f 2073 6f75 6e64 2e0d 0a0d 0a20  h no sound..... 
-0001e270: 2020 2020 2020 2020 2020 2073 6368 6564             sched
-0001e280: 756c 655f 6461 7465 2028 3a70 793a 6f62  ule_date (:py:ob
-0001e290: 6a3a 607e 6461 7465 7469 6d65 2e64 6174  j:`~datetime.dat
-0001e2a0: 6574 696d 6560 2c20 2a6f 7074 696f 6e61  etime`, *optiona
-0001e2b0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-0001e2c0: 2020 2020 2020 4461 7465 2077 6865 6e20        Date when 
-0001e2d0: 7468 6520 6d65 7373 6167 6520 7769 6c6c  the message will
-0001e2e0: 2062 6520 6175 746f 6d61 7469 6361 6c6c   be automaticall
-0001e2f0: 7920 7365 6e74 2e0d 0a0d 0a20 2020 2020  y sent.....     
-0001e300: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-0001e310: 2020 2020 2020 2020 204f 6e20 7375 6363           On succ
-0001e320: 6573 732c 2074 6865 2066 6f72 7761 7264  ess, the forward
-0001e330: 6564 204d 6573 7361 6765 2069 7320 7265  ed Message is re
-0001e340: 7475 726e 6564 2e0d 0a0d 0a20 2020 2020  turned.....     
-0001e350: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
-0001e360: 2020 2020 2020 2020 5250 4345 7272 6f72          RPCError
-0001e370: 3a20 496e 2063 6173 6520 6f66 2061 2054  : In case of a T
-0001e380: 656c 6567 7261 6d20 5250 4320 6572 726f  elegram RPC erro
-0001e390: 722e 0d0a 2020 2020 2020 2020 2222 220d  r...        """.
-0001e3a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001e3b0: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
-0001e3c0: 6e74 2e66 6f72 7761 7264 5f6d 6573 7361  nt.forward_messa
-0001e3d0: 6765 7328 0d0a 2020 2020 2020 2020 2020  ges(..          
-0001e3e0: 2020 6368 6174 5f69 643d 6368 6174 5f69    chat_id=chat_i
-0001e3f0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-0001e400: 6672 6f6d 5f63 6861 745f 6964 3d73 656c  from_chat_id=sel
-0001e410: 662e 6368 6174 2e69 642c 0d0a 2020 2020  f.chat.id,..    
-0001e420: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-0001e430: 6964 733d 7365 6c66 2e69 642c 0d0a 2020  ids=self.id,..  
-0001e440: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
-0001e450: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
-0001e460: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-0001e470: 696f 6e2c 0d0a 2020 2020 2020 2020 2020  ion,..          
-0001e480: 2020 7363 6865 6475 6c65 5f64 6174 653d    schedule_date=
-0001e490: 7363 6865 6475 6c65 5f64 6174 650d 0a20  schedule_date.. 
-0001e4a0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-0001e4b0: 6173 796e 6320 6465 6620 636f 7079 280d  async def copy(.
-0001e4c0: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
-0001e4d0: 2020 2020 2020 2020 6368 6174 5f69 643a          chat_id:
-0001e4e0: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
-0001e4f0: 2c0d 0a20 2020 2020 2020 2063 6170 7469  ,..        capti
-0001e500: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0d  on: str = None,.
-0001e510: 0a20 2020 2020 2020 2070 6172 7365 5f6d  .        parse_m
-0001e520: 6f64 653a 204f 7074 696f 6e61 6c5b 2265  ode: Optional["e
-0001e530: 6e75 6d73 2e50 6172 7365 4d6f 6465 225d  nums.ParseMode"]
-0001e540: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-0001e550: 2020 6361 7074 696f 6e5f 656e 7469 7469    caption_entiti
-0001e560: 6573 3a20 4c69 7374 5b22 7479 7065 732e  es: List["types.
-0001e570: 4d65 7373 6167 6545 6e74 6974 7922 5d20  MessageEntity"] 
-0001e580: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-0001e590: 2064 6973 6162 6c65 5f6e 6f74 6966 6963   disable_notific
-0001e5a0: 6174 696f 6e3a 2062 6f6f 6c20 3d20 4e6f  ation: bool = No
-0001e5b0: 6e65 2c0d 0a20 2020 2020 2020 2072 6570  ne,..        rep
-0001e5c0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-0001e5d0: 3a20 696e 7420 3d20 4e6f 6e65 2c0d 0a20  : int = None,.. 
-0001e5e0: 2020 2020 2020 2073 6368 6564 756c 655f         schedule_
-0001e5f0: 6461 7465 3a20 6461 7465 7469 6d65 203d  date: datetime =
-0001e600: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0001e610: 7072 6f74 6563 745f 636f 6e74 656e 743a  protect_content:
-0001e620: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20   bool = None,.. 
-0001e630: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
-0001e640: 6b75 703a 2055 6e69 6f6e 5b0d 0a20 2020  kup: Union[..   
-0001e650: 2020 2020 2020 2020 2022 7479 7065 732e           "types.
-0001e660: 496e 6c69 6e65 4b65 7962 6f61 7264 4d61  InlineKeyboardMa
-0001e670: 726b 7570 222c 0d0a 2020 2020 2020 2020  rkup",..        
-0001e680: 2020 2020 2274 7970 6573 2e52 6570 6c79      "types.Reply
-0001e690: 4b65 7962 6f61 7264 4d61 726b 7570 222c  KeyboardMarkup",
-0001e6a0: 0d0a 2020 2020 2020 2020 2020 2020 2274  ..            "t
-0001e6b0: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
-0001e6c0: 7264 5265 6d6f 7665 222c 0d0a 2020 2020  rdRemove",..    
-0001e6d0: 2020 2020 2020 2020 2274 7970 6573 2e46          "types.F
-0001e6e0: 6f72 6365 5265 706c 7922 0d0a 2020 2020  orceReply"..    
-0001e6f0: 2020 2020 5d20 3d20 6f62 6a65 6374 0d0a      ] = object..
-0001e700: 2020 2020 2920 2d3e 2055 6e69 6f6e 5b22      ) -> Union["
-0001e710: 7479 7065 732e 4d65 7373 6167 6522 2c20  types.Message", 
-0001e720: 4c69 7374 5b22 7479 7065 732e 4d65 7373  List["types.Mess
-0001e730: 6167 6522 5d5d 3a0d 0a20 2020 2020 2020  age"]]:..       
-0001e740: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
-0001e750: 202a 636f 7079 2a20 6f66 203a 6f62 6a3a   *copy* of :obj:
-0001e760: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
-0001e770: 6573 7361 6765 602e 0d0a 0d0a 2020 2020  essage`.....    
-0001e780: 2020 2020 5573 6520 6173 2061 2073 686f      Use as a sho
-0001e790: 7274 6375 7420 666f 723a 0d0a 0d0a 2020  rtcut for:....  
-0001e7a0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-0001e7b0: 6f63 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a  ock:: python....
-0001e7c0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0001e7d0: 7420 636c 6965 6e74 2e63 6f70 795f 6d65  t client.copy_me
-0001e7e0: 7373 6167 6528 0d0a 2020 2020 2020 2020  ssage(..        
-0001e7f0: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-0001e800: 6368 6174 5f69 642c 0d0a 2020 2020 2020  chat_id,..      
-0001e810: 2020 2020 2020 2020 2020 6672 6f6d 5f63            from_c
-0001e820: 6861 745f 6964 3d6d 6573 7361 6765 2e63  hat_id=message.c
-0001e830: 6861 742e 6964 2c0d 0a20 2020 2020 2020  hat.id,..       
-0001e840: 2020 2020 2020 2020 206d 6573 7361 6765           message
-0001e850: 5f69 643d 6d65 7373 6167 652e 6964 0d0a  _id=message.id..
-0001e860: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-0001e870: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0001e880: 3a0d 0a20 2020 2020 2020 2020 2020 202e  :..            .
-0001e890: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-0001e8a0: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
-0001e8b0: 2020 2020 2020 2020 2061 7761 6974 206d           await m
-0001e8c0: 6573 7361 6765 2e63 6f70 7928 6368 6174  essage.copy(chat
-0001e8d0: 5f69 6429 0d0a 0d0a 2020 2020 2020 2020  _id)....        
-0001e8e0: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-0001e8f0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-0001e900: 2028 6060 696e 7460 6020 7c20 6060 7374   (``int`` | ``st
-0001e910: 7260 6029 3a0d 0a20 2020 2020 2020 2020  r``):..         
-0001e920: 2020 2020 2020 2055 6e69 7175 6520 6964         Unique id
-0001e930: 656e 7469 6669 6572 2028 696e 7429 206f  entifier (int) o
-0001e940: 7220 7573 6572 6e61 6d65 2028 7374 7229  r username (str)
-0001e950: 206f 6620 7468 6520 7461 7267 6574 2063   of the target c
-0001e960: 6861 742e 0d0a 2020 2020 2020 2020 2020  hat...          
-0001e970: 2020 2020 2020 466f 7220 796f 7572 2070        For your p
-0001e980: 6572 736f 6e61 6c20 636c 6f75 6420 2853  ersonal cloud (S
-0001e990: 6176 6564 204d 6573 7361 6765 7329 2079  aved Messages) y
-0001e9a0: 6f75 2063 616e 2073 696d 706c 7920 7573  ou can simply us
-0001e9b0: 6520 226d 6522 206f 7220 2273 656c 6622  e "me" or "self"
-0001e9c0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001e9d0: 2020 2046 6f72 2061 2063 6f6e 7461 6374     For a contact
-0001e9e0: 2074 6861 7420 6578 6973 7473 2069 6e20   that exists in 
-0001e9f0: 796f 7572 2054 656c 6567 7261 6d20 6164  your Telegram ad
-0001ea00: 6472 6573 7320 626f 6f6b 2079 6f75 2063  dress book you c
-0001ea10: 616e 2075 7365 2068 6973 2070 686f 6e65  an use his phone
-0001ea20: 206e 756d 6265 7220 2873 7472 292e 0d0a   number (str)...
-0001ea30: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
-0001ea40: 7074 696f 6e20 2860 6073 7472 696e 6760  ption (``string`
-0001ea50: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-0001ea60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ea70: 204e 6577 2063 6170 7469 6f6e 2066 6f72   New caption for
-0001ea80: 206d 6564 6961 2c20 302d 3130 3234 2063   media, 0-1024 c
-0001ea90: 6861 7261 6374 6572 7320 6166 7465 7220  haracters after 
-0001eaa0: 656e 7469 7469 6573 2070 6172 7369 6e67  entities parsing
-0001eab0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001eac0: 2020 2049 6620 6e6f 7420 7370 6563 6966     If not specif
-0001ead0: 6965 642c 2074 6865 206f 7269 6769 6e61  ied, the origina
-0001eae0: 6c20 6361 7074 696f 6e20 6973 206b 6570  l caption is kep
-0001eaf0: 742e 0d0a 2020 2020 2020 2020 2020 2020  t...            
-0001eb00: 2020 2020 5061 7373 2022 2220 2865 6d70      Pass "" (emp
-0001eb10: 7479 2073 7472 696e 6729 2074 6f20 7265  ty string) to re
-0001eb20: 6d6f 7665 2074 6865 2063 6170 7469 6f6e  move the caption
-0001eb30: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-0001eb40: 2070 6172 7365 5f6d 6f64 6520 283a 6f62   parse_mode (:ob
-0001eb50: 6a3a 607e 6669 7070 6572 2e65 6e75 6d73  j:`~fipper.enums
-0001eb60: 2e50 6172 7365 4d6f 6465 602c 202a 6f70  .ParseMode`, *op
-0001eb70: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-0001eb80: 2020 2020 2020 2020 2020 2042 7920 6465             By de
-0001eb90: 6661 756c 742c 2074 6578 7473 2061 7265  fault, texts are
-0001eba0: 2070 6172 7365 6420 7573 696e 6720 626f   parsed using bo
-0001ebb0: 7468 204d 6172 6b64 6f77 6e20 616e 6420  th Markdown and 
-0001ebc0: 4854 4d4c 2073 7479 6c65 732e 0d0a 2020  HTML styles...  
-0001ebd0: 2020 2020 2020 2020 2020 2020 2020 596f                Yo
-0001ebe0: 7520 6361 6e20 636f 6d62 696e 6520 626f  u can combine bo
-0001ebf0: 7468 2073 796e 7461 7865 7320 746f 6765  th syntaxes toge
-0001ec00: 7468 6572 2e0d 0a0d 0a20 2020 2020 2020  ther.....       
-0001ec10: 2020 2020 2063 6170 7469 6f6e 5f65 6e74       caption_ent
-0001ec20: 6974 6965 7320 284c 6973 7420 6f66 203a  ities (List of :
-0001ec30: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
-0001ec40: 6573 2e4d 6573 7361 6765 456e 7469 7479  es.MessageEntity
-0001ec50: 6029 3a0d 0a20 2020 2020 2020 2020 2020  `):..           
-0001ec60: 2020 2020 204c 6973 7420 6f66 2073 7065       List of spe
-0001ec70: 6369 616c 2065 6e74 6974 6965 7320 7468  cial entities th
-0001ec80: 6174 2061 7070 6561 7220 696e 2074 6865  at appear in the
-0001ec90: 206e 6577 2063 6170 7469 6f6e 2c20 7768   new caption, wh
-0001eca0: 6963 6820 6361 6e20 6265 2073 7065 6369  ich can be speci
-0001ecb0: 6669 6564 2069 6e73 7465 6164 206f 6620  fied instead of 
-0001ecc0: 2a70 6172 7365 5f6d 6f64 652a 2e0d 0a0d  *parse_mode*....
-0001ecd0: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-0001ece0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-0001ecf0: 6e20 2860 6062 6f6f 6c60 602c 202a 6f70  n (``bool``, *op
-0001ed00: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-0001ed10: 2020 2020 2020 2020 2020 2053 656e 6473             Sends
-0001ed20: 2074 6865 206d 6573 7361 6765 2073 696c   the message sil
-0001ed30: 656e 746c 792e 0d0a 2020 2020 2020 2020  ently...        
-0001ed40: 2020 2020 2020 2020 5573 6572 7320 7769          Users wi
-0001ed50: 6c6c 2072 6563 6569 7665 2061 206e 6f74  ll receive a not
-0001ed60: 6966 6963 6174 696f 6e20 7769 7468 206e  ification with n
-0001ed70: 6f20 736f 756e 642e 0d0a 0d0a 2020 2020  o sound.....    
-0001ed80: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
-0001ed90: 5f6d 6573 7361 6765 5f69 6420 2860 6069  _message_id (``i
-0001eda0: 6e74 6060 2c20 2a6f 7074 696f 6e61 6c2a  nt``, *optional*
-0001edb0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001edc0: 2020 2020 4966 2074 6865 206d 6573 7361      If the messa
-0001edd0: 6765 2069 7320 6120 7265 706c 792c 2049  ge is a reply, I
-0001ede0: 4420 6f66 2074 6865 206f 7269 6769 6e61  D of the origina
-0001edf0: 6c20 6d65 7373 6167 652e 0d0a 0d0a 2020  l message.....  
-0001ee00: 2020 2020 2020 2020 2020 7363 6865 6475            schedu
-0001ee10: 6c65 5f64 6174 6520 283a 7079 3a6f 626a  le_date (:py:obj
-0001ee20: 3a60 7e64 6174 6574 696d 652e 6461 7465  :`~datetime.date
-0001ee30: 7469 6d65 602c 202a 6f70 7469 6f6e 616c  time`, *optional
-0001ee40: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-0001ee50: 2020 2020 2044 6174 6520 7768 656e 2074       Date when t
-0001ee60: 6865 206d 6573 7361 6765 2077 696c 6c20  he message will 
-0001ee70: 6265 2061 7574 6f6d 6174 6963 616c 6c79  be automatically
-0001ee80: 2073 656e 742e 0d0a 0d0a 2020 2020 2020   sent.....      
-0001ee90: 2020 2020 2020 7072 6f74 6563 745f 636f        protect_co
-0001eea0: 6e74 656e 7420 2860 6062 6f6f 6c60 602c  ntent (``bool``,
-0001eeb0: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
-0001eec0: 2020 2020 2020 2020 2020 2020 2020 2050                 P
-0001eed0: 726f 7465 6374 7320 7468 6520 636f 6e74  rotects the cont
-0001eee0: 656e 7473 206f 6620 7468 6520 7365 6e74  ents of the sent
-0001eef0: 206d 6573 7361 6765 2066 726f 6d20 666f   message from fo
-0001ef00: 7277 6172 6469 6e67 2061 6e64 2073 6176  rwarding and sav
-0001ef10: 696e 672e 0d0a 0d0a 2020 2020 2020 2020  ing.....        
-0001ef20: 2020 2020 7265 706c 795f 6d61 726b 7570      reply_markup
-0001ef30: 2028 3a6f 626a 3a60 7e66 6970 7065 722e   (:obj:`~fipper.
-0001ef40: 7479 7065 732e 496e 6c69 6e65 4b65 7962  types.InlineKeyb
-0001ef50: 6f61 7264 4d61 726b 7570 6020 7c20 3a6f  oardMarkup` | :o
-0001ef60: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
-0001ef70: 732e 5265 706c 794b 6579 626f 6172 644d  s.ReplyKeyboardM
-0001ef80: 6172 6b75 7060 207c 203a 6f62 6a3a 607e  arkup` | :obj:`~
-0001ef90: 6669 7070 6572 2e74 7970 6573 2e52 6570  fipper.types.Rep
-0001efa0: 6c79 4b65 7962 6f61 7264 5265 6d6f 7665  lyKeyboardRemove
-0001efb0: 6020 7c20 3a6f 626a 3a60 7e66 6970 7065  ` | :obj:`~fippe
-0001efc0: 722e 7479 7065 732e 466f 7263 6552 6570  r.types.ForceRep
-0001efd0: 6c79 602c 202a 6f70 7469 6f6e 616c 2a29  ly`, *optional*)
-0001efe0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001eff0: 2020 2041 6464 6974 696f 6e61 6c20 696e     Additional in
-0001f000: 7465 7266 6163 6520 6f70 7469 6f6e 732e  terface options.
-0001f010: 2041 6e20 6f62 6a65 6374 2066 6f72 2061   An object for a
-0001f020: 6e20 696e 6c69 6e65 206b 6579 626f 6172  n inline keyboar
-0001f030: 642c 2063 7573 746f 6d20 7265 706c 7920  d, custom reply 
-0001f040: 6b65 7962 6f61 7264 2c0d 0a20 2020 2020  keyboard,..     
-0001f050: 2020 2020 2020 2020 2020 2069 6e73 7472             instr
-0001f060: 7563 7469 6f6e 7320 746f 2072 656d 6f76  uctions to remov
-0001f070: 6520 7265 706c 7920 6b65 7962 6f61 7264  e reply keyboard
-0001f080: 206f 7220 746f 2066 6f72 6365 2061 2072   or to force a r
-0001f090: 6570 6c79 2066 726f 6d20 7468 6520 7573  eply from the us
-0001f0a0: 6572 2e0d 0a20 2020 2020 2020 2020 2020  er...           
-0001f0b0: 2020 2020 2049 6620 6e6f 7420 7370 6563       If not spec
-0001f0c0: 6966 6965 642c 2074 6865 206f 7269 6769  ified, the origi
-0001f0d0: 6e61 6c20 7265 706c 7920 6d61 726b 7570  nal reply markup
-0001f0e0: 2069 7320 6b65 7074 2e0d 0a20 2020 2020   is kept...     
-0001f0f0: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-0001f100: 4e6f 6e65 2074 6f20 7265 6d6f 7665 2074  None to remove t
-0001f110: 6865 2072 6570 6c79 206d 6172 6b75 702e  he reply markup.
-0001f120: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-0001f130: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
-0001f140: 2020 3a6f 626a 3a60 7e66 6970 7065 722e    :obj:`~fipper.
-0001f150: 7479 7065 732e 4d65 7373 6167 6560 3a20  types.Message`: 
-0001f160: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
-0001f170: 636f 7069 6564 206d 6573 7361 6765 2069  copied message i
-0001f180: 7320 7265 7475 726e 6564 2e0d 0a0d 0a20  s returned..... 
-0001f190: 2020 2020 2020 2052 6169 7365 733a 0d0a         Raises:..
-0001f1a0: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
-0001f1b0: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
-0001f1c0: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
-0001f1d0: 6572 726f 722e 0d0a 2020 2020 2020 2020  error...        
-0001f1e0: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-0001f1f0: 7365 6c66 2e73 6572 7669 6365 3a0d 0a20  self.service:.. 
-0001f200: 2020 2020 2020 2020 2020 206c 6f67 2e77             log.w
-0001f210: 6172 6e69 6e67 2866 2253 6572 7669 6365  arning(f"Service
-0001f220: 206d 6573 7361 6765 7320 6361 6e6e 6f74   messages cannot
-0001f230: 2062 6520 636f 7069 6564 2e20 220d 0a20   be copied. ".. 
-0001f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f250: 2020 2020 2020 2066 2263 6861 745f 6964         f"chat_id
-0001f260: 3a20 7b73 656c 662e 6368 6174 2e69 647d  : {self.chat.id}
-0001f270: 2c20 6d65 7373 6167 655f 6964 3a20 7b73  , message_id: {s
-0001f280: 656c 662e 6964 7d22 290d 0a20 2020 2020  elf.id}")..     
-0001f290: 2020 2065 6c69 6620 7365 6c66 2e67 616d     elif self.gam
-0001f2a0: 6520 616e 6420 6e6f 7420 6177 6169 7420  e and not await 
-0001f2b0: 7365 6c66 2e5f 636c 6965 6e74 2e73 746f  self._client.sto
-0001f2c0: 7261 6765 2e69 735f 626f 7428 293a 0d0a  rage.is_bot():..
-0001f2d0: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
-0001f2e0: 7761 726e 696e 6728 6622 5573 6572 7320  warning(f"Users 
-0001f2f0: 6361 6e6e 6f74 2073 656e 6420 6d65 7373  cannot send mess
-0001f300: 6167 6573 2077 6974 6820 4761 6d65 206d  ages with Game m
-0001f310: 6564 6961 2074 7970 652e 2022 0d0a 2020  edia type. "..  
-0001f320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f330: 2020 2020 2020 6622 6368 6174 5f69 643a        f"chat_id:
-0001f340: 207b 7365 6c66 2e63 6861 742e 6964 7d2c   {self.chat.id},
-0001f350: 206d 6573 7361 6765 5f69 643a 207b 7365   message_id: {se
-0001f360: 6c66 2e69 647d 2229 0d0a 2020 2020 2020  lf.id}")..      
-0001f370: 2020 656c 6966 2073 656c 662e 656d 7074    elif self.empt
-0001f380: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0001f390: 6c6f 672e 7761 726e 696e 6728 6622 456d  log.warning(f"Em
-0001f3a0: 7074 7920 6d65 7373 6167 6573 2063 616e  pty messages can
-0001f3b0: 6e6f 7420 6265 2063 6f70 6965 642e 2022  not be copied. "
-0001f3c0: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-0001f3d0: 7365 6c66 2e74 6578 743a 0d0a 2020 2020  self.text:..    
-0001f3e0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0001f3f0: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
-0001f400: 742e 7365 6e64 5f6d 6573 7361 6765 280d  t.send_message(.
-0001f410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f420: 2063 6861 745f 6964 2c0d 0a20 2020 2020   chat_id,..     
-0001f430: 2020 2020 2020 2020 2020 2074 6578 743d             text=
-0001f440: 7365 6c66 2e74 6578 742c 0d0a 2020 2020  self.text,..    
-0001f450: 2020 2020 2020 2020 2020 2020 656e 7469              enti
-0001f460: 7469 6573 3d73 656c 662e 656e 7469 7469  ties=self.entiti
-0001f470: 6573 2c0d 0a20 2020 2020 2020 2020 2020  es,..           
-0001f480: 2020 2020 2070 6172 7365 5f6d 6f64 653d       parse_mode=
-0001f490: 656e 756d 732e 5061 7273 654d 6f64 652e  enums.ParseMode.
-0001f4a0: 4449 5341 424c 4544 2c0d 0a20 2020 2020  DISABLED,..     
-0001f4b0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-0001f4c0: 6c65 5f77 6562 5f70 6167 655f 7072 6576  le_web_page_prev
-0001f4d0: 6965 773d 6e6f 7420 7365 6c66 2e77 6562  iew=not self.web
-0001f4e0: 5f70 6167 652c 0d0a 2020 2020 2020 2020  _page,..        
-0001f4f0: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-0001f500: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
-0001f510: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-0001f520: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
-0001f530: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
-0001f540: 7361 6765 5f69 643d 7265 706c 795f 746f  sage_id=reply_to
-0001f550: 5f6d 6573 7361 6765 5f69 642c 0d0a 2020  _message_id,..  
-0001f560: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0001f570: 6865 6475 6c65 5f64 6174 653d 7363 6865  hedule_date=sche
-0001f580: 6475 6c65 5f64 6174 652c 0d0a 2020 2020  dule_date,..    
-0001f590: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
-0001f5a0: 6563 745f 636f 6e74 656e 743d 7072 6f74  ect_content=prot
-0001f5b0: 6563 745f 636f 6e74 656e 742c 0d0a 2020  ect_content,..  
-0001f5c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001f5d0: 706c 795f 6d61 726b 7570 3d73 656c 662e  ply_markup=self.
-0001f5e0: 7265 706c 795f 6d61 726b 7570 2069 6620  reply_markup if 
-0001f5f0: 7265 706c 795f 6d61 726b 7570 2069 7320  reply_markup is 
-0001f600: 6f62 6a65 6374 2065 6c73 6520 7265 706c  object else repl
-0001f610: 795f 6d61 726b 7570 0d0a 2020 2020 2020  y_markup..      
-0001f620: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001f630: 2065 6c69 6620 7365 6c66 2e6d 6564 6961   elif self.media
-0001f640: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-0001f650: 656e 645f 6d65 6469 6120 3d20 7061 7274  end_media = part
-0001f660: 6961 6c28 0d0a 2020 2020 2020 2020 2020  ial(..          
-0001f670: 2020 2020 2020 7365 6c66 2e5f 636c 6965        self._clie
-0001f680: 6e74 2e73 656e 645f 6361 6368 6564 5f6d  nt.send_cached_m
-0001f690: 6564 6961 2c0d 0a20 2020 2020 2020 2020  edia,..         
-0001f6a0: 2020 2020 2020 2063 6861 745f 6964 3d63         chat_id=c
-0001f6b0: 6861 745f 6964 2c0d 0a20 2020 2020 2020  hat_id,..       
-0001f6c0: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-0001f6d0: 5f6e 6f74 6966 6963 6174 696f 6e3d 6469  _notification=di
-0001f6e0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
-0001f6f0: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
-0001f700: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
-0001f710: 7373 6167 655f 6964 3d72 6570 6c79 5f74  ssage_id=reply_t
-0001f720: 6f5f 6d65 7373 6167 655f 6964 2c0d 0a20  o_message_id,.. 
-0001f730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001f740: 6368 6564 756c 655f 6461 7465 3d73 6368  chedule_date=sch
-0001f750: 6564 756c 655f 6461 7465 2c0d 0a20 2020  edule_date,..   
-0001f760: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-0001f770: 7465 6374 5f63 6f6e 7465 6e74 3d70 726f  tect_content=pro
-0001f780: 7465 6374 5f63 6f6e 7465 6e74 2c0d 0a20  tect_content,.. 
-0001f790: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001f7a0: 6570 6c79 5f6d 6172 6b75 703d 7365 6c66  eply_markup=self
-0001f7b0: 2e72 6570 6c79 5f6d 6172 6b75 7020 6966  .reply_markup if
-0001f7c0: 2072 6570 6c79 5f6d 6172 6b75 7020 6973   reply_markup is
-0001f7d0: 206f 626a 6563 7420 656c 7365 2072 6570   object else rep
-0001f7e0: 6c79 5f6d 6172 6b75 700d 0a20 2020 2020  ly_markup..     
-0001f7f0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-0001f800: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001f810: 7068 6f74 6f3a 0d0a 2020 2020 2020 2020  photo:..        
-0001f820: 2020 2020 2020 2020 6669 6c65 5f69 6420          file_id 
-0001f830: 3d20 7365 6c66 2e70 686f 746f 2e66 696c  = self.photo.fil
-0001f840: 655f 6964 0d0a 2020 2020 2020 2020 2020  e_id..          
-0001f850: 2020 656c 6966 2073 656c 662e 6175 6469    elif self.audi
-0001f860: 6f3a 0d0a 2020 2020 2020 2020 2020 2020  o:..            
-0001f870: 2020 2020 6669 6c65 5f69 6420 3d20 7365      file_id = se
-0001f880: 6c66 2e61 7564 696f 2e66 696c 655f 6964  lf.audio.file_id
-0001f890: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0001f8a0: 6966 2073 656c 662e 646f 6375 6d65 6e74  if self.document
-0001f8b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001f8c0: 2020 2066 696c 655f 6964 203d 2073 656c     file_id = sel
-0001f8d0: 662e 646f 6375 6d65 6e74 2e66 696c 655f  f.document.file_
-0001f8e0: 6964 0d0a 2020 2020 2020 2020 2020 2020  id..            
-0001f8f0: 656c 6966 2073 656c 662e 7669 6465 6f3a  elif self.video:
-0001f900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001f910: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
-0001f920: 2e76 6964 656f 2e66 696c 655f 6964 0d0a  .video.file_id..
-0001f930: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0001f940: 2073 656c 662e 616e 696d 6174 696f 6e3a   self.animation:
-0001f950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001f960: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
-0001f970: 2e61 6e69 6d61 7469 6f6e 2e66 696c 655f  .animation.file_
-0001f980: 6964 0d0a 2020 2020 2020 2020 2020 2020  id..            
-0001f990: 656c 6966 2073 656c 662e 766f 6963 653a  elif self.voice:
-0001f9a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001f9b0: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
-0001f9c0: 2e76 6f69 6365 2e66 696c 655f 6964 0d0a  .voice.file_id..
-0001f9d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0001f9e0: 2073 656c 662e 7374 6963 6b65 723a 0d0a   self.sticker:..
-0001f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa00: 6669 6c65 5f69 6420 3d20 7365 6c66 2e73  file_id = self.s
-0001fa10: 7469 636b 6572 2e66 696c 655f 6964 0d0a  ticker.file_id..
-0001fa20: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0001fa30: 2073 656c 662e 7669 6465 6f5f 6e6f 7465   self.video_note
-0001fa40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001fa50: 2020 2066 696c 655f 6964 203d 2073 656c     file_id = sel
-0001fa60: 662e 7669 6465 6f5f 6e6f 7465 2e66 696c  f.video_note.fil
-0001fa70: 655f 6964 0d0a 2020 2020 2020 2020 2020  e_id..          
-0001fa80: 2020 656c 6966 2073 656c 662e 636f 6e74    elif self.cont
-0001fa90: 6163 743a 0d0a 2020 2020 2020 2020 2020  act:..          
-0001faa0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0001fab0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-0001fac0: 7365 6e64 5f63 6f6e 7461 6374 280d 0a20  send_contact(.. 
-0001fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fae0: 2020 2063 6861 745f 6964 2c0d 0a20 2020     chat_id,..   
-0001faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb00: 2070 686f 6e65 5f6e 756d 6265 723d 7365   phone_number=se
-0001fb10: 6c66 2e63 6f6e 7461 6374 2e70 686f 6e65  lf.contact.phone
-0001fb20: 5f6e 756d 6265 722c 0d0a 2020 2020 2020  _number,..      
-0001fb30: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0001fb40: 7273 745f 6e61 6d65 3d73 656c 662e 636f  rst_name=self.co
-0001fb50: 6e74 6163 742e 6669 7273 745f 6e61 6d65  ntact.first_name
-0001fb60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001fb70: 2020 2020 2020 206c 6173 745f 6e61 6d65         last_name
-0001fb80: 3d73 656c 662e 636f 6e74 6163 742e 6c61  =self.contact.la
-0001fb90: 7374 5f6e 616d 652c 0d0a 2020 2020 2020  st_name,..      
-0001fba0: 2020 2020 2020 2020 2020 2020 2020 7663                vc
-0001fbb0: 6172 643d 7365 6c66 2e63 6f6e 7461 6374  ard=self.contact
-0001fbc0: 2e76 6361 7264 2c0d 0a20 2020 2020 2020  .vcard,..       
-0001fbd0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-0001fbe0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-0001fbf0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
-0001fc00: 6361 7469 6f6e 2c0d 0a20 2020 2020 2020  cation,..       
-0001fc10: 2020 2020 2020 2020 2020 2020 2073 6368               sch
-0001fc20: 6564 756c 655f 6461 7465 3d73 6368 6564  edule_date=sched
-0001fc30: 756c 655f 6461 7465 0d0a 2020 2020 2020  ule_date..      
-0001fc40: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-0001fc50: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
-0001fc60: 6c66 2e6c 6f63 6174 696f 6e3a 0d0a 2020  lf.location:..  
-0001fc70: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001fc80: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-0001fc90: 5f63 6c69 656e 742e 7365 6e64 5f6c 6f63  _client.send_loc
-0001fca0: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
-0001fcb0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-0001fcc0: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
-0001fcd0: 2020 2020 2020 2020 2020 6c61 7469 7475            latitu
-0001fce0: 6465 3d73 656c 662e 6c6f 6361 7469 6f6e  de=self.location
-0001fcf0: 2e6c 6174 6974 7564 652c 0d0a 2020 2020  .latitude,..    
-0001fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd10: 6c6f 6e67 6974 7564 653d 7365 6c66 2e6c  longitude=self.l
-0001fd20: 6f63 6174 696f 6e2e 6c6f 6e67 6974 7564  ocation.longitud
-0001fd30: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0001fd40: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-0001fd50: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
-0001fd60: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-0001fd70: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
-0001fd80: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
-0001fd90: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
-0001fda0: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
-0001fdb0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001fdc0: 2020 2020 656c 6966 2073 656c 662e 7665      elif self.ve
-0001fdd0: 6e75 653a 0d0a 2020 2020 2020 2020 2020  nue:..          
-0001fde0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0001fdf0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-0001fe00: 7365 6e64 5f76 656e 7565 280d 0a20 2020  send_venue(..   
-0001fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe20: 2063 6861 745f 6964 2c0d 0a20 2020 2020   chat_id,..     
-0001fe30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001fe40: 6174 6974 7564 653d 7365 6c66 2e76 656e  atitude=self.ven
-0001fe50: 7565 2e6c 6f63 6174 696f 6e2e 6c61 7469  ue.location.lati
-0001fe60: 7475 6465 2c0d 0a20 2020 2020 2020 2020  tude,..         
-0001fe70: 2020 2020 2020 2020 2020 206c 6f6e 6769             longi
-0001fe80: 7475 6465 3d73 656c 662e 7665 6e75 652e  tude=self.venue.
-0001fe90: 6c6f 6361 7469 6f6e 2e6c 6f6e 6769 7475  location.longitu
-0001fea0: 6465 2c0d 0a20 2020 2020 2020 2020 2020  de,..           
-0001feb0: 2020 2020 2020 2020 2074 6974 6c65 3d73           title=s
-0001fec0: 656c 662e 7665 6e75 652e 7469 746c 652c  elf.venue.title,
-0001fed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001fee0: 2020 2020 2020 6164 6472 6573 733d 7365        address=se
-0001fef0: 6c66 2e76 656e 7565 2e61 6464 7265 7373  lf.venue.address
-0001ff00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001ff10: 2020 2020 2020 2066 6f75 7273 7175 6172         foursquar
-0001ff20: 655f 6964 3d73 656c 662e 7665 6e75 652e  e_id=self.venue.
-0001ff30: 666f 7572 7371 7561 7265 5f69 642c 0d0a  foursquare_id,..
-0001ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff50: 2020 2020 666f 7572 7371 7561 7265 5f74      foursquare_t
-0001ff60: 7970 653d 7365 6c66 2e76 656e 7565 2e66  ype=self.venue.f
-0001ff70: 6f75 7273 7175 6172 655f 7479 7065 2c0d  oursquare_type,.
-0001ff80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ff90: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
-0001ffa0: 6966 6963 6174 696f 6e3d 6469 7361 626c  ification=disabl
-0001ffb0: 655f 6e6f 7469 6669 6361 7469 6f6e 2c0d  e_notification,.
-0001ffc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ffd0: 2020 2020 2073 6368 6564 756c 655f 6461       schedule_da
-0001ffe0: 7465 3d73 6368 6564 756c 655f 6461 7465  te=schedule_date
-0001fff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020000: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00020010: 2065 6c69 6620 7365 6c66 2e70 6f6c 6c3a   elif self.poll:
-00020020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020030: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-00020040: 656c 662e 5f63 6c69 656e 742e 7365 6e64  elf._client.send
-00020050: 5f70 6f6c 6c28 0d0a 2020 2020 2020 2020  _poll(..        
-00020060: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00020070: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
-00020080: 2020 2020 2020 2020 2020 7175 6573 7469            questi
-00020090: 6f6e 3d73 656c 662e 706f 6c6c 2e71 7565  on=self.poll.que
-000200a0: 7374 696f 6e2c 0d0a 2020 2020 2020 2020  stion,..        
-000200b0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-000200c0: 6f6e 733d 5b6f 7074 2e74 6578 7420 666f  ons=[opt.text fo
-000200d0: 7220 6f70 7420 696e 2073 656c 662e 706f  r opt in self.po
-000200e0: 6c6c 2e6f 7074 696f 6e73 5d2c 0d0a 2020  ll.options],..  
-000200f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020100: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
-00020110: 6361 7469 6f6e 3d64 6973 6162 6c65 5f6e  cation=disable_n
-00020120: 6f74 6966 6963 6174 696f 6e2c 0d0a 2020  otification,..  
-00020130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020140: 2020 7363 6865 6475 6c65 5f64 6174 653d    schedule_date=
-00020150: 7363 6865 6475 6c65 5f64 6174 650d 0a20  schedule_date.. 
-00020160: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00020170: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00020180: 6966 2073 656c 662e 6761 6d65 3a0d 0a20  if self.game:.. 
-00020190: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000201a0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-000201b0: 2e5f 636c 6965 6e74 2e73 656e 645f 6761  ._client.send_ga
-000201c0: 6d65 280d 0a20 2020 2020 2020 2020 2020  me(..           
-000201d0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-000201e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000201f0: 2020 2020 2020 2067 616d 655f 7368 6f72         game_shor
-00020200: 745f 6e61 6d65 3d73 656c 662e 6761 6d65  t_name=self.game
-00020210: 2e73 686f 7274 5f6e 616d 652c 0d0a 2020  .short_name,..  
-00020220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020230: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
-00020240: 6361 7469 6f6e 3d64 6973 6162 6c65 5f6e  cation=disable_n
-00020250: 6f74 6966 6963 6174 696f 6e0d 0a20 2020  otification..   
-00020260: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00020270: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00020280: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00020290: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000202a0: 726f 7228 2255 6e6b 6e6f 776e 206d 6564  ror("Unknown med
-000202b0: 6961 2074 7970 6522 290d 0a0d 0a20 2020  ia type")....   
-000202c0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000202d0: 2e73 7469 636b 6572 206f 7220 7365 6c66  .sticker or self
-000202e0: 2e76 6964 656f 5f6e 6f74 653a 2020 2320  .video_note:  # 
-000202f0: 5374 6963 6b65 7220 616e 6420 5669 6465  Sticker and Vide
-00020300: 6f4e 6f74 6520 7368 6f75 6c64 2068 6176  oNote should hav
-00020310: 6520 6e6f 2063 6170 7469 6f6e 0d0a 2020  e no caption..  
-00020320: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00020330: 7475 726e 2061 7761 6974 2073 656e 645f  turn await send_
-00020340: 6d65 6469 6128 6669 6c65 5f69 643d 6669  media(file_id=fi
-00020350: 6c65 5f69 6429 0d0a 2020 2020 2020 2020  le_id)..        
-00020360: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00020370: 2020 2020 2020 2020 2020 2069 6620 6361             if ca
-00020380: 7074 696f 6e20 6973 204e 6f6e 653a 0d0a  ption is None:..
-00020390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000203a0: 2020 2020 6361 7074 696f 6e20 3d20 7365      caption = se
-000203b0: 6c66 2e63 6170 7469 6f6e 206f 7220 2222  lf.caption or ""
-000203c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000203d0: 2020 2020 2020 6361 7074 696f 6e5f 656e        caption_en
-000203e0: 7469 7469 6573 203d 2073 656c 662e 6361  tities = self.ca
-000203f0: 7074 696f 6e5f 656e 7469 7469 6573 0d0a  ption_entities..
-00020400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020410: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-00020420: 656e 645f 6d65 6469 6128 0d0a 2020 2020  end_media(..    
-00020430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020440: 6669 6c65 5f69 643d 6669 6c65 5f69 642c  file_id=file_id,
-00020450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020460: 2020 2020 2020 6361 7074 696f 6e3d 6361        caption=ca
-00020470: 7074 696f 6e2c 0d0a 2020 2020 2020 2020  ption,..        
-00020480: 2020 2020 2020 2020 2020 2020 7061 7273              pars
-00020490: 655f 6d6f 6465 3d70 6172 7365 5f6d 6f64  e_mode=parse_mod
-000204a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000204b0: 2020 2020 2020 2020 6361 7074 696f 6e5f          caption_
-000204c0: 656e 7469 7469 6573 3d63 6170 7469 6f6e  entities=caption
-000204d0: 5f65 6e74 6974 6965 730d 0a20 2020 2020  _entities..     
-000204e0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-000204f0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00020500: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00020510: 616c 7565 4572 726f 7228 2243 616e 2774  alueError("Can't
-00020520: 2063 6f70 7920 7468 6973 206d 6573 7361   copy this messa
-00020530: 6765 2229 0d0a 0d0a 2020 2020 6173 796e  ge")....    asyn
-00020540: 6320 6465 6620 6465 6c65 7465 2873 656c  c def delete(sel
-00020550: 662c 2072 6576 6f6b 653a 2062 6f6f 6c20  f, revoke: bool 
-00020560: 3d20 5472 7565 293a 0d0a 2020 2020 2020  = True):..      
-00020570: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
-00020580: 6420 2a64 656c 6574 652a 206f 6620 3a6f  d *delete* of :o
-00020590: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
-000205a0: 732e 4d65 7373 6167 6560 2e0d 0a0d 0a20  s.Message`..... 
-000205b0: 2020 2020 2020 2055 7365 2061 7320 6120         Use as a 
-000205c0: 7368 6f72 7463 7574 2066 6f72 3a0d 0a0d  shortcut for:...
-000205d0: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-000205e0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
-000205f0: 0a0d 0a20 2020 2020 2020 2020 2020 2061  ...            a
-00020600: 7761 6974 2063 6c69 656e 742e 6465 6c65  wait client.dele
-00020610: 7465 5f6d 6573 7361 6765 7328 0d0a 2020  te_messages(..  
-00020620: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00020630: 6174 5f69 643d 6368 6174 5f69 642c 0d0a  at_id=chat_id,..
-00020640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020650: 6d65 7373 6167 655f 6964 733d 6d65 7373  message_ids=mess
-00020660: 6167 652e 6964 0d0a 2020 2020 2020 2020  age.id..        
-00020670: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
-00020680: 2045 7861 6d70 6c65 3a0d 0a20 2020 2020   Example:..     
-00020690: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-000206a0: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
-000206b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000206c0: 2061 7761 6974 206d 6573 7361 6765 2e64   await message.d
-000206d0: 656c 6574 6528 290d 0a0d 0a20 2020 2020  elete()....     
-000206e0: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
-000206f0: 2020 2020 2020 2020 2020 2020 7265 766f              revo
-00020700: 6b65 2028 6060 626f 6f6c 6060 2c20 2a6f  ke (``bool``, *o
-00020710: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-00020720: 2020 2020 2020 2020 2020 2020 4465 6c65              Dele
-00020730: 7465 7320 6d65 7373 6167 6573 206f 6e20  tes messages on 
-00020740: 626f 7468 2070 6172 7473 2e0d 0a20 2020  both parts...   
-00020750: 2020 2020 2020 2020 2020 2020 2054 6869               Thi
-00020760: 7320 6973 206f 6e6c 7920 666f 7220 7072  s is only for pr
-00020770: 6976 6174 6520 636c 6f75 6420 6368 6174  ivate cloud chat
-00020780: 7320 616e 6420 6e6f 726d 616c 2067 726f  s and normal gro
-00020790: 7570 732c 206d 6573 7361 6765 7320 6f6e  ups, messages on
-000207a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000207b0: 2020 6368 616e 6e65 6c73 2061 6e64 2073    channels and s
-000207c0: 7570 6572 6772 6f75 7073 2061 7265 2061  upergroups are a
-000207d0: 6c77 6179 7320 7265 766f 6b65 6420 2869  lways revoked (i
-000207e0: 2e65 2e3a 2064 656c 6574 6564 2066 6f72  .e.: deleted for
-000207f0: 2065 7665 7279 6f6e 6529 2e0d 0a20 2020   everyone)...   
-00020800: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00020810: 6175 6c74 7320 746f 2054 7275 652e 0d0a  aults to True...
-00020820: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00020830: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00020840: 5472 7565 206f 6e20 7375 6363 6573 732c  True on success,
-00020850: 2046 616c 7365 206f 7468 6572 7769 7365   False otherwise
-00020860: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
-00020870: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
-00020880: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-00020890: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-000208a0: 6d20 5250 4320 6572 726f 722e 0d0a 2020  m RPC error...  
-000208b0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000208c0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-000208d0: 7365 6c66 2e5f 636c 6965 6e74 2e64 656c  self._client.del
-000208e0: 6574 655f 6d65 7373 6167 6573 280d 0a20  ete_messages(.. 
-000208f0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00020900: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
-00020910: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
-00020920: 7373 6167 655f 6964 733d 7365 6c66 2e69  ssage_ids=self.i
-00020930: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-00020940: 7265 766f 6b65 3d72 6576 6f6b 650d 0a20  revoke=revoke.. 
-00020950: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00020960: 6173 796e 6320 6465 6620 636c 6963 6b28  async def click(
-00020970: 7365 6c66 2c20 783a 2055 6e69 6f6e 5b69  self, x: Union[i
-00020980: 6e74 2c20 7374 725d 203d 2030 2c20 793a  nt, str] = 0, y:
-00020990: 2069 6e74 203d 204e 6f6e 652c 2071 756f   int = None, quo
-000209a0: 7465 3a20 626f 6f6c 203d 204e 6f6e 652c  te: bool = None,
-000209b0: 2074 696d 656f 7574 3a20 696e 7420 3d20   timeout: int = 
-000209c0: 3130 293a 0d0a 2020 2020 2020 2020 2222  10):..        ""
-000209d0: 2242 6f75 6e64 206d 6574 686f 6420 2a63  "Bound method *c
-000209e0: 6c69 636b 2a20 6f66 203a 6f62 6a3a 607e  lick* of :obj:`~
-000209f0: 6669 7070 6572 2e74 7970 6573 2e4d 6573  fipper.types.Mes
-00020a00: 7361 6765 602e 0d0a 0d0a 2020 2020 2020  sage`.....      
-00020a10: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
-00020a20: 6375 7420 666f 7220 636c 6963 6b69 6e67  cut for clicking
-00020a30: 2061 2062 7574 746f 6e20 6174 7461 6368   a button attach
-00020a40: 6564 2074 6f20 7468 6520 6d65 7373 6167  ed to the messag
-00020a50: 6520 696e 7374 6561 6420 6f66 3a0d 0a0d  e instead of:...
-00020a60: 0a20 2020 2020 2020 202d 2043 6c69 636b  .        - Click
-00020a70: 696e 6720 696e 6c69 6e65 2062 7574 746f  ing inline butto
-00020a80: 6e73 3a0d 0a0d 0a20 2020 2020 2020 202e  ns:....        .
-00020a90: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00020aa0: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
-00020ab0: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
-00020ac0: 742e 7265 7175 6573 745f 6361 6c6c 6261  t.request_callba
-00020ad0: 636b 5f61 6e73 7765 7228 0d0a 2020 2020  ck_answer(..    
-00020ae0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00020af0: 5f69 643d 6d65 7373 6167 652e 6368 6174  _id=message.chat
-00020b00: 2e69 642c 0d0a 2020 2020 2020 2020 2020  .id,..          
-00020b10: 2020 2020 2020 6d65 7373 6167 655f 6964        message_id
-00020b20: 3d6d 6573 7361 6765 2e69 642c 0d0a 2020  =message.id,..  
-00020b30: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00020b40: 6c6c 6261 636b 5f64 6174 613d 6d65 7373  llback_data=mess
-00020b50: 6167 652e 7265 706c 795f 6d61 726b 7570  age.reply_markup
-00020b60: 5b69 5d5b 6a5d 2e63 616c 6c62 6163 6b5f  [i][j].callback_
-00020b70: 6461 7461 0d0a 2020 2020 2020 2020 2020  data..          
-00020b80: 2020 290d 0a0d 0a20 2020 2020 2020 202d    )....        -
-00020b90: 2043 6c69 636b 696e 6720 6e6f 726d 616c   Clicking normal
-00020ba0: 2062 7574 746f 6e73 3a0d 0a0d 0a20 2020   buttons:....   
-00020bb0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-00020bc0: 636b 3a3a 2070 7974 686f 6e0d 0a0d 0a20  ck:: python.... 
-00020bd0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00020be0: 2063 6c69 656e 742e 7365 6e64 5f6d 6573   client.send_mes
-00020bf0: 7361 6765 280d 0a20 2020 2020 2020 2020  sage(..         
-00020c00: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
-00020c10: 6573 7361 6765 2e63 6861 742e 6964 2c0d  essage.chat.id,.
-00020c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020c30: 2074 6578 743d 6d65 7373 6167 652e 7265   text=message.re
-00020c40: 706c 795f 6d61 726b 7570 5b69 5d5b 6a5d  ply_markup[i][j]
-00020c50: 2e74 6578 740d 0a20 2020 2020 2020 2020  .text..         
-00020c60: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
-00020c70: 4578 616d 706c 653a 0d0a 2020 2020 2020  Example:..      
-00020c80: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
-00020c90: 6420 6361 6e20 6265 2075 7365 6420 696e  d can be used in
-00020ca0: 2074 6872 6565 2064 6966 6665 7265 6e74   three different
-00020cb0: 2077 6179 733a 0d0a 0d0a 2020 2020 2020   ways:....      
-00020cc0: 2020 2020 2020 312e 2020 5061 7373 206f        1.  Pass o
-00020cd0: 6e65 2069 6e74 6567 6572 2061 7267 756d  ne integer argum
-00020ce0: 656e 7420 6f6e 6c79 2028 652e 672e 3a20  ent only (e.g.: 
-00020cf0: 6060 2e63 6c69 636b 2832 2960 602c 2074  ``.click(2)``, t
-00020d00: 6f20 636c 6963 6b20 6120 6275 7474 6f6e  o click a button
-00020d10: 2061 7420 696e 6465 7820 3229 2e0d 0a20   at index 2)... 
-00020d20: 2020 2020 2020 2020 2020 2020 2020 2042                 B
-00020d30: 7574 746f 6e73 2061 7265 2063 6f75 6e74  uttons are count
-00020d40: 6564 206c 6566 7420 746f 2072 6967 6874  ed left to right
-00020d50: 2c20 7374 6172 7469 6e67 2066 726f 6d20  , starting from 
-00020d60: 7468 6520 746f 702e 0d0a 0d0a 2020 2020  the top.....    
-00020d70: 2020 2020 2020 2020 322e 2020 5061 7373          2.  Pass
-00020d80: 2074 776f 2069 6e74 6567 6572 2061 7267   two integer arg
-00020d90: 756d 656e 7473 2028 652e 672e 3a20 6060  uments (e.g.: ``
-00020da0: 2e63 6c69 636b 2831 2c20 3029 6060 2c20  .click(1, 0)``, 
-00020db0: 746f 2063 6c69 636b 2061 2062 7574 746f  to click a butto
-00020dc0: 6e20 6174 2070 6f73 6974 696f 6e20 2831  n at position (1
-00020dd0: 2c20 3029 292e 0d0a 2020 2020 2020 2020  , 0))...        
-00020de0: 2020 2020 2020 2020 5468 6520 6f72 6967          The orig
-00020df0: 696e 2028 302c 2030 2920 6973 2074 6f70  in (0, 0) is top
-00020e00: 2d6c 6566 742e 0d0a 0d0a 2020 2020 2020  -left.....      
-00020e10: 2020 2020 2020 332e 2020 5061 7373 206f        3.  Pass o
-00020e20: 6e65 2073 7472 696e 6720 6172 6775 6d65  ne string argume
-00020e30: 6e74 206f 6e6c 7920 2865 2e67 2e3a 2060  nt only (e.g.: `
-00020e40: 602e 636c 6963 6b28 2253 6574 7469 6e67  `.click("Setting
-00020e50: 7322 2960 602c 2074 6f20 636c 6963 6b20  s")``, to click 
-00020e60: 6120 6275 7474 6f6e 2062 7920 7573 696e  a button by usin
-00020e70: 6720 6974 7320 6c61 6265 6c29 2e0d 0a20  g its label)... 
-00020e80: 2020 2020 2020 2020 2020 2020 2020 204f                 O
-00020e90: 6e6c 7920 7468 6520 6669 7273 7420 6d61  nly the first ma
-00020ea0: 7463 6869 6e67 2062 7574 746f 6e20 7769  tching button wi
-00020eb0: 6c6c 2062 6520 7072 6573 7365 642e 0d0a  ll be pressed...
-00020ec0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00020ed0: 7465 7273 3a0d 0a20 2020 2020 2020 2020  ters:..         
-00020ee0: 2020 2078 2028 6060 696e 7460 6020 7c20     x (``int`` | 
-00020ef0: 6060 7374 7260 6029 3a0d 0a20 2020 2020  ``str``):..     
-00020f00: 2020 2020 2020 2020 2020 2055 7365 6420             Used 
-00020f10: 6173 2069 6e74 6567 6572 2069 6e64 6578  as integer index
-00020f20: 2c20 696e 7465 6765 7220 6162 7363 6973  , integer abscis
-00020f30: 7361 2028 696e 2070 6169 7220 7769 7468  sa (in pair with
-00020f40: 2079 2920 6f72 2061 7320 7374 7269 6e67   y) or as string
-00020f50: 206c 6162 656c 2e0d 0a20 2020 2020 2020   label...       
-00020f60: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00020f70: 7320 746f 2030 2028 6669 7273 7420 6275  s to 0 (first bu
-00020f80: 7474 6f6e 292e 0d0a 0d0a 2020 2020 2020  tton).....      
-00020f90: 2020 2020 2020 7920 2860 6069 6e74 6060        y (``int``
-00020fa0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
-00020fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020fc0: 5573 6564 2061 7320 6f72 6469 6e61 7465  Used as ordinate
-00020fd0: 206f 6e6c 7920 2869 6e20 7061 6972 2077   only (in pair w
-00020fe0: 6974 6820 7829 2e0d 0a0d 0a20 2020 2020  ith x).....     
-00020ff0: 2020 2020 2020 2071 756f 7465 2028 6060         quote (``
-00021000: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
-00021010: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
-00021020: 2020 2020 2020 5573 6566 756c 2066 6f72        Useful for
-00021030: 206e 6f72 6d61 6c20 6275 7474 6f6e 7320   normal buttons 
-00021040: 6f6e 6c79 2c20 7768 6572 6520 7072 6573  only, where pres
-00021050: 7369 6e67 2069 7420 7769 6c6c 2072 6573  sing it will res
-00021060: 756c 7420 696e 2061 206e 6577 206d 6573  ult in a new mes
-00021070: 7361 6765 2073 656e 742e 0d0a 2020 2020  sage sent...    
-00021080: 2020 2020 2020 2020 2020 2020 4966 2060              If `
-00021090: 6054 7275 6560 602c 2074 6865 206d 6573  `True``, the mes
-000210a0: 7361 6765 2077 696c 6c20 6265 2073 656e  sage will be sen
-000210b0: 7420 6173 2061 2072 6570 6c79 2074 6f20  t as a reply to 
-000210c0: 7468 6973 206d 6573 7361 6765 2e0d 0a20  this message... 
-000210d0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-000210e0: 6566 6175 6c74 7320 746f 2060 6054 7275  efaults to ``Tru
-000210f0: 6560 6020 696e 2067 726f 7570 2063 6861  e`` in group cha
-00021100: 7473 2061 6e64 2060 6046 616c 7365 6060  ts and ``False``
-00021110: 2069 6e20 7072 6976 6174 6520 6368 6174   in private chat
-00021120: 732e 0d0a 0d0a 2020 2020 2020 2020 2020  s.....          
-00021130: 2020 7469 6d65 6f75 7420 2860 6069 6e74    timeout (``int
-00021140: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-00021150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021160: 2020 5469 6d65 6f75 7420 696e 2073 6563    Timeout in sec
-00021170: 6f6e 6473 2e0d 0a0d 0a20 2020 2020 2020  onds.....       
-00021180: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-00021190: 2020 2020 2020 202d 2020 2054 6865 2072         -   The r
-000211a0: 6573 756c 7420 6f66 203a 6d65 7468 3a60  esult of :meth:`
-000211b0: 7e66 6970 7065 722e 436c 6965 6e74 2e72  ~fipper.Client.r
-000211c0: 6571 7565 7374 5f63 616c 6c62 6163 6b5f  equest_callback_
-000211d0: 616e 7377 6572 6020 696e 2063 6173 6520  answer` in case 
-000211e0: 6f66 2069 6e6c 696e 6520 6361 6c6c 6261  of inline callba
-000211f0: 636b 2062 7574 746f 6e20 636c 6963 6b73  ck button clicks
-00021200: 2e0d 0a20 2020 2020 2020 2020 2020 202d  ...            -
-00021210: 2020 2054 6865 2072 6573 756c 7420 6f66     The result of
-00021220: 203a 6d65 7468 3a60 7e4d 6573 7361 6765   :meth:`~Message
-00021230: 2e72 6570 6c79 2829 6020 696e 2063 6173  .reply()` in cas
-00021240: 6520 6f66 206e 6f72 6d61 6c20 6275 7474  e of normal butt
-00021250: 6f6e 2063 6c69 636b 732e 0d0a 2020 2020  on clicks...    
-00021260: 2020 2020 2020 2020 2d20 2020 4120 7374          -   A st
-00021270: 7269 6e67 2069 6e20 6361 7365 2074 6865  ring in case the
-00021280: 2069 6e6c 696e 6520 6275 7474 6f6e 2069   inline button i
-00021290: 7320 6120 5552 4c2c 2061 202a 7377 6974  s a URL, a *swit
-000212a0: 6368 5f69 6e6c 696e 655f 7175 6572 792a  ch_inline_query*
-000212b0: 206f 7220 610d 0a20 2020 2020 2020 2020   or a..         
-000212c0: 2020 2020 2020 202a 7377 6974 6368 5f69         *switch_i
-000212d0: 6e6c 696e 655f 7175 6572 795f 6375 7272  nline_query_curr
-000212e0: 656e 745f 6368 6174 2a20 6275 7474 6f6e  ent_chat* button
-000212f0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
-00021300: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
-00021310: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-00021320: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-00021330: 6d20 5250 4320 6572 726f 722e 0d0a 2020  m RPC error...  
-00021340: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
-00021350: 7272 6f72 3a20 496e 2063 6173 6520 7468  rror: In case th
-00021360: 6520 7072 6f76 6964 6564 2069 6e64 6578  e provided index
-00021370: 206f 7220 706f 7369 7469 6f6e 2069 7320   or position is 
-00021380: 6f75 7420 6f66 2072 616e 6765 206f 7220  out of range or 
-00021390: 7468 6520 6275 7474 6f6e 206c 6162 656c  the button label
-000213a0: 2077 6173 206e 6f74 2066 6f75 6e64 2e0d   was not found..
-000213b0: 0a20 2020 2020 2020 2020 2020 2054 696d  .            Tim
-000213c0: 656f 7574 4572 726f 723a 2049 6e20 6361  eoutError: In ca
-000213d0: 7365 2c20 6166 7465 7220 636c 6963 6b69  se, after clicki
-000213e0: 6e67 2061 6e20 696e 6c69 6e65 2062 7574  ng an inline but
-000213f0: 746f 6e2c 2074 6865 2062 6f74 2066 6169  ton, the bot fai
-00021400: 6c73 2074 6f20 616e 7377 6572 2077 6974  ls to answer wit
-00021410: 6869 6e20 7468 6520 7469 6d65 6f75 742e  hin the timeout.
-00021420: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-00021430: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00021440: 7374 616e 6365 2873 656c 662e 7265 706c  stance(self.repl
-00021450: 795f 6d61 726b 7570 2c20 7479 7065 732e  y_markup, types.
-00021460: 5265 706c 794b 6579 626f 6172 644d 6172  ReplyKeyboardMar
-00021470: 6b75 7029 3a0d 0a20 2020 2020 2020 2020  kup):..         
-00021480: 2020 206b 6579 626f 6172 6420 3d20 7365     keyboard = se
-00021490: 6c66 2e72 6570 6c79 5f6d 6172 6b75 702e  lf.reply_markup.
-000214a0: 6b65 7962 6f61 7264 0d0a 2020 2020 2020  keyboard..      
-000214b0: 2020 2020 2020 6973 5f69 6e6c 696e 6520        is_inline 
-000214c0: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-000214d0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-000214e0: 2873 656c 662e 7265 706c 795f 6d61 726b  (self.reply_mark
-000214f0: 7570 2c20 7479 7065 732e 496e 6c69 6e65  up, types.Inline
-00021500: 4b65 7962 6f61 7264 4d61 726b 7570 293a  KeyboardMarkup):
-00021510: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
-00021520: 7962 6f61 7264 203d 2073 656c 662e 7265  yboard = self.re
-00021530: 706c 795f 6d61 726b 7570 2e69 6e6c 696e  ply_markup.inlin
-00021540: 655f 6b65 7962 6f61 7264 0d0a 2020 2020  e_keyboard..    
-00021550: 2020 2020 2020 2020 6973 5f69 6e6c 696e          is_inlin
-00021560: 6520 3d20 5472 7565 0d0a 2020 2020 2020  e = True..      
-00021570: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00021580: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00021590: 4572 726f 7228 2254 6865 206d 6573 7361  Error("The messa
-000215a0: 6765 2064 6f65 736e 2774 2063 6f6e 7461  ge doesn't conta
-000215b0: 696e 2061 6e79 206b 6579 626f 6172 6422  in any keyboard"
-000215c0: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-000215d0: 6973 696e 7374 616e 6365 2878 2c20 696e  isinstance(x, in
-000215e0: 7429 2061 6e64 2079 2069 7320 4e6f 6e65  t) and y is None
-000215f0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00021600: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00021610: 2020 2020 2062 7574 746f 6e20 3d20 5b0d       button = [.
-00021620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021630: 2020 2020 2062 7574 746f 6e0d 0a20 2020       button..   
-00021640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021650: 2066 6f72 2072 6f77 2069 6e20 6b65 7962   for row in keyb
-00021660: 6f61 7264 0d0a 2020 2020 2020 2020 2020  oard..          
-00021670: 2020 2020 2020 2020 2020 666f 7220 6275            for bu
-00021680: 7474 6f6e 2069 6e20 726f 770d 0a20 2020  tton in row..   
-00021690: 2020 2020 2020 2020 2020 2020 205d 5b78               ][x
-000216a0: 5d0d 0a20 2020 2020 2020 2020 2020 2065  ]..            e
-000216b0: 7863 6570 7420 496e 6465 7845 7272 6f72  xcept IndexError
-000216c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000216d0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000216e0: 726f 7228 6622 5468 6520 6275 7474 6f6e  ror(f"The button
-000216f0: 2061 7420 696e 6465 7820 7b78 7d20 646f   at index {x} do
-00021700: 6573 6e27 7420 6578 6973 7422 290d 0a20  esn't exist").. 
-00021710: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00021720: 7374 616e 6365 2878 2c20 696e 7429 2061  stance(x, int) a
-00021730: 6e64 2069 7369 6e73 7461 6e63 6528 792c  nd isinstance(y,
-00021740: 2069 6e74 293a 0d0a 2020 2020 2020 2020   int):..        
-00021750: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00021760: 2020 2020 2020 2020 2020 6275 7474 6f6e            button
-00021770: 203d 206b 6579 626f 6172 645b 795d 5b78   = keyboard[y][x
-00021780: 5d0d 0a20 2020 2020 2020 2020 2020 2065  ]..            e
-00021790: 7863 6570 7420 496e 6465 7845 7272 6f72  xcept IndexError
-000217a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000217b0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000217c0: 726f 7228 6622 5468 6520 6275 7474 6f6e  ror(f"The button
-000217d0: 2061 7420 706f 7369 7469 6f6e 2028 7b78   at position ({x
-000217e0: 7d2c 207b 797d 2920 646f 6573 6e27 7420  }, {y}) doesn't 
-000217f0: 6578 6973 7422 290d 0a20 2020 2020 2020  exist")..       
-00021800: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00021810: 2878 2c20 7374 7229 2061 6e64 2079 2069  (x, str) and y i
-00021820: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00021830: 2020 2020 206c 6162 656c 203d 2078 2e65       label = x.e
-00021840: 6e63 6f64 6528 2275 7466 2d31 3622 2c20  ncode("utf-16", 
-00021850: 2273 7572 726f 6761 7465 7061 7373 2229  "surrogatepass")
-00021860: 2e64 6563 6f64 6528 2275 7466 2d31 3622  .decode("utf-16"
-00021870: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00021880: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00021890: 2020 2020 2020 2062 7574 746f 6e20 3d20         button = 
-000218a0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-000218b0: 2020 2020 2020 2062 7574 746f 6e0d 0a20         button.. 
-000218c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000218d0: 2020 2066 6f72 2072 6f77 2069 6e20 6b65     for row in ke
-000218e0: 7962 6f61 7264 0d0a 2020 2020 2020 2020  yboard..        
-000218f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00021900: 6275 7474 6f6e 2069 6e20 726f 770d 0a20  button in row.. 
-00021910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021920: 2020 2069 6620 6c61 6265 6c20 3d3d 2062     if label == b
-00021930: 7574 746f 6e2e 7465 7874 0d0a 2020 2020  utton.text..    
-00021940: 2020 2020 2020 2020 2020 2020 5d5b 305d              ][0]
-00021950: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00021960: 6365 7074 2049 6e64 6578 4572 726f 723a  cept IndexError:
-00021970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021980: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00021990: 6f72 2866 2254 6865 2062 7574 746f 6e20  or(f"The button 
-000219a0: 7769 7468 206c 6162 656c 2027 7b78 7d27  with label '{x}'
-000219b0: 2064 6f65 736e 2774 2065 7869 7374 7322   doesn't exists"
-000219c0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-000219d0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000219e0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-000219f0: 496e 7661 6c69 6420 6172 6775 6d65 6e74  Invalid argument
-00021a00: 7322 290d 0a0d 0a20 2020 2020 2020 2069  s")....        i
-00021a10: 6620 6973 5f69 6e6c 696e 653a 0d0a 2020  f is_inline:..  
-00021a20: 2020 2020 2020 2020 2020 6966 2062 7574            if but
-00021a30: 746f 6e2e 6361 6c6c 6261 636b 5f64 6174  ton.callback_dat
-00021a40: 613a 0d0a 2020 2020 2020 2020 2020 2020  a:..            
-00021a50: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00021a60: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
-00021a70: 7175 6573 745f 6361 6c6c 6261 636b 5f61  quest_callback_a
-00021a80: 6e73 7765 7228 0d0a 2020 2020 2020 2020  nswer(..        
-00021a90: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00021aa0: 5f69 643d 7365 6c66 2e63 6861 742e 6964  _id=self.chat.id
-00021ab0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00021ac0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-00021ad0: 643d 7365 6c66 2e69 642c 0d0a 2020 2020  d=self.id,..    
-00021ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021af0: 6361 6c6c 6261 636b 5f64 6174 613d 6275  callback_data=bu
-00021b00: 7474 6f6e 2e63 616c 6c62 6163 6b5f 6461  tton.callback_da
-00021b10: 7461 2c0d 0a20 2020 2020 2020 2020 2020  ta,..           
-00021b20: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-00021b30: 3d74 696d 656f 7574 0d0a 2020 2020 2020  =timeout..      
-00021b40: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00021b50: 2020 2020 2020 2020 2065 6c69 6620 6275           elif bu
-00021b60: 7474 6f6e 2e75 726c 3a0d 0a20 2020 2020  tton.url:..     
-00021b70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00021b80: 6e20 6275 7474 6f6e 2e75 726c 0d0a 2020  n button.url..  
-00021b90: 2020 2020 2020 2020 2020 656c 6966 2062            elif b
-00021ba0: 7574 746f 6e2e 7377 6974 6368 5f69 6e6c  utton.switch_inl
-00021bb0: 696e 655f 7175 6572 793a 0d0a 2020 2020  ine_query:..    
-00021bc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00021bd0: 726e 2062 7574 746f 6e2e 7377 6974 6368  rn button.switch
-00021be0: 5f69 6e6c 696e 655f 7175 6572 790d 0a20  _inline_query.. 
-00021bf0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00021c00: 6275 7474 6f6e 2e73 7769 7463 685f 696e  button.switch_in
-00021c10: 6c69 6e65 5f71 7565 7279 5f63 7572 7265  line_query_curre
-00021c20: 6e74 5f63 6861 743a 0d0a 2020 2020 2020  nt_chat:..      
-00021c30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00021c40: 2062 7574 746f 6e2e 7377 6974 6368 5f69   button.switch_i
-00021c50: 6e6c 696e 655f 7175 6572 795f 6375 7272  nline_query_curr
-00021c60: 656e 745f 6368 6174 0d0a 2020 2020 2020  ent_chat..      
-00021c70: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00021c80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00021c90: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
-00021ca0: 6869 7320 6275 7474 6f6e 2069 7320 6e6f  his button is no
-00021cb0: 7420 7375 7070 6f72 7465 6420 7965 7422  t supported yet"
-00021cc0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00021cd0: 0d0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
-00021ce0: 6169 7420 7365 6c66 2e72 6570 6c79 2862  ait self.reply(b
-00021cf0: 7574 746f 6e2c 2071 756f 7465 3d71 756f  utton, quote=quo
-00021d00: 7465 290d 0a0d 0a20 2020 2061 7379 6e63  te)....    async
-00021d10: 2064 6566 2072 6561 6374 2873 656c 662c   def react(self,
-00021d20: 2065 6d6f 6a69 3a20 7374 7220 3d20 2222   emoji: str = ""
-00021d30: 2c20 6269 673a 2062 6f6f 6c20 3d20 4661  , big: bool = Fa
-00021d40: 6c73 6529 202d 3e20 626f 6f6c 3a0d 0a20  lse) -> bool:.. 
-00021d50: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
-00021d60: 6d65 7468 6f64 202a 7265 6163 742a 206f  method *react* o
-00021d70: 6620 3a6f 626a 3a60 7e66 6970 7065 722e  f :obj:`~fipper.
-00021d80: 7479 7065 732e 4d65 7373 6167 6560 2e0d  types.Message`..
-00021d90: 0a0d 0a20 2020 2020 2020 2055 7365 2061  ...        Use a
-00021da0: 7320 6120 7368 6f72 7463 7574 2066 6f72  s a shortcut for
-00021db0: 3a0d 0a0d 0a20 2020 2020 2020 202e 2e20  :....        .. 
-00021dc0: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
-00021dd0: 686f 6e0d 0a0d 0a20 2020 2020 2020 2020  hon....         
-00021de0: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
-00021df0: 7365 6e64 5f72 6561 6374 696f 6e28 0d0a  send_reaction(..
-00021e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e10: 6368 6174 5f69 643d 6368 6174 5f69 642c  chat_id=chat_id,
-00021e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021e30: 2020 6d65 7373 6167 655f 6964 3d6d 6573    message_id=mes
-00021e40: 7361 6765 2e69 642c 0d0a 2020 2020 2020  sage.id,..      
-00021e50: 2020 2020 2020 2020 2020 656d 6f6a 693d            emoji=
-00021e60: 22f0 9f94 a522 0d0a 2020 2020 2020 2020  "...."..        
-00021e70: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
-00021e80: 2045 7861 6d70 6c65 3a0d 0a20 2020 2020   Example:..     
-00021e90: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-00021ea0: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
-00021eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021ec0: 2061 7761 6974 206d 6573 7361 6765 2e72   await message.r
-00021ed0: 6561 6374 2865 6d6f 6a69 3d22 f09f 94a5  eact(emoji="....
-00021ee0: 2229 0d0a 0d0a 2020 2020 2020 2020 5061  ")....        Pa
-00021ef0: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
-00021f00: 2020 2020 2020 2065 6d6f 6a69 2028 6060         emoji (``
-00021f10: 7374 7260 602c 202a 6f70 7469 6f6e 616c  str``, *optional
-00021f20: 2a29 3a0d 0a20 2020 2020 2020 2020 2020  *):..           
-00021f30: 2020 2020 2052 6561 6374 696f 6e20 656d       Reaction em
-00021f40: 6f6a 692e 0d0a 2020 2020 2020 2020 2020  oji...          
-00021f50: 2020 2020 2020 5061 7373 2022 2220 6173        Pass "" as
-00021f60: 2065 6d6f 6a69 2028 6465 6661 756c 7429   emoji (default)
-00021f70: 2074 6f20 7265 7472 6163 7420 7468 6520   to retract the 
-00021f80: 7265 6163 7469 6f6e 2e0d 0a20 2020 2020  reaction...     
-00021f90: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00021fa0: 2020 2020 2020 6269 6720 2860 6062 6f6f        big (``boo
-00021fb0: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
-00021fc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00021fd0: 2020 2050 6173 7320 5472 7565 2074 6f20     Pass True to 
-00021fe0: 7368 6f77 2061 2062 6967 6765 7220 616e  show a bigger an
-00021ff0: 6420 6c6f 6e67 6572 2072 6561 6374 696f  d longer reactio
-00022000: 6e2e 0d0a 2020 2020 2020 2020 2020 2020  n...            
-00022010: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00022020: 4661 6c73 652e 0d0a 0d0a 2020 2020 2020  False.....      
-00022030: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00022040: 2020 2020 2020 2020 6060 626f 6f6c 6060          ``bool``
-00022050: 3a20 4f6e 2073 7563 6365 7373 2c20 5472  : On success, Tr
-00022060: 7565 2069 7320 7265 7475 726e 6564 2e0d  ue is returned..
-00022070: 0a0d 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00022080: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00022090: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
-000220a0: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
-000220b0: 5250 4320 6572 726f 722e 0d0a 2020 2020  RPC error...    
-000220c0: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
-000220d0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-000220e0: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
-000220f0: 645f 7265 6163 7469 6f6e 280d 0a20 2020  d_reaction(..   
-00022100: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00022110: 3d73 656c 662e 6368 6174 2e69 642c 0d0a  =self.chat.id,..
-00022120: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00022130: 6167 655f 6964 3d73 656c 662e 6964 2c0d  age_id=self.id,.
-00022140: 0a20 2020 2020 2020 2020 2020 2065 6d6f  .            emo
-00022150: 6a69 3d65 6d6f 6a69 2c0d 0a20 2020 2020  ji=emoji,..     
-00022160: 2020 2020 2020 2062 6967 3d62 6967 0d0a         big=big..
-00022170: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00022180: 2061 7379 6e63 2064 6566 2072 6574 7261   async def retra
-00022190: 6374 5f76 6f74 6528 0d0a 2020 2020 2020  ct_vote(..      
-000221a0: 2020 7365 6c66 2c0d 0a20 2020 2029 202d    self,..    ) -
-000221b0: 3e20 2274 7970 6573 2e50 6f6c 6c22 3a0d  > "types.Poll":.
-000221c0: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
-000221d0: 6420 6d65 7468 6f64 202a 7265 7472 6163  d method *retrac
-000221e0: 745f 766f 7465 2a20 6f66 203a 6f62 6a3a  t_vote* of :obj:
-000221f0: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
-00022200: 6573 7361 6765 602e 0d0a 0d0a 2020 2020  essage`.....    
-00022210: 2020 2020 5573 6520 6173 2061 2073 686f      Use as a sho
-00022220: 7274 6375 7420 666f 723a 0d0a 0d0a 2020  rtcut for:....  
-00022230: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-00022240: 6f63 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a  ock:: python....
-00022250: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00022260: 6e74 2e72 6574 7261 6374 5f76 6f74 6528  nt.retract_vote(
-00022270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00022280: 2020 6368 6174 5f69 643d 6d65 7373 6167    chat_id=messag
-00022290: 652e 6368 6174 2e69 642c 0d0a 2020 2020  e.chat.id,..    
-000222a0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-000222b0: 6167 655f 6964 3d6d 6573 7361 6765 5f69  age_id=message_i
-000222c0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-000222d0: 290d 0a0d 0a20 2020 2020 2020 2045 7861  )....        Exa
-000222e0: 6d70 6c65 3a0d 0a20 2020 2020 2020 2020  mple:..         
-000222f0: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-00022300: 3a3a 2070 7974 686f 6e0d 0a0d 0a20 2020  :: python....   
-00022310: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00022320: 7361 6765 2e72 6574 7261 6374 5f76 6f74  sage.retract_vot
-00022330: 6528 290d 0a0d 0a20 2020 2020 2020 2052  e()....        R
-00022340: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00022350: 2020 2020 203a 6f62 6a3a 607e 6669 7070       :obj:`~fipp
-00022360: 6572 2e74 7970 6573 2e50 6f6c 6c60 3a20  er.types.Poll`: 
-00022370: 4f6e 2073 7563 6365 7373 2c20 7468 6520  On success, the 
-00022380: 706f 6c6c 2077 6974 6820 7468 6520 7265  poll with the re
-00022390: 7472 6163 7465 6420 766f 7465 2069 7320  tracted vote is 
-000223a0: 7265 7475 726e 6564 2e0d 0a0d 0a20 2020  returned.....   
-000223b0: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
-000223c0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
-000223d0: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
-000223e0: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
-000223f0: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
-00022400: 220d 0a0d 0a20 2020 2020 2020 2072 6574  "....        ret
-00022410: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-00022420: 636c 6965 6e74 2e72 6574 7261 6374 5f76  client.retract_v
-00022430: 6f74 6528 0d0a 2020 2020 2020 2020 2020  ote(..          
-00022440: 2020 6368 6174 5f69 643d 7365 6c66 2e63    chat_id=self.c
-00022450: 6861 742e 6964 2c0d 0a20 2020 2020 2020  hat.id,..       
-00022460: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
-00022470: 7365 6c66 2e69 640d 0a20 2020 2020 2020  self.id..       
-00022480: 2029 0d0a 0d0a 2020 2020 6173 796e 6320   )....    async 
-00022490: 6465 6620 646f 776e 6c6f 6164 280d 0a20  def download(.. 
-000224a0: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-000224b0: 2020 2020 2020 6669 6c65 5f6e 616d 653a        file_name:
-000224c0: 2073 7472 203d 2022 222c 0d0a 2020 2020   str = "",..    
-000224d0: 2020 2020 696e 5f6d 656d 6f72 793a 2062      in_memory: b
-000224e0: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
-000224f0: 2020 2020 2020 626c 6f63 6b3a 2062 6f6f        block: boo
-00022500: 6c20 3d20 5472 7565 2c0d 0a20 2020 2020  l = True,..     
-00022510: 2020 2070 726f 6772 6573 733a 2043 616c     progress: Cal
-00022520: 6c61 626c 6520 3d20 4e6f 6e65 2c0d 0a20  lable = None,.. 
-00022530: 2020 2020 2020 2070 726f 6772 6573 735f         progress_
-00022540: 6172 6773 3a20 7475 706c 6520 3d20 2829  args: tuple = ()
-00022550: 0d0a 2020 2020 2920 2d3e 2073 7472 3a0d  ..    ) -> str:.
-00022560: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
-00022570: 6420 6d65 7468 6f64 202a 646f 776e 6c6f  d method *downlo
-00022580: 6164 2a20 6f66 203a 6f62 6a3a 607e 6669  ad* of :obj:`~fi
-00022590: 7070 6572 2e74 7970 6573 2e4d 6573 7361  pper.types.Messa
-000225a0: 6765 602e 0d0a 0d0a 2020 2020 2020 2020  ge`.....        
-000225b0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
-000225c0: 7420 666f 723a 0d0a 0d0a 2020 2020 2020  t for:....      
-000225d0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-000225e0: 3a20 7079 7468 6f6e 0d0a 0d0a 2020 2020  : python....    
-000225f0: 2020 2020 2020 2020 6177 6169 7420 636c          await cl
-00022600: 6965 6e74 2e64 6f77 6e6c 6f61 645f 6d65  ient.download_me
-00022610: 6469 6128 6d65 7373 6167 6529 0d0a 0d0a  dia(message)....
-00022620: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-00022630: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-00022640: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00022650: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
-00022660: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
-00022670: 7373 6167 652e 646f 776e 6c6f 6164 2829  ssage.download()
-00022680: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-00022690: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
-000226a0: 2020 2020 2066 696c 655f 6e61 6d65 2028       file_name (
-000226b0: 6060 7374 7260 602c 202a 6f70 7469 6f6e  ``str``, *option
-000226c0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
-000226d0: 2020 2020 2020 2041 2063 7573 746f 6d20         A custom 
-000226e0: 2a66 696c 655f 6e61 6d65 2a20 746f 2062  *file_name* to b
-000226f0: 6520 7573 6564 2069 6e73 7465 6164 206f  e used instead o
-00022700: 6620 7468 6520 6f6e 6520 7072 6f76 6964  f the one provid
-00022710: 6564 2062 7920 5465 6c65 6772 616d 2e0d  ed by Telegram..
-00022720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022730: 2042 7920 6465 6661 756c 742c 2061 6c6c   By default, all
-00022740: 2066 696c 6573 2061 7265 2064 6f77 6e6c   files are downl
-00022750: 6f61 6465 6420 696e 2074 6865 202a 646f  oaded in the *do
-00022760: 776e 6c6f 6164 732a 2066 6f6c 6465 7220  wnloads* folder 
-00022770: 696e 2079 6f75 7220 776f 726b 696e 6720  in your working 
-00022780: 6469 7265 6374 6f72 792e 0d0a 2020 2020  directory...    
-00022790: 2020 2020 2020 2020 2020 2020 596f 7520              You 
-000227a0: 6361 6e20 616c 736f 2073 7065 6369 6679  can also specify
-000227b0: 2061 2070 6174 6820 666f 7220 646f 776e   a path for down
-000227c0: 6c6f 6164 696e 6720 6669 6c65 7320 696e  loading files in
-000227d0: 2061 2063 7573 746f 6d20 6c6f 6361 7469   a custom locati
-000227e0: 6f6e 3a20 7061 7468 7320 7468 6174 2065  on: paths that e
-000227f0: 6e64 2077 6974 6820 222f 220d 0a20 2020  nd with "/"..   
-00022800: 2020 2020 2020 2020 2020 2020 2061 7265               are
-00022810: 2063 6f6e 7369 6465 7265 6420 6469 7265   considered dire
-00022820: 6374 6f72 6965 732e 2041 6c6c 206e 6f6e  ctories. All non
-00022830: 2d65 7869 7374 656e 7420 666f 6c64 6572  -existent folder
-00022840: 7320 7769 6c6c 2062 6520 6372 6561 7465  s will be create
-00022850: 6420 6175 746f 6d61 7469 6361 6c6c 792e  d automatically.
-00022860: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00022870: 696e 5f6d 656d 6f72 7920 2860 6062 6f6f  in_memory (``boo
-00022880: 6c60 602c 202a 6f70 7469 6f6e 616c 2a29  l``, *optional*)
-00022890: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000228a0: 2020 2050 6173 7320 5472 7565 2074 6f20     Pass True to 
-000228b0: 646f 776e 6c6f 6164 2074 6865 206d 6564  download the med
-000228c0: 6961 2069 6e2d 6d65 6d6f 7279 2e0d 0a20  ia in-memory... 
-000228d0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-000228e0: 2062 696e 6172 7920 6669 6c65 2d6c 696b   binary file-lik
-000228f0: 6520 6f62 6a65 6374 2077 6974 6820 6974  e object with it
-00022900: 7320 6174 7472 6962 7574 6520 222e 6e61  s attribute ".na
-00022910: 6d65 2220 7365 7420 7769 6c6c 2062 6520  me" set will be 
-00022920: 7265 7475 726e 6564 2e0d 0a20 2020 2020  returned...     
-00022930: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00022940: 6c74 7320 746f 2046 616c 7365 2e0d 0a0d  lts to False....
-00022950: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
-00022960: 636b 2028 6060 626f 6f6c 6060 2c20 2a6f  ck (``bool``, *o
-00022970: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-00022980: 2020 2020 2020 2020 2020 2020 426c 6f63              Bloc
-00022990: 6b73 2074 6865 2063 6f64 6520 6578 6563  ks the code exec
-000229a0: 7574 696f 6e20 756e 7469 6c20 7468 6520  ution until the 
-000229b0: 6669 6c65 2068 6173 2062 6565 6e20 646f  file has been do
-000229c0: 776e 6c6f 6164 6564 2e0d 0a20 2020 2020  wnloaded...     
-000229d0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-000229e0: 6c74 7320 746f 2054 7275 652e 0d0a 0d0a  lts to True.....
-000229f0: 2020 2020 2020 2020 2020 2020 7072 6f67              prog
-00022a00: 7265 7373 2028 6060 4361 6c6c 6162 6c65  ress (``Callable
-00022a10: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-00022a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00022a30: 2020 5061 7373 2061 2063 616c 6c62 6163    Pass a callbac
-00022a40: 6b20 6675 6e63 7469 6f6e 2074 6f20 7669  k function to vi
-00022a50: 6577 2074 6865 2066 696c 6520 7472 616e  ew the file tran
-00022a60: 736d 6973 7369 6f6e 2070 726f 6772 6573  smission progres
-00022a70: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
-00022a80: 2020 2020 5468 6520 6675 6e63 7469 6f6e      The function
-00022a90: 206d 7573 7420 7461 6b65 202a 2863 7572   must take *(cur
-00022aa0: 7265 6e74 2c20 746f 7461 6c29 2a20 6173  rent, total)* as
-00022ab0: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
-00022ac0: 6d65 6e74 7320 286c 6f6f 6b20 6174 204f  ments (look at O
-00022ad0: 7468 6572 2050 6172 616d 6574 6572 7320  ther Parameters 
-00022ae0: 6265 6c6f 7720 666f 7220 610d 0a20 2020  below for a..   
-00022af0: 2020 2020 2020 2020 2020 2020 2064 6574               det
-00022b00: 6169 6c65 6420 6465 7363 7269 7074 696f  ailed descriptio
-00022b10: 6e29 2061 6e64 2077 696c 6c20 6265 2063  n) and will be c
-00022b20: 616c 6c65 6420 6261 636b 2065 6163 6820  alled back each 
-00022b30: 7469 6d65 2061 206e 6577 2066 696c 6520  time a new file 
-00022b40: 6368 756e 6b20 6861 7320 6265 656e 2073  chunk has been s
-00022b50: 7563 6365 7373 6675 6c6c 790d 0a20 2020  uccessfully..   
-00022b60: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00022b70: 6e73 6d69 7474 6564 2e0d 0a0d 0a20 2020  nsmitted.....   
-00022b80: 2020 2020 2020 2020 2070 726f 6772 6573           progres
-00022b90: 735f 6172 6773 2028 6060 7475 706c 6560  s_args (``tuple`
-00022ba0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-00022bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022bc0: 2045 7874 7261 2063 7573 746f 6d20 6172   Extra custom ar
-00022bd0: 6775 6d65 6e74 7320 666f 7220 7468 6520  guments for the 
-00022be0: 7072 6f67 7265 7373 2063 616c 6c62 6163  progress callbac
-00022bf0: 6b20 6675 6e63 7469 6f6e 2e0d 0a20 2020  k function...   
-00022c00: 2020 2020 2020 2020 2020 2020 2059 6f75               You
-00022c10: 2063 616e 2070 6173 7320 616e 7974 6869   can pass anythi
-00022c20: 6e67 2079 6f75 206e 6565 6420 746f 2062  ng you need to b
-00022c30: 6520 6176 6169 6c61 626c 6520 696e 2074  e available in t
-00022c40: 6865 2070 726f 6772 6573 7320 6361 6c6c  he progress call
-00022c50: 6261 636b 2073 636f 7065 3b20 666f 7220  back scope; for 
-00022c60: 6578 616d 706c 652c 2061 204d 6573 7361  example, a Messa
-00022c70: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
-00022c80: 2020 2020 6f62 6a65 6374 206f 7220 6120      object or a 
-00022c90: 436c 6965 6e74 2069 6e73 7461 6e63 6520  Client instance 
-00022ca0: 696e 206f 7264 6572 2074 6f20 6564 6974  in order to edit
-00022cb0: 2074 6865 206d 6573 7361 6765 2077 6974   the message wit
-00022cc0: 6820 7468 6520 7570 6461 7465 6420 7072  h the updated pr
-00022cd0: 6f67 7265 7373 2073 7461 7475 732e 0d0a  ogress status...
-00022ce0: 0d0a 2020 2020 2020 2020 4f74 6865 7220  ..        Other 
-00022cf0: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-00022d00: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00022d10: 2028 6060 696e 7460 6029 3a0d 0a20 2020   (``int``):..   
-00022d20: 2020 2020 2020 2020 2020 2020 2054 6865               The
-00022d30: 2061 6d6f 756e 7420 6f66 2062 7974 6573   amount of bytes
-00022d40: 2074 7261 6e73 6d69 7474 6564 2073 6f20   transmitted so 
-00022d50: 6661 722e 0d0a 0d0a 2020 2020 2020 2020  far.....        
-00022d60: 2020 2020 746f 7461 6c20 2860 6069 6e74      total (``int
-00022d70: 6060 293a 0d0a 2020 2020 2020 2020 2020  ``):..          
-00022d80: 2020 2020 2020 5468 6520 746f 7461 6c20        The total 
-00022d90: 7369 7a65 206f 6620 7468 6520 6669 6c65  size of the file
-00022da0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00022db0: 202a 6172 6773 2028 6060 7475 706c 6560   *args (``tuple`
-00022dc0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-00022dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022de0: 2045 7874 7261 2063 7573 746f 6d20 6172   Extra custom ar
-00022df0: 6775 6d65 6e74 7320 6173 2064 6566 696e  guments as defin
-00022e00: 6564 2069 6e20 7468 6520 6060 7072 6f67  ed in the ``prog
-00022e10: 7265 7373 5f61 7267 7360 6020 7061 7261  ress_args`` para
-00022e20: 6d65 7465 722e 0d0a 2020 2020 2020 2020  meter...        
-00022e30: 2020 2020 2020 2020 596f 7520 6361 6e20          You can 
-00022e40: 6569 7468 6572 206b 6565 7020 6060 2a61  either keep ``*a
-00022e50: 7267 7360 6020 6f72 2061 6464 2065 7665  rgs`` or add eve
-00022e60: 7279 2073 696e 676c 6520 6578 7472 6120  ry single extra 
-00022e70: 6172 6775 6d65 6e74 2069 6e20 796f 7572  argument in your
-00022e80: 2066 756e 6374 696f 6e20 7369 676e 6174   function signat
-00022e90: 7572 652e 0d0a 0d0a 2020 2020 2020 2020  ure.....        
-00022ea0: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
-00022eb0: 2020 2020 2020 4f6e 2073 7563 6365 7373        On success
-00022ec0: 2c20 7468 6520 6162 736f 6c75 7465 2070  , the absolute p
-00022ed0: 6174 6820 6f66 2074 6865 2064 6f77 6e6c  ath of the downl
-00022ee0: 6f61 6465 6420 6669 6c65 2061 7320 7374  oaded file as st
-00022ef0: 7269 6e67 2069 7320 7265 7475 726e 6564  ring is returned
-00022f00: 2c20 4e6f 6e65 206f 7468 6572 7769 7365  , None otherwise
-00022f10: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
-00022f20: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
-00022f30: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-00022f40: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-00022f50: 6d20 5250 4320 6572 726f 722e 0d0a 2020  m RPC error...  
-00022f60: 2020 2020 2020 2020 2020 6060 5661 6c75            ``Valu
-00022f70: 6545 7272 6f72 6060 3a20 4966 2074 6865  eError``: If the
-00022f80: 206d 6573 7361 6765 2064 6f65 736e 2774   message doesn't
-00022f90: 2063 6f6e 7461 696e 2061 6e79 2064 6f77   contain any dow
-00022fa0: 6e6c 6f61 6461 626c 6520 6d65 6469 610d  nloadable media.
-00022fb0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00022fc0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-00022fd0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
-00022fe0: 646f 776e 6c6f 6164 5f6d 6564 6961 280d  download_media(.
-00022ff0: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00023000: 7361 6765 3d73 656c 662c 0d0a 2020 2020  sage=self,..    
-00023010: 2020 2020 2020 2020 6669 6c65 5f6e 616d          file_nam
-00023020: 653d 6669 6c65 5f6e 616d 652c 0d0a 2020  e=file_name,..  
-00023030: 2020 2020 2020 2020 2020 696e 5f6d 656d            in_mem
-00023040: 6f72 793d 696e 5f6d 656d 6f72 792c 0d0a  ory=in_memory,..
-00023050: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
-00023060: 6b3d 626c 6f63 6b2c 0d0a 2020 2020 2020  k=block,..      
-00023070: 2020 2020 2020 7072 6f67 7265 7373 3d70        progress=p
-00023080: 726f 6772 6573 732c 0d0a 2020 2020 2020  rogress,..      
-00023090: 2020 2020 2020 7072 6f67 7265 7373 5f61        progress_a
-000230a0: 7267 733d 7072 6f67 7265 7373 5f61 7267  rgs=progress_arg
-000230b0: 732c 0d0a 2020 2020 2020 2020 290d 0a0d  s,..        )...
-000230c0: 0a20 2020 2061 7379 6e63 2064 6566 2076  .    async def v
-000230d0: 6f74 6528 0d0a 2020 2020 2020 2020 7365  ote(..        se
-000230e0: 6c66 2c0d 0a20 2020 2020 2020 206f 7074  lf,..        opt
-000230f0: 696f 6e3a 2069 6e74 2c0d 0a20 2020 2029  ion: int,..    )
-00023100: 202d 3e20 2274 7970 6573 2e50 6f6c 6c22   -> "types.Poll"
-00023110: 3a0d 0a20 2020 2020 2020 2022 2222 426f  :..        """Bo
-00023120: 756e 6420 6d65 7468 6f64 202a 766f 7465  und method *vote
-00023130: 2a20 6f66 203a 6f62 6a3a 607e 6669 7070  * of :obj:`~fipp
-00023140: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
-00023150: 602e 0d0a 0d0a 2020 2020 2020 2020 5573  `.....        Us
-00023160: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-00023170: 666f 723a 0d0a 0d0a 2020 2020 2020 2020  for:....        
-00023180: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00023190: 7079 7468 6f6e 0d0a 0d0a 2020 2020 2020  python....      
-000231a0: 2020 2020 2020 636c 6965 6e74 2e76 6f74        client.vot
-000231b0: 655f 706f 6c6c 280d 0a20 2020 2020 2020  e_poll(..       
-000231c0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-000231d0: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
-000231e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000231f0: 2020 206d 6573 7361 6765 5f69 643d 6d65     message_id=me
-00023200: 7373 6167 652e 6964 2c0d 0a20 2020 2020  ssage.id,..     
-00023210: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00023220: 6e3d 310d 0a20 2020 2020 2020 2020 2020  n=1..           
-00023230: 2029 0d0a 0d0a 2020 2020 2020 2020 4578   )....        Ex
-00023240: 616d 706c 653a 0d0a 2020 2020 2020 2020  ample:..        
-00023250: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00023260: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
-00023270: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00023280: 7373 6167 652e 766f 7465 2836 290d 0a0d  ssage.vote(6)...
-00023290: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000232a0: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
-000232b0: 2020 6f70 7469 6f6e 2028 6060 696e 7460    option (``int`
-000232c0: 6029 3a0d 0a20 2020 2020 2020 2020 2020  `):..           
-000232d0: 2020 2020 2049 6e64 6578 206f 6620 7468       Index of th
-000232e0: 6520 706f 6c6c 206f 7074 696f 6e20 796f  e poll option yo
-000232f0: 7520 7761 6e74 2074 6f20 766f 7465 2066  u want to vote f
-00023300: 6f72 2028 3020 746f 2039 292e 0d0a 0d0a  or (0 to 9).....
-00023310: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00023320: 0d0a 2020 2020 2020 2020 2020 2020 3a6f  ..            :o
-00023330: 626a 3a60 7e66 6970 7065 722e 7479 7065  bj:`~fipper.type
-00023340: 732e 506f 6c6c 603a 204f 6e20 7375 6363  s.Poll`: On succ
-00023350: 6573 732c 2074 6865 2070 6f6c 6c20 7769  ess, the poll wi
-00023360: 7468 2074 6865 2063 686f 7365 6e20 6f70  th the chosen op
-00023370: 7469 6f6e 2069 7320 7265 7475 726e 6564  tion is returned
-00023380: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
-00023390: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
-000233a0: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-000233b0: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-000233c0: 6d20 5250 4320 6572 726f 722e 0d0a 2020  m RPC error...  
-000233d0: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
-000233e0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-000233f0: 7420 7365 6c66 2e5f 636c 6965 6e74 2e76  t self._client.v
-00023400: 6f74 655f 706f 6c6c 280d 0a20 2020 2020  ote_poll(..     
-00023410: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
-00023420: 656c 662e 6368 6174 2e69 642c 0d0a 2020  elf.chat.id,..  
-00023430: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00023440: 655f 6964 3d73 656c 662e 6964 2c0d 0a20  e_id=self.id,.. 
-00023450: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00023460: 6e73 3d6f 7074 696f 6e0d 0a20 2020 2020  ns=option..     
-00023470: 2020 2029 0d0a 0d0a 2020 2020 6173 796e     )....    asyn
-00023480: 6320 6465 6620 7069 6e28 7365 6c66 2c20  c def pin(self, 
-00023490: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-000234a0: 7469 6f6e 3a20 626f 6f6c 203d 2046 616c  tion: bool = Fal
-000234b0: 7365 2c20 626f 7468 5f73 6964 6573 3a20  se, both_sides: 
-000234c0: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
-000234d0: 2022 7479 7065 732e 4d65 7373 6167 6522   "types.Message"
-000234e0: 3a0d 0a20 2020 2020 2020 2022 2222 426f  :..        """Bo
-000234f0: 756e 6420 6d65 7468 6f64 202a 7069 6e2a  und method *pin*
-00023500: 206f 6620 3a6f 626a 3a60 7e66 6970 7065   of :obj:`~fippe
-00023510: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
-00023520: 2e0d 0a0d 0a20 2020 2020 2020 2055 7365  .....        Use
-00023530: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
-00023540: 6f72 3a0d 0a0d 0a20 2020 2020 2020 202e  or:....        .
-00023550: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00023560: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
-00023570: 2020 2020 2061 7761 6974 2063 6c69 656e       await clien
-00023580: 742e 7069 6e5f 6368 6174 5f6d 6573 7361  t.pin_chat_messa
-00023590: 6765 280d 0a20 2020 2020 2020 2020 2020  ge(..           
-000235a0: 2020 2020 2063 6861 745f 6964 3d6d 6573       chat_id=mes
-000235b0: 7361 6765 2e63 6861 742e 6964 2c0d 0a20  sage.chat.id,.. 
-000235c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000235d0: 6573 7361 6765 5f69 643d 6d65 7373 6167  essage_id=messag
-000235e0: 655f 6964 0d0a 2020 2020 2020 2020 2020  e_id..          
-000235f0: 2020 290d 0a0d 0a20 2020 2020 2020 2045    )....        E
-00023600: 7861 6d70 6c65 3a0d 0a20 2020 2020 2020  xample:..       
-00023610: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-00023620: 636b 3a3a 2070 7974 686f 6e0d 0a0d 0a20  ck:: python.... 
-00023630: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00023640: 7761 6974 206d 6573 7361 6765 2e70 696e  wait message.pin
-00023650: 2829 0d0a 0d0a 2020 2020 2020 2020 5061  ()....        Pa
-00023660: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
-00023670: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
-00023680: 6f74 6966 6963 6174 696f 6e20 2860 6062  otification (``b
-00023690: 6f6f 6c60 6029 3a0d 0a20 2020 2020 2020  ool``):..       
-000236a0: 2020 2020 2020 2020 2050 6173 7320 5472           Pass Tr
-000236b0: 7565 2c20 6966 2069 7420 6973 206e 6f74  ue, if it is not
-000236c0: 206e 6563 6573 7361 7279 2074 6f20 7365   necessary to se
-000236d0: 6e64 2061 206e 6f74 6966 6963 6174 696f  nd a notificatio
-000236e0: 6e20 746f 2061 6c6c 2063 6861 7420 6d65  n to all chat me
-000236f0: 6d62 6572 7320 6162 6f75 7420 7468 6520  mbers about the 
-00023700: 6e65 7720 7069 6e6e 6564 0d0a 2020 2020  new pinned..    
-00023710: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00023720: 6167 652e 204e 6f74 6966 6963 6174 696f  age. Notificatio
-00023730: 6e73 2061 7265 2061 6c77 6179 7320 6469  ns are always di
-00023740: 7361 626c 6564 2069 6e20 6368 616e 6e65  sabled in channe
-00023750: 6c73 2e0d 0a0d 0a20 2020 2020 2020 2020  ls.....         
-00023760: 2020 2062 6f74 685f 7369 6465 7320 2860     both_sides (`
-00023770: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
-00023780: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
-00023790: 2020 2020 2020 2050 6173 7320 5472 7565         Pass True
-000237a0: 2074 6f20 7069 6e20 7468 6520 6d65 7373   to pin the mess
-000237b0: 6167 6520 666f 7220 626f 7468 2073 6964  age for both sid
-000237c0: 6573 2028 796f 7520 616e 6420 7265 6369  es (you and reci
-000237d0: 7069 656e 7429 2e0d 0a20 2020 2020 2020  pient)...       
-000237e0: 2020 2020 2020 2020 2041 7070 6c69 6361           Applica
-000237f0: 626c 6520 746f 2070 7269 7661 7465 2063  ble to private c
-00023800: 6861 7473 206f 6e6c 792e 2044 6566 6175  hats only. Defau
-00023810: 6c74 7320 746f 2046 616c 7365 2e0d 0a0d  lts to False....
-00023820: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00023830: 3a0d 0a20 2020 2020 2020 2020 2020 203a  :..            :
-00023840: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
-00023850: 6573 2e4d 6573 7361 6765 603a 204f 6e20  es.Message`: On 
-00023860: 7375 6363 6573 732c 2074 6865 2073 6572  success, the ser
-00023870: 7669 6365 206d 6573 7361 6765 2069 7320  vice message is 
-00023880: 7265 7475 726e 6564 2e0d 0a0d 0a20 2020  returned.....   
-00023890: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
-000238a0: 2020 2020 2020 2020 2020 5250 4345 7272            RPCErr
-000238b0: 6f72 3a20 496e 2063 6173 6520 6f66 2061  or: In case of a
-000238c0: 2054 656c 6567 7261 6d20 5250 4320 6572   Telegram RPC er
-000238d0: 726f 722e 0d0a 2020 2020 2020 2020 2222  ror...        ""
-000238e0: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-000238f0: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-00023900: 6965 6e74 2e70 696e 5f63 6861 745f 6d65  ient.pin_chat_me
-00023910: 7373 6167 6528 0d0a 2020 2020 2020 2020  ssage(..        
-00023920: 2020 2020 6368 6174 5f69 643d 7365 6c66      chat_id=self
-00023930: 2e63 6861 742e 6964 2c0d 0a20 2020 2020  .chat.id,..     
-00023940: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-00023950: 643d 7365 6c66 2e69 642c 0d0a 2020 2020  d=self.id,..    
-00023960: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-00023970: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
-00023980: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-00023990: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
-000239a0: 626f 7468 5f73 6964 6573 3d62 6f74 685f  both_sides=both_
-000239b0: 7369 6465 730d 0a20 2020 2020 2020 2029  sides..        )
-000239c0: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
-000239d0: 6620 756e 7069 6e28 7365 6c66 2920 2d3e  f unpin(self) ->
-000239e0: 2062 6f6f 6c3a 0d0a 2020 2020 2020 2020   bool:..        
-000239f0: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
-00023a00: 2a75 6e70 696e 2a20 6f66 203a 6f62 6a3a  *unpin* of :obj:
-00023a10: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
-00023a20: 6573 7361 6765 602e 0d0a 0d0a 2020 2020  essage`.....    
-00023a30: 2020 2020 5573 6520 6173 2061 2073 686f      Use as a sho
-00023a40: 7274 6375 7420 666f 723a 0d0a 0d0a 2020  rtcut for:....  
-00023a50: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-00023a60: 6f63 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a  ock:: python....
-00023a70: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00023a80: 7420 636c 6965 6e74 2e75 6e70 696e 5f63  t client.unpin_c
-00023a90: 6861 745f 6d65 7373 6167 6528 0d0a 2020  hat_message(..  
-00023aa0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00023ab0: 6174 5f69 643d 6d65 7373 6167 652e 6368  at_id=message.ch
-00023ac0: 6174 2e69 642c 0d0a 2020 2020 2020 2020  at.id,..        
-00023ad0: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-00023ae0: 6964 3d6d 6573 7361 6765 5f69 640d 0a20  id=message_id.. 
-00023af0: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
-00023b00: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-00023b10: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-00023b20: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00023b30: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
-00023b40: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
-00023b50: 7373 6167 652e 756e 7069 6e28 290d 0a0d  ssage.unpin()...
-00023b60: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00023b70: 3a0d 0a20 2020 2020 2020 2020 2020 2054  :..            T
-00023b80: 7275 6520 6f6e 2073 7563 6365 7373 2e0d  rue on success..
-00023b90: 0a0d 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00023ba0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00023bb0: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
-00023bc0: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
-00023bd0: 5250 4320 6572 726f 722e 0d0a 2020 2020  RPC error...    
-00023be0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00023bf0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-00023c00: 6c66 2e5f 636c 6965 6e74 2e75 6e70 696e  lf._client.unpin
-00023c10: 5f63 6861 745f 6d65 7373 6167 6528 0d0a  _chat_message(..
-00023c20: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00023c30: 5f69 643d 7365 6c66 2e63 6861 742e 6964  _id=self.chat.id
-00023c40: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-00023c50: 6573 7361 6765 5f69 643d 7365 6c66 2e69  essage_id=self.i
-00023c60: 640d 0a20 2020 2020 2020 2029 0d0a 0d0a  d..        )....
-00023c70: 2020 2020 6173 796e 6320 6465 6620 6173      async def as
-00023c80: 6b28 0d0a 2020 2020 2020 2020 7365 6c66  k(..        self
-00023c90: 2c0d 0a20 2020 2020 2020 2074 6578 743a  ,..        text:
-00023ca0: 2073 7472 2c0d 0a20 2020 2020 2020 2071   str,..        q
-00023cb0: 756f 7465 3a20 626f 6f6c 203d 204e 6f6e  uote: bool = Non
-00023cc0: 652c 0d0a 2020 2020 2020 2020 7061 7273  e,..        pars
-00023cd0: 655f 6d6f 6465 3a20 4f70 7469 6f6e 616c  e_mode: Optional
-00023ce0: 5b22 656e 756d 732e 5061 7273 654d 6f64  ["enums.ParseMod
-00023cf0: 6522 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  e"] = None,..   
-00023d00: 2020 2020 2065 6e74 6974 6965 733a 204c       entities: L
-00023d10: 6973 745b 2274 7970 6573 2e4d 6573 7361  ist["types.Messa
-00023d20: 6765 456e 7469 7479 225d 203d 204e 6f6e  geEntity"] = Non
-00023d30: 652c 0d0a 2020 2020 2020 2020 6469 7361  e,..        disa
-00023d40: 626c 655f 7765 625f 7061 6765 5f70 7265  ble_web_page_pre
-00023d50: 7669 6577 3a20 626f 6f6c 203d 204e 6f6e  view: bool = Non
-00023d60: 652c 0d0a 2020 2020 2020 2020 6469 7361  e,..        disa
-00023d70: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00023d80: 3a20 626f 6f6c 203d 204e 6f6e 652c 0d0a  : bool = None,..
-00023d90: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
-00023da0: 5f6d 6573 7361 6765 5f69 643a 2069 6e74  _message_id: int
-00023db0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00023dc0: 2020 7265 706c 795f 6d61 726b 7570 3d4e    reply_markup=N
-00023dd0: 6f6e 652c 0d0a 2020 2020 2020 2020 6669  one,..        fi
-00023de0: 6c74 6572 733d 4e6f 6e65 2c0d 0a20 2020  lters=None,..   
-00023df0: 2020 2020 2074 696d 656f 7574 3a20 696e       timeout: in
-00023e00: 7420 3d20 4e6f 6e65 0d0a 2020 2020 2920  t = None..    ) 
-00023e10: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
-00023e20: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
-00023e30: 6d65 7468 6f64 202a 6173 6b2a 206f 6620  method *ask* of 
-00023e40: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
-00023e50: 7065 732e 4d65 7373 6167 6560 2e0d 0a20  pes.Message`... 
-00023e60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00023e70: 2055 7365 2061 7320 6120 7368 6f72 7463   Use as a shortc
-00023e80: 7574 2066 6f72 3a0d 0a20 2020 2020 2020  ut for:..       
-00023e90: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
-00023ea0: 2070 7974 686f 6e0d 0a20 2020 2020 2020   python..       
-00023eb0: 2020 2020 2063 6c69 656e 742e 7365 6e64       client.send
-00023ec0: 5f6d 6573 7361 6765 2863 6861 745f 6964  _message(chat_id
-00023ed0: 2c20 2257 6861 7420 6973 2079 6f75 7220  , "What is your 
-00023ee0: 6e61 6d65 3f22 290d 0a20 2020 2020 2020  name?")..       
-00023ef0: 2020 2020 2063 6c69 656e 742e 7761 6974       client.wait
-00023f00: 5f66 6f72 5f6d 6573 7361 6765 2863 6861  _for_message(cha
-00023f10: 745f 6964 290d 0a20 2020 2020 2020 2020  t_id)..         
-00023f20: 2020 200d 0a20 2020 2020 2020 2045 7861     ..        Exa
-00023f30: 6d70 6c65 3a0d 0a20 2020 2020 2020 2020  mple:..         
-00023f40: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-00023f50: 3a3a 2070 7974 686f 6e0d 0a20 2020 2020  :: python..     
-00023f60: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00023f70: 6765 2e61 736b 2822 5768 6174 2069 7320  ge.ask("What is 
-00023f80: 796f 7572 206e 616d 653f 2229 0d0a 2020  your name?")..  
-00023f90: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00023fa0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00023fb0: 6578 7420 2860 6073 7472 6060 293a 0d0a  ext (``str``):..
-00023fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023fd0: 5465 7874 206f 6620 7468 6520 6d65 7373  Text of the mess
-00023fe0: 6167 6520 746f 2062 6520 7365 6e74 2e0d  age to be sent..
-00023ff0: 0a20 2020 2020 2020 2020 2020 2071 756f  .            quo
-00024000: 7465 2028 6060 626f 6f6c 6060 2c20 2a6f  te (``bool``, *o
-00024010: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
-00024020: 2020 2020 2020 2020 2020 2020 4966 2060              If `
-00024030: 6054 7275 6560 602c 2074 6865 206d 6573  `True``, the mes
-00024040: 7361 6765 2077 696c 6c20 6265 2073 656e  sage will be sen
-00024050: 7420 6173 2061 2072 6570 6c79 2074 6f20  t as a reply to 
-00024060: 7468 6973 206d 6573 7361 6765 2e0d 0a20  this message... 
-00024070: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-00024080: 6620 2a72 6570 6c79 5f74 6f5f 6d65 7373  f *reply_to_mess
-00024090: 6167 655f 6964 2a20 6973 2070 6173 7365  age_id* is passe
-000240a0: 642c 2074 6869 7320 7061 7261 6d65 7465  d, this paramete
-000240b0: 7220 7769 6c6c 2062 6520 6967 6e6f 7265  r will be ignore
-000240c0: 642e 0d0a 2020 2020 2020 2020 2020 2020  d...            
-000240d0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-000240e0: 6060 5472 7565 6060 2069 6e20 6772 6f75  ``True`` in grou
-000240f0: 7020 6368 6174 7320 616e 6420 6060 4661  p chats and ``Fa
-00024100: 6c73 6560 6020 696e 2070 7269 7661 7465  lse`` in private
-00024110: 2063 6861 7473 2e0d 0a20 2020 2020 2020   chats...       
-00024120: 2020 2020 2070 6172 7365 5f6d 6f64 6520       parse_mode 
-00024130: 283a 6f62 6a3a 607e 6669 7070 6572 2e65  (:obj:`~fipper.e
-00024140: 6e75 6d73 2e50 6172 7365 4d6f 6465 602c  nums.ParseMode`,
-00024150: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
-00024160: 2020 2020 2020 2020 2020 2020 2020 2042                 B
-00024170: 7920 6465 6661 756c 742c 2074 6578 7473  y default, texts
-00024180: 2061 7265 2070 6172 7365 6420 7573 696e   are parsed usin
-00024190: 6720 626f 7468 204d 6172 6b64 6f77 6e20  g both Markdown 
-000241a0: 616e 6420 4854 4d4c 2073 7479 6c65 732e  and HTML styles.
-000241b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000241c0: 2020 596f 7520 6361 6e20 636f 6d62 696e    You can combin
-000241d0: 6520 626f 7468 2073 796e 7461 7865 7320  e both syntaxes 
-000241e0: 746f 6765 7468 6572 2e0d 0a20 2020 2020  together...     
-000241f0: 2020 2020 2020 2065 6e74 6974 6965 7320         entities 
-00024200: 284c 6973 7420 6f66 203a 6f62 6a3a 607e  (List of :obj:`~
-00024210: 6669 7070 6572 2e74 7970 6573 2e4d 6573  fipper.types.Mes
-00024220: 7361 6765 456e 7469 7479 6029 3a0d 0a20  sageEntity`):.. 
-00024230: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-00024240: 6973 7420 6f66 2073 7065 6369 616c 2065  ist of special e
-00024250: 6e74 6974 6965 7320 7468 6174 2061 7070  ntities that app
-00024260: 6561 7220 696e 206d 6573 7361 6765 2074  ear in message t
-00024270: 6578 742c 2077 6869 6368 2063 616e 2062  ext, which can b
-00024280: 6520 7370 6563 6966 6965 6420 696e 7374  e specified inst
-00024290: 6561 6420 6f66 202a 7061 7273 655f 6d6f  ead of *parse_mo
-000242a0: 6465 2a2e 0d0a 2020 2020 2020 2020 2020  de*...          
-000242b0: 2020 6469 7361 626c 655f 7765 625f 7061    disable_web_pa
-000242c0: 6765 5f70 7265 7669 6577 2028 6060 626f  ge_preview (``bo
-000242d0: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
-000242e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000242f0: 2020 2020 4469 7361 626c 6573 206c 696e      Disables lin
-00024300: 6b20 7072 6576 6965 7773 2066 6f72 206c  k previews for l
-00024310: 696e 6b73 2069 6e20 7468 6973 206d 6573  inks in this mes
-00024320: 7361 6765 2e0d 0a20 2020 2020 2020 2020  sage...         
-00024330: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
-00024340: 6963 6174 696f 6e20 2860 6062 6f6f 6c60  ication (``bool`
-00024350: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
-00024360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024370: 2053 656e 6473 2074 6865 206d 6573 7361   Sends the messa
-00024380: 6765 2073 696c 656e 746c 792e 0d0a 2020  ge silently...  
-00024390: 2020 2020 2020 2020 2020 2020 2020 5573                Us
-000243a0: 6572 7320 7769 6c6c 2072 6563 6569 7665  ers will receive
-000243b0: 2061 206e 6f74 6966 6963 6174 696f 6e20   a notification 
-000243c0: 7769 7468 206e 6f20 736f 756e 642e 0d0a  with no sound...
-000243d0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-000243e0: 795f 746f 5f6d 6573 7361 6765 5f69 6420  y_to_message_id 
-000243f0: 2860 6069 6e74 6060 2c20 2a6f 7074 696f  (``int``, *optio
-00024400: 6e61 6c2a 293a 0d0a 2020 2020 2020 2020  nal*):..        
-00024410: 2020 2020 2020 2020 4966 2074 6865 206d          If the m
-00024420: 6573 7361 6765 2069 7320 6120 7265 706c  essage is a repl
-00024430: 792c 2049 4420 6f66 2074 6865 206f 7269  y, ID of the ori
-00024440: 6769 6e61 6c20 6d65 7373 6167 652e 0d0a  ginal message...
-00024450: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-00024460: 795f 6d61 726b 7570 2028 3a6f 626a 3a60  y_markup (:obj:`
-00024470: 7e66 6970 7065 722e 7479 7065 732e 496e  ~fipper.types.In
-00024480: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
-00024490: 7570 6020 7c20 3a6f 626a 3a60 7e66 6970  up` | :obj:`~fip
-000244a0: 7065 722e 7479 7065 732e 5265 706c 794b  per.types.ReplyK
-000244b0: 6579 626f 6172 644d 6172 6b75 7060 207c  eyboardMarkup` |
-000244c0: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
-000244d0: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
-000244e0: 7264 5265 6d6f 7665 6020 7c20 3a6f 626a  rdRemove` | :obj
-000244f0: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
-00024500: 466f 7263 6552 6570 6c79 602c 202a 6f70  ForceReply`, *op
-00024510: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
-00024520: 2020 2020 2020 2020 2020 2041 6464 6974             Addit
-00024530: 696f 6e61 6c20 696e 7465 7266 6163 6520  ional interface 
-00024540: 6f70 7469 6f6e 732e 2041 6e20 6f62 6a65  options. An obje
-00024550: 6374 2066 6f72 2061 6e20 696e 6c69 6e65  ct for an inline
-00024560: 206b 6579 626f 6172 642c 2063 7573 746f   keyboard, custo
-00024570: 6d20 7265 706c 7920 6b65 7962 6f61 7264  m reply keyboard
-00024580: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00024590: 2020 2069 6e73 7472 7563 7469 6f6e 7320     instructions 
-000245a0: 746f 2072 656d 6f76 6520 7265 706c 7920  to remove reply 
-000245b0: 6b65 7962 6f61 7264 206f 7220 746f 2066  keyboard or to f
-000245c0: 6f72 6365 2061 2072 6570 6c79 2066 726f  orce a reply fro
-000245d0: 6d20 7468 6520 7573 6572 2e0d 0a20 2020  m the user...   
-000245e0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
-000245f0: 2028 3a6f 626a 3a60 4669 6c74 6572 7360   (:obj:`Filters`
-00024600: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00024610: 2020 2020 5061 7373 206f 6e65 206f 7220      Pass one or 
-00024620: 6d6f 7265 2066 696c 7465 7273 2074 6f20  more filters to 
-00024630: 616c 6c6f 7720 6f6e 6c79 2061 2073 7562  allow only a sub
-00024640: 7365 7420 6f66 2063 616c 6c62 6163 6b20  set of callback 
-00024650: 7175 6572 6965 7320 746f 2062 6520 7061  queries to be pa
-00024660: 7373 6564 0d0a 2020 2020 2020 2020 2020  ssed..          
-00024670: 2020 2020 2020 696e 2079 6f75 7220 6361        in your ca
-00024680: 6c6c 6261 636b 2066 756e 6374 696f 6e2e  llback function.
-00024690: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-000246a0: 6d65 6f75 7420 2860 6069 6e74 6060 2c20  meout (``int``, 
-000246b0: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
-000246c0: 2020 2020 2020 2020 2020 2020 2020 5469                Ti
-000246d0: 6d65 6f75 7420 696e 2073 6563 6f6e 6473  meout in seconds
-000246e0: 2e0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000246f0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-00024700: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
-00024710: 7970 6573 2e4d 6573 7361 6765 603a 204f  ypes.Message`: O
-00024720: 6e20 7375 6363 6573 732c 2074 6865 2072  n success, the r
-00024730: 6570 6c79 206d 6573 7361 6765 2069 7320  eply message is 
-00024740: 7265 7475 726e 6564 2e0d 0a20 2020 2020  returned...     
-00024750: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
-00024760: 2020 2020 2020 2020 5250 4345 7272 6f72          RPCError
-00024770: 3a20 496e 2063 6173 6520 6f66 2061 2054  : In case of a T
-00024780: 656c 6567 7261 6d20 5250 4320 6572 726f  elegram RPC erro
-00024790: 722e 0d0a 2020 2020 2020 2020 2020 2020  r...            
-000247a0: 6173 796e 6369 6f2e 5469 6d65 6f75 7445  asyncio.TimeoutE
-000247b0: 7272 6f72 3a20 496e 2063 6173 6520 7265  rror: In case re
-000247c0: 706c 7920 6e6f 7420 7265 6365 6976 6564  ply not received
-000247d0: 2077 6974 6869 6e20 7468 6520 7469 6d65   within the time
-000247e0: 6f75 742e 0d0a 2020 2020 2020 2020 2222  out...        ""
-000247f0: 220d 0a20 2020 2020 2020 2069 6620 7175  "..        if qu
-00024800: 6f74 6520 6973 204e 6f6e 653a 0d0a 2020  ote is None:..  
-00024810: 2020 2020 2020 2020 2020 7175 6f74 6520            quote 
-00024820: 3d20 7365 6c66 2e63 6861 742e 7479 7065  = self.chat.type
-00024830: 2021 3d20 656e 756d 732e 4368 6174 5479   != enums.ChatTy
-00024840: 7065 2e50 5249 5641 5445 0d0a 0d0a 2020  pe.PRIVATE....  
-00024850: 2020 2020 2020 6966 2072 6570 6c79 5f74        if reply_t
-00024860: 6f5f 6d65 7373 6167 655f 6964 2069 7320  o_message_id is 
-00024870: 4e6f 6e65 2061 6e64 2071 756f 7465 3a0d  None and quote:.
-00024880: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-00024890: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
-000248a0: 203d 2073 656c 662e 6964 0d0a 0d0a 2020   = self.id....  
-000248b0: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
-000248c0: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
-000248d0: 6e74 2e73 656e 645f 6d65 7373 6167 6528  nt.send_message(
-000248e0: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-000248f0: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
-00024900: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
-00024910: 2074 6578 743d 7465 7874 2c0d 0a20 2020   text=text,..   
-00024920: 2020 2020 2020 2020 2070 6172 7365 5f6d           parse_m
-00024930: 6f64 653d 7061 7273 655f 6d6f 6465 2c0d  ode=parse_mode,.
-00024940: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-00024950: 6974 6965 733d 656e 7469 7469 6573 2c0d  ities=entities,.
-00024960: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00024970: 6162 6c65 5f77 6562 5f70 6167 655f 7072  able_web_page_pr
-00024980: 6576 6965 773d 6469 7361 626c 655f 7765  eview=disable_we
-00024990: 625f 7061 6765 5f70 7265 7669 6577 2c0d  b_page_preview,.
-000249a0: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-000249b0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
-000249c0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
-000249d0: 6361 7469 6f6e 2c0d 0a20 2020 2020 2020  cation,..       
-000249e0: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
-000249f0: 7373 6167 655f 6964 3d72 6570 6c79 5f74  ssage_id=reply_t
-00024a00: 6f5f 6d65 7373 6167 655f 6964 2c0d 0a20  o_message_id,.. 
-00024a10: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-00024a20: 5f6d 6172 6b75 703d 7265 706c 795f 6d61  _markup=reply_ma
-00024a30: 726b 7570 0d0a 2020 2020 2020 2020 290d  rkup..        ).
-00024a40: 0a0d 0a20 2020 2020 2020 2072 6570 6c79  ...        reply
-00024a50: 5f6d 6573 7361 6765 203d 2061 7761 6974  _message = await
-00024a60: 2073 656c 662e 5f63 6c69 656e 742e 7761   self._client.wa
-00024a70: 6974 5f66 6f72 5f6d 6573 7361 6765 280d  it_for_message(.
-00024a80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00024a90: 662e 6368 6174 2e69 642c 0d0a 2020 2020  f.chat.id,..    
-00024aa0: 2020 2020 2020 2020 6669 6c74 6572 733d          filters=
-00024ab0: 6669 6c74 6572 732c 0d0a 2020 2020 2020  filters,..      
-00024ac0: 2020 2020 2020 7469 6d65 6f75 743d 7469        timeout=ti
-00024ad0: 6d65 6f75 740d 0a20 2020 2020 2020 2029  meout..        )
-00024ae0: 0d0a 0d0a 2020 2020 2020 2020 7265 706c  ....        repl
-00024af0: 795f 6d65 7373 6167 652e 7265 7175 6573  y_message.reques
-00024b00: 7420 3d20 7265 7175 6573 740d 0a20 2020  t = request..   
-00024b10: 2020 2020 2072 6574 7572 6e20 7265 706c       return repl
-00024b20: 795f 6d65 7373 6167 650d 0a              y_message..
+0001a650: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+0001a660: 7469 6f6e 2028 6060 626f 6f6c 6060 2c20  tion (``bool``, 
+0001a670: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+0001a680: 2020 2020 2020 2020 2020 2020 2020 5365                Se
+0001a690: 6e64 7320 7468 6520 6d65 7373 6167 6520  nds the message 
+0001a6a0: 7369 6c65 6e74 6c79 2e0d 0a20 2020 2020  silently...     
+0001a6b0: 2020 2020 2020 2020 2020 2055 7365 7273             Users
+0001a6c0: 2077 696c 6c20 7265 6365 6976 6520 6120   will receive a 
+0001a6d0: 6e6f 7469 6669 6361 7469 6f6e 2077 6974  notification wit
+0001a6e0: 6820 6e6f 2073 6f75 6e64 2e0d 0a0d 0a20  h no sound..... 
+0001a6f0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+0001a700: 5f74 6f5f 6d65 7373 6167 655f 6964 2028  _to_message_id (
+0001a710: 6060 696e 7460 602c 202a 6f70 7469 6f6e  ``int``, *option
+0001a720: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+0001a730: 2020 2020 2020 2049 6620 7468 6520 6d65         If the me
+0001a740: 7373 6167 6520 6973 2061 2072 6570 6c79  ssage is a reply
+0001a750: 2c20 4944 206f 6620 7468 6520 6f72 6967  , ID of the orig
+0001a760: 696e 616c 206d 6573 7361 6765 0d0a 0d0a  inal message....
+0001a770: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+0001a780: 795f 6d61 726b 7570 2028 3a6f 626a 3a60  y_markup (:obj:`
+0001a790: 7e66 6970 7065 722e 7479 7065 732e 496e  ~fipper.types.In
+0001a7a0: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
+0001a7b0: 7570 6020 7c20 3a6f 626a 3a60 7e66 6970  up` | :obj:`~fip
+0001a7c0: 7065 722e 7479 7065 732e 5265 706c 794b  per.types.ReplyK
+0001a7d0: 6579 626f 6172 644d 6172 6b75 7060 207c  eyboardMarkup` |
+0001a7e0: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
+0001a7f0: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
+0001a800: 7264 5265 6d6f 7665 6020 7c20 3a6f 626a  rdRemove` | :obj
+0001a810: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
+0001a820: 466f 7263 6552 6570 6c79 602c 202a 6f70  ForceReply`, *op
+0001a830: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+0001a840: 2020 2020 2020 2020 2020 2041 6464 6974             Addit
+0001a850: 696f 6e61 6c20 696e 7465 7266 6163 6520  ional interface 
+0001a860: 6f70 7469 6f6e 732e 2041 6e20 6f62 6a65  options. An obje
+0001a870: 6374 2066 6f72 2061 6e20 696e 6c69 6e65  ct for an inline
+0001a880: 206b 6579 626f 6172 642c 2063 7573 746f   keyboard, custo
+0001a890: 6d20 7265 706c 7920 6b65 7962 6f61 7264  m reply keyboard
+0001a8a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001a8b0: 2020 2069 6e73 7472 7563 7469 6f6e 7320     instructions 
+0001a8c0: 746f 2072 656d 6f76 6520 7265 706c 7920  to remove reply 
+0001a8d0: 6b65 7962 6f61 7264 206f 7220 746f 2066  keyboard or to f
+0001a8e0: 6f72 6365 2061 2072 6570 6c79 2066 726f  orce a reply fro
+0001a8f0: 6d20 7468 6520 7573 6572 2e0d 0a0d 0a20  m the user..... 
+0001a900: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+0001a910: 6573 7320 2860 6043 616c 6c61 626c 6560  ess (``Callable`
+0001a920: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+0001a930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a940: 2050 6173 7320 6120 6361 6c6c 6261 636b   Pass a callback
+0001a950: 2066 756e 6374 696f 6e20 746f 2076 6965   function to vie
+0001a960: 7720 7468 6520 6669 6c65 2074 7261 6e73  w the file trans
+0001a970: 6d69 7373 696f 6e20 7072 6f67 7265 7373  mission progress
+0001a980: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a990: 2020 2054 6865 2066 756e 6374 696f 6e20     The function 
+0001a9a0: 6d75 7374 2074 616b 6520 2a28 6375 7272  must take *(curr
+0001a9b0: 656e 742c 2074 6f74 616c 292a 2061 7320  ent, total)* as 
+0001a9c0: 706f 7369 7469 6f6e 616c 2061 7267 756d  positional argum
+0001a9d0: 656e 7473 2028 6c6f 6f6b 2061 7420 4f74  ents (look at Ot
+0001a9e0: 6865 7220 5061 7261 6d65 7465 7273 2062  her Parameters b
+0001a9f0: 656c 6f77 2066 6f72 2061 0d0a 2020 2020  elow for a..    
+0001aa00: 2020 2020 2020 2020 2020 2020 6465 7461              deta
+0001aa10: 696c 6564 2064 6573 6372 6970 7469 6f6e  iled description
+0001aa20: 2920 616e 6420 7769 6c6c 2062 6520 6361  ) and will be ca
+0001aa30: 6c6c 6564 2062 6163 6b20 6561 6368 2074  lled back each t
+0001aa40: 696d 6520 6120 6e65 7720 6669 6c65 2063  ime a new file c
+0001aa50: 6875 6e6b 2068 6173 2062 6565 6e20 7375  hunk has been su
+0001aa60: 6363 6573 7366 756c 6c79 0d0a 2020 2020  ccessfully..    
+0001aa70: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+0001aa80: 736d 6974 7465 642e 0d0a 0d0a 2020 2020  smitted.....    
+0001aa90: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
+0001aaa0: 5f61 7267 7320 2860 6074 7570 6c65 6060  _args (``tuple``
+0001aab0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+0001aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aad0: 4578 7472 6120 6375 7374 6f6d 2061 7267  Extra custom arg
+0001aae0: 756d 656e 7473 2066 6f72 2074 6865 2070  uments for the p
+0001aaf0: 726f 6772 6573 7320 6361 6c6c 6261 636b  rogress callback
+0001ab00: 2066 756e 6374 696f 6e2e 0d0a 2020 2020   function...    
+0001ab10: 2020 2020 2020 2020 2020 2020 596f 7520              You 
+0001ab20: 6361 6e20 7061 7373 2061 6e79 7468 696e  can pass anythin
+0001ab30: 6720 796f 7520 6e65 6564 2074 6f20 6265  g you need to be
+0001ab40: 2061 7661 696c 6162 6c65 2069 6e20 7468   available in th
+0001ab50: 6520 7072 6f67 7265 7373 2063 616c 6c62  e progress callb
+0001ab60: 6163 6b20 7363 6f70 653b 2066 6f72 2065  ack scope; for e
+0001ab70: 7861 6d70 6c65 2c20 6120 4d65 7373 6167  xample, a Messag
+0001ab80: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+0001ab90: 2020 206f 626a 6563 7420 6f72 2061 2043     object or a C
+0001aba0: 6c69 656e 7420 696e 7374 616e 6365 2069  lient instance i
+0001abb0: 6e20 6f72 6465 7220 746f 2065 6469 7420  n order to edit 
+0001abc0: 7468 6520 6d65 7373 6167 6520 7769 7468  the message with
+0001abd0: 2074 6865 2075 7064 6174 6564 2070 726f   the updated pro
+0001abe0: 6772 6573 7320 7374 6174 7573 2e0d 0a0d  gress status....
+0001abf0: 0a20 2020 2020 2020 204f 7468 6572 2050  .        Other P
+0001ac00: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+0001ac10: 2020 2020 2020 2020 6375 7272 656e 7420          current 
+0001ac20: 2860 6069 6e74 6060 293a 0d0a 2020 2020  (``int``):..    
+0001ac30: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0001ac40: 616d 6f75 6e74 206f 6620 6279 7465 7320  amount of bytes 
+0001ac50: 7472 616e 736d 6974 7465 6420 736f 2066  transmitted so f
+0001ac60: 6172 2e0d 0a0d 0a20 2020 2020 2020 2020  ar.....         
+0001ac70: 2020 2074 6f74 616c 2028 6060 696e 7460     total (``int`
+0001ac80: 6029 3a0d 0a20 2020 2020 2020 2020 2020  `):..           
+0001ac90: 2020 2020 2054 6865 2074 6f74 616c 2073       The total s
+0001aca0: 697a 6520 6f66 2074 6865 2066 696c 652e  ize of the file.
+0001acb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001acc0: 2a61 7267 7320 2860 6074 7570 6c65 6060  *args (``tuple``
+0001acd0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+0001ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acf0: 4578 7472 6120 6375 7374 6f6d 2061 7267  Extra custom arg
+0001ad00: 756d 656e 7473 2061 7320 6465 6669 6e65  uments as define
+0001ad10: 6420 696e 2074 6865 2060 6070 726f 6772  d in the ``progr
+0001ad20: 6573 735f 6172 6773 6060 2070 6172 616d  ess_args`` param
+0001ad30: 6574 6572 2e0d 0a20 2020 2020 2020 2020  eter...         
+0001ad40: 2020 2020 2020 2059 6f75 2063 616e 2065         You can e
+0001ad50: 6974 6865 7220 6b65 6570 2060 602a 6172  ither keep ``*ar
+0001ad60: 6773 6060 206f 7220 6164 6420 6576 6572  gs`` or add ever
+0001ad70: 7920 7369 6e67 6c65 2065 7874 7261 2061  y single extra a
+0001ad80: 7267 756d 656e 7420 696e 2079 6f75 7220  rgument in your 
+0001ad90: 6675 6e63 7469 6f6e 2073 6967 6e61 7475  function signatu
+0001ada0: 7265 2e0d 0a0d 0a20 2020 2020 2020 2052  re.....        R
+0001adb0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+0001adc0: 2020 2020 204f 6e20 7375 6363 6573 732c       On success,
+0001add0: 2074 6865 2073 656e 7420 3a6f 626a 3a60   the sent :obj:`
+0001ade0: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
+0001adf0: 7373 6167 6560 2069 7320 7265 7475 726e  ssage` is return
+0001ae00: 6564 2e0d 0a20 2020 2020 2020 2020 2020  ed...           
+0001ae10: 2049 6e20 6361 7365 2074 6865 2075 706c   In case the upl
+0001ae20: 6f61 6420 6973 2064 656c 6962 6572 6174  oad is deliberat
+0001ae30: 656c 7920 7374 6f70 7065 6420 7769 7468  ely stopped with
+0001ae40: 203a 6d65 7468 3a60 7e66 6970 7065 722e   :meth:`~fipper.
+0001ae50: 436c 6965 6e74 2e73 746f 705f 7472 616e  Client.stop_tran
+0001ae60: 736d 6973 7369 6f6e 602c 204e 6f6e 6520  smission`, None 
+0001ae70: 6973 2072 6574 7572 6e65 640d 0a20 2020  is returned..   
+0001ae80: 2020 2020 2020 2020 2069 6e73 7465 6164           instead
+0001ae90: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
+0001aea0: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
+0001aeb0: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
+0001aec0: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
+0001aed0: 6d20 5250 4320 6572 726f 722e 0d0a 2020  m RPC error...  
+0001aee0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0001aef0: 2020 2069 6620 7175 6f74 6520 6973 204e     if quote is N
+0001af00: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0001af10: 2020 7175 6f74 6520 3d20 7365 6c66 2e63    quote = self.c
+0001af20: 6861 742e 7479 7065 2021 3d20 656e 756d  hat.type != enum
+0001af30: 732e 4368 6174 5479 7065 2e50 5249 5641  s.ChatType.PRIVA
+0001af40: 5445 0d0a 0d0a 2020 2020 2020 2020 6966  TE....        if
+0001af50: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+0001af60: 655f 6964 2069 7320 4e6f 6e65 2061 6e64  e_id is None and
+0001af70: 2071 756f 7465 3a0d 0a20 2020 2020 2020   quote:..       
+0001af80: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
+0001af90: 7373 6167 655f 6964 203d 2073 656c 662e  ssage_id = self.
+0001afa0: 6964 0d0a 0d0a 2020 2020 2020 2020 7265  id....        re
+0001afb0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+0001afc0: 5f63 6c69 656e 742e 7365 6e64 5f76 6964  _client.send_vid
+0001afd0: 656f 5f6e 6f74 6528 0d0a 2020 2020 2020  eo_note(..      
+0001afe0: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
+0001aff0: 6c66 2e63 6861 742e 6964 2c0d 0a20 2020  lf.chat.id,..   
+0001b000: 2020 2020 2020 2020 2076 6964 656f 5f6e           video_n
+0001b010: 6f74 653d 7669 6465 6f5f 6e6f 7465 2c0d  ote=video_note,.
+0001b020: 0a20 2020 2020 2020 2020 2020 2064 7572  .            dur
+0001b030: 6174 696f 6e3d 6475 7261 7469 6f6e 2c0d  ation=duration,.
+0001b040: 0a20 2020 2020 2020 2020 2020 206c 656e  .            len
+0001b050: 6774 683d 6c65 6e67 7468 2c0d 0a20 2020  gth=length,..   
+0001b060: 2020 2020 2020 2020 2074 6875 6d62 3d74           thumb=t
+0001b070: 6875 6d62 2c0d 0a20 2020 2020 2020 2020  humb,..         
+0001b080: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+0001b090: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
+0001b0a0: 6e6f 7469 6669 6361 7469 6f6e 2c0d 0a20  notification,.. 
+0001b0b0: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+0001b0c0: 5f74 6f5f 6d65 7373 6167 655f 6964 3d72  _to_message_id=r
+0001b0d0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+0001b0e0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+0001b0f0: 2072 6570 6c79 5f6d 6172 6b75 703d 7265   reply_markup=re
+0001b100: 706c 795f 6d61 726b 7570 2c0d 0a20 2020  ply_markup,..   
+0001b110: 2020 2020 2020 2020 2070 726f 6772 6573           progres
+0001b120: 733d 7072 6f67 7265 7373 2c0d 0a20 2020  s=progress,..   
+0001b130: 2020 2020 2020 2020 2070 726f 6772 6573           progres
+0001b140: 735f 6172 6773 3d70 726f 6772 6573 735f  s_args=progress_
+0001b150: 6172 6773 0d0a 2020 2020 2020 2020 290d  args..        ).
+0001b160: 0a0d 0a20 2020 2061 7379 6e63 2064 6566  ...    async def
+0001b170: 2072 6570 6c79 5f76 6f69 6365 280d 0a20   reply_voice(.. 
+0001b180: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+0001b190: 2020 2020 2020 766f 6963 653a 2055 6e69        voice: Uni
+0001b1a0: 6f6e 5b73 7472 2c20 4269 6e61 7279 494f  on[str, BinaryIO
+0001b1b0: 5d2c 0d0a 2020 2020 2020 2020 7175 6f74  ],..        quot
+0001b1c0: 653a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d  e: bool = None,.
+0001b1d0: 0a20 2020 2020 2020 2063 6170 7469 6f6e  .        caption
+0001b1e0: 3a20 7374 7220 3d20 2222 2c0d 0a20 2020  : str = "",..   
+0001b1f0: 2020 2020 2070 6172 7365 5f6d 6f64 653a       parse_mode:
+0001b200: 204f 7074 696f 6e61 6c5b 2265 6e75 6d73   Optional["enums
+0001b210: 2e50 6172 7365 4d6f 6465 225d 203d 204e  .ParseMode"] = N
+0001b220: 6f6e 652c 0d0a 2020 2020 2020 2020 6361  one,..        ca
+0001b230: 7074 696f 6e5f 656e 7469 7469 6573 3a20  ption_entities: 
+0001b240: 4c69 7374 5b22 7479 7065 732e 4d65 7373  List["types.Mess
+0001b250: 6167 6545 6e74 6974 7922 5d20 3d20 4e6f  ageEntity"] = No
+0001b260: 6e65 2c0d 0a20 2020 2020 2020 2064 7572  ne,..        dur
+0001b270: 6174 696f 6e3a 2069 6e74 203d 2030 2c0d  ation: int = 0,.
+0001b280: 0a20 2020 2020 2020 2064 6973 6162 6c65  .        disable
+0001b290: 5f6e 6f74 6966 6963 6174 696f 6e3a 2062  _notification: b
+0001b2a0: 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20 2020  ool = None,..   
+0001b2b0: 2020 2020 2072 6570 6c79 5f74 6f5f 6d65       reply_to_me
+0001b2c0: 7373 6167 655f 6964 3a20 696e 7420 3d20  ssage_id: int = 
+0001b2d0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2072  None,..        r
+0001b2e0: 6570 6c79 5f6d 6172 6b75 703a 2055 6e69  eply_markup: Uni
+0001b2f0: 6f6e 5b0d 0a20 2020 2020 2020 2020 2020  on[..           
+0001b300: 2022 7479 7065 732e 496e 6c69 6e65 4b65   "types.InlineKe
+0001b310: 7962 6f61 7264 4d61 726b 7570 222c 0d0a  yboardMarkup",..
+0001b320: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+0001b330: 6573 2e52 6570 6c79 4b65 7962 6f61 7264  es.ReplyKeyboard
+0001b340: 4d61 726b 7570 222c 0d0a 2020 2020 2020  Markup",..      
+0001b350: 2020 2020 2020 2274 7970 6573 2e52 6570        "types.Rep
+0001b360: 6c79 4b65 7962 6f61 7264 5265 6d6f 7665  lyKeyboardRemove
+0001b370: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001b380: 2274 7970 6573 2e46 6f72 6365 5265 706c  "types.ForceRepl
+0001b390: 7922 0d0a 2020 2020 2020 2020 5d20 3d20  y"..        ] = 
+0001b3a0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2070  None,..        p
+0001b3b0: 726f 6772 6573 733a 2043 616c 6c61 626c  rogress: Callabl
+0001b3c0: 6520 3d20 4e6f 6e65 2c0d 0a20 2020 2020  e = None,..     
+0001b3d0: 2020 2070 726f 6772 6573 735f 6172 6773     progress_args
+0001b3e0: 3a20 7475 706c 6520 3d20 2829 0d0a 2020  : tuple = ()..  
+0001b3f0: 2020 2920 2d3e 2022 4d65 7373 6167 6522    ) -> "Message"
+0001b400: 3a0d 0a20 2020 2020 2020 2022 2222 426f  :..        """Bo
+0001b410: 756e 6420 6d65 7468 6f64 202a 7265 706c  und method *repl
+0001b420: 795f 766f 6963 652a 206f 6620 3a6f 626a  y_voice* of :obj
+0001b430: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
+0001b440: 4d65 7373 6167 6560 2e0d 0a0d 0a20 2020  Message`.....   
+0001b450: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
+0001b460: 6f72 7463 7574 2066 6f72 3a0d 0a0d 0a20  ortcut for:.... 
+0001b470: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0001b480: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
+0001b490: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+0001b4a0: 6974 2063 6c69 656e 742e 7365 6e64 5f76  it client.send_v
+0001b4b0: 6f69 6365 280d 0a20 2020 2020 2020 2020  oice(..         
+0001b4c0: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
+0001b4d0: 6573 7361 6765 2e63 6861 742e 6964 2c0d  essage.chat.id,.
+0001b4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b4f0: 2076 6f69 6365 3d76 6f69 6365 0d0a 2020   voice=voice..  
+0001b500: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+0001b510: 2020 2020 2020 2045 7861 6d70 6c65 3a0d         Example:.
+0001b520: 0a20 2020 2020 2020 2020 2020 202e 2e20  .            .. 
+0001b530: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+0001b540: 686f 6e0d 0a0d 0a20 2020 2020 2020 2020  hon....         
+0001b550: 2020 2020 2020 2061 7761 6974 206d 6573         await mes
+0001b560: 7361 6765 2e72 6570 6c79 5f76 6f69 6365  sage.reply_voice
+0001b570: 2876 6f69 6365 290d 0a0d 0a20 2020 2020  (voice)....     
+0001b580: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
+0001b590: 2020 2020 2020 2020 2020 2020 766f 6963              voic
+0001b5a0: 6520 2860 6073 7472 6060 293a 0d0a 2020  e (``str``):..  
+0001b5b0: 2020 2020 2020 2020 2020 2020 2020 4175                Au
+0001b5c0: 6469 6f20 6669 6c65 2074 6f20 7365 6e64  dio file to send
+0001b5d0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b5e0: 2020 2050 6173 7320 6120 6669 6c65 5f69     Pass a file_i
+0001b5f0: 6420 6173 2073 7472 696e 6720 746f 2073  d as string to s
+0001b600: 656e 6420 616e 2061 7564 696f 2074 6861  end an audio tha
+0001b610: 7420 6578 6973 7473 206f 6e20 7468 6520  t exists on the 
+0001b620: 5465 6c65 6772 616d 2073 6572 7665 7273  Telegram servers
+0001b630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001b640: 2020 2070 6173 7320 616e 2048 5454 5020     pass an HTTP 
+0001b650: 5552 4c20 6173 2061 2073 7472 696e 6720  URL as a string 
+0001b660: 666f 7220 5465 6c65 6772 616d 2074 6f20  for Telegram to 
+0001b670: 6765 7420 616e 2061 7564 696f 2066 726f  get an audio fro
+0001b680: 6d20 7468 6520 496e 7465 726e 6574 2c20  m the Internet, 
+0001b690: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
+0001b6a0: 2020 2020 7061 7373 2061 2066 696c 6520      pass a file 
+0001b6b0: 7061 7468 2061 7320 7374 7269 6e67 2074  path as string t
+0001b6c0: 6f20 7570 6c6f 6164 2061 206e 6577 2061  o upload a new a
+0001b6d0: 7564 696f 2074 6861 7420 6578 6973 7473  udio that exists
+0001b6e0: 206f 6e20 796f 7572 206c 6f63 616c 206d   on your local m
+0001b6f0: 6163 6869 6e65 2e0d 0a0d 0a20 2020 2020  achine.....     
+0001b700: 2020 2020 2020 2071 756f 7465 2028 6060         quote (``
+0001b710: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
+0001b720: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+0001b730: 2020 2020 2020 4966 2060 6054 7275 6560        If ``True`
+0001b740: 602c 2074 6865 206d 6573 7361 6765 2077  `, the message w
+0001b750: 696c 6c20 6265 2073 656e 7420 6173 2061  ill be sent as a
+0001b760: 2072 6570 6c79 2074 6f20 7468 6973 206d   reply to this m
+0001b770: 6573 7361 6765 2e0d 0a20 2020 2020 2020  essage...       
+0001b780: 2020 2020 2020 2020 2049 6620 2a72 6570           If *rep
+0001b790: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+0001b7a0: 2a20 6973 2070 6173 7365 642c 2074 6869  * is passed, thi
+0001b7b0: 7320 7061 7261 6d65 7465 7220 7769 6c6c  s parameter will
+0001b7c0: 2062 6520 6967 6e6f 7265 642e 0d0a 2020   be ignored...  
+0001b7d0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+0001b7e0: 6661 756c 7473 2074 6f20 6060 5472 7565  faults to ``True
+0001b7f0: 6060 2069 6e20 6772 6f75 7020 6368 6174  `` in group chat
+0001b800: 7320 616e 6420 6060 4661 6c73 6560 6020  s and ``False`` 
+0001b810: 696e 2070 7269 7661 7465 2063 6861 7473  in private chats
+0001b820: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+0001b830: 2063 6170 7469 6f6e 2028 6060 7374 7260   caption (``str`
+0001b840: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+0001b850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b860: 2056 6f69 6365 206d 6573 7361 6765 2063   Voice message c
+0001b870: 6170 7469 6f6e 2c20 302d 3130 3234 2063  aption, 0-1024 c
+0001b880: 6861 7261 6374 6572 732e 0d0a 0d0a 2020  haracters.....  
+0001b890: 2020 2020 2020 2020 2020 7061 7273 655f            parse_
+0001b8a0: 6d6f 6465 2028 3a6f 626a 3a60 7e66 6970  mode (:obj:`~fip
+0001b8b0: 7065 722e 656e 756d 732e 5061 7273 654d  per.enums.ParseM
+0001b8c0: 6f64 6560 2c20 2a6f 7074 696f 6e61 6c2a  ode`, *optional*
+0001b8d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001b8e0: 2020 2020 4279 2064 6566 6175 6c74 2c20      By default, 
+0001b8f0: 7465 7874 7320 6172 6520 7061 7273 6564  texts are parsed
+0001b900: 2075 7369 6e67 2062 6f74 6820 4d61 726b   using both Mark
+0001b910: 646f 776e 2061 6e64 2048 544d 4c20 7374  down and HTML st
+0001b920: 796c 6573 2e0d 0a20 2020 2020 2020 2020  yles...         
+0001b930: 2020 2020 2020 2059 6f75 2063 616e 2063         You can c
+0001b940: 6f6d 6269 6e65 2062 6f74 6820 7379 6e74  ombine both synt
+0001b950: 6178 6573 2074 6f67 6574 6865 722e 0d0a  axes together...
+0001b960: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
+0001b970: 7074 696f 6e5f 656e 7469 7469 6573 2028  ption_entities (
+0001b980: 4c69 7374 206f 6620 3a6f 626a 3a60 7e66  List of :obj:`~f
+0001b990: 6970 7065 722e 7479 7065 732e 4d65 7373  ipper.types.Mess
+0001b9a0: 6167 6545 6e74 6974 7960 293a 0d0a 2020  ageEntity`):..  
+0001b9b0: 2020 2020 2020 2020 2020 2020 2020 4c69                Li
+0001b9c0: 7374 206f 6620 7370 6563 6961 6c20 656e  st of special en
+0001b9d0: 7469 7469 6573 2074 6861 7420 6170 7065  tities that appe
+0001b9e0: 6172 2069 6e20 7468 6520 6361 7074 696f  ar in the captio
+0001b9f0: 6e2c 2077 6869 6368 2063 616e 2062 6520  n, which can be 
+0001ba00: 7370 6563 6966 6965 6420 696e 7374 6561  specified instea
+0001ba10: 6420 6f66 202a 7061 7273 655f 6d6f 6465  d of *parse_mode
+0001ba20: 2a2e 0d0a 0d0a 2020 2020 2020 2020 2020  *.....          
+0001ba30: 2020 6475 7261 7469 6f6e 2028 6060 696e    duration (``in
+0001ba40: 7460 602c 202a 6f70 7469 6f6e 616c 2a29  t``, *optional*)
+0001ba50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001ba60: 2020 2044 7572 6174 696f 6e20 6f66 2074     Duration of t
+0001ba70: 6865 2076 6f69 6365 206d 6573 7361 6765  he voice message
+0001ba80: 2069 6e20 7365 636f 6e64 732e 0d0a 0d0a   in seconds.....
+0001ba90: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+0001baa0: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+0001bab0: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+0001bac0: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+0001bad0: 2020 2020 2020 2020 2020 5365 6e64 7320            Sends 
+0001bae0: 7468 6520 6d65 7373 6167 6520 7369 6c65  the message sile
+0001baf0: 6e74 6c79 2e0d 0a20 2020 2020 2020 2020  ntly...         
+0001bb00: 2020 2020 2020 2055 7365 7273 2077 696c         Users wil
+0001bb10: 6c20 7265 6365 6976 6520 6120 6e6f 7469  l receive a noti
+0001bb20: 6669 6361 7469 6f6e 2077 6974 6820 6e6f  fication with no
+0001bb30: 2073 6f75 6e64 2e0d 0a0d 0a20 2020 2020   sound.....     
+0001bb40: 2020 2020 2020 2072 6570 6c79 5f74 6f5f         reply_to_
+0001bb50: 6d65 7373 6167 655f 6964 2028 6060 696e  message_id (``in
+0001bb60: 7460 602c 202a 6f70 7469 6f6e 616c 2a29  t``, *optional*)
+0001bb70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001bb80: 2020 2049 6620 7468 6520 6d65 7373 6167     If the messag
+0001bb90: 6520 6973 2061 2072 6570 6c79 2c20 4944  e is a reply, ID
+0001bba0: 206f 6620 7468 6520 6f72 6967 696e 616c   of the original
+0001bbb0: 206d 6573 7361 6765 0d0a 0d0a 2020 2020   message....    
+0001bbc0: 2020 2020 2020 2020 7265 706c 795f 6d61          reply_ma
+0001bbd0: 726b 7570 2028 3a6f 626a 3a60 7e66 6970  rkup (:obj:`~fip
+0001bbe0: 7065 722e 7479 7065 732e 496e 6c69 6e65  per.types.Inline
+0001bbf0: 4b65 7962 6f61 7264 4d61 726b 7570 6020  KeyboardMarkup` 
+0001bc00: 7c20 3a6f 626a 3a60 7e66 6970 7065 722e  | :obj:`~fipper.
+0001bc10: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
+0001bc20: 6172 644d 6172 6b75 7060 207c 203a 6f62  ardMarkup` | :ob
+0001bc30: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+0001bc40: 2e52 6570 6c79 4b65 7962 6f61 7264 5265  .ReplyKeyboardRe
+0001bc50: 6d6f 7665 6020 7c20 3a6f 626a 3a60 7e66  move` | :obj:`~f
+0001bc60: 6970 7065 722e 7479 7065 732e 466f 7263  ipper.types.Forc
+0001bc70: 6552 6570 6c79 602c 202a 6f70 7469 6f6e  eReply`, *option
+0001bc80: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+0001bc90: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
+0001bca0: 6c20 696e 7465 7266 6163 6520 6f70 7469  l interface opti
+0001bcb0: 6f6e 732e 2041 6e20 6f62 6a65 6374 2066  ons. An object f
+0001bcc0: 6f72 2061 6e20 696e 6c69 6e65 206b 6579  or an inline key
+0001bcd0: 626f 6172 642c 2063 7573 746f 6d20 7265  board, custom re
+0001bce0: 706c 7920 6b65 7962 6f61 7264 2c0d 0a20  ply keyboard,.. 
+0001bcf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001bd00: 6e73 7472 7563 7469 6f6e 7320 746f 2072  nstructions to r
+0001bd10: 656d 6f76 6520 7265 706c 7920 6b65 7962  emove reply keyb
+0001bd20: 6f61 7264 206f 7220 746f 2066 6f72 6365  oard or to force
+0001bd30: 2061 2072 6570 6c79 2066 726f 6d20 7468   a reply from th
+0001bd40: 6520 7573 6572 2e0d 0a0d 0a20 2020 2020  e user.....     
+0001bd50: 2020 2020 2020 2070 726f 6772 6573 7320         progress 
+0001bd60: 2860 6043 616c 6c61 626c 6560 602c 202a  (``Callable``, *
+0001bd70: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
+0001bd80: 2020 2020 2020 2020 2020 2020 2050 6173               Pas
+0001bd90: 7320 6120 6361 6c6c 6261 636b 2066 756e  s a callback fun
+0001bda0: 6374 696f 6e20 746f 2076 6965 7720 7468  ction to view th
+0001bdb0: 6520 6669 6c65 2074 7261 6e73 6d69 7373  e file transmiss
+0001bdc0: 696f 6e20 7072 6f67 7265 7373 2e0d 0a20  ion progress... 
+0001bdd0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0001bde0: 6865 2066 756e 6374 696f 6e20 6d75 7374  he function must
+0001bdf0: 2074 616b 6520 2a28 6375 7272 656e 742c   take *(current,
+0001be00: 2074 6f74 616c 292a 2061 7320 706f 7369   total)* as posi
+0001be10: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
+0001be20: 2028 6c6f 6f6b 2061 7420 4f74 6865 7220   (look at Other 
+0001be30: 5061 7261 6d65 7465 7273 2062 656c 6f77  Parameters below
+0001be40: 2066 6f72 2061 0d0a 2020 2020 2020 2020   for a..        
+0001be50: 2020 2020 2020 2020 6465 7461 696c 6564          detailed
+0001be60: 2064 6573 6372 6970 7469 6f6e 2920 616e   description) an
+0001be70: 6420 7769 6c6c 2062 6520 6361 6c6c 6564  d will be called
+0001be80: 2062 6163 6b20 6561 6368 2074 696d 6520   back each time 
+0001be90: 6120 6e65 7720 6669 6c65 2063 6875 6e6b  a new file chunk
+0001bea0: 2068 6173 2062 6565 6e20 7375 6363 6573   has been succes
+0001beb0: 7366 756c 6c79 0d0a 2020 2020 2020 2020  sfully..        
+0001bec0: 2020 2020 2020 2020 7472 616e 736d 6974          transmit
+0001bed0: 7465 642e 0d0a 0d0a 2020 2020 2020 2020  ted.....        
+0001bee0: 2020 2020 7072 6f67 7265 7373 5f61 7267      progress_arg
+0001bef0: 7320 2860 6074 7570 6c65 6060 2c20 2a6f  s (``tuple``, *o
+0001bf00: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+0001bf10: 2020 2020 2020 2020 2020 2020 4578 7472              Extr
+0001bf20: 6120 6375 7374 6f6d 2061 7267 756d 656e  a custom argumen
+0001bf30: 7473 2066 6f72 2074 6865 2070 726f 6772  ts for the progr
+0001bf40: 6573 7320 6361 6c6c 6261 636b 2066 756e  ess callback fun
+0001bf50: 6374 696f 6e2e 0d0a 2020 2020 2020 2020  ction...        
+0001bf60: 2020 2020 2020 2020 596f 7520 6361 6e20          You can 
+0001bf70: 7061 7373 2061 6e79 7468 696e 6720 796f  pass anything yo
+0001bf80: 7520 6e65 6564 2074 6f20 6265 2061 7661  u need to be ava
+0001bf90: 696c 6162 6c65 2069 6e20 7468 6520 7072  ilable in the pr
+0001bfa0: 6f67 7265 7373 2063 616c 6c62 6163 6b20  ogress callback 
+0001bfb0: 7363 6f70 653b 2066 6f72 2065 7861 6d70  scope; for examp
+0001bfc0: 6c65 2c20 6120 4d65 7373 6167 650d 0a20  le, a Message.. 
+0001bfd0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001bfe0: 626a 6563 7420 6f72 2061 2043 6c69 656e  bject or a Clien
+0001bff0: 7420 696e 7374 616e 6365 2069 6e20 6f72  t instance in or
+0001c000: 6465 7220 746f 2065 6469 7420 7468 6520  der to edit the 
+0001c010: 6d65 7373 6167 6520 7769 7468 2074 6865  message with the
+0001c020: 2075 7064 6174 6564 2070 726f 6772 6573   updated progres
+0001c030: 7320 7374 6174 7573 2e0d 0a0d 0a20 2020  s status.....   
+0001c040: 2020 2020 204f 7468 6572 2050 6172 616d       Other Param
+0001c050: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
+0001c060: 2020 2020 6375 7272 656e 7420 2860 6069      current (``i
+0001c070: 6e74 6060 293a 0d0a 2020 2020 2020 2020  nt``):..        
+0001c080: 2020 2020 2020 2020 5468 6520 616d 6f75          The amou
+0001c090: 6e74 206f 6620 6279 7465 7320 7472 616e  nt of bytes tran
+0001c0a0: 736d 6974 7465 6420 736f 2066 6172 2e0d  smitted so far..
+0001c0b0: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+0001c0c0: 6f74 616c 2028 6060 696e 7460 6029 3a0d  otal (``int``):.
+0001c0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c0e0: 2054 6865 2074 6f74 616c 2073 697a 6520   The total size 
+0001c0f0: 6f66 2074 6865 2066 696c 652e 0d0a 0d0a  of the file.....
+0001c100: 2020 2020 2020 2020 2020 2020 2a61 7267              *arg
+0001c110: 7320 2860 6074 7570 6c65 6060 2c20 2a6f  s (``tuple``, *o
+0001c120: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+0001c130: 2020 2020 2020 2020 2020 2020 4578 7472              Extr
+0001c140: 6120 6375 7374 6f6d 2061 7267 756d 656e  a custom argumen
+0001c150: 7473 2061 7320 6465 6669 6e65 6420 696e  ts as defined in
+0001c160: 2074 6865 2060 6070 726f 6772 6573 735f   the ``progress_
+0001c170: 6172 6773 6060 2070 6172 616d 6574 6572  args`` parameter
+0001c180: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001c190: 2020 2059 6f75 2063 616e 2065 6974 6865     You can eithe
+0001c1a0: 7220 6b65 6570 2060 602a 6172 6773 6060  r keep ``*args``
+0001c1b0: 206f 7220 6164 6420 6576 6572 7920 7369   or add every si
+0001c1c0: 6e67 6c65 2065 7874 7261 2061 7267 756d  ngle extra argum
+0001c1d0: 656e 7420 696e 2079 6f75 7220 6675 6e63  ent in your func
+0001c1e0: 7469 6f6e 2073 6967 6e61 7475 7265 2e0d  tion signature..
+0001c1f0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0001c200: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+0001c210: 204f 6e20 7375 6363 6573 732c 2074 6865   On success, the
+0001c220: 2073 656e 7420 3a6f 626a 3a60 7e66 6970   sent :obj:`~fip
+0001c230: 7065 722e 7479 7065 732e 4d65 7373 6167  per.types.Messag
+0001c240: 6560 2069 7320 7265 7475 726e 6564 2e0d  e` is returned..
+0001c250: 0a20 2020 2020 2020 2020 2020 2049 6e20  .            In 
+0001c260: 6361 7365 2074 6865 2075 706c 6f61 6420  case the upload 
+0001c270: 6973 2064 656c 6962 6572 6174 656c 7920  is deliberately 
+0001c280: 7374 6f70 7065 6420 7769 7468 203a 6d65  stopped with :me
+0001c290: 7468 3a60 7e66 6970 7065 722e 436c 6965  th:`~fipper.Clie
+0001c2a0: 6e74 2e73 746f 705f 7472 616e 736d 6973  nt.stop_transmis
+0001c2b0: 7369 6f6e 602c 204e 6f6e 6520 6973 2072  sion`, None is r
+0001c2c0: 6574 7572 6e65 640d 0a20 2020 2020 2020  eturned..       
+0001c2d0: 2020 2020 2069 6e73 7465 6164 2e0d 0a0d       instead....
+0001c2e0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+0001c2f0: 0d0a 2020 2020 2020 2020 2020 2020 5250  ..            RP
+0001c300: 4345 7272 6f72 3a20 496e 2063 6173 6520  CError: In case 
+0001c310: 6f66 2061 2054 656c 6567 7261 6d20 5250  of a Telegram RP
+0001c320: 4320 6572 726f 722e 0d0a 2020 2020 2020  C error...      
+0001c330: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
+0001c340: 6620 7175 6f74 6520 6973 204e 6f6e 653a  f quote is None:
+0001c350: 0d0a 2020 2020 2020 2020 2020 2020 7175  ..            qu
+0001c360: 6f74 6520 3d20 7365 6c66 2e63 6861 742e  ote = self.chat.
+0001c370: 7479 7065 2021 3d20 656e 756d 732e 4368  type != enums.Ch
+0001c380: 6174 5479 7065 2e50 5249 5641 5445 0d0a  atType.PRIVATE..
+0001c390: 0d0a 2020 2020 2020 2020 6966 2072 6570  ..        if rep
+0001c3a0: 6c79 5f74 6f5f 6d65 7373 6167 655f 6964  ly_to_message_id
+0001c3b0: 2069 7320 4e6f 6e65 2061 6e64 2071 756f   is None and quo
+0001c3c0: 7465 3a0d 0a20 2020 2020 2020 2020 2020  te:..           
+0001c3d0: 2072 6570 6c79 5f74 6f5f 6d65 7373 6167   reply_to_messag
+0001c3e0: 655f 6964 203d 2073 656c 662e 6964 0d0a  e_id = self.id..
+0001c3f0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001c400: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
+0001c410: 656e 742e 7365 6e64 5f76 6f69 6365 280d  ent.send_voice(.
+0001c420: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+0001c430: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
+0001c440: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+0001c450: 766f 6963 653d 766f 6963 652c 0d0a 2020  voice=voice,..  
+0001c460: 2020 2020 2020 2020 2020 6361 7074 696f            captio
+0001c470: 6e3d 6361 7074 696f 6e2c 0d0a 2020 2020  n=caption,..    
+0001c480: 2020 2020 2020 2020 7061 7273 655f 6d6f          parse_mo
+0001c490: 6465 3d70 6172 7365 5f6d 6f64 652c 0d0a  de=parse_mode,..
+0001c4a0: 2020 2020 2020 2020 2020 2020 6361 7074              capt
+0001c4b0: 696f 6e5f 656e 7469 7469 6573 3d63 6170  ion_entities=cap
+0001c4c0: 7469 6f6e 5f65 6e74 6974 6965 732c 0d0a  tion_entities,..
+0001c4d0: 2020 2020 2020 2020 2020 2020 6475 7261              dura
+0001c4e0: 7469 6f6e 3d64 7572 6174 696f 6e2c 0d0a  tion=duration,..
+0001c4f0: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+0001c500: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+0001c510: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
+0001c520: 6174 696f 6e2c 0d0a 2020 2020 2020 2020  ation,..        
+0001c530: 2020 2020 7265 706c 795f 746f 5f6d 6573      reply_to_mes
+0001c540: 7361 6765 5f69 643d 7265 706c 795f 746f  sage_id=reply_to
+0001c550: 5f6d 6573 7361 6765 5f69 642c 0d0a 2020  _message_id,..  
+0001c560: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+0001c570: 6d61 726b 7570 3d72 6570 6c79 5f6d 6172  markup=reply_mar
+0001c580: 6b75 702c 0d0a 2020 2020 2020 2020 2020  kup,..          
+0001c590: 2020 7072 6f67 7265 7373 3d70 726f 6772    progress=progr
+0001c5a0: 6573 732c 0d0a 2020 2020 2020 2020 2020  ess,..          
+0001c5b0: 2020 7072 6f67 7265 7373 5f61 7267 733d    progress_args=
+0001c5c0: 7072 6f67 7265 7373 5f61 7267 730d 0a20  progress_args.. 
+0001c5d0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+0001c5e0: 6173 796e 6320 6465 6620 6564 6974 5f74  async def edit_t
+0001c5f0: 6578 7428 0d0a 2020 2020 2020 2020 7365  ext(..        se
+0001c600: 6c66 2c0d 0a20 2020 2020 2020 2074 6578  lf,..        tex
+0001c610: 743a 2073 7472 2c0d 0a20 2020 2020 2020  t: str,..       
+0001c620: 2070 6172 7365 5f6d 6f64 653a 204f 7074   parse_mode: Opt
+0001c630: 696f 6e61 6c5b 2265 6e75 6d73 2e50 6172  ional["enums.Par
+0001c640: 7365 4d6f 6465 225d 203d 204e 6f6e 652c  seMode"] = None,
+0001c650: 0d0a 2020 2020 2020 2020 656e 7469 7469  ..        entiti
+0001c660: 6573 3a20 4c69 7374 5b22 7479 7065 732e  es: List["types.
+0001c670: 4d65 7373 6167 6545 6e74 6974 7922 5d20  MessageEntity"] 
+0001c680: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+0001c690: 2064 6973 6162 6c65 5f77 6562 5f70 6167   disable_web_pag
+0001c6a0: 655f 7072 6576 6965 773a 2062 6f6f 6c20  e_preview: bool 
+0001c6b0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+0001c6c0: 2072 6570 6c79 5f6d 6172 6b75 703a 2022   reply_markup: "
+0001c6d0: 7479 7065 732e 496e 6c69 6e65 4b65 7962  types.InlineKeyb
+0001c6e0: 6f61 7264 4d61 726b 7570 2220 3d20 4e6f  oardMarkup" = No
+0001c6f0: 6e65 0d0a 2020 2020 2920 2d3e 2022 4d65  ne..    ) -> "Me
+0001c700: 7373 6167 6522 3a0d 0a20 2020 2020 2020  ssage":..       
+0001c710: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
+0001c720: 202a 6564 6974 5f74 6578 742a 206f 6620   *edit_text* of 
+0001c730: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
+0001c740: 7065 732e 4d65 7373 6167 6560 2e0d 0a0d  pes.Message`....
+0001c750: 0a20 2020 2020 2020 2041 6e20 616c 6961  .        An alia
+0001c760: 7320 6578 6973 7473 2061 7320 2a65 6469  s exists as *edi
+0001c770: 742a 2e0d 0a0d 0a20 2020 2020 2020 2055  t*.....        U
+0001c780: 7365 2061 7320 6120 7368 6f72 7463 7574  se as a shortcut
+0001c790: 2066 6f72 3a0d 0a0d 0a20 2020 2020 2020   for:....       
+0001c7a0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+0001c7b0: 2070 7974 686f 6e0d 0a0d 0a20 2020 2020   python....     
+0001c7c0: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
+0001c7d0: 656e 742e 6564 6974 5f6d 6573 7361 6765  ent.edit_message
+0001c7e0: 5f74 6578 7428 0d0a 2020 2020 2020 2020  _text(..        
+0001c7f0: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+0001c800: 6d65 7373 6167 652e 6368 6174 2e69 642c  message.chat.id,
+0001c810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c820: 2020 6d65 7373 6167 655f 6964 3d6d 6573    message_id=mes
+0001c830: 7361 6765 2e69 642c 0d0a 2020 2020 2020  sage.id,..      
+0001c840: 2020 2020 2020 2020 2020 7465 7874 3d22            text="
+0001c850: 6865 6c6c 6f22 0d0a 2020 2020 2020 2020  hello"..        
+0001c860: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+0001c870: 2045 7861 6d70 6c65 3a0d 0a20 2020 2020   Example:..     
+0001c880: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0001c890: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
+0001c8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c8b0: 2061 7761 6974 206d 6573 7361 6765 2e65   await message.e
+0001c8c0: 6469 745f 7465 7874 2822 6865 6c6c 6f22  dit_text("hello"
+0001c8d0: 290d 0a0d 0a20 2020 2020 2020 2050 6172  )....        Par
+0001c8e0: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+0001c8f0: 2020 2020 2020 7465 7874 2028 6060 7374        text (``st
+0001c900: 7260 6029 3a0d 0a20 2020 2020 2020 2020  r``):..         
+0001c910: 2020 2020 2020 204e 6577 2074 6578 7420         New text 
+0001c920: 6f66 2074 6865 206d 6573 7361 6765 2e0d  of the message..
+0001c930: 0a0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
+0001c940: 6172 7365 5f6d 6f64 6520 283a 6f62 6a3a  arse_mode (:obj:
+0001c950: 607e 6669 7070 6572 2e65 6e75 6d73 2e50  `~fipper.enums.P
+0001c960: 6172 7365 4d6f 6465 602c 202a 6f70 7469  arseMode`, *opti
+0001c970: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
+0001c980: 2020 2020 2020 2020 2042 7920 6465 6661           By defa
+0001c990: 756c 742c 2074 6578 7473 2061 7265 2070  ult, texts are p
+0001c9a0: 6172 7365 6420 7573 696e 6720 626f 7468  arsed using both
+0001c9b0: 204d 6172 6b64 6f77 6e20 616e 6420 4854   Markdown and HT
+0001c9c0: 4d4c 2073 7479 6c65 732e 0d0a 2020 2020  ML styles...    
+0001c9d0: 2020 2020 2020 2020 2020 2020 596f 7520              You 
+0001c9e0: 6361 6e20 636f 6d62 696e 6520 626f 7468  can combine both
+0001c9f0: 2073 796e 7461 7865 7320 746f 6765 7468   syntaxes togeth
+0001ca00: 6572 2e0d 0a0d 0a20 2020 2020 2020 2020  er.....         
+0001ca10: 2020 2065 6e74 6974 6965 7320 284c 6973     entities (Lis
+0001ca20: 7420 6f66 203a 6f62 6a3a 607e 6669 7070  t of :obj:`~fipp
+0001ca30: 6572 2e74 7970 6573 2e4d 6573 7361 6765  er.types.Message
+0001ca40: 456e 7469 7479 6029 3a0d 0a20 2020 2020  Entity`):..     
+0001ca50: 2020 2020 2020 2020 2020 204c 6973 7420             List 
+0001ca60: 6f66 2073 7065 6369 616c 2065 6e74 6974  of special entit
+0001ca70: 6965 7320 7468 6174 2061 7070 6561 7220  ies that appear 
+0001ca80: 696e 206d 6573 7361 6765 2074 6578 742c  in message text,
+0001ca90: 2077 6869 6368 2063 616e 2062 6520 7370   which can be sp
+0001caa0: 6563 6966 6965 6420 696e 7374 6561 6420  ecified instead 
+0001cab0: 6f66 202a 7061 7273 655f 6d6f 6465 2a2e  of *parse_mode*.
+0001cac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001cad0: 6469 7361 626c 655f 7765 625f 7061 6765  disable_web_page
+0001cae0: 5f70 7265 7669 6577 2028 6060 626f 6f6c  _preview (``bool
+0001caf0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+0001cb00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001cb10: 2020 4469 7361 626c 6573 206c 696e 6b20    Disables link 
+0001cb20: 7072 6576 6965 7773 2066 6f72 206c 696e  previews for lin
+0001cb30: 6b73 2069 6e20 7468 6973 206d 6573 7361  ks in this messa
+0001cb40: 6765 2e0d 0a0d 0a20 2020 2020 2020 2020  ge.....         
+0001cb50: 2020 2072 6570 6c79 5f6d 6172 6b75 7020     reply_markup 
+0001cb60: 283a 6f62 6a3a 607e 6669 7070 6572 2e74  (:obj:`~fipper.t
+0001cb70: 7970 6573 2e49 6e6c 696e 654b 6579 626f  ypes.InlineKeybo
+0001cb80: 6172 644d 6172 6b75 7060 2c20 2a6f 7074  ardMarkup`, *opt
+0001cb90: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+0001cba0: 2020 2020 2020 2020 2020 416e 2049 6e6c            An Inl
+0001cbb0: 696e 654b 6579 626f 6172 644d 6172 6b75  ineKeyboardMarku
+0001cbc0: 7020 6f62 6a65 6374 2e0d 0a0d 0a20 2020  p object.....   
+0001cbd0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+0001cbe0: 2020 2020 2020 2020 2020 204f 6e20 7375             On su
+0001cbf0: 6363 6573 732c 2074 6865 2065 6469 7465  ccess, the edite
+0001cc00: 6420 3a6f 626a 3a60 7e66 6970 7065 722e  d :obj:`~fipper.
+0001cc10: 7479 7065 732e 4d65 7373 6167 6560 2069  types.Message` i
+0001cc20: 7320 7265 7475 726e 6564 2e0d 0a0d 0a20  s returned..... 
+0001cc30: 2020 2020 2020 2052 6169 7365 733a 0d0a         Raises:..
+0001cc40: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
+0001cc50: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
+0001cc60: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
+0001cc70: 6572 726f 722e 0d0a 2020 2020 2020 2020  error...        
+0001cc80: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+0001cc90: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
+0001cca0: 636c 6965 6e74 2e65 6469 745f 6d65 7373  client.edit_mess
+0001ccb0: 6167 655f 7465 7874 280d 0a20 2020 2020  age_text(..     
+0001ccc0: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
+0001ccd0: 656c 662e 6368 6174 2e69 642c 0d0a 2020  elf.chat.id,..  
+0001cce0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+0001ccf0: 655f 6964 3d73 656c 662e 6964 2c0d 0a20  e_id=self.id,.. 
+0001cd00: 2020 2020 2020 2020 2020 2074 6578 743d             text=
+0001cd10: 7465 7874 2c0d 0a20 2020 2020 2020 2020  text,..         
+0001cd20: 2020 2070 6172 7365 5f6d 6f64 653d 7061     parse_mode=pa
+0001cd30: 7273 655f 6d6f 6465 2c0d 0a20 2020 2020  rse_mode,..     
+0001cd40: 2020 2020 2020 2065 6e74 6974 6965 733d         entities=
+0001cd50: 656e 7469 7469 6573 2c0d 0a20 2020 2020  entities,..     
+0001cd60: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
+0001cd70: 6562 5f70 6167 655f 7072 6576 6965 773d  eb_page_preview=
+0001cd80: 6469 7361 626c 655f 7765 625f 7061 6765  disable_web_page
+0001cd90: 5f70 7265 7669 6577 2c0d 0a20 2020 2020  _preview,..     
+0001cda0: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
+0001cdb0: 6b75 703d 7265 706c 795f 6d61 726b 7570  kup=reply_markup
+0001cdc0: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+0001cdd0: 2020 2065 6469 7420 3d20 6564 6974 5f74     edit = edit_t
+0001cde0: 6578 740d 0a0d 0a20 2020 2061 7379 6e63  ext....    async
+0001cdf0: 2064 6566 2065 6469 745f 6361 7074 696f   def edit_captio
+0001ce00: 6e28 0d0a 2020 2020 2020 2020 7365 6c66  n(..        self
+0001ce10: 2c0d 0a20 2020 2020 2020 2063 6170 7469  ,..        capti
+0001ce20: 6f6e 3a20 7374 722c 0d0a 2020 2020 2020  on: str,..      
+0001ce30: 2020 7061 7273 655f 6d6f 6465 3a20 4f70    parse_mode: Op
+0001ce40: 7469 6f6e 616c 5b22 656e 756d 732e 5061  tional["enums.Pa
+0001ce50: 7273 654d 6f64 6522 5d20 3d20 4e6f 6e65  rseMode"] = None
+0001ce60: 2c0d 0a20 2020 2020 2020 2063 6170 7469  ,..        capti
+0001ce70: 6f6e 5f65 6e74 6974 6965 733a 204c 6973  on_entities: Lis
+0001ce80: 745b 2274 7970 6573 2e4d 6573 7361 6765  t["types.Message
+0001ce90: 456e 7469 7479 225d 203d 204e 6f6e 652c  Entity"] = None,
+0001cea0: 0d0a 2020 2020 2020 2020 7265 706c 795f  ..        reply_
+0001ceb0: 6d61 726b 7570 3a20 2274 7970 6573 2e49  markup: "types.I
+0001cec0: 6e6c 696e 654b 6579 626f 6172 644d 6172  nlineKeyboardMar
+0001ced0: 6b75 7022 203d 204e 6f6e 650d 0a20 2020  kup" = None..   
+0001cee0: 2029 202d 3e20 224d 6573 7361 6765 223a   ) -> "Message":
+0001cef0: 0d0a 2020 2020 2020 2020 2222 2242 6f75  ..        """Bou
+0001cf00: 6e64 206d 6574 686f 6420 2a65 6469 745f  nd method *edit_
+0001cf10: 6361 7074 696f 6e2a 206f 6620 3a6f 626a  caption* of :obj
+0001cf20: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
+0001cf30: 4d65 7373 6167 6560 2e0d 0a0d 0a20 2020  Message`.....   
+0001cf40: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
+0001cf50: 6f72 7463 7574 2066 6f72 3a0d 0a0d 0a20  ortcut for:.... 
+0001cf60: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+0001cf70: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
+0001cf80: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+0001cf90: 6974 2063 6c69 656e 742e 6564 6974 5f6d  it client.edit_m
+0001cfa0: 6573 7361 6765 5f63 6170 7469 6f6e 280d  essage_caption(.
+0001cfb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cfc0: 2063 6861 745f 6964 3d6d 6573 7361 6765   chat_id=message
+0001cfd0: 2e63 6861 742e 6964 2c0d 0a20 2020 2020  .chat.id,..     
+0001cfe0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+0001cff0: 6765 5f69 643d 6d65 7373 6167 652e 6964  ge_id=message.id
+0001d000: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001d010: 2020 2063 6170 7469 6f6e 3d22 6865 6c6c     caption="hell
+0001d020: 6f22 0d0a 2020 2020 2020 2020 2020 2020  o"..            
+0001d030: 290d 0a0d 0a20 2020 2020 2020 2045 7861  )....        Exa
+0001d040: 6d70 6c65 3a0d 0a20 2020 2020 2020 2020  mple:..         
+0001d050: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+0001d060: 3a3a 2070 7974 686f 6e0d 0a0d 0a20 2020  :: python....   
+0001d070: 2020 2020 2020 2020 2020 2020 2061 7761               awa
+0001d080: 6974 206d 6573 7361 6765 2e65 6469 745f  it message.edit_
+0001d090: 6361 7074 696f 6e28 2268 656c 6c6f 2229  caption("hello")
+0001d0a0: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+0001d0b0: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+0001d0c0: 2020 2020 2063 6170 7469 6f6e 2028 6060       caption (``
+0001d0d0: 7374 7260 6029 3a0d 0a20 2020 2020 2020  str``):..       
+0001d0e0: 2020 2020 2020 2020 204e 6577 2063 6170           New cap
+0001d0f0: 7469 6f6e 206f 6620 7468 6520 6d65 7373  tion of the mess
+0001d100: 6167 652e 0d0a 0d0a 2020 2020 2020 2020  age.....        
+0001d110: 2020 2020 7061 7273 655f 6d6f 6465 2028      parse_mode (
+0001d120: 3a6f 626a 3a60 7e66 6970 7065 722e 656e  :obj:`~fipper.en
+0001d130: 756d 732e 5061 7273 654d 6f64 6560 2c20  ums.ParseMode`, 
+0001d140: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+0001d150: 2020 2020 2020 2020 2020 2020 2020 4279                By
+0001d160: 2064 6566 6175 6c74 2c20 7465 7874 7320   default, texts 
+0001d170: 6172 6520 7061 7273 6564 2075 7369 6e67  are parsed using
+0001d180: 2062 6f74 6820 4d61 726b 646f 776e 2061   both Markdown a
+0001d190: 6e64 2048 544d 4c20 7374 796c 6573 2e0d  nd HTML styles..
+0001d1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d1b0: 2059 6f75 2063 616e 2063 6f6d 6269 6e65   You can combine
+0001d1c0: 2062 6f74 6820 7379 6e74 6178 6573 2074   both syntaxes t
+0001d1d0: 6f67 6574 6865 722e 0d0a 0d0a 2020 2020  ogether.....    
+0001d1e0: 2020 2020 2020 2020 6361 7074 696f 6e5f          caption_
+0001d1f0: 656e 7469 7469 6573 2028 4c69 7374 206f  entities (List o
+0001d200: 6620 3a6f 626a 3a60 7e66 6970 7065 722e  f :obj:`~fipper.
+0001d210: 7479 7065 732e 4d65 7373 6167 6545 6e74  types.MessageEnt
+0001d220: 6974 7960 293a 0d0a 2020 2020 2020 2020  ity`):..        
+0001d230: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
+0001d240: 7370 6563 6961 6c20 656e 7469 7469 6573  special entities
+0001d250: 2074 6861 7420 6170 7065 6172 2069 6e20   that appear in 
+0001d260: 7468 6520 6361 7074 696f 6e2c 2077 6869  the caption, whi
+0001d270: 6368 2063 616e 2062 6520 7370 6563 6966  ch can be specif
+0001d280: 6965 6420 696e 7374 6561 6420 6f66 202a  ied instead of *
+0001d290: 7061 7273 655f 6d6f 6465 2a2e 0d0a 0d0a  parse_mode*.....
+0001d2a0: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+0001d2b0: 795f 6d61 726b 7570 2028 3a6f 626a 3a60  y_markup (:obj:`
+0001d2c0: 7e66 6970 7065 722e 7479 7065 732e 496e  ~fipper.types.In
+0001d2d0: 6c69 6e65 4b65 7962 6f61 7264 4d61 726b  lineKeyboardMark
+0001d2e0: 7570 602c 202a 6f70 7469 6f6e 616c 2a29  up`, *optional*)
+0001d2f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001d300: 2020 2041 6e20 496e 6c69 6e65 4b65 7962     An InlineKeyb
+0001d310: 6f61 7264 4d61 726b 7570 206f 626a 6563  oardMarkup objec
+0001d320: 742e 0d0a 0d0a 2020 2020 2020 2020 5265  t.....        Re
+0001d330: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+0001d340: 2020 2020 4f6e 2073 7563 6365 7373 2c20      On success, 
+0001d350: 7468 6520 6564 6974 6564 203a 6f62 6a3a  the edited :obj:
+0001d360: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
+0001d370: 6573 7361 6765 6020 6973 2072 6574 7572  essage` is retur
+0001d380: 6e65 642e 0d0a 0d0a 2020 2020 2020 2020  ned.....        
+0001d390: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+0001d3a0: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+0001d3b0: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+0001d3c0: 6772 616d 2052 5043 2065 7272 6f72 2e0d  gram RPC error..
+0001d3d0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0001d3e0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0001d3f0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+0001d400: 6564 6974 5f6d 6573 7361 6765 5f63 6170  edit_message_cap
+0001d410: 7469 6f6e 280d 0a20 2020 2020 2020 2020  tion(..         
+0001d420: 2020 2063 6861 745f 6964 3d73 656c 662e     chat_id=self.
+0001d430: 6368 6174 2e69 642c 0d0a 2020 2020 2020  chat.id,..      
+0001d440: 2020 2020 2020 6d65 7373 6167 655f 6964        message_id
+0001d450: 3d73 656c 662e 6964 2c0d 0a20 2020 2020  =self.id,..     
+0001d460: 2020 2020 2020 2063 6170 7469 6f6e 3d63         caption=c
+0001d470: 6170 7469 6f6e 2c0d 0a20 2020 2020 2020  aption,..       
+0001d480: 2020 2020 2070 6172 7365 5f6d 6f64 653d       parse_mode=
+0001d490: 7061 7273 655f 6d6f 6465 2c0d 0a20 2020  parse_mode,..   
+0001d4a0: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
+0001d4b0: 5f65 6e74 6974 6965 733d 6361 7074 696f  _entities=captio
+0001d4c0: 6e5f 656e 7469 7469 6573 2c0d 0a20 2020  n_entities,..   
+0001d4d0: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+0001d4e0: 6172 6b75 703d 7265 706c 795f 6d61 726b  arkup=reply_mark
+0001d4f0: 7570 0d0a 2020 2020 2020 2020 290d 0a0d  up..        )...
+0001d500: 0a20 2020 2061 7379 6e63 2064 6566 2065  .    async def e
+0001d510: 6469 745f 6d65 6469 6128 0d0a 2020 2020  dit_media(..    
+0001d520: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+0001d530: 2020 206d 6564 6961 3a20 2274 7970 6573     media: "types
+0001d540: 2e49 6e70 7574 4d65 6469 6122 2c0d 0a20  .InputMedia",.. 
+0001d550: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
+0001d560: 6b75 703a 2022 7479 7065 732e 496e 6c69  kup: "types.Inli
+0001d570: 6e65 4b65 7962 6f61 7264 4d61 726b 7570  neKeyboardMarkup
+0001d580: 2220 3d20 4e6f 6e65 0d0a 2020 2020 2920  " = None..    ) 
+0001d590: 2d3e 2022 4d65 7373 6167 6522 3a0d 0a20  -> "Message":.. 
+0001d5a0: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
+0001d5b0: 6d65 7468 6f64 202a 6564 6974 5f6d 6564  method *edit_med
+0001d5c0: 6961 2a20 6f66 203a 6f62 6a3a 607e 6669  ia* of :obj:`~fi
+0001d5d0: 7070 6572 2e74 7970 6573 2e4d 6573 7361  pper.types.Messa
+0001d5e0: 6765 602e 0d0a 0d0a 2020 2020 2020 2020  ge`.....        
+0001d5f0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
+0001d600: 7420 666f 723a 0d0a 0d0a 2020 2020 2020  t for:....      
+0001d610: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+0001d620: 3a20 7079 7468 6f6e 0d0a 0d0a 2020 2020  : python....    
+0001d630: 2020 2020 2020 2020 6177 6169 7420 636c          await cl
+0001d640: 6965 6e74 2e65 6469 745f 6d65 7373 6167  ient.edit_messag
+0001d650: 655f 6d65 6469 6128 0d0a 2020 2020 2020  e_media(..      
+0001d660: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
+0001d670: 643d 6d65 7373 6167 652e 6368 6174 2e69  d=message.chat.i
+0001d680: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+0001d690: 2020 2020 6d65 7373 6167 655f 6964 3d6d      message_id=m
+0001d6a0: 6573 7361 6765 2e69 642c 0d0a 2020 2020  essage.id,..    
+0001d6b0: 2020 2020 2020 2020 2020 2020 6d65 6469              medi
+0001d6c0: 613d 6d65 6469 610d 0a20 2020 2020 2020  a=media..       
+0001d6d0: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+0001d6e0: 2020 4578 616d 706c 653a 0d0a 2020 2020    Example:..    
+0001d6f0: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+0001d700: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0d0a  block:: python..
+0001d710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d720: 2020 6177 6169 7420 6d65 7373 6167 652e    await message.
+0001d730: 6564 6974 5f6d 6564 6961 286d 6564 6961  edit_media(media
+0001d740: 290d 0a0d 0a20 2020 2020 2020 2050 6172  )....        Par
+0001d750: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+0001d760: 2020 2020 2020 6d65 6469 6120 283a 6f62        media (:ob
+0001d770: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+0001d780: 2e49 6e70 7574 4d65 6469 6160 293a 0d0a  .InputMedia`):..
+0001d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7a0: 4f6e 6520 6f66 2074 6865 2049 6e70 7574  One of the Input
+0001d7b0: 4d65 6469 6120 6f62 6a65 6374 7320 6465  Media objects de
+0001d7c0: 7363 7269 6269 6e67 2061 6e20 616e 696d  scribing an anim
+0001d7d0: 6174 696f 6e2c 2061 7564 696f 2c20 646f  ation, audio, do
+0001d7e0: 6375 6d65 6e74 2c20 7068 6f74 6f20 6f72  cument, photo or
+0001d7f0: 2076 6964 656f 2e0d 0a0d 0a20 2020 2020   video.....     
+0001d800: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
+0001d810: 6b75 7020 283a 6f62 6a3a 607e 6669 7070  kup (:obj:`~fipp
+0001d820: 6572 2e74 7970 6573 2e49 6e6c 696e 654b  er.types.InlineK
+0001d830: 6579 626f 6172 644d 6172 6b75 7060 2c20  eyboardMarkup`, 
+0001d840: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+0001d850: 2020 2020 2020 2020 2020 2020 2020 416e                An
+0001d860: 2049 6e6c 696e 654b 6579 626f 6172 644d   InlineKeyboardM
+0001d870: 6172 6b75 7020 6f62 6a65 6374 2e0d 0a0d  arkup object....
+0001d880: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0001d890: 3a0d 0a20 2020 2020 2020 2020 2020 204f  :..            O
+0001d8a0: 6e20 7375 6363 6573 732c 2074 6865 2065  n success, the e
+0001d8b0: 6469 7465 6420 3a6f 626a 3a60 7e66 6970  dited :obj:`~fip
+0001d8c0: 7065 722e 7479 7065 732e 4d65 7373 6167  per.types.Messag
+0001d8d0: 6560 2069 7320 7265 7475 726e 6564 2e0d  e` is returned..
+0001d8e0: 0a0d 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+0001d8f0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0001d900: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+0001d910: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+0001d920: 5250 4320 6572 726f 722e 0d0a 2020 2020  RPC error...    
+0001d930: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0001d940: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+0001d950: 6c66 2e5f 636c 6965 6e74 2e65 6469 745f  lf._client.edit_
+0001d960: 6d65 7373 6167 655f 6d65 6469 6128 0d0a  message_media(..
+0001d970: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+0001d980: 5f69 643d 7365 6c66 2e63 6861 742e 6964  _id=self.chat.id
+0001d990: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+0001d9a0: 6573 7361 6765 5f69 643d 7365 6c66 2e69  essage_id=self.i
+0001d9b0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+0001d9c0: 6d65 6469 613d 6d65 6469 612c 0d0a 2020  media=media,..  
+0001d9d0: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+0001d9e0: 6d61 726b 7570 3d72 6570 6c79 5f6d 6172  markup=reply_mar
+0001d9f0: 6b75 700d 0a20 2020 2020 2020 2029 0d0a  kup..        )..
+0001da00: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+0001da10: 6564 6974 5f72 6570 6c79 5f6d 6172 6b75  edit_reply_marku
+0001da20: 7028 7365 6c66 2c20 7265 706c 795f 6d61  p(self, reply_ma
+0001da30: 726b 7570 3a20 2274 7970 6573 2e49 6e6c  rkup: "types.Inl
+0001da40: 696e 654b 6579 626f 6172 644d 6172 6b75  ineKeyboardMarku
+0001da50: 7022 203d 204e 6f6e 6529 202d 3e20 224d  p" = None) -> "M
+0001da60: 6573 7361 6765 223a 0d0a 2020 2020 2020  essage":..      
+0001da70: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
+0001da80: 6420 2a65 6469 745f 7265 706c 795f 6d61  d *edit_reply_ma
+0001da90: 726b 7570 2a20 6f66 203a 6f62 6a3a 607e  rkup* of :obj:`~
+0001daa0: 6669 7070 6572 2e74 7970 6573 2e4d 6573  fipper.types.Mes
+0001dab0: 7361 6765 602e 0d0a 0d0a 2020 2020 2020  sage`.....      
+0001dac0: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
+0001dad0: 6375 7420 666f 723a 0d0a 0d0a 2020 2020  cut for:....    
+0001dae0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+0001daf0: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
+0001db00: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+0001db10: 636c 6965 6e74 2e65 6469 745f 6d65 7373  client.edit_mess
+0001db20: 6167 655f 7265 706c 795f 6d61 726b 7570  age_reply_markup
+0001db30: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001db40: 2020 2063 6861 745f 6964 3d6d 6573 7361     chat_id=messa
+0001db50: 6765 2e63 6861 742e 6964 2c0d 0a20 2020  ge.chat.id,..   
+0001db60: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+0001db70: 7361 6765 5f69 643d 6d65 7373 6167 652e  sage_id=message.
+0001db80: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+0001db90: 2020 2020 2072 6570 6c79 5f6d 6172 6b75       reply_marku
+0001dba0: 703d 696e 6c69 6e65 5f72 6570 6c79 5f6d  p=inline_reply_m
+0001dbb0: 6172 6b75 700d 0a20 2020 2020 2020 2020  arkup..         
+0001dbc0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+0001dbd0: 4578 616d 706c 653a 0d0a 2020 2020 2020  Example:..      
+0001dbe0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+0001dbf0: 6f63 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a  ock:: python....
+0001dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc10: 6177 6169 7420 6d65 7373 6167 652e 6564  await message.ed
+0001dc20: 6974 5f72 6570 6c79 5f6d 6172 6b75 7028  it_reply_markup(
+0001dc30: 696e 6c69 6e65 5f72 6570 6c79 5f6d 6172  inline_reply_mar
+0001dc40: 6b75 7029 0d0a 0d0a 2020 2020 2020 2020  kup)....        
+0001dc50: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
+0001dc60: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+0001dc70: 6172 6b75 7020 283a 6f62 6a3a 607e 6669  arkup (:obj:`~fi
+0001dc80: 7070 6572 2e74 7970 6573 2e49 6e6c 696e  pper.types.Inlin
+0001dc90: 654b 6579 626f 6172 644d 6172 6b75 7060  eKeyboardMarkup`
+0001dca0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001dcb0: 2020 2020 416e 2049 6e6c 696e 654b 6579      An InlineKey
+0001dcc0: 626f 6172 644d 6172 6b75 7020 6f62 6a65  boardMarkup obje
+0001dcd0: 6374 2e0d 0a0d 0a20 2020 2020 2020 2052  ct.....        R
+0001dce0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+0001dcf0: 2020 2020 204f 6e20 7375 6363 6573 732c       On success,
+0001dd00: 2069 6620 6564 6974 6564 206d 6573 7361   if edited messa
+0001dd10: 6765 2069 7320 7365 6e74 2062 7920 7468  ge is sent by th
+0001dd20: 6520 626f 742c 2074 6865 2065 6469 7465  e bot, the edite
+0001dd30: 640d 0a20 2020 2020 2020 2020 2020 203a  d..            :
+0001dd40: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+0001dd50: 6573 2e4d 6573 7361 6765 6020 6973 2072  es.Message` is r
+0001dd60: 6574 7572 6e65 642c 206f 7468 6572 7769  eturned, otherwi
+0001dd70: 7365 2054 7275 6520 6973 2072 6574 7572  se True is retur
+0001dd80: 6e65 642e 0d0a 0d0a 2020 2020 2020 2020  ned.....        
+0001dd90: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+0001dda0: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+0001ddb0: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+0001ddc0: 6772 616d 2052 5043 2065 7272 6f72 2e0d  gram RPC error..
+0001ddd0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0001dde0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0001ddf0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+0001de00: 6564 6974 5f6d 6573 7361 6765 5f72 6570  edit_message_rep
+0001de10: 6c79 5f6d 6172 6b75 7028 0d0a 2020 2020  ly_markup(..    
+0001de20: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+0001de30: 7365 6c66 2e63 6861 742e 6964 2c0d 0a20  self.chat.id,.. 
+0001de40: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+0001de50: 6765 5f69 643d 7365 6c66 2e69 642c 0d0a  ge_id=self.id,..
+0001de60: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+0001de70: 795f 6d61 726b 7570 3d72 6570 6c79 5f6d  y_markup=reply_m
+0001de80: 6172 6b75 700d 0a20 2020 2020 2020 2029  arkup..        )
+0001de90: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
+0001dea0: 6620 666f 7277 6172 6428 0d0a 2020 2020  f forward(..    
+0001deb0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+0001dec0: 2020 2063 6861 745f 6964 3a20 556e 696f     chat_id: Unio
+0001ded0: 6e5b 696e 742c 2073 7472 5d2c 0d0a 2020  n[int, str],..  
+0001dee0: 2020 2020 2020 6469 7361 626c 655f 6e6f        disable_no
+0001def0: 7469 6669 6361 7469 6f6e 3a20 626f 6f6c  tification: bool
+0001df00: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0001df10: 2020 7363 6865 6475 6c65 5f64 6174 653a    schedule_date:
+0001df20: 2064 6174 6574 696d 6520 3d20 4e6f 6e65   datetime = None
+0001df30: 0d0a 2020 2020 2920 2d3e 2055 6e69 6f6e  ..    ) -> Union
+0001df40: 5b22 7479 7065 732e 4d65 7373 6167 6522  ["types.Message"
+0001df50: 2c20 4c69 7374 5b22 7479 7065 732e 4d65  , List["types.Me
+0001df60: 7373 6167 6522 5d5d 3a0d 0a20 2020 2020  ssage"]]:..     
+0001df70: 2020 2022 2222 426f 756e 6420 6d65 7468     """Bound meth
+0001df80: 6f64 202a 666f 7277 6172 642a 206f 6620  od *forward* of 
+0001df90: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
+0001dfa0: 7065 732e 4d65 7373 6167 6560 2e0d 0a0d  pes.Message`....
+0001dfb0: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
+0001dfc0: 6120 7368 6f72 7463 7574 2066 6f72 3a0d  a shortcut for:.
+0001dfd0: 0a0d 0a20 2020 2020 2020 202e 2e20 636f  ...        .. co
+0001dfe0: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+0001dff0: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
+0001e000: 2061 7761 6974 2063 6c69 656e 742e 666f   await client.fo
+0001e010: 7277 6172 645f 6d65 7373 6167 6573 280d  rward_messages(.
+0001e020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e030: 2063 6861 745f 6964 3d63 6861 745f 6964   chat_id=chat_id
+0001e040: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001e050: 2020 2066 726f 6d5f 6368 6174 5f69 643d     from_chat_id=
+0001e060: 6d65 7373 6167 652e 6368 6174 2e69 642c  message.chat.id,
+0001e070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e080: 2020 6d65 7373 6167 655f 6964 733d 6d65    message_ids=me
+0001e090: 7373 6167 652e 6964 0d0a 2020 2020 2020  ssage.id..      
+0001e0a0: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+0001e0b0: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
+0001e0c0: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
+0001e0d0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
+0001e0e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001e0f0: 2020 2061 7761 6974 206d 6573 7361 6765     await message
+0001e100: 2e66 6f72 7761 7264 2863 6861 745f 6964  .forward(chat_id
+0001e110: 290d 0a0d 0a20 2020 2020 2020 2050 6172  )....        Par
+0001e120: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+0001e130: 2020 2020 2020 6368 6174 5f69 6420 2860        chat_id (`
+0001e140: 6069 6e74 6060 207c 2060 6073 7472 6060  `int`` | ``str``
+0001e150: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001e160: 2020 2020 556e 6971 7565 2069 6465 6e74      Unique ident
+0001e170: 6966 6965 7220 2869 6e74 2920 6f72 2075  ifier (int) or u
+0001e180: 7365 726e 616d 6520 2873 7472 2920 6f66  sername (str) of
+0001e190: 2074 6865 2074 6172 6765 7420 6368 6174   the target chat
+0001e1a0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001e1b0: 2020 2046 6f72 2079 6f75 7220 7065 7273     For your pers
+0001e1c0: 6f6e 616c 2063 6c6f 7564 2028 5361 7665  onal cloud (Save
+0001e1d0: 6420 4d65 7373 6167 6573 2920 796f 7520  d Messages) you 
+0001e1e0: 6361 6e20 7369 6d70 6c79 2075 7365 2022  can simply use "
+0001e1f0: 6d65 2220 6f72 2022 7365 6c66 222e 0d0a  me" or "self"...
+0001e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e210: 466f 7220 6120 636f 6e74 6163 7420 7468  For a contact th
+0001e220: 6174 2065 7869 7374 7320 696e 2079 6f75  at exists in you
+0001e230: 7220 5465 6c65 6772 616d 2061 6464 7265  r Telegram addre
+0001e240: 7373 2062 6f6f 6b20 796f 7520 6361 6e20  ss book you can 
+0001e250: 7573 6520 6869 7320 7068 6f6e 6520 6e75  use his phone nu
+0001e260: 6d62 6572 2028 7374 7229 2e0d 0a0d 0a20  mber (str)..... 
+0001e270: 2020 2020 2020 2020 2020 2064 6973 6162             disab
+0001e280: 6c65 5f6e 6f74 6966 6963 6174 696f 6e20  le_notification 
+0001e290: 2860 6062 6f6f 6c60 602c 202a 6f70 7469  (``bool``, *opti
+0001e2a0: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
+0001e2b0: 2020 2020 2020 2020 2053 656e 6473 2074           Sends t
+0001e2c0: 6865 206d 6573 7361 6765 2073 696c 656e  he message silen
+0001e2d0: 746c 792e 0d0a 2020 2020 2020 2020 2020  tly...          
+0001e2e0: 2020 2020 2020 5573 6572 7320 7769 6c6c        Users will
+0001e2f0: 2072 6563 6569 7665 2061 206e 6f74 6966   receive a notif
+0001e300: 6963 6174 696f 6e20 7769 7468 206e 6f20  ication with no 
+0001e310: 736f 756e 642e 0d0a 0d0a 2020 2020 2020  sound.....      
+0001e320: 2020 2020 2020 7363 6865 6475 6c65 5f64        schedule_d
+0001e330: 6174 6520 283a 7079 3a6f 626a 3a60 7e64  ate (:py:obj:`~d
+0001e340: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+0001e350: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+0001e360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e370: 2044 6174 6520 7768 656e 2074 6865 206d   Date when the m
+0001e380: 6573 7361 6765 2077 696c 6c20 6265 2061  essage will be a
+0001e390: 7574 6f6d 6174 6963 616c 6c79 2073 656e  utomatically sen
+0001e3a0: 742e 0d0a 0d0a 2020 2020 2020 2020 5265  t.....        Re
+0001e3b0: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+0001e3c0: 2020 2020 4f6e 2073 7563 6365 7373 2c20      On success, 
+0001e3d0: 7468 6520 666f 7277 6172 6465 6420 4d65  the forwarded Me
+0001e3e0: 7373 6167 6520 6973 2072 6574 7572 6e65  ssage is returne
+0001e3f0: 642e 0d0a 0d0a 2020 2020 2020 2020 5261  d.....        Ra
+0001e400: 6973 6573 3a0d 0a20 2020 2020 2020 2020  ises:..         
+0001e410: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
+0001e420: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
+0001e430: 616d 2052 5043 2065 7272 6f72 2e0d 0a20  am RPC error... 
+0001e440: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0001e450: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+0001e460: 2073 656c 662e 5f63 6c69 656e 742e 666f   self._client.fo
+0001e470: 7277 6172 645f 6d65 7373 6167 6573 280d  rward_messages(.
+0001e480: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+0001e490: 745f 6964 3d63 6861 745f 6964 2c0d 0a20  t_id=chat_id,.. 
+0001e4a0: 2020 2020 2020 2020 2020 2066 726f 6d5f             from_
+0001e4b0: 6368 6174 5f69 643d 7365 6c66 2e63 6861  chat_id=self.cha
+0001e4c0: 742e 6964 2c0d 0a20 2020 2020 2020 2020  t.id,..         
+0001e4d0: 2020 206d 6573 7361 6765 5f69 6473 3d73     message_ids=s
+0001e4e0: 656c 662e 6964 2c0d 0a20 2020 2020 2020  elf.id,..       
+0001e4f0: 2020 2020 2064 6973 6162 6c65 5f6e 6f74       disable_not
+0001e500: 6966 6963 6174 696f 6e3d 6469 7361 626c  ification=disabl
+0001e510: 655f 6e6f 7469 6669 6361 7469 6f6e 2c0d  e_notification,.
+0001e520: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
+0001e530: 6564 756c 655f 6461 7465 3d73 6368 6564  edule_date=sched
+0001e540: 756c 655f 6461 7465 0d0a 2020 2020 2020  ule_date..      
+0001e550: 2020 290d 0a0d 0a20 2020 2061 7379 6e63    )....    async
+0001e560: 2064 6566 2063 6f70 7928 0d0a 2020 2020   def copy(..    
+0001e570: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+0001e580: 2020 2063 6861 745f 6964 3a20 556e 696f     chat_id: Unio
+0001e590: 6e5b 696e 742c 2073 7472 5d2c 0d0a 2020  n[int, str],..  
+0001e5a0: 2020 2020 2020 6361 7074 696f 6e3a 2073        caption: s
+0001e5b0: 7472 203d 204e 6f6e 652c 0d0a 2020 2020  tr = None,..    
+0001e5c0: 2020 2020 7061 7273 655f 6d6f 6465 3a20      parse_mode: 
+0001e5d0: 4f70 7469 6f6e 616c 5b22 656e 756d 732e  Optional["enums.
+0001e5e0: 5061 7273 654d 6f64 6522 5d20 3d20 4e6f  ParseMode"] = No
+0001e5f0: 6e65 2c0d 0a20 2020 2020 2020 2063 6170  ne,..        cap
+0001e600: 7469 6f6e 5f65 6e74 6974 6965 733a 204c  tion_entities: L
+0001e610: 6973 745b 2274 7970 6573 2e4d 6573 7361  ist["types.Messa
+0001e620: 6765 456e 7469 7479 225d 203d 204e 6f6e  geEntity"] = Non
+0001e630: 652c 0d0a 2020 2020 2020 2020 6469 7361  e,..        disa
+0001e640: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
+0001e650: 3a20 626f 6f6c 203d 204e 6f6e 652c 0d0a  : bool = None,..
+0001e660: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
+0001e670: 5f6d 6573 7361 6765 5f69 643a 2069 6e74  _message_id: int
+0001e680: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0001e690: 2020 7363 6865 6475 6c65 5f64 6174 653a    schedule_date:
+0001e6a0: 2064 6174 6574 696d 6520 3d20 4e6f 6e65   datetime = None
+0001e6b0: 2c0d 0a20 2020 2020 2020 2070 726f 7465  ,..        prote
+0001e6c0: 6374 5f63 6f6e 7465 6e74 3a20 626f 6f6c  ct_content: bool
+0001e6d0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+0001e6e0: 2020 7265 706c 795f 6d61 726b 7570 3a20    reply_markup: 
+0001e6f0: 556e 696f 6e5b 0d0a 2020 2020 2020 2020  Union[..        
+0001e700: 2020 2020 2274 7970 6573 2e49 6e6c 696e      "types.Inlin
+0001e710: 654b 6579 626f 6172 644d 6172 6b75 7022  eKeyboardMarkup"
+0001e720: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+0001e730: 7479 7065 732e 5265 706c 794b 6579 626f  types.ReplyKeybo
+0001e740: 6172 644d 6172 6b75 7022 2c0d 0a20 2020  ardMarkup",..   
+0001e750: 2020 2020 2020 2020 2022 7479 7065 732e           "types.
+0001e760: 5265 706c 794b 6579 626f 6172 6452 656d  ReplyKeyboardRem
+0001e770: 6f76 6522 2c0d 0a20 2020 2020 2020 2020  ove",..         
+0001e780: 2020 2022 7479 7065 732e 466f 7263 6552     "types.ForceR
+0001e790: 6570 6c79 220d 0a20 2020 2020 2020 205d  eply"..        ]
+0001e7a0: 203d 206f 626a 6563 740d 0a20 2020 2029   = object..    )
+0001e7b0: 202d 3e20 556e 696f 6e5b 2274 7970 6573   -> Union["types
+0001e7c0: 2e4d 6573 7361 6765 222c 204c 6973 745b  .Message", List[
+0001e7d0: 2274 7970 6573 2e4d 6573 7361 6765 225d  "types.Message"]
+0001e7e0: 5d3a 0d0a 2020 2020 2020 2020 2222 2242  ]:..        """B
+0001e7f0: 6f75 6e64 206d 6574 686f 6420 2a63 6f70  ound method *cop
+0001e800: 792a 206f 6620 3a6f 626a 3a60 7e66 6970  y* of :obj:`~fip
+0001e810: 7065 722e 7479 7065 732e 4d65 7373 6167  per.types.Messag
+0001e820: 6560 2e0d 0a0d 0a20 2020 2020 2020 2055  e`.....        U
+0001e830: 7365 2061 7320 6120 7368 6f72 7463 7574  se as a shortcut
+0001e840: 2066 6f72 3a0d 0a0d 0a20 2020 2020 2020   for:....       
+0001e850: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+0001e860: 2070 7974 686f 6e0d 0a0d 0a20 2020 2020   python....     
+0001e870: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
+0001e880: 656e 742e 636f 7079 5f6d 6573 7361 6765  ent.copy_message
+0001e890: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001e8a0: 2020 2063 6861 745f 6964 3d63 6861 745f     chat_id=chat_
+0001e8b0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+0001e8c0: 2020 2020 2066 726f 6d5f 6368 6174 5f69       from_chat_i
+0001e8d0: 643d 6d65 7373 6167 652e 6368 6174 2e69  d=message.chat.i
+0001e8e0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+0001e8f0: 2020 2020 6d65 7373 6167 655f 6964 3d6d      message_id=m
+0001e900: 6573 7361 6765 2e69 640d 0a20 2020 2020  essage.id..     
+0001e910: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+0001e920: 2020 2020 4578 616d 706c 653a 0d0a 2020      Example:..  
+0001e930: 2020 2020 2020 2020 2020 2e2e 2063 6f64            .. cod
+0001e940: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+0001e950: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001e960: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
+0001e970: 652e 636f 7079 2863 6861 745f 6964 290d  e.copy(chat_id).
+0001e980: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0001e990: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
+0001e9a0: 2020 2020 6368 6174 5f69 6420 2860 6069      chat_id (``i
+0001e9b0: 6e74 6060 207c 2060 6073 7472 6060 293a  nt`` | ``str``):
+0001e9c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e9d0: 2020 556e 6971 7565 2069 6465 6e74 6966    Unique identif
+0001e9e0: 6965 7220 2869 6e74 2920 6f72 2075 7365  ier (int) or use
+0001e9f0: 726e 616d 6520 2873 7472 2920 6f66 2074  rname (str) of t
+0001ea00: 6865 2074 6172 6765 7420 6368 6174 2e0d  he target chat..
+0001ea10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ea20: 2046 6f72 2079 6f75 7220 7065 7273 6f6e   For your person
+0001ea30: 616c 2063 6c6f 7564 2028 5361 7665 6420  al cloud (Saved 
+0001ea40: 4d65 7373 6167 6573 2920 796f 7520 6361  Messages) you ca
+0001ea50: 6e20 7369 6d70 6c79 2075 7365 2022 6d65  n simply use "me
+0001ea60: 2220 6f72 2022 7365 6c66 222e 0d0a 2020  " or "self"...  
+0001ea70: 2020 2020 2020 2020 2020 2020 2020 466f                Fo
+0001ea80: 7220 6120 636f 6e74 6163 7420 7468 6174  r a contact that
+0001ea90: 2065 7869 7374 7320 696e 2079 6f75 7220   exists in your 
+0001eaa0: 5465 6c65 6772 616d 2061 6464 7265 7373  Telegram address
+0001eab0: 2062 6f6f 6b20 796f 7520 6361 6e20 7573   book you can us
+0001eac0: 6520 6869 7320 7068 6f6e 6520 6e75 6d62  e his phone numb
+0001ead0: 6572 2028 7374 7229 2e0d 0a0d 0a20 2020  er (str).....   
+0001eae0: 2020 2020 2020 2020 2063 6170 7469 6f6e           caption
+0001eaf0: 2028 6060 7374 7269 6e67 6060 2c20 2a6f   (``string``, *o
+0001eb00: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+0001eb10: 2020 2020 2020 2020 2020 2020 4e65 7720              New 
+0001eb20: 6361 7074 696f 6e20 666f 7220 6d65 6469  caption for medi
+0001eb30: 612c 2030 2d31 3032 3420 6368 6172 6163  a, 0-1024 charac
+0001eb40: 7465 7273 2061 6674 6572 2065 6e74 6974  ters after entit
+0001eb50: 6965 7320 7061 7273 696e 672e 0d0a 2020  ies parsing...  
+0001eb60: 2020 2020 2020 2020 2020 2020 2020 4966                If
+0001eb70: 206e 6f74 2073 7065 6369 6669 6564 2c20   not specified, 
+0001eb80: 7468 6520 6f72 6967 696e 616c 2063 6170  the original cap
+0001eb90: 7469 6f6e 2069 7320 6b65 7074 2e0d 0a20  tion is kept... 
+0001eba0: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+0001ebb0: 6173 7320 2222 2028 656d 7074 7920 7374  ass "" (empty st
+0001ebc0: 7269 6e67 2920 746f 2072 656d 6f76 6520  ring) to remove 
+0001ebd0: 7468 6520 6361 7074 696f 6e2e 0d0a 0d0a  the caption.....
+0001ebe0: 2020 2020 2020 2020 2020 2020 7061 7273              pars
+0001ebf0: 655f 6d6f 6465 2028 3a6f 626a 3a60 7e66  e_mode (:obj:`~f
+0001ec00: 6970 7065 722e 656e 756d 732e 5061 7273  ipper.enums.Pars
+0001ec10: 654d 6f64 6560 2c20 2a6f 7074 696f 6e61  eMode`, *optiona
+0001ec20: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+0001ec30: 2020 2020 2020 4279 2064 6566 6175 6c74        By default
+0001ec40: 2c20 7465 7874 7320 6172 6520 7061 7273  , texts are pars
+0001ec50: 6564 2075 7369 6e67 2062 6f74 6820 4d61  ed using both Ma
+0001ec60: 726b 646f 776e 2061 6e64 2048 544d 4c20  rkdown and HTML 
+0001ec70: 7374 796c 6573 2e0d 0a20 2020 2020 2020  styles...       
+0001ec80: 2020 2020 2020 2020 2059 6f75 2063 616e           You can
+0001ec90: 2063 6f6d 6269 6e65 2062 6f74 6820 7379   combine both sy
+0001eca0: 6e74 6178 6573 2074 6f67 6574 6865 722e  ntaxes together.
+0001ecb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001ecc0: 6361 7074 696f 6e5f 656e 7469 7469 6573  caption_entities
+0001ecd0: 2028 4c69 7374 206f 6620 3a6f 626a 3a60   (List of :obj:`
+0001ece0: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
+0001ecf0: 7373 6167 6545 6e74 6974 7960 293a 0d0a  ssageEntity`):..
+0001ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed10: 4c69 7374 206f 6620 7370 6563 6961 6c20  List of special 
+0001ed20: 656e 7469 7469 6573 2074 6861 7420 6170  entities that ap
+0001ed30: 7065 6172 2069 6e20 7468 6520 6e65 7720  pear in the new 
+0001ed40: 6361 7074 696f 6e2c 2077 6869 6368 2063  caption, which c
+0001ed50: 616e 2062 6520 7370 6563 6966 6965 6420  an be specified 
+0001ed60: 696e 7374 6561 6420 6f66 202a 7061 7273  instead of *pars
+0001ed70: 655f 6d6f 6465 2a2e 0d0a 0d0a 2020 2020  e_mode*.....    
+0001ed80: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+0001ed90: 6e6f 7469 6669 6361 7469 6f6e 2028 6060  notification (``
+0001eda0: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
+0001edb0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+0001edc0: 2020 2020 2020 5365 6e64 7320 7468 6520        Sends the 
+0001edd0: 6d65 7373 6167 6520 7369 6c65 6e74 6c79  message silently
+0001ede0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001edf0: 2020 2055 7365 7273 2077 696c 6c20 7265     Users will re
+0001ee00: 6365 6976 6520 6120 6e6f 7469 6669 6361  ceive a notifica
+0001ee10: 7469 6f6e 2077 6974 6820 6e6f 2073 6f75  tion with no sou
+0001ee20: 6e64 2e0d 0a0d 0a20 2020 2020 2020 2020  nd.....         
+0001ee30: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
+0001ee40: 6167 655f 6964 2028 6060 696e 7460 602c  age_id (``int``,
+0001ee50: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
+0001ee60: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+0001ee70: 6620 7468 6520 6d65 7373 6167 6520 6973  f the message is
+0001ee80: 2061 2072 6570 6c79 2c20 4944 206f 6620   a reply, ID of 
+0001ee90: 7468 6520 6f72 6967 696e 616c 206d 6573  the original mes
+0001eea0: 7361 6765 2e0d 0a0d 0a20 2020 2020 2020  sage.....       
+0001eeb0: 2020 2020 2073 6368 6564 756c 655f 6461       schedule_da
+0001eec0: 7465 2028 3a70 793a 6f62 6a3a 607e 6461  te (:py:obj:`~da
+0001eed0: 7465 7469 6d65 2e64 6174 6574 696d 6560  tetime.datetime`
+0001eee0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+0001eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ef00: 4461 7465 2077 6865 6e20 7468 6520 6d65  Date when the me
+0001ef10: 7373 6167 6520 7769 6c6c 2062 6520 6175  ssage will be au
+0001ef20: 746f 6d61 7469 6361 6c6c 7920 7365 6e74  tomatically sent
+0001ef30: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+0001ef40: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
+0001ef50: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+0001ef60: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+0001ef70: 2020 2020 2020 2020 2020 5072 6f74 6563            Protec
+0001ef80: 7473 2074 6865 2063 6f6e 7465 6e74 7320  ts the contents 
+0001ef90: 6f66 2074 6865 2073 656e 7420 6d65 7373  of the sent mess
+0001efa0: 6167 6520 6672 6f6d 2066 6f72 7761 7264  age from forward
+0001efb0: 696e 6720 616e 6420 7361 7669 6e67 2e0d  ing and saving..
+0001efc0: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+0001efd0: 6570 6c79 5f6d 6172 6b75 7020 283a 6f62  eply_markup (:ob
+0001efe0: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+0001eff0: 2e49 6e6c 696e 654b 6579 626f 6172 644d  .InlineKeyboardM
+0001f000: 6172 6b75 7060 207c 203a 6f62 6a3a 607e  arkup` | :obj:`~
+0001f010: 6669 7070 6572 2e74 7970 6573 2e52 6570  fipper.types.Rep
+0001f020: 6c79 4b65 7962 6f61 7264 4d61 726b 7570  lyKeyboardMarkup
+0001f030: 6020 7c20 3a6f 626a 3a60 7e66 6970 7065  ` | :obj:`~fippe
+0001f040: 722e 7479 7065 732e 5265 706c 794b 6579  r.types.ReplyKey
+0001f050: 626f 6172 6452 656d 6f76 6560 207c 203a  boardRemove` | :
+0001f060: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+0001f070: 6573 2e46 6f72 6365 5265 706c 7960 2c20  es.ForceReply`, 
+0001f080: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+0001f090: 2020 2020 2020 2020 2020 2020 2020 4164                Ad
+0001f0a0: 6469 7469 6f6e 616c 2069 6e74 6572 6661  ditional interfa
+0001f0b0: 6365 206f 7074 696f 6e73 2e20 416e 206f  ce options. An o
+0001f0c0: 626a 6563 7420 666f 7220 616e 2069 6e6c  bject for an inl
+0001f0d0: 696e 6520 6b65 7962 6f61 7264 2c20 6375  ine keyboard, cu
+0001f0e0: 7374 6f6d 2072 6570 6c79 206b 6579 626f  stom reply keybo
+0001f0f0: 6172 642c 0d0a 2020 2020 2020 2020 2020  ard,..          
+0001f100: 2020 2020 2020 696e 7374 7275 6374 696f        instructio
+0001f110: 6e73 2074 6f20 7265 6d6f 7665 2072 6570  ns to remove rep
+0001f120: 6c79 206b 6579 626f 6172 6420 6f72 2074  ly keyboard or t
+0001f130: 6f20 666f 7263 6520 6120 7265 706c 7920  o force a reply 
+0001f140: 6672 6f6d 2074 6865 2075 7365 722e 0d0a  from the user...
+0001f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f160: 4966 206e 6f74 2073 7065 6369 6669 6564  If not specified
+0001f170: 2c20 7468 6520 6f72 6967 696e 616c 2072  , the original r
+0001f180: 6570 6c79 206d 6172 6b75 7020 6973 206b  eply markup is k
+0001f190: 6570 742e 0d0a 2020 2020 2020 2020 2020  ept...          
+0001f1a0: 2020 2020 2020 5061 7373 204e 6f6e 6520        Pass None 
+0001f1b0: 746f 2072 656d 6f76 6520 7468 6520 7265  to remove the re
+0001f1c0: 706c 7920 6d61 726b 7570 2e0d 0a0d 0a20  ply markup..... 
+0001f1d0: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
+0001f1e0: 0a20 2020 2020 2020 2020 2020 203a 6f62  .            :ob
+0001f1f0: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+0001f200: 2e4d 6573 7361 6765 603a 204f 6e20 7375  .Message`: On su
+0001f210: 6363 6573 732c 2074 6865 2063 6f70 6965  ccess, the copie
+0001f220: 6420 6d65 7373 6167 6520 6973 2072 6574  d message is ret
+0001f230: 7572 6e65 642e 0d0a 0d0a 2020 2020 2020  urned.....      
+0001f240: 2020 5261 6973 6573 3a0d 0a20 2020 2020    Raises:..     
+0001f250: 2020 2020 2020 2052 5043 4572 726f 723a         RPCError:
+0001f260: 2049 6e20 6361 7365 206f 6620 6120 5465   In case of a Te
+0001f270: 6c65 6772 616d 2052 5043 2065 7272 6f72  legram RPC error
+0001f280: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+0001f290: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001f2a0: 7365 7276 6963 653a 0d0a 2020 2020 2020  service:..      
+0001f2b0: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+0001f2c0: 6728 6622 5365 7276 6963 6520 6d65 7373  g(f"Service mess
+0001f2d0: 6167 6573 2063 616e 6e6f 7420 6265 2063  ages cannot be c
+0001f2e0: 6f70 6965 642e 2022 0d0a 2020 2020 2020  opied. "..      
+0001f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f300: 2020 6622 6368 6174 5f69 643a 207b 7365    f"chat_id: {se
+0001f310: 6c66 2e63 6861 742e 6964 7d2c 206d 6573  lf.chat.id}, mes
+0001f320: 7361 6765 5f69 643a 207b 7365 6c66 2e69  sage_id: {self.i
+0001f330: 647d 2229 0d0a 2020 2020 2020 2020 656c  d}")..        el
+0001f340: 6966 2073 656c 662e 6761 6d65 2061 6e64  if self.game and
+0001f350: 206e 6f74 2061 7761 6974 2073 656c 662e   not await self.
+0001f360: 5f63 6c69 656e 742e 7374 6f72 6167 652e  _client.storage.
+0001f370: 6973 5f62 6f74 2829 3a0d 0a20 2020 2020  is_bot():..     
+0001f380: 2020 2020 2020 206c 6f67 2e77 6172 6e69         log.warni
+0001f390: 6e67 2866 2255 7365 7273 2063 616e 6e6f  ng(f"Users canno
+0001f3a0: 7420 7365 6e64 206d 6573 7361 6765 7320  t send messages 
+0001f3b0: 7769 7468 2047 616d 6520 6d65 6469 6120  with Game media 
+0001f3c0: 7479 7065 2e20 220d 0a20 2020 2020 2020  type. "..       
+0001f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3e0: 2066 2263 6861 745f 6964 3a20 7b73 656c   f"chat_id: {sel
+0001f3f0: 662e 6368 6174 2e69 647d 2c20 6d65 7373  f.chat.id}, mess
+0001f400: 6167 655f 6964 3a20 7b73 656c 662e 6964  age_id: {self.id
+0001f410: 7d22 290d 0a20 2020 2020 2020 2065 6c69  }")..        eli
+0001f420: 6620 7365 6c66 2e65 6d70 7479 3a0d 0a20  f self.empty:.. 
+0001f430: 2020 2020 2020 2020 2020 206c 6f67 2e77             log.w
+0001f440: 6172 6e69 6e67 2866 2245 6d70 7479 206d  arning(f"Empty m
+0001f450: 6573 7361 6765 7320 6361 6e6e 6f74 2062  essages cannot b
+0001f460: 6520 636f 7069 6564 2e20 2229 0d0a 2020  e copied. ")..  
+0001f470: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+0001f480: 7465 7874 3a0d 0a20 2020 2020 2020 2020  text:..         
+0001f490: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+0001f4a0: 7365 6c66 2e5f 636c 6965 6e74 2e73 656e  self._client.sen
+0001f4b0: 645f 6d65 7373 6167 6528 0d0a 2020 2020  d_message(..    
+0001f4c0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+0001f4d0: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
+0001f4e0: 2020 2020 2020 7465 7874 3d73 656c 662e        text=self.
+0001f4f0: 7465 7874 2c0d 0a20 2020 2020 2020 2020  text,..         
+0001f500: 2020 2020 2020 2065 6e74 6974 6965 733d         entities=
+0001f510: 7365 6c66 2e65 6e74 6974 6965 732c 0d0a  self.entities,..
+0001f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f530: 7061 7273 655f 6d6f 6465 3d65 6e75 6d73  parse_mode=enums
+0001f540: 2e50 6172 7365 4d6f 6465 2e44 4953 4142  .ParseMode.DISAB
+0001f550: 4c45 442c 0d0a 2020 2020 2020 2020 2020  LED,..          
+0001f560: 2020 2020 2020 6469 7361 626c 655f 7765        disable_we
+0001f570: 625f 7061 6765 5f70 7265 7669 6577 3d6e  b_page_preview=n
+0001f580: 6f74 2073 656c 662e 7765 625f 7061 6765  ot self.web_page
+0001f590: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001f5a0: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+0001f5b0: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
+0001f5c0: 6e6f 7469 6669 6361 7469 6f6e 2c0d 0a20  notification,.. 
+0001f5d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001f5e0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+0001f5f0: 6964 3d72 6570 6c79 5f74 6f5f 6d65 7373  id=reply_to_mess
+0001f600: 6167 655f 6964 2c0d 0a20 2020 2020 2020  age_id,..       
+0001f610: 2020 2020 2020 2020 2073 6368 6564 756c           schedul
+0001f620: 655f 6461 7465 3d73 6368 6564 756c 655f  e_date=schedule_
+0001f630: 6461 7465 2c0d 0a20 2020 2020 2020 2020  date,..         
+0001f640: 2020 2020 2020 2070 726f 7465 6374 5f63         protect_c
+0001f650: 6f6e 7465 6e74 3d70 726f 7465 6374 5f63  ontent=protect_c
+0001f660: 6f6e 7465 6e74 2c0d 0a20 2020 2020 2020  ontent,..       
+0001f670: 2020 2020 2020 2020 2072 6570 6c79 5f6d           reply_m
+0001f680: 6172 6b75 703d 7365 6c66 2e72 6570 6c79  arkup=self.reply
+0001f690: 5f6d 6172 6b75 7020 6966 2072 6570 6c79  _markup if reply
+0001f6a0: 5f6d 6172 6b75 7020 6973 206f 626a 6563  _markup is objec
+0001f6b0: 7420 656c 7365 2072 6570 6c79 5f6d 6172  t else reply_mar
+0001f6c0: 6b75 700d 0a20 2020 2020 2020 2020 2020  kup..           
+0001f6d0: 2029 0d0a 2020 2020 2020 2020 656c 6966   )..        elif
+0001f6e0: 2073 656c 662e 6d65 6469 613a 0d0a 2020   self.media:..  
+0001f6f0: 2020 2020 2020 2020 2020 7365 6e64 5f6d            send_m
+0001f700: 6564 6961 203d 2070 6172 7469 616c 280d  edia = partial(.
+0001f710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f720: 2073 656c 662e 5f63 6c69 656e 742e 7365   self._client.se
+0001f730: 6e64 5f63 6163 6865 645f 6d65 6469 612c  nd_cached_media,
+0001f740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f750: 2020 6368 6174 5f69 643d 6368 6174 5f69    chat_id=chat_i
+0001f760: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+0001f770: 2020 2020 6469 7361 626c 655f 6e6f 7469      disable_noti
+0001f780: 6669 6361 7469 6f6e 3d64 6973 6162 6c65  fication=disable
+0001f790: 5f6e 6f74 6966 6963 6174 696f 6e2c 0d0a  _notification,..
+0001f7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f7b0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+0001f7c0: 5f69 643d 7265 706c 795f 746f 5f6d 6573  _id=reply_to_mes
+0001f7d0: 7361 6765 5f69 642c 0d0a 2020 2020 2020  sage_id,..      
+0001f7e0: 2020 2020 2020 2020 2020 7363 6865 6475            schedu
+0001f7f0: 6c65 5f64 6174 653d 7363 6865 6475 6c65  le_date=schedule
+0001f800: 5f64 6174 652c 0d0a 2020 2020 2020 2020  _date,..        
+0001f810: 2020 2020 2020 2020 7072 6f74 6563 745f          protect_
+0001f820: 636f 6e74 656e 743d 7072 6f74 6563 745f  content=protect_
+0001f830: 636f 6e74 656e 742c 0d0a 2020 2020 2020  content,..      
+0001f840: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+0001f850: 6d61 726b 7570 3d73 656c 662e 7265 706c  markup=self.repl
+0001f860: 795f 6d61 726b 7570 2069 6620 7265 706c  y_markup if repl
+0001f870: 795f 6d61 726b 7570 2069 7320 6f62 6a65  y_markup is obje
+0001f880: 6374 2065 6c73 6520 7265 706c 795f 6d61  ct else reply_ma
+0001f890: 726b 7570 0d0a 2020 2020 2020 2020 2020  rkup..          
+0001f8a0: 2020 290d 0a0d 0a20 2020 2020 2020 2020    )....         
+0001f8b0: 2020 2069 6620 7365 6c66 2e70 686f 746f     if self.photo
+0001f8c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001f8d0: 2020 2066 696c 655f 6964 203d 2073 656c     file_id = sel
+0001f8e0: 662e 7068 6f74 6f2e 6669 6c65 5f69 640d  f.photo.file_id.
+0001f8f0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0001f900: 6620 7365 6c66 2e61 7564 696f 3a0d 0a20  f self.audio:.. 
+0001f910: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001f920: 696c 655f 6964 203d 2073 656c 662e 6175  ile_id = self.au
+0001f930: 6469 6f2e 6669 6c65 5f69 640d 0a20 2020  dio.file_id..   
+0001f940: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
+0001f950: 6c66 2e64 6f63 756d 656e 743a 0d0a 2020  lf.document:..  
+0001f960: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0001f970: 6c65 5f69 6420 3d20 7365 6c66 2e64 6f63  le_id = self.doc
+0001f980: 756d 656e 742e 6669 6c65 5f69 640d 0a20  ument.file_id.. 
+0001f990: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0001f9a0: 7365 6c66 2e76 6964 656f 3a0d 0a20 2020  self.video:..   
+0001f9b0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0001f9c0: 655f 6964 203d 2073 656c 662e 7669 6465  e_id = self.vide
+0001f9d0: 6f2e 6669 6c65 5f69 640d 0a20 2020 2020  o.file_id..     
+0001f9e0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+0001f9f0: 2e61 6e69 6d61 7469 6f6e 3a0d 0a20 2020  .animation:..   
+0001fa00: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0001fa10: 655f 6964 203d 2073 656c 662e 616e 696d  e_id = self.anim
+0001fa20: 6174 696f 6e2e 6669 6c65 5f69 640d 0a20  ation.file_id.. 
+0001fa30: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0001fa40: 7365 6c66 2e76 6f69 6365 3a0d 0a20 2020  self.voice:..   
+0001fa50: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0001fa60: 655f 6964 203d 2073 656c 662e 766f 6963  e_id = self.voic
+0001fa70: 652e 6669 6c65 5f69 640d 0a20 2020 2020  e.file_id..     
+0001fa80: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+0001fa90: 2e73 7469 636b 6572 3a0d 0a20 2020 2020  .sticker:..     
+0001faa0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+0001fab0: 6964 203d 2073 656c 662e 7374 6963 6b65  id = self.sticke
+0001fac0: 722e 6669 6c65 5f69 640d 0a20 2020 2020  r.file_id..     
+0001fad0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+0001fae0: 2e76 6964 656f 5f6e 6f74 653a 0d0a 2020  .video_note:..  
+0001faf0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0001fb00: 6c65 5f69 6420 3d20 7365 6c66 2e76 6964  le_id = self.vid
+0001fb10: 656f 5f6e 6f74 652e 6669 6c65 5f69 640d  eo_note.file_id.
+0001fb20: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0001fb30: 6620 7365 6c66 2e63 6f6e 7461 6374 3a0d  f self.contact:.
+0001fb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fb50: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+0001fb60: 6c66 2e5f 636c 6965 6e74 2e73 656e 645f  lf._client.send_
+0001fb70: 636f 6e74 6163 7428 0d0a 2020 2020 2020  contact(..      
+0001fb80: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+0001fb90: 6174 5f69 642c 0d0a 2020 2020 2020 2020  at_id,..        
+0001fba0: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
+0001fbb0: 655f 6e75 6d62 6572 3d73 656c 662e 636f  e_number=self.co
+0001fbc0: 6e74 6163 742e 7068 6f6e 655f 6e75 6d62  ntact.phone_numb
+0001fbd0: 6572 2c0d 0a20 2020 2020 2020 2020 2020  er,..           
+0001fbe0: 2020 2020 2020 2020 2066 6972 7374 5f6e           first_n
+0001fbf0: 616d 653d 7365 6c66 2e63 6f6e 7461 6374  ame=self.contact
+0001fc00: 2e66 6972 7374 5f6e 616d 652c 0d0a 2020  .first_name,..  
+0001fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fc20: 2020 6c61 7374 5f6e 616d 653d 7365 6c66    last_name=self
+0001fc30: 2e63 6f6e 7461 6374 2e6c 6173 745f 6e61  .contact.last_na
+0001fc40: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
+0001fc50: 2020 2020 2020 2020 2076 6361 7264 3d73           vcard=s
+0001fc60: 656c 662e 636f 6e74 6163 742e 7663 6172  elf.contact.vcar
+0001fc70: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+0001fc80: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+0001fc90: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
+0001fca0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+0001fcb0: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
+0001fcc0: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+0001fcd0: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
+0001fce0: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
+0001fcf0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0001fd00: 2020 2020 656c 6966 2073 656c 662e 6c6f      elif self.lo
+0001fd10: 6361 7469 6f6e 3a0d 0a20 2020 2020 2020  cation:..       
+0001fd20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001fd30: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+0001fd40: 6e74 2e73 656e 645f 6c6f 6361 7469 6f6e  nt.send_location
+0001fd50: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001fd60: 2020 2020 2020 2063 6861 745f 6964 2c0d         chat_id,.
+0001fd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fd80: 2020 2020 206c 6174 6974 7564 653d 7365       latitude=se
+0001fd90: 6c66 2e6c 6f63 6174 696f 6e2e 6c61 7469  lf.location.lati
+0001fda0: 7475 6465 2c0d 0a20 2020 2020 2020 2020  tude,..         
+0001fdb0: 2020 2020 2020 2020 2020 206c 6f6e 6769             longi
+0001fdc0: 7475 6465 3d73 656c 662e 6c6f 6361 7469  tude=self.locati
+0001fdd0: 6f6e 2e6c 6f6e 6769 7475 6465 2c0d 0a20  on.longitude,.. 
+0001fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fdf0: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+0001fe00: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
+0001fe10: 6e6f 7469 6669 6361 7469 6f6e 2c0d 0a20  notification,.. 
+0001fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe30: 2020 2073 6368 6564 756c 655f 6461 7465     schedule_date
+0001fe40: 3d73 6368 6564 756c 655f 6461 7465 0d0a  =schedule_date..
+0001fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe60: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0001fe70: 6c69 6620 7365 6c66 2e76 656e 7565 3a0d  lif self.venue:.
+0001fe80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fe90: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+0001fea0: 6c66 2e5f 636c 6965 6e74 2e73 656e 645f  lf._client.send_
+0001feb0: 7665 6e75 6528 0d0a 2020 2020 2020 2020  venue(..        
+0001fec0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+0001fed0: 5f69 642c 0d0a 2020 2020 2020 2020 2020  _id,..          
+0001fee0: 2020 2020 2020 2020 2020 6c61 7469 7475            latitu
+0001fef0: 6465 3d73 656c 662e 7665 6e75 652e 6c6f  de=self.venue.lo
+0001ff00: 6361 7469 6f6e 2e6c 6174 6974 7564 652c  cation.latitude,
+0001ff10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ff20: 2020 2020 2020 6c6f 6e67 6974 7564 653d        longitude=
+0001ff30: 7365 6c66 2e76 656e 7565 2e6c 6f63 6174  self.venue.locat
+0001ff40: 696f 6e2e 6c6f 6e67 6974 7564 652c 0d0a  ion.longitude,..
+0001ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff60: 2020 2020 7469 746c 653d 7365 6c66 2e76      title=self.v
+0001ff70: 656e 7565 2e74 6974 6c65 2c0d 0a20 2020  enue.title,..   
+0001ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff90: 2061 6464 7265 7373 3d73 656c 662e 7665   address=self.ve
+0001ffa0: 6e75 652e 6164 6472 6573 732c 0d0a 2020  nue.address,..  
+0001ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffc0: 2020 666f 7572 7371 7561 7265 5f69 643d    foursquare_id=
+0001ffd0: 7365 6c66 2e76 656e 7565 2e66 6f75 7273  self.venue.fours
+0001ffe0: 7175 6172 655f 6964 2c0d 0a20 2020 2020  quare_id,..     
+0001fff0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00020000: 6f75 7273 7175 6172 655f 7479 7065 3d73  oursquare_type=s
+00020010: 656c 662e 7665 6e75 652e 666f 7572 7371  elf.venue.foursq
+00020020: 7561 7265 5f74 7970 652c 0d0a 2020 2020  uare_type,..    
+00020030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020040: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00020050: 7469 6f6e 3d64 6973 6162 6c65 5f6e 6f74  tion=disable_not
+00020060: 6966 6963 6174 696f 6e2c 0d0a 2020 2020  ification,..    
+00020070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020080: 7363 6865 6475 6c65 5f64 6174 653d 7363  schedule_date=sc
+00020090: 6865 6475 6c65 5f64 6174 650d 0a20 2020  hedule_date..   
+000200a0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+000200b0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000200c0: 2073 656c 662e 706f 6c6c 3a0d 0a20 2020   self.poll:..   
+000200d0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000200e0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
+000200f0: 636c 6965 6e74 2e73 656e 645f 706f 6c6c  client.send_poll
+00020100: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00020110: 2020 2020 2020 2063 6861 745f 6964 2c0d         chat_id,.
+00020120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020130: 2020 2020 2071 7565 7374 696f 6e3d 7365       question=se
+00020140: 6c66 2e70 6f6c 6c2e 7175 6573 7469 6f6e  lf.poll.question
+00020150: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00020160: 2020 2020 2020 206f 7074 696f 6e73 3d5b         options=[
+00020170: 6f70 742e 7465 7874 2066 6f72 206f 7074  opt.text for opt
+00020180: 2069 6e20 7365 6c66 2e70 6f6c 6c2e 6f70   in self.poll.op
+00020190: 7469 6f6e 735d 2c0d 0a20 2020 2020 2020  tions],..       
+000201a0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000201b0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+000201c0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
+000201d0: 6361 7469 6f6e 2c0d 0a20 2020 2020 2020  cation,..       
+000201e0: 2020 2020 2020 2020 2020 2020 2073 6368               sch
+000201f0: 6564 756c 655f 6461 7465 3d73 6368 6564  edule_date=sched
+00020200: 756c 655f 6461 7465 0d0a 2020 2020 2020  ule_date..      
+00020210: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00020220: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
+00020230: 6c66 2e67 616d 653a 0d0a 2020 2020 2020  lf.game:..      
+00020240: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00020250: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
+00020260: 656e 742e 7365 6e64 5f67 616d 6528 0d0a  ent.send_game(..
+00020270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020280: 2020 2020 6368 6174 5f69 642c 0d0a 2020      chat_id,..  
+00020290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000202a0: 2020 6761 6d65 5f73 686f 7274 5f6e 616d    game_short_nam
+000202b0: 653d 7365 6c66 2e67 616d 652e 7368 6f72  e=self.game.shor
+000202c0: 745f 6e61 6d65 2c0d 0a20 2020 2020 2020  t_name,..       
+000202d0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000202e0: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+000202f0: 6e3d 6469 7361 626c 655f 6e6f 7469 6669  n=disable_notifi
+00020300: 6361 7469 6f6e 0d0a 2020 2020 2020 2020  cation..        
+00020310: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00020320: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00020330: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00020340: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00020350: 556e 6b6e 6f77 6e20 6d65 6469 6120 7479  Unknown media ty
+00020360: 7065 2229 0d0a 0d0a 2020 2020 2020 2020  pe")....        
+00020370: 2020 2020 6966 2073 656c 662e 7374 6963      if self.stic
+00020380: 6b65 7220 6f72 2073 656c 662e 7669 6465  ker or self.vide
+00020390: 6f5f 6e6f 7465 3a20 2023 2053 7469 636b  o_note:  # Stick
+000203a0: 6572 2061 6e64 2056 6964 656f 4e6f 7465  er and VideoNote
+000203b0: 2073 686f 756c 6420 6861 7665 206e 6f20   should have no 
+000203c0: 6361 7074 696f 6e0d 0a20 2020 2020 2020  caption..       
+000203d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000203e0: 6177 6169 7420 7365 6e64 5f6d 6564 6961  await send_media
+000203f0: 2866 696c 655f 6964 3d66 696c 655f 6964  (file_id=file_id
+00020400: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00020410: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00020420: 2020 2020 2020 6966 2063 6170 7469 6f6e        if caption
+00020430: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00020440: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00020450: 6170 7469 6f6e 203d 2073 656c 662e 6361  aption = self.ca
+00020460: 7074 696f 6e20 6f72 2022 220d 0a20 2020  ption or ""..   
+00020470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020480: 2063 6170 7469 6f6e 5f65 6e74 6974 6965   caption_entitie
+00020490: 7320 3d20 7365 6c66 2e63 6170 7469 6f6e  s = self.caption
+000204a0: 5f65 6e74 6974 6965 730d 0a0d 0a20 2020  _entities....   
+000204b0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000204c0: 7572 6e20 6177 6169 7420 7365 6e64 5f6d  urn await send_m
+000204d0: 6564 6961 280d 0a20 2020 2020 2020 2020  edia(..         
+000204e0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+000204f0: 6964 3d66 696c 655f 6964 2c0d 0a20 2020  id=file_id,..   
+00020500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020510: 2063 6170 7469 6f6e 3d63 6170 7469 6f6e   caption=caption
+00020520: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00020530: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
+00020540: 653d 7061 7273 655f 6d6f 6465 2c0d 0a20  e=parse_mode,.. 
+00020550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020560: 2020 2063 6170 7469 6f6e 5f65 6e74 6974     caption_entit
+00020570: 6965 733d 6361 7074 696f 6e5f 656e 7469  ies=caption_enti
+00020580: 7469 6573 0d0a 2020 2020 2020 2020 2020  ties..          
+00020590: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000205a0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000205b0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000205c0: 7272 6f72 2822 4361 6e27 7420 636f 7079  rror("Can't copy
+000205d0: 2074 6869 7320 6d65 7373 6167 6522 290d   this message").
+000205e0: 0a0d 0a20 2020 2061 7379 6e63 2064 6566  ...    async def
+000205f0: 2064 656c 6574 6528 7365 6c66 2c20 7265   delete(self, re
+00020600: 766f 6b65 3a20 626f 6f6c 203d 2054 7275  voke: bool = Tru
+00020610: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
+00020620: 426f 756e 6420 6d65 7468 6f64 202a 6465  Bound method *de
+00020630: 6c65 7465 2a20 6f66 203a 6f62 6a3a 607e  lete* of :obj:`~
+00020640: 6669 7070 6572 2e74 7970 6573 2e4d 6573  fipper.types.Mes
+00020650: 7361 6765 602e 0d0a 0d0a 2020 2020 2020  sage`.....      
+00020660: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
+00020670: 6375 7420 666f 723a 0d0a 0d0a 2020 2020  cut for:....    
+00020680: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+00020690: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
+000206a0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+000206b0: 636c 6965 6e74 2e64 656c 6574 655f 6d65  client.delete_me
+000206c0: 7373 6167 6573 280d 0a20 2020 2020 2020  ssages(..       
+000206d0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+000206e0: 3d63 6861 745f 6964 2c0d 0a20 2020 2020  =chat_id,..     
+000206f0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00020700: 6765 5f69 6473 3d6d 6573 7361 6765 2e69  ge_ids=message.i
+00020710: 640d 0a20 2020 2020 2020 2020 2020 2029  d..            )
+00020720: 0d0a 0d0a 2020 2020 2020 2020 4578 616d  ....        Exam
+00020730: 706c 653a 0d0a 2020 2020 2020 2020 2020  ple:..          
+00020740: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00020750: 3a20 7079 7468 6f6e 0d0a 0d0a 2020 2020  : python....    
+00020760: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00020770: 7420 6d65 7373 6167 652e 6465 6c65 7465  t message.delete
+00020780: 2829 0d0a 0d0a 2020 2020 2020 2020 5061  ()....        Pa
+00020790: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
+000207a0: 2020 2020 2020 2072 6576 6f6b 6520 2860         revoke (`
+000207b0: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
+000207c0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+000207d0: 2020 2020 2020 2044 656c 6574 6573 206d         Deletes m
+000207e0: 6573 7361 6765 7320 6f6e 2062 6f74 6820  essages on both 
+000207f0: 7061 7274 732e 0d0a 2020 2020 2020 2020  parts...        
+00020800: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+00020810: 6f6e 6c79 2066 6f72 2070 7269 7661 7465  only for private
+00020820: 2063 6c6f 7564 2063 6861 7473 2061 6e64   cloud chats and
+00020830: 206e 6f72 6d61 6c20 6772 6f75 7073 2c20   normal groups, 
+00020840: 6d65 7373 6167 6573 206f 6e0d 0a20 2020  messages on..   
+00020850: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00020860: 6e6e 656c 7320 616e 6420 7375 7065 7267  nnels and superg
+00020870: 726f 7570 7320 6172 6520 616c 7761 7973  roups are always
+00020880: 2072 6576 6f6b 6564 2028 692e 652e 3a20   revoked (i.e.: 
+00020890: 6465 6c65 7465 6420 666f 7220 6576 6572  deleted for ever
+000208a0: 796f 6e65 292e 0d0a 2020 2020 2020 2020  yone)...        
+000208b0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+000208c0: 2074 6f20 5472 7565 2e0d 0a0d 0a20 2020   to True.....   
+000208d0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+000208e0: 2020 2020 2020 2020 2020 2054 7275 6520             True 
+000208f0: 6f6e 2073 7563 6365 7373 2c20 4661 6c73  on success, Fals
+00020900: 6520 6f74 6865 7277 6973 652e 0d0a 0d0a  e otherwise.....
+00020910: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
+00020920: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
+00020930: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
+00020940: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
+00020950: 2065 7272 6f72 2e0d 0a20 2020 2020 2020   error...       
+00020960: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+00020970: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00020980: 5f63 6c69 656e 742e 6465 6c65 7465 5f6d  _client.delete_m
+00020990: 6573 7361 6765 7328 0d0a 2020 2020 2020  essages(..      
+000209a0: 2020 2020 2020 6368 6174 5f69 643d 7365        chat_id=se
+000209b0: 6c66 2e63 6861 742e 6964 2c0d 0a20 2020  lf.chat.id,..   
+000209c0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000209d0: 5f69 6473 3d73 656c 662e 6964 2c0d 0a20  _ids=self.id,.. 
+000209e0: 2020 2020 2020 2020 2020 2072 6576 6f6b             revok
+000209f0: 653d 7265 766f 6b65 0d0a 2020 2020 2020  e=revoke..      
+00020a00: 2020 290d 0a0d 0a20 2020 2061 7379 6e63    )....    async
+00020a10: 2064 6566 2063 6c69 636b 2873 656c 662c   def click(self,
+00020a20: 2078 3a20 556e 696f 6e5b 696e 742c 2073   x: Union[int, s
+00020a30: 7472 5d20 3d20 302c 2079 3a20 696e 7420  tr] = 0, y: int 
+00020a40: 3d20 4e6f 6e65 2c20 7175 6f74 653a 2062  = None, quote: b
+00020a50: 6f6f 6c20 3d20 4e6f 6e65 2c20 7469 6d65  ool = None, time
+00020a60: 6f75 743a 2069 6e74 203d 2031 3029 3a0d  out: int = 10):.
+00020a70: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
+00020a80: 6420 6d65 7468 6f64 202a 636c 6963 6b2a  d method *click*
+00020a90: 206f 6620 3a6f 626a 3a60 7e66 6970 7065   of :obj:`~fippe
+00020aa0: 722e 7479 7065 732e 4d65 7373 6167 6560  r.types.Message`
+00020ab0: 2e0d 0a0d 0a20 2020 2020 2020 2055 7365  .....        Use
+00020ac0: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
+00020ad0: 6f72 2063 6c69 636b 696e 6720 6120 6275  or clicking a bu
+00020ae0: 7474 6f6e 2061 7474 6163 6865 6420 746f  tton attached to
+00020af0: 2074 6865 206d 6573 7361 6765 2069 6e73   the message ins
+00020b00: 7465 6164 206f 663a 0d0a 0d0a 2020 2020  tead of:....    
+00020b10: 2020 2020 2d20 436c 6963 6b69 6e67 2069      - Clicking i
+00020b20: 6e6c 696e 6520 6275 7474 6f6e 733a 0d0a  nline buttons:..
+00020b30: 0d0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+00020b40: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+00020b50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00020b60: 6177 6169 7420 636c 6965 6e74 2e72 6571  await client.req
+00020b70: 7565 7374 5f63 616c 6c62 6163 6b5f 616e  uest_callback_an
+00020b80: 7377 6572 280d 0a20 2020 2020 2020 2020  swer(..         
+00020b90: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
+00020ba0: 6573 7361 6765 2e63 6861 742e 6964 2c0d  essage.chat.id,.
+00020bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020bc0: 206d 6573 7361 6765 5f69 643d 6d65 7373   message_id=mess
+00020bd0: 6167 652e 6964 2c0d 0a20 2020 2020 2020  age.id,..       
+00020be0: 2020 2020 2020 2020 2063 616c 6c62 6163           callbac
+00020bf0: 6b5f 6461 7461 3d6d 6573 7361 6765 2e72  k_data=message.r
+00020c00: 6570 6c79 5f6d 6172 6b75 705b 695d 5b6a  eply_markup[i][j
+00020c10: 5d2e 6361 6c6c 6261 636b 5f64 6174 610d  ].callback_data.
+00020c20: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00020c30: 0d0a 2020 2020 2020 2020 2d20 436c 6963  ..        - Clic
+00020c40: 6b69 6e67 206e 6f72 6d61 6c20 6275 7474  king normal butt
+00020c50: 6f6e 733a 0d0a 0d0a 2020 2020 2020 2020  ons:....        
+00020c60: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00020c70: 7079 7468 6f6e 0d0a 0d0a 2020 2020 2020  python....      
+00020c80: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
+00020c90: 6e74 2e73 656e 645f 6d65 7373 6167 6528  nt.send_message(
+00020ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020cb0: 2020 6368 6174 5f69 643d 6d65 7373 6167    chat_id=messag
+00020cc0: 652e 6368 6174 2e69 642c 0d0a 2020 2020  e.chat.id,..    
+00020cd0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00020ce0: 3d6d 6573 7361 6765 2e72 6570 6c79 5f6d  =message.reply_m
+00020cf0: 6172 6b75 705b 695d 5b6a 5d2e 7465 7874  arkup[i][j].text
+00020d00: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00020d10: 0a0d 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00020d20: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
+00020d30: 2054 6869 7320 6d65 7468 6f64 2063 616e   This method can
+00020d40: 2062 6520 7573 6564 2069 6e20 7468 7265   be used in thre
+00020d50: 6520 6469 6666 6572 656e 7420 7761 7973  e different ways
+00020d60: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+00020d70: 2031 2e20 2050 6173 7320 6f6e 6520 696e   1.  Pass one in
+00020d80: 7465 6765 7220 6172 6775 6d65 6e74 206f  teger argument o
+00020d90: 6e6c 7920 2865 2e67 2e3a 2060 602e 636c  nly (e.g.: ``.cl
+00020da0: 6963 6b28 3229 6060 2c20 746f 2063 6c69  ick(2)``, to cli
+00020db0: 636b 2061 2062 7574 746f 6e20 6174 2069  ck a button at i
+00020dc0: 6e64 6578 2032 292e 0d0a 2020 2020 2020  ndex 2)...      
+00020dd0: 2020 2020 2020 2020 2020 4275 7474 6f6e            Button
+00020de0: 7320 6172 6520 636f 756e 7465 6420 6c65  s are counted le
+00020df0: 6674 2074 6f20 7269 6768 742c 2073 7461  ft to right, sta
+00020e00: 7274 696e 6720 6672 6f6d 2074 6865 2074  rting from the t
+00020e10: 6f70 2e0d 0a0d 0a20 2020 2020 2020 2020  op.....         
+00020e20: 2020 2032 2e20 2050 6173 7320 7477 6f20     2.  Pass two 
+00020e30: 696e 7465 6765 7220 6172 6775 6d65 6e74  integer argument
+00020e40: 7320 2865 2e67 2e3a 2060 602e 636c 6963  s (e.g.: ``.clic
+00020e50: 6b28 312c 2030 2960 602c 2074 6f20 636c  k(1, 0)``, to cl
+00020e60: 6963 6b20 6120 6275 7474 6f6e 2061 7420  ick a button at 
+00020e70: 706f 7369 7469 6f6e 2028 312c 2030 2929  position (1, 0))
+00020e80: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00020e90: 2020 2054 6865 206f 7269 6769 6e20 2830     The origin (0
+00020ea0: 2c20 3029 2069 7320 746f 702d 6c65 6674  , 0) is top-left
+00020eb0: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00020ec0: 2033 2e20 2050 6173 7320 6f6e 6520 7374   3.  Pass one st
+00020ed0: 7269 6e67 2061 7267 756d 656e 7420 6f6e  ring argument on
+00020ee0: 6c79 2028 652e 672e 3a20 6060 2e63 6c69  ly (e.g.: ``.cli
+00020ef0: 636b 2822 5365 7474 696e 6773 2229 6060  ck("Settings")``
+00020f00: 2c20 746f 2063 6c69 636b 2061 2062 7574  , to click a but
+00020f10: 746f 6e20 6279 2075 7369 6e67 2069 7473  ton by using its
+00020f20: 206c 6162 656c 292e 0d0a 2020 2020 2020   label)...      
+00020f30: 2020 2020 2020 2020 2020 4f6e 6c79 2074            Only t
+00020f40: 6865 2066 6972 7374 206d 6174 6368 696e  he first matchin
+00020f50: 6720 6275 7474 6f6e 2077 696c 6c20 6265  g button will be
+00020f60: 2070 7265 7373 6564 2e0d 0a0d 0a20 2020   pressed.....   
+00020f70: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+00020f80: 0d0a 2020 2020 2020 2020 2020 2020 7820  ..            x 
+00020f90: 2860 6069 6e74 6060 207c 2060 6073 7472  (``int`` | ``str
+00020fa0: 6060 293a 0d0a 2020 2020 2020 2020 2020  ``):..          
+00020fb0: 2020 2020 2020 5573 6564 2061 7320 696e        Used as in
+00020fc0: 7465 6765 7220 696e 6465 782c 2069 6e74  teger index, int
+00020fd0: 6567 6572 2061 6273 6369 7373 6120 2869  eger abscissa (i
+00020fe0: 6e20 7061 6972 2077 6974 6820 7929 206f  n pair with y) o
+00020ff0: 7220 6173 2073 7472 696e 6720 6c61 6265  r as string labe
+00021000: 6c2e 0d0a 2020 2020 2020 2020 2020 2020  l...            
+00021010: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00021020: 3020 2866 6972 7374 2062 7574 746f 6e29  0 (first button)
+00021030: 2e0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00021040: 2079 2028 6060 696e 7460 602c 202a 6f70   y (``int``, *op
+00021050: 7469 6f6e 616c 2a29 3a0d 0a20 2020 2020  tional*):..     
+00021060: 2020 2020 2020 2020 2020 2055 7365 6420             Used 
+00021070: 6173 206f 7264 696e 6174 6520 6f6e 6c79  as ordinate only
+00021080: 2028 696e 2070 6169 7220 7769 7468 2078   (in pair with x
+00021090: 292e 0d0a 0d0a 2020 2020 2020 2020 2020  ).....          
+000210a0: 2020 7175 6f74 6520 2860 6062 6f6f 6c60    quote (``bool`
+000210b0: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0d  `, *optional*):.
+000210c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000210d0: 2055 7365 6675 6c20 666f 7220 6e6f 726d   Useful for norm
+000210e0: 616c 2062 7574 746f 6e73 206f 6e6c 792c  al buttons only,
+000210f0: 2077 6865 7265 2070 7265 7373 696e 6720   where pressing 
+00021100: 6974 2077 696c 6c20 7265 7375 6c74 2069  it will result i
+00021110: 6e20 6120 6e65 7720 6d65 7373 6167 6520  n a new message 
+00021120: 7365 6e74 2e0d 0a20 2020 2020 2020 2020  sent...         
+00021130: 2020 2020 2020 2049 6620 6060 5472 7565         If ``True
+00021140: 6060 2c20 7468 6520 6d65 7373 6167 6520  ``, the message 
+00021150: 7769 6c6c 2062 6520 7365 6e74 2061 7320  will be sent as 
+00021160: 6120 7265 706c 7920 746f 2074 6869 7320  a reply to this 
+00021170: 6d65 7373 6167 652e 0d0a 2020 2020 2020  message...      
+00021180: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00021190: 7473 2074 6f20 6060 5472 7565 6060 2069  ts to ``True`` i
+000211a0: 6e20 6772 6f75 7020 6368 6174 7320 616e  n group chats an
+000211b0: 6420 6060 4661 6c73 6560 6020 696e 2070  d ``False`` in p
+000211c0: 7269 7661 7465 2063 6861 7473 2e0d 0a0d  rivate chats....
+000211d0: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+000211e0: 656f 7574 2028 6060 696e 7460 602c 202a  eout (``int``, *
+000211f0: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
+00021200: 2020 2020 2020 2020 2020 2020 2054 696d               Tim
+00021210: 656f 7574 2069 6e20 7365 636f 6e64 732e  eout in seconds.
+00021220: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00021230: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+00021240: 2020 2d20 2020 5468 6520 7265 7375 6c74    -   The result
+00021250: 206f 6620 3a6d 6574 683a 607e 6669 7070   of :meth:`~fipp
+00021260: 6572 2e43 6c69 656e 742e 7265 7175 6573  er.Client.reques
+00021270: 745f 6361 6c6c 6261 636b 5f61 6e73 7765  t_callback_answe
+00021280: 7260 2069 6e20 6361 7365 206f 6620 696e  r` in case of in
+00021290: 6c69 6e65 2063 616c 6c62 6163 6b20 6275  line callback bu
+000212a0: 7474 6f6e 2063 6c69 636b 732e 0d0a 2020  tton clicks...  
+000212b0: 2020 2020 2020 2020 2020 2d20 2020 5468            -   Th
+000212c0: 6520 7265 7375 6c74 206f 6620 3a6d 6574  e result of :met
+000212d0: 683a 607e 4d65 7373 6167 652e 7265 706c  h:`~Message.repl
+000212e0: 7928 2960 2069 6e20 6361 7365 206f 6620  y()` in case of 
+000212f0: 6e6f 726d 616c 2062 7574 746f 6e20 636c  normal button cl
+00021300: 6963 6b73 2e0d 0a20 2020 2020 2020 2020  icks...         
+00021310: 2020 202d 2020 2041 2073 7472 696e 6720     -   A string 
+00021320: 696e 2063 6173 6520 7468 6520 696e 6c69  in case the inli
+00021330: 6e65 2062 7574 746f 6e20 6973 2061 2055  ne button is a U
+00021340: 524c 2c20 6120 2a73 7769 7463 685f 696e  RL, a *switch_in
+00021350: 6c69 6e65 5f71 7565 7279 2a20 6f72 2061  line_query* or a
+00021360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00021370: 2020 2a73 7769 7463 685f 696e 6c69 6e65    *switch_inline
+00021380: 5f71 7565 7279 5f63 7572 7265 6e74 5f63  _query_current_c
+00021390: 6861 742a 2062 7574 746f 6e2e 0d0a 0d0a  hat* button.....
+000213a0: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
+000213b0: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
+000213c0: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
+000213d0: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
+000213e0: 2065 7272 6f72 2e0d 0a20 2020 2020 2020   error...       
+000213f0: 2020 2020 2056 616c 7565 4572 726f 723a       ValueError:
+00021400: 2049 6e20 6361 7365 2074 6865 2070 726f   In case the pro
+00021410: 7669 6465 6420 696e 6465 7820 6f72 2070  vided index or p
+00021420: 6f73 6974 696f 6e20 6973 206f 7574 206f  osition is out o
+00021430: 6620 7261 6e67 6520 6f72 2074 6865 2062  f range or the b
+00021440: 7574 746f 6e20 6c61 6265 6c20 7761 7320  utton label was 
+00021450: 6e6f 7420 666f 756e 642e 0d0a 2020 2020  not found...    
+00021460: 2020 2020 2020 2020 5469 6d65 6f75 7445          TimeoutE
+00021470: 7272 6f72 3a20 496e 2063 6173 652c 2061  rror: In case, a
+00021480: 6674 6572 2063 6c69 636b 696e 6720 616e  fter clicking an
+00021490: 2069 6e6c 696e 6520 6275 7474 6f6e 2c20   inline button, 
+000214a0: 7468 6520 626f 7420 6661 696c 7320 746f  the bot fails to
+000214b0: 2061 6e73 7765 7220 7769 7468 696e 2074   answer within t
+000214c0: 6865 2074 696d 656f 7574 2e0d 0a20 2020  he timeout...   
+000214d0: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
+000214e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000214f0: 6528 7365 6c66 2e72 6570 6c79 5f6d 6172  e(self.reply_mar
+00021500: 6b75 702c 2074 7970 6573 2e52 6570 6c79  kup, types.Reply
+00021510: 4b65 7962 6f61 7264 4d61 726b 7570 293a  KeyboardMarkup):
+00021520: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
+00021530: 7962 6f61 7264 203d 2073 656c 662e 7265  yboard = self.re
+00021540: 706c 795f 6d61 726b 7570 2e6b 6579 626f  ply_markup.keybo
+00021550: 6172 640d 0a20 2020 2020 2020 2020 2020  ard..           
+00021560: 2069 735f 696e 6c69 6e65 203d 2046 616c   is_inline = Fal
+00021570: 7365 0d0a 2020 2020 2020 2020 656c 6966  se..        elif
+00021580: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
+00021590: 2e72 6570 6c79 5f6d 6172 6b75 702c 2074  .reply_markup, t
+000215a0: 7970 6573 2e49 6e6c 696e 654b 6579 626f  ypes.InlineKeybo
+000215b0: 6172 644d 6172 6b75 7029 3a0d 0a20 2020  ardMarkup):..   
+000215c0: 2020 2020 2020 2020 206b 6579 626f 6172           keyboar
+000215d0: 6420 3d20 7365 6c66 2e72 6570 6c79 5f6d  d = self.reply_m
+000215e0: 6172 6b75 702e 696e 6c69 6e65 5f6b 6579  arkup.inline_key
+000215f0: 626f 6172 640d 0a20 2020 2020 2020 2020  board..         
+00021600: 2020 2069 735f 696e 6c69 6e65 203d 2054     is_inline = T
+00021610: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
+00021620: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00021630: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00021640: 2822 5468 6520 6d65 7373 6167 6520 646f  ("The message do
+00021650: 6573 6e27 7420 636f 6e74 6169 6e20 616e  esn't contain an
+00021660: 7920 6b65 7962 6f61 7264 2229 0d0a 0d0a  y keyboard")....
+00021670: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00021680: 7461 6e63 6528 782c 2069 6e74 2920 616e  tance(x, int) an
+00021690: 6420 7920 6973 204e 6f6e 653a 0d0a 2020  d y is None:..  
+000216a0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+000216b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216c0: 6275 7474 6f6e 203d 205b 0d0a 2020 2020  button = [..    
+000216d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216e0: 6275 7474 6f6e 0d0a 2020 2020 2020 2020  button..        
+000216f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00021700: 726f 7720 696e 206b 6579 626f 6172 640d  row in keyboard.
+00021710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021720: 2020 2020 2066 6f72 2062 7574 746f 6e20       for button 
+00021730: 696e 2072 6f77 0d0a 2020 2020 2020 2020  in row..        
+00021740: 2020 2020 2020 2020 5d5b 785d 0d0a 2020          ][x]..  
+00021750: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00021760: 2049 6e64 6578 4572 726f 723a 0d0a 2020   IndexError:..  
+00021770: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00021780: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00021790: 2254 6865 2062 7574 746f 6e20 6174 2069  "The button at i
+000217a0: 6e64 6578 207b 787d 2064 6f65 736e 2774  ndex {x} doesn't
+000217b0: 2065 7869 7374 2229 0d0a 2020 2020 2020   exist")..      
+000217c0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+000217d0: 6528 782c 2069 6e74 2920 616e 6420 6973  e(x, int) and is
+000217e0: 696e 7374 616e 6365 2879 2c20 696e 7429  instance(y, int)
+000217f0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00021800: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00021810: 2020 2020 2062 7574 746f 6e20 3d20 6b65       button = ke
+00021820: 7962 6f61 7264 5b79 5d5b 785d 0d0a 2020  yboard[y][x]..  
+00021830: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00021840: 2049 6e64 6578 4572 726f 723a 0d0a 2020   IndexError:..  
+00021850: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00021860: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00021870: 2254 6865 2062 7574 746f 6e20 6174 2070  "The button at p
+00021880: 6f73 6974 696f 6e20 287b 787d 2c20 7b79  osition ({x}, {y
+00021890: 7d29 2064 6f65 736e 2774 2065 7869 7374  }) doesn't exist
+000218a0: 2229 0d0a 2020 2020 2020 2020 656c 6966  ")..        elif
+000218b0: 2069 7369 6e73 7461 6e63 6528 782c 2073   isinstance(x, s
+000218c0: 7472 2920 616e 6420 7920 6973 204e 6f6e  tr) and y is Non
+000218d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000218e0: 6c61 6265 6c20 3d20 782e 656e 636f 6465  label = x.encode
+000218f0: 2822 7574 662d 3136 222c 2022 7375 7272  ("utf-16", "surr
+00021900: 6f67 6174 6570 6173 7322 292e 6465 636f  ogatepass").deco
+00021910: 6465 2822 7574 662d 3136 2229 0d0a 0d0a  de("utf-16")....
+00021920: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00021930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00021940: 2020 6275 7474 6f6e 203d 205b 0d0a 2020    button = [..  
+00021950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021960: 2020 6275 7474 6f6e 0d0a 2020 2020 2020    button..      
+00021970: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00021980: 7220 726f 7720 696e 206b 6579 626f 6172  r row in keyboar
+00021990: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+000219a0: 2020 2020 2020 2066 6f72 2062 7574 746f         for butto
+000219b0: 6e20 696e 2072 6f77 0d0a 2020 2020 2020  n in row..      
+000219c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000219d0: 206c 6162 656c 203d 3d20 6275 7474 6f6e   label == button
+000219e0: 2e74 6578 740d 0a20 2020 2020 2020 2020  .text..         
+000219f0: 2020 2020 2020 205d 5b30 5d0d 0a20 2020         ][0]..   
+00021a00: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00021a10: 496e 6465 7845 7272 6f72 3a0d 0a20 2020  IndexError:..   
+00021a20: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00021a30: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00021a40: 5468 6520 6275 7474 6f6e 2077 6974 6820  The button with 
+00021a50: 6c61 6265 6c20 277b 787d 2720 646f 6573  label '{x}' does
+00021a60: 6e27 7420 6578 6973 7473 2229 0d0a 2020  n't exists")..  
+00021a70: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00021a80: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00021a90: 616c 7565 4572 726f 7228 2249 6e76 616c  alueError("Inval
+00021aa0: 6964 2061 7267 756d 656e 7473 2229 0d0a  id arguments")..
+00021ab0: 0d0a 2020 2020 2020 2020 6966 2069 735f  ..        if is_
+00021ac0: 696e 6c69 6e65 3a0d 0a20 2020 2020 2020  inline:..       
+00021ad0: 2020 2020 2069 6620 6275 7474 6f6e 2e63       if button.c
+00021ae0: 616c 6c62 6163 6b5f 6461 7461 3a0d 0a20  allback_data:.. 
+00021af0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00021b00: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00021b10: 2e5f 636c 6965 6e74 2e72 6571 7565 7374  ._client.request
+00021b20: 5f63 616c 6c62 6163 6b5f 616e 7377 6572  _callback_answer
+00021b30: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00021b40: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
+00021b50: 656c 662e 6368 6174 2e69 642c 0d0a 2020  elf.chat.id,..  
+00021b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021b70: 2020 6d65 7373 6167 655f 6964 3d73 656c    message_id=sel
+00021b80: 662e 6964 2c0d 0a20 2020 2020 2020 2020  f.id,..         
+00021b90: 2020 2020 2020 2020 2020 2063 616c 6c62             callb
+00021ba0: 6163 6b5f 6461 7461 3d62 7574 746f 6e2e  ack_data=button.
+00021bb0: 6361 6c6c 6261 636b 5f64 6174 612c 0d0a  callback_data,..
+00021bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021bd0: 2020 2020 7469 6d65 6f75 743d 7469 6d65      timeout=time
+00021be0: 6f75 740d 0a20 2020 2020 2020 2020 2020  out..           
+00021bf0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00021c00: 2020 2020 656c 6966 2062 7574 746f 6e2e      elif button.
+00021c10: 7572 6c3a 0d0a 2020 2020 2020 2020 2020  url:..          
+00021c20: 2020 2020 2020 7265 7475 726e 2062 7574        return but
+00021c30: 746f 6e2e 7572 6c0d 0a20 2020 2020 2020  ton.url..       
+00021c40: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
+00021c50: 2e73 7769 7463 685f 696e 6c69 6e65 5f71  .switch_inline_q
+00021c60: 7565 7279 3a0d 0a20 2020 2020 2020 2020  uery:..         
+00021c70: 2020 2020 2020 2072 6574 7572 6e20 6275         return bu
+00021c80: 7474 6f6e 2e73 7769 7463 685f 696e 6c69  tton.switch_inli
+00021c90: 6e65 5f71 7565 7279 0d0a 2020 2020 2020  ne_query..      
+00021ca0: 2020 2020 2020 656c 6966 2062 7574 746f        elif butto
+00021cb0: 6e2e 7377 6974 6368 5f69 6e6c 696e 655f  n.switch_inline_
+00021cc0: 7175 6572 795f 6375 7272 656e 745f 6368  query_current_ch
+00021cd0: 6174 3a0d 0a20 2020 2020 2020 2020 2020  at:..           
+00021ce0: 2020 2020 2072 6574 7572 6e20 6275 7474       return butt
+00021cf0: 6f6e 2e73 7769 7463 685f 696e 6c69 6e65  on.switch_inline
+00021d00: 5f71 7565 7279 5f63 7572 7265 6e74 5f63  _query_current_c
+00021d10: 6861 740d 0a20 2020 2020 2020 2020 2020  hat..           
+00021d20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00021d30: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00021d40: 6c75 6545 7272 6f72 2822 5468 6973 2062  lueError("This b
+00021d50: 7574 746f 6e20 6973 206e 6f74 2073 7570  utton is not sup
+00021d60: 706f 7274 6564 2079 6574 2229 0d0a 2020  ported yet")..  
+00021d70: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00021d80: 2020 2020 2020 2020 2061 7761 6974 2073           await s
+00021d90: 656c 662e 7265 706c 7928 6275 7474 6f6e  elf.reply(button
+00021da0: 2c20 7175 6f74 653d 7175 6f74 6529 0d0a  , quote=quote)..
+00021db0: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00021dc0: 7265 6163 7428 7365 6c66 2c20 656d 6f6a  react(self, emoj
+00021dd0: 693a 2073 7472 203d 2022 222c 2062 6967  i: str = "", big
+00021de0: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
+00021df0: 2d3e 2062 6f6f 6c3a 0d0a 2020 2020 2020  -> bool:..      
+00021e00: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
+00021e10: 6420 2a72 6561 6374 2a20 6f66 203a 6f62  d *react* of :ob
+00021e20: 6a3a 607e 6669 7070 6572 2e74 7970 6573  j:`~fipper.types
+00021e30: 2e4d 6573 7361 6765 602e 0d0a 0d0a 2020  .Message`.....  
+00021e40: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
+00021e50: 686f 7274 6375 7420 666f 723a 0d0a 0d0a  hortcut for:....
+00021e60: 2020 2020 2020 2020 2e2e 2063 6f64 652d          .. code-
+00021e70: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0d0a  block:: python..
+00021e80: 0d0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
+00021e90: 6169 7420 636c 6965 6e74 2e73 656e 645f  ait client.send_
+00021ea0: 7265 6163 7469 6f6e 280d 0a20 2020 2020  reaction(..     
+00021eb0: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00021ec0: 6964 3d63 6861 745f 6964 2c0d 0a20 2020  id=chat_id,..   
+00021ed0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+00021ee0: 7361 6765 5f69 643d 6d65 7373 6167 652e  sage_id=message.
+00021ef0: 6964 2c0d 0a20 2020 2020 2020 2020 2020  id,..           
+00021f00: 2020 2020 2065 6d6f 6a69 3d22 f09f 94a5       emoji="....
+00021f10: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
+00021f20: 0d0a 0d0a 2020 2020 2020 2020 4578 616d  ....        Exam
+00021f30: 706c 653a 0d0a 2020 2020 2020 2020 2020  ple:..          
+00021f40: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00021f50: 3a20 7079 7468 6f6e 0d0a 0d0a 2020 2020  : python....    
+00021f60: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00021f70: 7420 6d65 7373 6167 652e 7265 6163 7428  t message.react(
+00021f80: 656d 6f6a 693d 22f0 9f94 a522 290d 0a0d  emoji="....")...
+00021f90: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00021fa0: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
+00021fb0: 2020 656d 6f6a 6920 2860 6073 7472 6060    emoji (``str``
+00021fc0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0d0a  , *optional*):..
+00021fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021fe0: 5265 6163 7469 6f6e 2065 6d6f 6a69 2e0d  Reaction emoji..
+00021ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022000: 2050 6173 7320 2222 2061 7320 656d 6f6a   Pass "" as emoj
+00022010: 6920 2864 6566 6175 6c74 2920 746f 2072  i (default) to r
+00022020: 6574 7261 6374 2074 6865 2072 6561 6374  etract the react
+00022030: 696f 6e2e 0d0a 2020 2020 2020 2020 2020  ion...          
+00022040: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00022050: 2062 6967 2028 6060 626f 6f6c 6060 2c20   big (``bool``, 
+00022060: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+00022070: 2020 2020 2020 2020 2020 2020 2020 5061                Pa
+00022080: 7373 2054 7275 6520 746f 2073 686f 7720  ss True to show 
+00022090: 6120 6269 6767 6572 2061 6e64 206c 6f6e  a bigger and lon
+000220a0: 6765 7220 7265 6163 7469 6f6e 2e0d 0a20  ger reaction... 
+000220b0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+000220c0: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+000220d0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+000220e0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+000220f0: 2020 2060 6062 6f6f 6c60 603a 204f 6e20     ``bool``: On 
+00022100: 7375 6363 6573 732c 2054 7275 6520 6973  success, True is
+00022110: 2072 6574 7572 6e65 642e 0d0a 0d0a 2020   returned.....  
+00022120: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
+00022130: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
+00022140: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
+00022150: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
+00022160: 7272 6f72 2e0d 0a20 2020 2020 2020 2022  rror...        "
+00022170: 2222 0d0a 0d0a 2020 2020 2020 2020 7265  ""....        re
+00022180: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00022190: 5f63 6c69 656e 742e 7365 6e64 5f72 6561  _client.send_rea
+000221a0: 6374 696f 6e28 0d0a 2020 2020 2020 2020  ction(..        
+000221b0: 2020 2020 6368 6174 5f69 643d 7365 6c66      chat_id=self
+000221c0: 2e63 6861 742e 6964 2c0d 0a20 2020 2020  .chat.id,..     
+000221d0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
+000221e0: 643d 7365 6c66 2e69 642c 0d0a 2020 2020  d=self.id,..    
+000221f0: 2020 2020 2020 2020 656d 6f6a 693d 656d          emoji=em
+00022200: 6f6a 692c 0d0a 2020 2020 2020 2020 2020  oji,..          
+00022210: 2020 6269 673d 6269 670d 0a20 2020 2020    big=big..     
+00022220: 2020 2029 0d0a 0d0a 2020 2020 6173 796e     )....    asyn
+00022230: 6320 6465 6620 7265 7472 6163 745f 766f  c def retract_vo
+00022240: 7465 280d 0a20 2020 2020 2020 2073 656c  te(..        sel
+00022250: 662c 0d0a 2020 2020 2920 2d3e 2022 7479  f,..    ) -> "ty
+00022260: 7065 732e 506f 6c6c 223a 0d0a 2020 2020  pes.Poll":..    
+00022270: 2020 2020 2222 2242 6f75 6e64 206d 6574      """Bound met
+00022280: 686f 6420 2a72 6574 7261 6374 5f76 6f74  hod *retract_vot
+00022290: 652a 206f 6620 3a6f 626a 3a60 7e66 6970  e* of :obj:`~fip
+000222a0: 7065 722e 7479 7065 732e 4d65 7373 6167  per.types.Messag
+000222b0: 6560 2e0d 0a0d 0a20 2020 2020 2020 2055  e`.....        U
+000222c0: 7365 2061 7320 6120 7368 6f72 7463 7574  se as a shortcut
+000222d0: 2066 6f72 3a0d 0a0d 0a20 2020 2020 2020   for:....       
+000222e0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+000222f0: 2070 7974 686f 6e0d 0a0d 0a20 2020 2020   python....     
+00022300: 2020 2020 2020 2063 6c69 656e 742e 7265         client.re
+00022310: 7472 6163 745f 766f 7465 280d 0a20 2020  tract_vote(..   
+00022320: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00022330: 745f 6964 3d6d 6573 7361 6765 2e63 6861  t_id=message.cha
+00022340: 742e 6964 2c0d 0a20 2020 2020 2020 2020  t.id,..         
+00022350: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
+00022360: 643d 6d65 7373 6167 655f 6964 2c0d 0a20  d=message_id,.. 
+00022370: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
+00022380: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+00022390: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
+000223a0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+000223b0: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
+000223c0: 2020 2020 2020 2020 6d65 7373 6167 652e          message.
+000223d0: 7265 7472 6163 745f 766f 7465 2829 0d0a  retract_vote()..
+000223e0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000223f0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00022400: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
+00022410: 7065 732e 506f 6c6c 603a 204f 6e20 7375  pes.Poll`: On su
+00022420: 6363 6573 732c 2074 6865 2070 6f6c 6c20  ccess, the poll 
+00022430: 7769 7468 2074 6865 2072 6574 7261 6374  with the retract
+00022440: 6564 2076 6f74 6520 6973 2072 6574 7572  ed vote is retur
+00022450: 6e65 642e 0d0a 0d0a 2020 2020 2020 2020  ned.....        
+00022460: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+00022470: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+00022480: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+00022490: 6772 616d 2052 5043 2065 7272 6f72 2e0d  gram RPC error..
+000224a0: 0a20 2020 2020 2020 2022 2222 0d0a 0d0a  .        """....
+000224b0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+000224c0: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+000224d0: 742e 7265 7472 6163 745f 766f 7465 280d  t.retract_vote(.
+000224e0: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+000224f0: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
+00022500: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+00022510: 6d65 7373 6167 655f 6964 3d73 656c 662e  message_id=self.
+00022520: 6964 0d0a 2020 2020 2020 2020 290d 0a0d  id..        )...
+00022530: 0a20 2020 2061 7379 6e63 2064 6566 2064  .    async def d
+00022540: 6f77 6e6c 6f61 6428 0d0a 2020 2020 2020  ownload(..      
+00022550: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00022560: 2066 696c 655f 6e61 6d65 3a20 7374 7220   file_name: str 
+00022570: 3d20 2222 2c0d 0a20 2020 2020 2020 2069  = "",..        i
+00022580: 6e5f 6d65 6d6f 7279 3a20 626f 6f6c 203d  n_memory: bool =
+00022590: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
+000225a0: 2062 6c6f 636b 3a20 626f 6f6c 203d 2054   block: bool = T
+000225b0: 7275 652c 0d0a 2020 2020 2020 2020 7072  rue,..        pr
+000225c0: 6f67 7265 7373 3a20 4361 6c6c 6162 6c65  ogress: Callable
+000225d0: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
+000225e0: 2020 7072 6f67 7265 7373 5f61 7267 733a    progress_args:
+000225f0: 2074 7570 6c65 203d 2028 290d 0a20 2020   tuple = ()..   
+00022600: 2029 202d 3e20 7374 723a 0d0a 2020 2020   ) -> str:..    
+00022610: 2020 2020 2222 2242 6f75 6e64 206d 6574      """Bound met
+00022620: 686f 6420 2a64 6f77 6e6c 6f61 642a 206f  hod *download* o
+00022630: 6620 3a6f 626a 3a60 7e66 6970 7065 722e  f :obj:`~fipper.
+00022640: 7479 7065 732e 4d65 7373 6167 6560 2e0d  types.Message`..
+00022650: 0a0d 0a20 2020 2020 2020 2055 7365 2061  ...        Use a
+00022660: 7320 6120 7368 6f72 7463 7574 2066 6f72  s a shortcut for
+00022670: 3a0d 0a0d 0a20 2020 2020 2020 202e 2e20  :....        .. 
+00022680: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00022690: 686f 6e0d 0a0d 0a20 2020 2020 2020 2020  hon....         
+000226a0: 2020 2061 7761 6974 2063 6c69 656e 742e     await client.
+000226b0: 646f 776e 6c6f 6164 5f6d 6564 6961 286d  download_media(m
+000226c0: 6573 7361 6765 290d 0a0d 0a20 2020 2020  essage)....     
+000226d0: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
+000226e0: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
+000226f0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
+00022700: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00022710: 2020 2061 7761 6974 206d 6573 7361 6765     await message
+00022720: 2e64 6f77 6e6c 6f61 6428 290d 0a0d 0a20  .download().... 
+00022730: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00022740: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00022750: 6669 6c65 5f6e 616d 6520 2860 6073 7472  file_name (``str
+00022760: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+00022770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00022780: 2020 4120 6375 7374 6f6d 202a 6669 6c65    A custom *file
+00022790: 5f6e 616d 652a 2074 6f20 6265 2075 7365  _name* to be use
+000227a0: 6420 696e 7374 6561 6420 6f66 2074 6865  d instead of the
+000227b0: 206f 6e65 2070 726f 7669 6465 6420 6279   one provided by
+000227c0: 2054 656c 6567 7261 6d2e 0d0a 2020 2020   Telegram...    
+000227d0: 2020 2020 2020 2020 2020 2020 4279 2064              By d
+000227e0: 6566 6175 6c74 2c20 616c 6c20 6669 6c65  efault, all file
+000227f0: 7320 6172 6520 646f 776e 6c6f 6164 6564  s are downloaded
+00022800: 2069 6e20 7468 6520 2a64 6f77 6e6c 6f61   in the *downloa
+00022810: 6473 2a20 666f 6c64 6572 2069 6e20 796f  ds* folder in yo
+00022820: 7572 2077 6f72 6b69 6e67 2064 6972 6563  ur working direc
+00022830: 746f 7279 2e0d 0a20 2020 2020 2020 2020  tory...         
+00022840: 2020 2020 2020 2059 6f75 2063 616e 2061         You can a
+00022850: 6c73 6f20 7370 6563 6966 7920 6120 7061  lso specify a pa
+00022860: 7468 2066 6f72 2064 6f77 6e6c 6f61 6469  th for downloadi
+00022870: 6e67 2066 696c 6573 2069 6e20 6120 6375  ng files in a cu
+00022880: 7374 6f6d 206c 6f63 6174 696f 6e3a 2070  stom location: p
+00022890: 6174 6873 2074 6861 7420 656e 6420 7769  aths that end wi
+000228a0: 7468 2022 2f22 0d0a 2020 2020 2020 2020  th "/"..        
+000228b0: 2020 2020 2020 2020 6172 6520 636f 6e73          are cons
+000228c0: 6964 6572 6564 2064 6972 6563 746f 7269  idered directori
+000228d0: 6573 2e20 416c 6c20 6e6f 6e2d 6578 6973  es. All non-exis
+000228e0: 7465 6e74 2066 6f6c 6465 7273 2077 696c  tent folders wil
+000228f0: 6c20 6265 2063 7265 6174 6564 2061 7574  l be created aut
+00022900: 6f6d 6174 6963 616c 6c79 2e0d 0a0d 0a20  omatically..... 
+00022910: 2020 2020 2020 2020 2020 2069 6e5f 6d65             in_me
+00022920: 6d6f 7279 2028 6060 626f 6f6c 6060 2c20  mory (``bool``, 
+00022930: 2a6f 7074 696f 6e61 6c2a 293a 0d0a 2020  *optional*):..  
+00022940: 2020 2020 2020 2020 2020 2020 2020 5061                Pa
+00022950: 7373 2054 7275 6520 746f 2064 6f77 6e6c  ss True to downl
+00022960: 6f61 6420 7468 6520 6d65 6469 6120 696e  oad the media in
+00022970: 2d6d 656d 6f72 792e 0d0a 2020 2020 2020  -memory...      
+00022980: 2020 2020 2020 2020 2020 4120 6269 6e61            A bina
+00022990: 7279 2066 696c 652d 6c69 6b65 206f 626a  ry file-like obj
+000229a0: 6563 7420 7769 7468 2069 7473 2061 7474  ect with its att
+000229b0: 7269 6275 7465 2022 2e6e 616d 6522 2073  ribute ".name" s
+000229c0: 6574 2077 696c 6c20 6265 2072 6574 7572  et will be retur
+000229d0: 6e65 642e 0d0a 2020 2020 2020 2020 2020  ned...          
+000229e0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+000229f0: 6f20 4661 6c73 652e 0d0a 0d0a 2020 2020  o False.....    
+00022a00: 2020 2020 2020 2020 626c 6f63 6b20 2860          block (`
+00022a10: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
+00022a20: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+00022a30: 2020 2020 2020 2042 6c6f 636b 7320 7468         Blocks th
+00022a40: 6520 636f 6465 2065 7865 6375 7469 6f6e  e code execution
+00022a50: 2075 6e74 696c 2074 6865 2066 696c 6520   until the file 
+00022a60: 6861 7320 6265 656e 2064 6f77 6e6c 6f61  has been downloa
+00022a70: 6465 642e 0d0a 2020 2020 2020 2020 2020  ded...          
+00022a80: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00022a90: 6f20 5472 7565 2e0d 0a0d 0a20 2020 2020  o True.....     
+00022aa0: 2020 2020 2020 2070 726f 6772 6573 7320         progress 
+00022ab0: 2860 6043 616c 6c61 626c 6560 602c 202a  (``Callable``, *
+00022ac0: 6f70 7469 6f6e 616c 2a29 3a0d 0a20 2020  optional*):..   
+00022ad0: 2020 2020 2020 2020 2020 2020 2050 6173               Pas
+00022ae0: 7320 6120 6361 6c6c 6261 636b 2066 756e  s a callback fun
+00022af0: 6374 696f 6e20 746f 2076 6965 7720 7468  ction to view th
+00022b00: 6520 6669 6c65 2074 7261 6e73 6d69 7373  e file transmiss
+00022b10: 696f 6e20 7072 6f67 7265 7373 2e0d 0a20  ion progress... 
+00022b20: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00022b30: 6865 2066 756e 6374 696f 6e20 6d75 7374  he function must
+00022b40: 2074 616b 6520 2a28 6375 7272 656e 742c   take *(current,
+00022b50: 2074 6f74 616c 292a 2061 7320 706f 7369   total)* as posi
+00022b60: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
+00022b70: 2028 6c6f 6f6b 2061 7420 4f74 6865 7220   (look at Other 
+00022b80: 5061 7261 6d65 7465 7273 2062 656c 6f77  Parameters below
+00022b90: 2066 6f72 2061 0d0a 2020 2020 2020 2020   for a..        
+00022ba0: 2020 2020 2020 2020 6465 7461 696c 6564          detailed
+00022bb0: 2064 6573 6372 6970 7469 6f6e 2920 616e   description) an
+00022bc0: 6420 7769 6c6c 2062 6520 6361 6c6c 6564  d will be called
+00022bd0: 2062 6163 6b20 6561 6368 2074 696d 6520   back each time 
+00022be0: 6120 6e65 7720 6669 6c65 2063 6875 6e6b  a new file chunk
+00022bf0: 2068 6173 2062 6565 6e20 7375 6363 6573   has been succes
+00022c00: 7366 756c 6c79 0d0a 2020 2020 2020 2020  sfully..        
+00022c10: 2020 2020 2020 2020 7472 616e 736d 6974          transmit
+00022c20: 7465 642e 0d0a 0d0a 2020 2020 2020 2020  ted.....        
+00022c30: 2020 2020 7072 6f67 7265 7373 5f61 7267      progress_arg
+00022c40: 7320 2860 6074 7570 6c65 6060 2c20 2a6f  s (``tuple``, *o
+00022c50: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+00022c60: 2020 2020 2020 2020 2020 2020 4578 7472              Extr
+00022c70: 6120 6375 7374 6f6d 2061 7267 756d 656e  a custom argumen
+00022c80: 7473 2066 6f72 2074 6865 2070 726f 6772  ts for the progr
+00022c90: 6573 7320 6361 6c6c 6261 636b 2066 756e  ess callback fun
+00022ca0: 6374 696f 6e2e 0d0a 2020 2020 2020 2020  ction...        
+00022cb0: 2020 2020 2020 2020 596f 7520 6361 6e20          You can 
+00022cc0: 7061 7373 2061 6e79 7468 696e 6720 796f  pass anything yo
+00022cd0: 7520 6e65 6564 2074 6f20 6265 2061 7661  u need to be ava
+00022ce0: 696c 6162 6c65 2069 6e20 7468 6520 7072  ilable in the pr
+00022cf0: 6f67 7265 7373 2063 616c 6c62 6163 6b20  ogress callback 
+00022d00: 7363 6f70 653b 2066 6f72 2065 7861 6d70  scope; for examp
+00022d10: 6c65 2c20 6120 4d65 7373 6167 650d 0a20  le, a Message.. 
+00022d20: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00022d30: 626a 6563 7420 6f72 2061 2043 6c69 656e  bject or a Clien
+00022d40: 7420 696e 7374 616e 6365 2069 6e20 6f72  t instance in or
+00022d50: 6465 7220 746f 2065 6469 7420 7468 6520  der to edit the 
+00022d60: 6d65 7373 6167 6520 7769 7468 2074 6865  message with the
+00022d70: 2075 7064 6174 6564 2070 726f 6772 6573   updated progres
+00022d80: 7320 7374 6174 7573 2e0d 0a0d 0a20 2020  s status.....   
+00022d90: 2020 2020 204f 7468 6572 2050 6172 616d       Other Param
+00022da0: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
+00022db0: 2020 2020 6375 7272 656e 7420 2860 6069      current (``i
+00022dc0: 6e74 6060 293a 0d0a 2020 2020 2020 2020  nt``):..        
+00022dd0: 2020 2020 2020 2020 5468 6520 616d 6f75          The amou
+00022de0: 6e74 206f 6620 6279 7465 7320 7472 616e  nt of bytes tran
+00022df0: 736d 6974 7465 6420 736f 2066 6172 2e0d  smitted so far..
+00022e00: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+00022e10: 6f74 616c 2028 6060 696e 7460 6029 3a0d  otal (``int``):.
+00022e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022e30: 2054 6865 2074 6f74 616c 2073 697a 6520   The total size 
+00022e40: 6f66 2074 6865 2066 696c 652e 0d0a 0d0a  of the file.....
+00022e50: 2020 2020 2020 2020 2020 2020 2a61 7267              *arg
+00022e60: 7320 2860 6074 7570 6c65 6060 2c20 2a6f  s (``tuple``, *o
+00022e70: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+00022e80: 2020 2020 2020 2020 2020 2020 4578 7472              Extr
+00022e90: 6120 6375 7374 6f6d 2061 7267 756d 656e  a custom argumen
+00022ea0: 7473 2061 7320 6465 6669 6e65 6420 696e  ts as defined in
+00022eb0: 2074 6865 2060 6070 726f 6772 6573 735f   the ``progress_
+00022ec0: 6172 6773 6060 2070 6172 616d 6574 6572  args`` parameter
+00022ed0: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00022ee0: 2020 2059 6f75 2063 616e 2065 6974 6865     You can eithe
+00022ef0: 7220 6b65 6570 2060 602a 6172 6773 6060  r keep ``*args``
+00022f00: 206f 7220 6164 6420 6576 6572 7920 7369   or add every si
+00022f10: 6e67 6c65 2065 7874 7261 2061 7267 756d  ngle extra argum
+00022f20: 656e 7420 696e 2079 6f75 7220 6675 6e63  ent in your func
+00022f30: 7469 6f6e 2073 6967 6e61 7475 7265 2e0d  tion signature..
+00022f40: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00022f50: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+00022f60: 204f 6e20 7375 6363 6573 732c 2074 6865   On success, the
+00022f70: 2061 6273 6f6c 7574 6520 7061 7468 206f   absolute path o
+00022f80: 6620 7468 6520 646f 776e 6c6f 6164 6564  f the downloaded
+00022f90: 2066 696c 6520 6173 2073 7472 696e 6720   file as string 
+00022fa0: 6973 2072 6574 7572 6e65 642c 204e 6f6e  is returned, Non
+00022fb0: 6520 6f74 6865 7277 6973 652e 0d0a 0d0a  e otherwise.....
+00022fc0: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
+00022fd0: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
+00022fe0: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
+00022ff0: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
+00023000: 2065 7272 6f72 2e0d 0a20 2020 2020 2020   error...       
+00023010: 2020 2020 2060 6056 616c 7565 4572 726f       ``ValueErro
+00023020: 7260 603a 2049 6620 7468 6520 6d65 7373  r``: If the mess
+00023030: 6167 6520 646f 6573 6e27 7420 636f 6e74  age doesn't cont
+00023040: 6169 6e20 616e 7920 646f 776e 6c6f 6164  ain any download
+00023050: 6162 6c65 206d 6564 6961 0d0a 2020 2020  able media..    
+00023060: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00023070: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00023080: 6c66 2e5f 636c 6965 6e74 2e64 6f77 6e6c  lf._client.downl
+00023090: 6f61 645f 6d65 6469 6128 0d0a 2020 2020  oad_media(..    
+000230a0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+000230b0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+000230c0: 2020 2066 696c 655f 6e61 6d65 3d66 696c     file_name=fil
+000230d0: 655f 6e61 6d65 2c0d 0a20 2020 2020 2020  e_name,..       
+000230e0: 2020 2020 2069 6e5f 6d65 6d6f 7279 3d69       in_memory=i
+000230f0: 6e5f 6d65 6d6f 7279 2c0d 0a20 2020 2020  n_memory,..     
+00023100: 2020 2020 2020 2062 6c6f 636b 3d62 6c6f         block=blo
+00023110: 636b 2c0d 0a20 2020 2020 2020 2020 2020  ck,..           
+00023120: 2070 726f 6772 6573 733d 7072 6f67 7265   progress=progre
+00023130: 7373 2c0d 0a20 2020 2020 2020 2020 2020  ss,..           
+00023140: 2070 726f 6772 6573 735f 6172 6773 3d70   progress_args=p
+00023150: 726f 6772 6573 735f 6172 6773 2c0d 0a20  rogress_args,.. 
+00023160: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00023170: 6173 796e 6320 6465 6620 766f 7465 280d  async def vote(.
+00023180: 0a20 2020 2020 2020 2073 656c 662c 0d0a  .        self,..
+00023190: 2020 2020 2020 2020 6f70 7469 6f6e 3a20          option: 
+000231a0: 696e 742c 0d0a 2020 2020 2920 2d3e 2022  int,..    ) -> "
+000231b0: 7479 7065 732e 506f 6c6c 223a 0d0a 2020  types.Poll":..  
+000231c0: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+000231d0: 6574 686f 6420 2a76 6f74 652a 206f 6620  ethod *vote* of 
+000231e0: 3a6f 626a 3a60 7e66 6970 7065 722e 7479  :obj:`~fipper.ty
+000231f0: 7065 732e 4d65 7373 6167 6560 2e0d 0a0d  pes.Message`....
+00023200: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
+00023210: 6120 7368 6f72 7463 7574 2066 6f72 3a0d  a shortcut for:.
+00023220: 0a0d 0a20 2020 2020 2020 202e 2e20 636f  ...        .. co
+00023230: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+00023240: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
+00023250: 2063 6c69 656e 742e 766f 7465 5f70 6f6c   client.vote_pol
+00023260: 6c28 0d0a 2020 2020 2020 2020 2020 2020  l(..            
+00023270: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
+00023280: 6167 652e 6368 6174 2e69 642c 0d0a 2020  age.chat.id,..  
+00023290: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+000232a0: 7373 6167 655f 6964 3d6d 6573 7361 6765  ssage_id=message
+000232b0: 2e69 642c 0d0a 2020 2020 2020 2020 2020  .id,..          
+000232c0: 2020 2020 2020 6f70 7469 6f6e 3d31 0d0a        option=1..
+000232d0: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
+000232e0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+000232f0: 3a0d 0a20 2020 2020 2020 2020 2020 202e  :..            .
+00023300: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+00023310: 7974 686f 6e0d 0a0d 0a20 2020 2020 2020  ython....       
+00023320: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00023330: 2e76 6f74 6528 3629 0d0a 0d0a 2020 2020  .vote(6)....    
+00023340: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
+00023350: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+00023360: 696f 6e20 2860 6069 6e74 6060 293a 0d0a  ion (``int``):..
+00023370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023380: 496e 6465 7820 6f66 2074 6865 2070 6f6c  Index of the pol
+00023390: 6c20 6f70 7469 6f6e 2079 6f75 2077 616e  l option you wan
+000233a0: 7420 746f 2076 6f74 6520 666f 7220 2830  t to vote for (0
+000233b0: 2074 6f20 3929 2e0d 0a0d 0a20 2020 2020   to 9).....     
+000233c0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+000233d0: 2020 2020 2020 2020 203a 6f62 6a3a 607e           :obj:`~
+000233e0: 6669 7070 6572 2e74 7970 6573 2e50 6f6c  fipper.types.Pol
+000233f0: 6c60 3a20 4f6e 2073 7563 6365 7373 2c20  l`: On success, 
+00023400: 7468 6520 706f 6c6c 2077 6974 6820 7468  the poll with th
+00023410: 6520 6368 6f73 656e 206f 7074 696f 6e20  e chosen option 
+00023420: 6973 2072 6574 7572 6e65 642e 0d0a 0d0a  is returned.....
+00023430: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
+00023440: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
+00023450: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
+00023460: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
+00023470: 2065 7272 6f72 2e0d 0a20 2020 2020 2020   error...       
+00023480: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+00023490: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+000234a0: 662e 5f63 6c69 656e 742e 766f 7465 5f70  f._client.vote_p
+000234b0: 6f6c 6c28 0d0a 2020 2020 2020 2020 2020  oll(..          
+000234c0: 2020 6368 6174 5f69 643d 7365 6c66 2e63    chat_id=self.c
+000234d0: 6861 742e 6964 2c0d 0a20 2020 2020 2020  hat.id,..       
+000234e0: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
+000234f0: 7365 6c66 2e69 642c 0d0a 2020 2020 2020  self.id,..      
+00023500: 2020 2020 2020 6f70 7469 6f6e 733d 6f70        options=op
+00023510: 7469 6f6e 0d0a 2020 2020 2020 2020 290d  tion..        ).
+00023520: 0a0d 0a20 2020 2061 7379 6e63 2064 6566  ...    async def
+00023530: 2070 696e 2873 656c 662c 2064 6973 6162   pin(self, disab
+00023540: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3a  le_notification:
+00023550: 2062 6f6f 6c20 3d20 4661 6c73 652c 2062   bool = False, b
+00023560: 6f74 685f 7369 6465 733a 2062 6f6f 6c20  oth_sides: bool 
+00023570: 3d20 4661 6c73 6529 202d 3e20 2274 7970  = False) -> "typ
+00023580: 6573 2e4d 6573 7361 6765 223a 0d0a 2020  es.Message":..  
+00023590: 2020 2020 2020 2222 2242 6f75 6e64 206d        """Bound m
+000235a0: 6574 686f 6420 2a70 696e 2a20 6f66 203a  ethod *pin* of :
+000235b0: 6f62 6a3a 607e 6669 7070 6572 2e74 7970  obj:`~fipper.typ
+000235c0: 6573 2e4d 6573 7361 6765 602e 0d0a 0d0a  es.Message`.....
+000235d0: 2020 2020 2020 2020 5573 6520 6173 2061          Use as a
+000235e0: 2073 686f 7274 6375 7420 666f 723a 0d0a   shortcut for:..
+000235f0: 0d0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+00023600: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+00023610: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00023620: 6177 6169 7420 636c 6965 6e74 2e70 696e  await client.pin
+00023630: 5f63 6861 745f 6d65 7373 6167 6528 0d0a  _chat_message(..
+00023640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023650: 6368 6174 5f69 643d 6d65 7373 6167 652e  chat_id=message.
+00023660: 6368 6174 2e69 642c 0d0a 2020 2020 2020  chat.id,..      
+00023670: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00023680: 655f 6964 3d6d 6573 7361 6765 5f69 640d  e_id=message_id.
+00023690: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+000236a0: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+000236b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000236c0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+000236d0: 7079 7468 6f6e 0d0a 0d0a 2020 2020 2020  python....      
+000236e0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+000236f0: 6d65 7373 6167 652e 7069 6e28 290d 0a0d  message.pin()...
+00023700: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00023710: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
+00023720: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
+00023730: 6361 7469 6f6e 2028 6060 626f 6f6c 6060  cation (``bool``
+00023740: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00023750: 2020 2020 5061 7373 2054 7275 652c 2069      Pass True, i
+00023760: 6620 6974 2069 7320 6e6f 7420 6e65 6365  f it is not nece
+00023770: 7373 6172 7920 746f 2073 656e 6420 6120  ssary to send a 
+00023780: 6e6f 7469 6669 6361 7469 6f6e 2074 6f20  notification to 
+00023790: 616c 6c20 6368 6174 206d 656d 6265 7273  all chat members
+000237a0: 2061 626f 7574 2074 6865 206e 6577 2070   about the new p
+000237b0: 696e 6e65 640d 0a20 2020 2020 2020 2020  inned..         
+000237c0: 2020 2020 2020 206d 6573 7361 6765 2e20         message. 
+000237d0: 4e6f 7469 6669 6361 7469 6f6e 7320 6172  Notifications ar
+000237e0: 6520 616c 7761 7973 2064 6973 6162 6c65  e always disable
+000237f0: 6420 696e 2063 6861 6e6e 656c 732e 0d0a  d in channels...
+00023800: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
+00023810: 7468 5f73 6964 6573 2028 6060 626f 6f6c  th_sides (``bool
+00023820: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
+00023830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00023840: 2020 5061 7373 2054 7275 6520 746f 2070    Pass True to p
+00023850: 696e 2074 6865 206d 6573 7361 6765 2066  in the message f
+00023860: 6f72 2062 6f74 6820 7369 6465 7320 2879  or both sides (y
+00023870: 6f75 2061 6e64 2072 6563 6970 6965 6e74  ou and recipient
+00023880: 292e 0d0a 2020 2020 2020 2020 2020 2020  )...            
+00023890: 2020 2020 4170 706c 6963 6162 6c65 2074      Applicable t
+000238a0: 6f20 7072 6976 6174 6520 6368 6174 7320  o private chats 
+000238b0: 6f6e 6c79 2e20 4465 6661 756c 7473 2074  only. Defaults t
+000238c0: 6f20 4661 6c73 652e 0d0a 0d0a 2020 2020  o False.....    
+000238d0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+000238e0: 2020 2020 2020 2020 2020 3a6f 626a 3a60            :obj:`
+000238f0: 7e66 6970 7065 722e 7479 7065 732e 4d65  ~fipper.types.Me
+00023900: 7373 6167 6560 3a20 4f6e 2073 7563 6365  ssage`: On succe
+00023910: 7373 2c20 7468 6520 7365 7276 6963 6520  ss, the service 
+00023920: 6d65 7373 6167 6520 6973 2072 6574 7572  message is retur
+00023930: 6e65 642e 0d0a 0d0a 2020 2020 2020 2020  ned.....        
+00023940: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+00023950: 2020 2020 2052 5043 4572 726f 723a 2049       RPCError: I
+00023960: 6e20 6361 7365 206f 6620 6120 5465 6c65  n case of a Tele
+00023970: 6772 616d 2052 5043 2065 7272 6f72 2e0d  gram RPC error..
+00023980: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00023990: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+000239a0: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+000239b0: 7069 6e5f 6368 6174 5f6d 6573 7361 6765  pin_chat_message
+000239c0: 280d 0a20 2020 2020 2020 2020 2020 2063  (..            c
+000239d0: 6861 745f 6964 3d73 656c 662e 6368 6174  hat_id=self.chat
+000239e0: 2e69 642c 0d0a 2020 2020 2020 2020 2020  .id,..          
+000239f0: 2020 6d65 7373 6167 655f 6964 3d73 656c    message_id=sel
+00023a00: 662e 6964 2c0d 0a20 2020 2020 2020 2020  f.id,..         
+00023a10: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+00023a20: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
+00023a30: 6e6f 7469 6669 6361 7469 6f6e 2c0d 0a20  notification,.. 
+00023a40: 2020 2020 2020 2020 2020 2062 6f74 685f             both_
+00023a50: 7369 6465 733d 626f 7468 5f73 6964 6573  sides=both_sides
+00023a60: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+00023a70: 2020 2061 7379 6e63 2064 6566 2075 6e70     async def unp
+00023a80: 696e 2873 656c 6629 202d 3e20 626f 6f6c  in(self) -> bool
+00023a90: 3a0d 0a20 2020 2020 2020 2022 2222 426f  :..        """Bo
+00023aa0: 756e 6420 6d65 7468 6f64 202a 756e 7069  und method *unpi
+00023ab0: 6e2a 206f 6620 3a6f 626a 3a60 7e66 6970  n* of :obj:`~fip
+00023ac0: 7065 722e 7479 7065 732e 4d65 7373 6167  per.types.Messag
+00023ad0: 6560 2e0d 0a0d 0a20 2020 2020 2020 2055  e`.....        U
+00023ae0: 7365 2061 7320 6120 7368 6f72 7463 7574  se as a shortcut
+00023af0: 2066 6f72 3a0d 0a0d 0a20 2020 2020 2020   for:....       
+00023b00: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+00023b10: 2070 7974 686f 6e0d 0a0d 0a20 2020 2020   python....     
+00023b20: 2020 2020 2020 2061 7761 6974 2063 6c69         await cli
+00023b30: 656e 742e 756e 7069 6e5f 6368 6174 5f6d  ent.unpin_chat_m
+00023b40: 6573 7361 6765 280d 0a20 2020 2020 2020  essage(..       
+00023b50: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+00023b60: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
+00023b70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00023b80: 2020 206d 6573 7361 6765 5f69 643d 6d65     message_id=me
+00023b90: 7373 6167 655f 6964 0d0a 2020 2020 2020  ssage_id..      
+00023ba0: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+00023bb0: 2020 2045 7861 6d70 6c65 3a0d 0a20 2020     Example:..   
+00023bc0: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
+00023bd0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
+00023be0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00023bf0: 2020 2061 7761 6974 206d 6573 7361 6765     await message
+00023c00: 2e75 6e70 696e 2829 0d0a 0d0a 2020 2020  .unpin()....    
+00023c10: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00023c20: 2020 2020 2020 2020 2020 5472 7565 206f            True o
+00023c30: 6e20 7375 6363 6573 732e 0d0a 0d0a 2020  n success.....  
+00023c40: 2020 2020 2020 5261 6973 6573 3a0d 0a20        Raises:.. 
+00023c50: 2020 2020 2020 2020 2020 2052 5043 4572             RPCEr
+00023c60: 726f 723a 2049 6e20 6361 7365 206f 6620  ror: In case of 
+00023c70: 6120 5465 6c65 6772 616d 2052 5043 2065  a Telegram RPC e
+00023c80: 7272 6f72 2e0d 0a20 2020 2020 2020 2022  rror...        "
+00023c90: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+00023ca0: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
+00023cb0: 6c69 656e 742e 756e 7069 6e5f 6368 6174  lient.unpin_chat
+00023cc0: 5f6d 6573 7361 6765 280d 0a20 2020 2020  _message(..     
+00023cd0: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
+00023ce0: 656c 662e 6368 6174 2e69 642c 0d0a 2020  elf.chat.id,..  
+00023cf0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00023d00: 655f 6964 3d73 656c 662e 6964 0d0a 2020  e_id=self.id..  
+00023d10: 2020 2020 2020 290d 0a0d 0a20 2020 2061        )....    a
+00023d20: 7379 6e63 2064 6566 2061 736b 280d 0a20  sync def ask(.. 
+00023d30: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+00023d40: 2020 2020 2020 7465 7874 3a20 7374 722c        text: str,
+00023d50: 0d0a 2020 2020 2020 2020 7175 6f74 653a  ..        quote:
+00023d60: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20   bool = None,.. 
+00023d70: 2020 2020 2020 2070 6172 7365 5f6d 6f64         parse_mod
+00023d80: 653a 204f 7074 696f 6e61 6c5b 2265 6e75  e: Optional["enu
+00023d90: 6d73 2e50 6172 7365 4d6f 6465 225d 203d  ms.ParseMode"] =
+00023da0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00023db0: 656e 7469 7469 6573 3a20 4c69 7374 5b22  entities: List["
+00023dc0: 7479 7065 732e 4d65 7373 6167 6545 6e74  types.MessageEnt
+00023dd0: 6974 7922 5d20 3d20 4e6f 6e65 2c0d 0a20  ity"] = None,.. 
+00023de0: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
+00023df0: 6562 5f70 6167 655f 7072 6576 6965 773a  eb_page_preview:
+00023e00: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0d 0a20   bool = None,.. 
+00023e10: 2020 2020 2020 2064 6973 6162 6c65 5f6e         disable_n
+00023e20: 6f74 6966 6963 6174 696f 6e3a 2062 6f6f  otification: boo
+00023e30: 6c20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  l = None,..     
+00023e40: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
+00023e50: 6167 655f 6964 3a20 696e 7420 3d20 4e6f  age_id: int = No
+00023e60: 6e65 2c0d 0a20 2020 2020 2020 2072 6570  ne,..        rep
+00023e70: 6c79 5f6d 6172 6b75 703d 4e6f 6e65 2c0d  ly_markup=None,.
+00023e80: 0a20 2020 2020 2020 2066 696c 7465 7273  .        filters
+00023e90: 3d4e 6f6e 652c 0d0a 2020 2020 2020 2020  =None,..        
+00023ea0: 7469 6d65 6f75 743a 2069 6e74 203d 204e  timeout: int = N
+00023eb0: 6f6e 650d 0a20 2020 2029 202d 3e20 224d  one..    ) -> "M
+00023ec0: 6573 7361 6765 223a 0d0a 2020 2020 2020  essage":..      
+00023ed0: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
+00023ee0: 6420 2a61 736b 2a20 6f66 203a 6f62 6a3a  d *ask* of :obj:
+00023ef0: 607e 6669 7070 6572 2e74 7970 6573 2e4d  `~fipper.types.M
+00023f00: 6573 7361 6765 602e 0d0a 2020 2020 2020  essage`...      
+00023f10: 2020 0d0a 2020 2020 2020 2020 5573 6520    ..        Use 
+00023f20: 6173 2061 2073 686f 7274 6375 7420 666f  as a shortcut fo
+00023f30: 723a 0d0a 2020 2020 2020 2020 2e2e 2063  r:..        .. c
+00023f40: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+00023f50: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00023f60: 636c 6965 6e74 2e73 656e 645f 6d65 7373  client.send_mess
+00023f70: 6167 6528 6368 6174 5f69 642c 2022 5768  age(chat_id, "Wh
+00023f80: 6174 2069 7320 796f 7572 206e 616d 653f  at is your name?
+00023f90: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00023fa0: 636c 6965 6e74 2e77 6169 745f 666f 725f  client.wait_for_
+00023fb0: 6d65 7373 6167 6528 6368 6174 5f69 6429  message(chat_id)
+00023fc0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00023fd0: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+00023fe0: 0d0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
+00023ff0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00024000: 7468 6f6e 0d0a 2020 2020 2020 2020 2020  thon..          
+00024010: 2020 2020 2020 6d65 7373 6167 652e 6173        message.as
+00024020: 6b28 2257 6861 7420 6973 2079 6f75 7220  k("What is your 
+00024030: 6e61 6d65 3f22 290d 0a20 2020 2020 2020  name?")..       
+00024040: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
+00024050: 2020 2020 2020 2020 2020 7465 7874 2028            text (
+00024060: 6060 7374 7260 6029 3a0d 0a20 2020 2020  ``str``):..     
+00024070: 2020 2020 2020 2020 2020 2054 6578 7420             Text 
+00024080: 6f66 2074 6865 206d 6573 7361 6765 2074  of the message t
+00024090: 6f20 6265 2073 656e 742e 0d0a 2020 2020  o be sent...    
+000240a0: 2020 2020 2020 2020 7175 6f74 6520 2860          quote (`
+000240b0: 6062 6f6f 6c60 602c 202a 6f70 7469 6f6e  `bool``, *option
+000240c0: 616c 2a29 3a0d 0a20 2020 2020 2020 2020  al*):..         
+000240d0: 2020 2020 2020 2049 6620 6060 5472 7565         If ``True
+000240e0: 6060 2c20 7468 6520 6d65 7373 6167 6520  ``, the message 
+000240f0: 7769 6c6c 2062 6520 7365 6e74 2061 7320  will be sent as 
+00024100: 6120 7265 706c 7920 746f 2074 6869 7320  a reply to this 
+00024110: 6d65 7373 6167 652e 0d0a 2020 2020 2020  message...      
+00024120: 2020 2020 2020 2020 2020 4966 202a 7265            If *re
+00024130: 706c 795f 746f 5f6d 6573 7361 6765 5f69  ply_to_message_i
+00024140: 642a 2069 7320 7061 7373 6564 2c20 7468  d* is passed, th
+00024150: 6973 2070 6172 616d 6574 6572 2077 696c  is parameter wil
+00024160: 6c20 6265 2069 676e 6f72 6564 2e0d 0a20  l be ignored... 
+00024170: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00024180: 6566 6175 6c74 7320 746f 2060 6054 7275  efaults to ``Tru
+00024190: 6560 6020 696e 2067 726f 7570 2063 6861  e`` in group cha
+000241a0: 7473 2061 6e64 2060 6046 616c 7365 6060  ts and ``False``
+000241b0: 2069 6e20 7072 6976 6174 6520 6368 6174   in private chat
+000241c0: 732e 0d0a 2020 2020 2020 2020 2020 2020  s...            
+000241d0: 7061 7273 655f 6d6f 6465 2028 3a6f 626a  parse_mode (:obj
+000241e0: 3a60 7e66 6970 7065 722e 656e 756d 732e  :`~fipper.enums.
+000241f0: 5061 7273 654d 6f64 6560 2c20 2a6f 7074  ParseMode`, *opt
+00024200: 696f 6e61 6c2a 293a 0d0a 2020 2020 2020  ional*):..      
+00024210: 2020 2020 2020 2020 2020 4279 2064 6566            By def
+00024220: 6175 6c74 2c20 7465 7874 7320 6172 6520  ault, texts are 
+00024230: 7061 7273 6564 2075 7369 6e67 2062 6f74  parsed using bot
+00024240: 6820 4d61 726b 646f 776e 2061 6e64 2048  h Markdown and H
+00024250: 544d 4c20 7374 796c 6573 2e0d 0a20 2020  TML styles...   
+00024260: 2020 2020 2020 2020 2020 2020 2059 6f75               You
+00024270: 2063 616e 2063 6f6d 6269 6e65 2062 6f74   can combine bot
+00024280: 6820 7379 6e74 6178 6573 2074 6f67 6574  h syntaxes toget
+00024290: 6865 722e 0d0a 2020 2020 2020 2020 2020  her...          
+000242a0: 2020 656e 7469 7469 6573 2028 4c69 7374    entities (List
+000242b0: 206f 6620 3a6f 626a 3a60 7e66 6970 7065   of :obj:`~fippe
+000242c0: 722e 7479 7065 732e 4d65 7373 6167 6545  r.types.MessageE
+000242d0: 6e74 6974 7960 293a 0d0a 2020 2020 2020  ntity`):..      
+000242e0: 2020 2020 2020 2020 2020 4c69 7374 206f            List o
+000242f0: 6620 7370 6563 6961 6c20 656e 7469 7469  f special entiti
+00024300: 6573 2074 6861 7420 6170 7065 6172 2069  es that appear i
+00024310: 6e20 6d65 7373 6167 6520 7465 7874 2c20  n message text, 
+00024320: 7768 6963 6820 6361 6e20 6265 2073 7065  which can be spe
+00024330: 6369 6669 6564 2069 6e73 7465 6164 206f  cified instead o
+00024340: 6620 2a70 6172 7365 5f6d 6f64 652a 2e0d  f *parse_mode*..
+00024350: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00024360: 6162 6c65 5f77 6562 5f70 6167 655f 7072  able_web_page_pr
+00024370: 6576 6965 7720 2860 6062 6f6f 6c60 602c  eview (``bool``,
+00024380: 202a 6f70 7469 6f6e 616c 2a29 3a0d 0a20   *optional*):.. 
+00024390: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+000243a0: 6973 6162 6c65 7320 6c69 6e6b 2070 7265  isables link pre
+000243b0: 7669 6577 7320 666f 7220 6c69 6e6b 7320  views for links 
+000243c0: 696e 2074 6869 7320 6d65 7373 6167 652e  in this message.
+000243d0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+000243e0: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+000243f0: 6f6e 2028 6060 626f 6f6c 6060 2c20 2a6f  on (``bool``, *o
+00024400: 7074 696f 6e61 6c2a 293a 0d0a 2020 2020  ptional*):..    
+00024410: 2020 2020 2020 2020 2020 2020 5365 6e64              Send
+00024420: 7320 7468 6520 6d65 7373 6167 6520 7369  s the message si
+00024430: 6c65 6e74 6c79 2e0d 0a20 2020 2020 2020  lently...       
+00024440: 2020 2020 2020 2020 2055 7365 7273 2077           Users w
+00024450: 696c 6c20 7265 6365 6976 6520 6120 6e6f  ill receive a no
+00024460: 7469 6669 6361 7469 6f6e 2077 6974 6820  tification with 
+00024470: 6e6f 2073 6f75 6e64 2e0d 0a20 2020 2020  no sound...     
+00024480: 2020 2020 2020 2072 6570 6c79 5f74 6f5f         reply_to_
+00024490: 6d65 7373 6167 655f 6964 2028 6060 696e  message_id (``in
+000244a0: 7460 602c 202a 6f70 7469 6f6e 616c 2a29  t``, *optional*)
+000244b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000244c0: 2020 2049 6620 7468 6520 6d65 7373 6167     If the messag
+000244d0: 6520 6973 2061 2072 6570 6c79 2c20 4944  e is a reply, ID
+000244e0: 206f 6620 7468 6520 6f72 6967 696e 616c   of the original
+000244f0: 206d 6573 7361 6765 2e0d 0a20 2020 2020   message...     
+00024500: 2020 2020 2020 2072 6570 6c79 5f6d 6172         reply_mar
+00024510: 6b75 7020 283a 6f62 6a3a 607e 6669 7070  kup (:obj:`~fipp
+00024520: 6572 2e74 7970 6573 2e49 6e6c 696e 654b  er.types.InlineK
+00024530: 6579 626f 6172 644d 6172 6b75 7060 207c  eyboardMarkup` |
+00024540: 203a 6f62 6a3a 607e 6669 7070 6572 2e74   :obj:`~fipper.t
+00024550: 7970 6573 2e52 6570 6c79 4b65 7962 6f61  ypes.ReplyKeyboa
+00024560: 7264 4d61 726b 7570 6020 7c20 3a6f 626a  rdMarkup` | :obj
+00024570: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
+00024580: 5265 706c 794b 6579 626f 6172 6452 656d  ReplyKeyboardRem
+00024590: 6f76 6560 207c 203a 6f62 6a3a 607e 6669  ove` | :obj:`~fi
+000245a0: 7070 6572 2e74 7970 6573 2e46 6f72 6365  pper.types.Force
+000245b0: 5265 706c 7960 2c20 2a6f 7074 696f 6e61  Reply`, *optiona
+000245c0: 6c2a 293a 0d0a 2020 2020 2020 2020 2020  l*):..          
+000245d0: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+000245e0: 2069 6e74 6572 6661 6365 206f 7074 696f   interface optio
+000245f0: 6e73 2e20 416e 206f 626a 6563 7420 666f  ns. An object fo
+00024600: 7220 616e 2069 6e6c 696e 6520 6b65 7962  r an inline keyb
+00024610: 6f61 7264 2c20 6375 7374 6f6d 2072 6570  oard, custom rep
+00024620: 6c79 206b 6579 626f 6172 642c 0d0a 2020  ly keyboard,..  
+00024630: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00024640: 7374 7275 6374 696f 6e73 2074 6f20 7265  structions to re
+00024650: 6d6f 7665 2072 6570 6c79 206b 6579 626f  move reply keybo
+00024660: 6172 6420 6f72 2074 6f20 666f 7263 6520  ard or to force 
+00024670: 6120 7265 706c 7920 6672 6f6d 2074 6865  a reply from the
+00024680: 2075 7365 722e 0d0a 2020 2020 2020 2020   user...        
+00024690: 2020 2020 6669 6c74 6572 7320 283a 6f62      filters (:ob
+000246a0: 6a3a 6046 696c 7465 7273 6029 3a0d 0a20  j:`Filters`):.. 
+000246b0: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+000246c0: 6173 7320 6f6e 6520 6f72 206d 6f72 6520  ass one or more 
+000246d0: 6669 6c74 6572 7320 746f 2061 6c6c 6f77  filters to allow
+000246e0: 206f 6e6c 7920 6120 7375 6273 6574 206f   only a subset o
+000246f0: 6620 6361 6c6c 6261 636b 2071 7565 7269  f callback queri
+00024700: 6573 2074 6f20 6265 2070 6173 7365 640d  es to be passed.
+00024710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024720: 2069 6e20 796f 7572 2063 616c 6c62 6163   in your callbac
+00024730: 6b20 6675 6e63 7469 6f6e 2e0d 0a20 2020  k function...   
+00024740: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+00024750: 2028 6060 696e 7460 602c 202a 6f70 7469   (``int``, *opti
+00024760: 6f6e 616c 2a29 3a0d 0a20 2020 2020 2020  onal*):..       
+00024770: 2020 2020 2020 2020 2054 696d 656f 7574           Timeout
+00024780: 2069 6e20 7365 636f 6e64 732e 0d0a 2020   in seconds...  
+00024790: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+000247a0: 2020 2020 2020 2020 2020 2020 3a6f 626a              :obj
+000247b0: 3a60 7e66 6970 7065 722e 7479 7065 732e  :`~fipper.types.
+000247c0: 4d65 7373 6167 6560 3a20 4f6e 2073 7563  Message`: On suc
+000247d0: 6365 7373 2c20 7468 6520 7265 706c 7920  cess, the reply 
+000247e0: 6d65 7373 6167 6520 6973 2072 6574 7572  message is retur
+000247f0: 6e65 642e 0d0a 2020 2020 2020 2020 5261  ned...        Ra
+00024800: 6973 6573 3a0d 0a20 2020 2020 2020 2020  ises:..         
+00024810: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
+00024820: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
+00024830: 616d 2052 5043 2065 7272 6f72 2e0d 0a20  am RPC error... 
+00024840: 2020 2020 2020 2020 2020 2061 7379 6e63             async
+00024850: 696f 2e54 696d 656f 7574 4572 726f 723a  io.TimeoutError:
+00024860: 2049 6e20 6361 7365 2072 6570 6c79 206e   In case reply n
+00024870: 6f74 2072 6563 6569 7665 6420 7769 7468  ot received with
+00024880: 696e 2074 6865 2074 696d 656f 7574 2e0d  in the timeout..
+00024890: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000248a0: 2020 2020 2020 6966 2071 756f 7465 2069        if quote i
+000248b0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+000248c0: 2020 2020 2071 756f 7465 203d 2073 656c       quote = sel
+000248d0: 662e 6368 6174 2e74 7970 6520 213d 2065  f.chat.type != e
+000248e0: 6e75 6d73 2e43 6861 7454 7970 652e 5052  nums.ChatType.PR
+000248f0: 4956 4154 450d 0a0d 0a20 2020 2020 2020  IVATE....       
+00024900: 2069 6620 7265 706c 795f 746f 5f6d 6573   if reply_to_mes
+00024910: 7361 6765 5f69 6420 6973 204e 6f6e 6520  sage_id is None 
+00024920: 616e 6420 7175 6f74 653a 0d0a 2020 2020  and quote:..    
+00024930: 2020 2020 2020 2020 7265 706c 795f 746f          reply_to
+00024940: 5f6d 6573 7361 6765 5f69 6420 3d20 7365  _message_id = se
+00024950: 6c66 2e69 640d 0a0d 0a20 2020 2020 2020  lf.id....       
+00024960: 2072 6571 7565 7374 203d 2061 7761 6974   request = await
+00024970: 2073 656c 662e 5f63 6c69 656e 742e 7365   self._client.se
+00024980: 6e64 5f6d 6573 7361 6765 280d 0a20 2020  nd_message(..   
+00024990: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+000249a0: 3d73 656c 662e 6368 6174 2e69 642c 0d0a  =self.chat.id,..
+000249b0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+000249c0: 3d74 6578 742c 0d0a 2020 2020 2020 2020  =text,..        
+000249d0: 2020 2020 7061 7273 655f 6d6f 6465 3d70      parse_mode=p
+000249e0: 6172 7365 5f6d 6f64 652c 0d0a 2020 2020  arse_mode,..    
+000249f0: 2020 2020 2020 2020 656e 7469 7469 6573          entities
+00024a00: 3d65 6e74 6974 6965 732c 0d0a 2020 2020  =entities,..    
+00024a10: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+00024a20: 7765 625f 7061 6765 5f70 7265 7669 6577  web_page_preview
+00024a30: 3d64 6973 6162 6c65 5f77 6562 5f70 6167  =disable_web_pag
+00024a40: 655f 7072 6576 6965 772c 0d0a 2020 2020  e_preview,..    
+00024a50: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
+00024a60: 6e6f 7469 6669 6361 7469 6f6e 3d64 6973  notification=dis
+00024a70: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00024a80: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
+00024a90: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
+00024aa0: 5f69 643d 7265 706c 795f 746f 5f6d 6573  _id=reply_to_mes
+00024ab0: 7361 6765 5f69 642c 0d0a 2020 2020 2020  sage_id,..      
+00024ac0: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+00024ad0: 7570 3d72 6570 6c79 5f6d 6172 6b75 700d  up=reply_markup.
+00024ae0: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
+00024af0: 2020 2020 2020 7265 706c 795f 6d65 7373        reply_mess
+00024b00: 6167 6520 3d20 6177 6169 7420 7365 6c66  age = await self
+00024b10: 2e5f 636c 6965 6e74 2e77 6169 745f 666f  ._client.wait_fo
+00024b20: 725f 6d65 7373 6167 6528 0d0a 2020 2020  r_message(..    
+00024b30: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+00024b40: 742e 6964 2c0d 0a20 2020 2020 2020 2020  t.id,..         
+00024b50: 2020 2066 696c 7465 7273 3d66 696c 7465     filters=filte
+00024b60: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+00024b70: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+00024b80: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+00024b90: 2020 2020 2020 2072 6570 6c79 5f6d 6573         reply_mes
+00024ba0: 7361 6765 2e72 6571 7565 7374 203d 2072  sage.request = r
+00024bb0: 6571 7565 7374 0d0a 2020 2020 2020 2020  equest..        
+00024bc0: 7265 7475 726e 2072 6570 6c79 5f6d 6573  return reply_mes
+00024bd0: 7361 6765 0d0a                           sage..
```

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/message_entity.py` & `fipper-0.0.2/fipper/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/message_reactions.py` & `fipper-0.0.2/fipper/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/photo.py` & `fipper-0.0.2/fipper/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/poll.py` & `fipper-0.0.2/fipper/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/poll_option.py` & `fipper-0.0.2/fipper/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/reaction.py` & `fipper-0.0.2/fipper/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/sticker.py` & `fipper-0.0.2/fipper/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/stripped_thumbnail.py` & `fipper-0.0.2/fipper/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/thumbnail.py` & `fipper-0.0.2/fipper/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/venue.py` & `fipper-0.0.2/fipper/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/video.py` & `fipper-0.0.2/fipper/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/video_note.py` & `fipper-0.0.2/fipper/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/voice.py` & `fipper-0.0.2/fipper/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/web_app_data.py` & `fipper-0.0.2/fipper/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/messages_and_media/web_page.py` & `fipper-0.0.2/fipper/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/object.py` & `fipper-0.0.2/fipper/types/object.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/update.py` & `fipper-0.0.2/fipper/types/update.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/__init__.py` & `fipper-0.0.2/fipper/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_admin_with_invite_links.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_event.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_event_filter.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_invite_link.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_join_request.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_joiner.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_member.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_member_updated.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_permissions.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_photo.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_preview.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_privileges.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/chat_reactions.py` & `fipper-0.0.2/fipper/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/dialog.py` & `fipper-0.0.2/fipper/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/emoji_status.py` & `fipper-0.0.2/fipper/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/invite_link_importer.py` & `fipper-0.0.2/fipper/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/restriction.py` & `fipper-0.0.2/fipper/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/user.py` & `fipper-0.0.2/fipper/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_ended.py` & `fipper-0.0.2/fipper/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_members_invited.py` & `fipper-0.0.2/fipper/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_scheduled.py` & `fipper-0.0.2/fipper/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/types/user_and_chats/video_chat_started.py` & `fipper-0.0.2/fipper/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper/utils.py` & `fipper-0.0.2/fipper/utils.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/fipper.egg-info/PKG-INFO` & `fipper-0.0.2/fipper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fipper
-Version: 0.0.1.dev5
+Version: 0.0.2
 Summary: Fipper - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/AyiinXd/fipper
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/fipper/issues
 Project-URL: Documentation, https://fipper.tech
```

### Comparing `fipper-0.0.1.dev5/fipper.egg-info/SOURCES.txt` & `fipper-0.0.2/fipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/setup.py` & `fipper-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/tests/__init__.py` & `fipper-0.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/tests/filters/__init__.py` & `fipper-0.0.2/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/tests/filters/test_command.py` & `fipper-0.0.2/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.1.dev5/tests/test_file_id.py` & `fipper-0.0.2/tests/test_file_id.py`

 * *Files identical despite different names*

