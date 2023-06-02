# Comparing `tmp/zen_engine-0.6.0.tar.gz` & `tmp/zen_engine-0.6.1.tar.gz`

## Comparing `zen_engine-0.6.0.tar` & `zen_engine-0.6.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 zen_engine-0.6.0/local_dependencies/zen-engine/Cargo.toml
--rw-r--r--   0     1001      123     4305 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/README.md
--rw-r--r--   0     1001      123     1558 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/benches/engine.rs
--rw-r--r--   0     1001      123     2031 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/decision.rs
--rw-r--r--   0     1001      123     2605 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/engine.rs
--rw-r--r--   0     1001      123      972 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/error.rs
--rw-r--r--   0     1001      123     1651 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/decision.rs
--rw-r--r--   0     1001      123     2136 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/expression/mod.rs
--rw-r--r--   0     1001      123     1097 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/mod.rs
--rw-r--r--   0     1001      123     3046 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/script.rs
--rw-r--r--   0     1001      123     6485 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
--rw-r--r--   0     1001      123      528 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
--rw-r--r--   0     1001      123     1747 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/vm.rs
--rw-r--r--   0     1001      123    11347 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/graph.rs
--rw-r--r--   0     1001      123      115 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/mod.rs
--rw-r--r--   0     1001      123      745 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/node.rs
--rw-r--r--   0     1001      123      807 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/table/mod.rs
--rw-r--r--   0     1001      123     4940 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/table/zen.rs
--rw-r--r--   0     1001      123     4796 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/lib.rs
--rw-r--r--   0     1001      123      715 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/closure.rs
--rw-r--r--   0     1001      123     2449 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/filesystem.rs
--rw-r--r--   0     1001      123     1245 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/memory.rs
--rw-r--r--   0     1001      123      892 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/mod.rs
--rw-r--r--   0     1001      123      466 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/noop.rs
--rw-r--r--   0     1001      123     3152 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/model/mod.rs
--rw-r--r--   0     1001      123     9076 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/util/json_map.rs
--rw-r--r--   0     1001      123       25 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/src/util/mod.rs
--rw-r--r--   0     1001      123     2081 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/tests/decision.rs
--rw-r--r--   0     1001      123     4759 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/tests/engine.rs
--rw-r--r--   0     1001      123     1381 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/tests/model.rs
--rw-r--r--   0     1001      123      884 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-engine/tests/support/mod.rs
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 zen_engine-0.6.0/local_dependencies/zen-expression/Cargo.toml
--rw-r--r--   0     1001      123     2347 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/README.md
--rw-r--r--   0     1001      123      625 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/benches/isolate.rs
--rw-r--r--   0     1001      123    93335 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/benches/lexer.rs
--rw-r--r--   0     1001      123    93602 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/benches/standard.rs
--rw-r--r--   0     1001      123      867 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/benches/unary.rs
--rw-r--r--   0     1001      123      970 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/ast.rs
--rw-r--r--   0     1001      123    18474 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/compiler.rs
--rw-r--r--   0     1001      123     1479 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/helpers.rs
--rw-r--r--   0     1001      123     6819 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/isolate.rs
--rw-r--r--   0     1001      123      769 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/codes.rs
--rw-r--r--   0     1001      123     2035 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/cursor.rs
--rw-r--r--   0     1001      123      404 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/error.rs
--rw-r--r--   0     1001      123     6311 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/lexer.rs
--rw-r--r--   0     1001      123       88 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/mod.rs
--rw-r--r--   0     1001      123      273 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/token.rs
--rw-r--r--   0     1001      123      203 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/lib.rs
--rw-r--r--   0     1001      123     3950 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/opcodes.rs
--rw-r--r--   0     1001      123      922 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/definitions.rs
--rw-r--r--   0     1001      123      638 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/error.rs
--rw-r--r--   0     1001      123     4684 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/iter.rs
--rw-r--r--   0     1001      123      131 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/mod.rs
--rw-r--r--   0     1001      123     4073 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/standard/constants.rs
--rw-r--r--   0     1001      123    13361 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/standard/mod.rs
--rw-r--r--   0     1001      123     2506 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/unary/constants.rs
--rw-r--r--   0     1001      123     9209 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/unary/mod.rs
--rw-r--r--   0     1001      123    45084 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/src/vm.rs
--rw-r--r--   0     1001      123    20080 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/tests/isolate.rs
--rw-r--r--   0     1001      123    11822 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/tests/lexer.rs
--rw-r--r--   0     1001      123     9097 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/tests/standard.rs
--rw-r--r--   0     1001      123     5185 2023-05-09 22:32:34.000000 zen_engine-0.6.0/local_dependencies/zen-expression/tests/unary.rs
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 zen_engine-0.6.0/Cargo.toml
--rw-r--r--   0     1001      123      135 2023-05-09 22:32:34.000000 zen_engine-0.6.0/.bumpversion.cfg
--rw-r--r--   0     1001      123      691 2023-05-09 22:32:34.000000 zen_engine-0.6.0/.gitignore
--rw-r--r--   0     1001      123     1057 2023-05-09 22:32:34.000000 zen_engine-0.6.0/LICENSE
--rw-r--r--   0     1001      123     5965 2023-05-09 22:32:34.000000 zen_engine-0.6.0/README.md
--rw-r--r--   0     1001      123     1578 2023-05-09 22:32:34.000000 zen_engine-0.6.0/index.py
--rw-r--r--   0     1001      123      966 2023-05-09 22:32:34.000000 zen_engine-0.6.0/pyproject.toml
--rw-r--r--   0     1001      123     1429 2023-05-09 22:32:34.000000 zen_engine-0.6.0/src/decision.rs
--rw-r--r--   0     1001      123     3012 2023-05-09 22:32:34.000000 zen_engine-0.6.0/src/engine.rs
--rw-r--r--   0     1001      123      335 2023-05-09 22:32:34.000000 zen_engine-0.6.0/src/lib.rs
--rw-r--r--   0     1001      123     1188 2023-05-09 22:32:34.000000 zen_engine-0.6.0/src/loader.rs
--rw-r--r--   0     1001      123     1122 2023-05-09 22:32:34.000000 zen_engine-0.6.0/src/value.rs
--rw-r--r--   0     1001      123    48426 2023-05-09 22:34:49.000000 zen_engine-0.6.0/Cargo.lock
--rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 zen_engine-0.6.1/local_dependencies/zen-expression/Cargo.toml
+-rw-r--r--   0     1001      123     2347 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/README.md
+-rw-r--r--   0     1001      123      625 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/isolate.rs
+-rw-r--r--   0     1001      123    93335 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/lexer.rs
+-rw-r--r--   0     1001      123    93602 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/standard.rs
+-rw-r--r--   0     1001      123      867 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/benches/unary.rs
+-rw-r--r--   0     1001      123      970 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/ast.rs
+-rw-r--r--   0     1001      123    18474 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/compiler.rs
+-rw-r--r--   0     1001      123     1479 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/helpers.rs
+-rw-r--r--   0     1001      123     6819 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/isolate.rs
+-rw-r--r--   0     1001      123      769 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/codes.rs
+-rw-r--r--   0     1001      123     2035 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/cursor.rs
+-rw-r--r--   0     1001      123      404 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/error.rs
+-rw-r--r--   0     1001      123     6311 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/lexer.rs
+-rw-r--r--   0     1001      123       88 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/mod.rs
+-rw-r--r--   0     1001      123      273 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/token.rs
+-rw-r--r--   0     1001      123      203 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/lib.rs
+-rw-r--r--   0     1001      123     3950 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/opcodes.rs
+-rw-r--r--   0     1001      123      922 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/definitions.rs
+-rw-r--r--   0     1001      123      638 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/error.rs
+-rw-r--r--   0     1001      123     4684 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/iter.rs
+-rw-r--r--   0     1001      123      131 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/mod.rs
+-rw-r--r--   0     1001      123     4073 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/constants.rs
+-rw-r--r--   0     1001      123    13361 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/mod.rs
+-rw-r--r--   0     1001      123     2506 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/constants.rs
+-rw-r--r--   0     1001      123     9209 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/mod.rs
+-rw-r--r--   0     1001      123    45084 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/src/vm.rs
+-rw-r--r--   0     1001      123    20080 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/isolate.rs
+-rw-r--r--   0     1001      123    11822 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/lexer.rs
+-rw-r--r--   0     1001      123     9097 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/standard.rs
+-rw-r--r--   0     1001      123     5185 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-expression/tests/unary.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.6.1/local_dependencies/zen-engine/Cargo.toml
+-rw-r--r--   0     1001      123     4305 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/README.md
+-rw-r--r--   0     1001      123     1558 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/benches/engine.rs
+-rw-r--r--   0     1001      123     2031 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/decision.rs
+-rw-r--r--   0     1001      123     2605 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/engine.rs
+-rw-r--r--   0     1001      123      972 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/error.rs
+-rw-r--r--   0     1001      123     1651 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/decision.rs
+-rw-r--r--   0     1001      123     2136 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/expression/mod.rs
+-rw-r--r--   0     1001      123     1097 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/mod.rs
+-rw-r--r--   0     1001      123     3046 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/script.rs
+-rw-r--r--   0     1001      123     6485 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
+-rw-r--r--   0     1001      123      528 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
+-rw-r--r--   0     1001      123     1747 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/vm.rs
+-rw-r--r--   0     1001      123    11347 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/graph.rs
+-rw-r--r--   0     1001      123      115 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/mod.rs
+-rw-r--r--   0     1001      123      745 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/node.rs
+-rw-r--r--   0     1001      123      807 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/mod.rs
+-rw-r--r--   0     1001      123     4940 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/zen.rs
+-rw-r--r--   0     1001      123     4796 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/lib.rs
+-rw-r--r--   0     1001      123      715 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/closure.rs
+-rw-r--r--   0     1001      123     2449 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/filesystem.rs
+-rw-r--r--   0     1001      123     1245 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/memory.rs
+-rw-r--r--   0     1001      123      892 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/mod.rs
+-rw-r--r--   0     1001      123      466 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/noop.rs
+-rw-r--r--   0     1001      123     3152 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/model/mod.rs
+-rw-r--r--   0     1001      123     9076 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/util/json_map.rs
+-rw-r--r--   0     1001      123       25 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/src/util/mod.rs
+-rw-r--r--   0     1001      123     2081 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/decision.rs
+-rw-r--r--   0     1001      123     4759 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/engine.rs
+-rw-r--r--   0     1001      123     1381 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/model.rs
+-rw-r--r--   0     1001      123      884 2023-06-02 14:18:17.000000 zen_engine-0.6.1/local_dependencies/zen-engine/tests/support/mod.rs
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.6.1/Cargo.toml
+-rw-r--r--   0     1001      123      135 2023-06-02 14:18:17.000000 zen_engine-0.6.1/.bumpversion.cfg
+-rw-r--r--   0     1001      123      691 2023-06-02 14:18:17.000000 zen_engine-0.6.1/.gitignore
+-rw-r--r--   0     1001      123     1057 2023-06-02 14:18:17.000000 zen_engine-0.6.1/LICENSE
+-rw-r--r--   0     1001      123     5965 2023-06-02 14:18:17.000000 zen_engine-0.6.1/README.md
+-rw-r--r--   0     1001      123     1578 2023-06-02 14:18:17.000000 zen_engine-0.6.1/index.py
+-rw-r--r--   0     1001      123      966 2023-06-02 14:18:17.000000 zen_engine-0.6.1/pyproject.toml
+-rw-r--r--   0     1001      123     1429 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/decision.rs
+-rw-r--r--   0     1001      123     3012 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/engine.rs
+-rw-r--r--   0     1001      123      335 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/lib.rs
+-rw-r--r--   0     1001      123     1188 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/loader.rs
+-rw-r--r--   0     1001      123     1122 2023-06-02 14:18:17.000000 zen_engine-0.6.1/src/value.rs
+-rw-r--r--   0     1001      123    48962 2023-06-02 14:20:03.000000 zen_engine-0.6.1/Cargo.lock
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.6.1/PKG-INFO
```

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/Cargo.toml` & `zen_engine-0.6.1/local_dependencies/zen-engine/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Business rules engine"
 name = "zen-engine"
 license = "MIT"
-version = "0.5.1"
+version = "0.5.2"
 edition = "2021"
 repository = "https://github.com/gorules/zen.git"
 
 [lib]
 doctest = false
 
 [dependencies]
 async-recursion = "1.0.4"
-anyhow = "1.0.70"
+anyhow = "1.0.71"
 thiserror = "1.0.40"
 async-trait = "0.1.68"
-bincode = { version = "2.0.0-rc.2", optional = true }
-serde_json = { version = "1.0.95", features = ["arbitrary_precision"] }
-serde = { version = "1", features = ["derive"] }
-serde_v8 = { version = "0.88.0" }
-once_cell = { version = "1.17.1" }
-futures = "0.3.27"
-v8 = { version = "0.66.0" }
-zen-expression = { path = "../zen-expression", version = "0.5.1" }
+bincode = { version = "2.0.0-rc.3", optional = true }
+serde_json = { version = "1.0.96", features = ["arbitrary_precision"] }
+serde = { version = "1.0.163", features = ["derive"] }
+serde_v8 = { version = "0.100.0" }
+once_cell = { version = "1.17.2" }
+futures = "0.3.28"
+v8 = { version = "0.73.0" }
+zen-expression = { path = "../zen-expression", version = "0.5.2" }
 
 [features]
 bincode = ["dep:bincode"]
 
 [[bench]]
 harness = false
 name = "engine"
```

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/README.md` & `zen_engine-0.6.1/local_dependencies/zen-engine/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/benches/engine.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/benches/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/decision.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/engine.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/error.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/decision.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/expression/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/script.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/script.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/scripts/internals.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/function/vm.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/function/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/graph.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/graph.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/node.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/node.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/table/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/handler/table/zen.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/handler/table/zen.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/lib.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/closure.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/closure.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/filesystem.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/filesystem.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/memory.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/memory.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/loader/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/loader/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/model/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/model/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/src/util/json_map.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/src/util/json_map.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/tests/decision.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/tests/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/tests/engine.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/tests/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/tests/model.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/tests/model.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-engine/tests/support/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-engine/tests/support/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/Cargo.toml` & `zen_engine-0.6.1/local_dependencies/zen-expression/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Zen Expression Language"
 name = "zen-expression"
 license = "MIT"
-version = "0.5.1"
+version = "0.5.2"
 edition = "2021"
 repository = "https://github.com/gorules/zen.git"
 
 
 [dependencies]
 ahash = "0.8.3"
-bumpalo = "3.12.0"
-chrono = "0.4.24"
+bumpalo = "3.13.0"
+chrono = "0.4.26"
 hashbrown = { version = "0.13.2", features = ["bumpalo"] }
 humantime = "2.1.0"
 fastrand = "1.9.0"
-once_cell = "1.17.1"
+once_cell = "1.17.2"
 phf = { version = "0.11.1", features = ["macros"] }
-serde_json = { version = "1.0.95", features = ["arbitrary_precision"] }
+serde_json = { version = "1.0.96", features = ["arbitrary_precision"] }
 thiserror = "1.0.40"
 rust_decimal = { version = "1.29.1", features = ["maths-nopanic"] }
 rust_decimal_macros = "1.29.1"
 
 [[bench]]
 harness = false
 name = "unary"
```

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/README.md` & `zen_engine-0.6.1/local_dependencies/zen-expression/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/benches/isolate.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/benches/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/benches/lexer.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/benches/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/benches/standard.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/benches/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/benches/unary.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/benches/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/ast.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/ast.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/compiler.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/helpers.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/isolate.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/codes.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/codes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/cursor.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/cursor.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/lexer/lexer.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/lexer/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/opcodes.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/opcodes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/definitions.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/definitions.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/error.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/iter.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/iter.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/standard/constants.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/standard/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/standard/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/unary/constants.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/parser/unary/mod.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/parser/unary/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/src/vm.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/src/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/tests/isolate.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/tests/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/tests/lexer.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/tests/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/tests/standard.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/tests/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/local_dependencies/zen-expression/tests/unary.rs` & `zen_engine-0.6.1/local_dependencies/zen-expression/tests/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/.gitignore` & `zen_engine-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/LICENSE` & `zen_engine-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/README.md` & `zen_engine-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/index.py` & `zen_engine-0.6.1/index.py`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/pyproject.toml` & `zen_engine-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/src/decision.rs` & `zen_engine-0.6.1/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/src/engine.rs` & `zen_engine-0.6.1/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/src/loader.rs` & `zen_engine-0.6.1/src/loader.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/src/value.rs` & `zen_engine-0.6.1/src/value.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.6.0/Cargo.lock` & `zen_engine-0.6.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -46,14 +52,20 @@
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
+name = "anstyle"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+
+[[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arrayvec"
@@ -65,37 +77,26 @@
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
-]
-
-[[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -123,17 +124,29 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.2.1"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24a6904aef64d73cf10ab17ebace7befb918b82164785cb89907993be7f83813"
+checksum = "6776fc96284a0bb647b615056fc496d1fe1644a7ab01829818a6d91cae888b84"
+
+[[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
 
 [[package]]
 name = "borsh"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4114279215a005bc675e386011e594e1d9b800918cea18fcadadcce864a2046b"
 dependencies = [
@@ -174,34 +187,34 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.2"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytecheck"
-version = "0.6.10"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13fe11640a23eb24562225322cd3e452b93a3d4091d62fab69c70542fcd17d1f"
+checksum = "8b6372023ac861f6e6dc89c8344a8f398fb42aaba2b5dbc649ca0c0e9dbcb627"
 dependencies = [
  "bytecheck_derive",
  "ptr_meta",
  "simdutf8",
 ]
 
 [[package]]
 name = "bytecheck_derive"
-version = "0.6.10"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e31225543cb46f81a7e224762764f4a6a0f097b1db0b175f69e8065efaa42de5"
+checksum = "a7ec4c6f261935ad534c0c22dbef2201b45918860eb1c574b972bd213a76af61"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -232,21 +245,21 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
@@ -274,42 +287,37 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.25"
+version = "4.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
+checksum = "b4ed2379f8603fa2b7509891660e802b88c70a79a6427a70abb5968054de2c28"
 dependencies = [
- "bitflags 1.3.2",
- "clap_lex",
- "indexmap",
- "textwrap",
+ "clap_builder",
 ]
 
 [[package]]
-name = "clap_lex"
-version = "0.2.4"
+name = "clap_builder"
+version = "4.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
+checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
 dependencies = [
- "os_str_bytes",
+ "anstyle",
+ "bitflags 1.3.2",
+ "clap_lex",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
+name = "clap_lex"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
@@ -326,28 +334,28 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "criterion"
-version = "0.4.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
 dependencies = [
  "anes",
- "atty",
  "cast",
  "ciborium",
  "clap",
  "criterion-plot",
  "futures",
+ "is-terminal",
  "itertools",
- "lazy_static",
  "num-traits",
+ "once_cell",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
  "serde_derive",
  "serde_json",
@@ -406,86 +414,63 @@
 checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.2.0"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
+checksum = "1586fa608b1dab41f667475b4a41faec5ba680aee428bfa5de4ea520fdc6e901"
 dependencies = [
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.94"
+name = "derive_more"
+version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
+checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
+ "convert_case 0.4.0",
  "proc-macro2",
  "quote",
- "scratch",
- "syn 2.0.15",
+ "rustc_version",
+ "syn 1.0.109",
 ]
 
 [[package]]
-name = "cxxbridge-flags"
-version = "1.0.94"
+name = "either"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
-name = "cxxbridge-macro"
-version = "1.0.94"
+name = "errno"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.15",
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "derive_more"
-version = "0.99.17"
+name = "errno-dragonfly"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
- "convert_case 0.4.0",
- "proc-macro2",
- "quote",
- "rustc_version",
- "syn 1.0.109",
+ "cc",
+ "libc",
 ]
 
 [[package]]
-name = "either"
-version = "1.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
-
-[[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
@@ -497,14 +482,20 @@
 checksum = "57eafdd0c16f57161105ae1b98a1238f97645f2f588438b2949c99a2af9616bf"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "funty"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
+
+[[package]]
 name = "futures"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -552,15 +543,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -623,29 +614,26 @@
 dependencies = [
  "ahash 0.8.3",
  "bumpalo",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
@@ -661,30 +649,19 @@
  "js-sys",
  "wasm-bindgen",
  "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
-dependencies = [
- "cxx",
- "cxx-build",
-]
-
-[[package]]
-name = "indexmap"
-version = "1.9.3"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "autocfg",
- "hashbrown 0.12.3",
+ "cc",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
@@ -695,14 +672,37 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "io-lifetimes"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "is-terminal"
+version = "0.4.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "io-lifetimes",
+ "rustix",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -711,28 +711,22 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.62"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68c16e1bfd491478ab155fd8b4896b86f9ede344949b641e61501e07c2b8b4d5"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "lazy_static"
-version = "1.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
-
-[[package]]
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libloading"
@@ -741,40 +735,34 @@
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
-name = "link-cplusplus"
-version = "1.0.8"
+name = "linux-raw-sys"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -785,20 +773,20 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "napi"
-version = "2.12.6"
+version = "2.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49ac8112fe5998579b22e29903c7b277fc7f91c7860c0236f35792caf8156e18"
+checksum = "d7f0a2e93526dd9c8c522d72a4d0c88678be8966fabe9fb8f2947fde6339b682"
 dependencies = [
  "anyhow",
- "bitflags 2.2.1",
+ "bitflags 2.3.1",
  "ctor",
  "napi-derive",
  "napi-sys",
  "once_cell",
  "serde",
  "serde_json",
  "tokio",
@@ -808,31 +796,31 @@
 name = "napi-build"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "882a73d9ef23e8dc2ebbffb6a6ae2ef467c0f18ac10711e4cc59c5485d41df0e"
 
 [[package]]
 name = "napi-derive"
-version = "2.12.5"
+version = "2.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c47e0f395207c062e680a158f0624ec456c1dfb3c96a8cb888e0401506d50ae9"
+checksum = "da1c6a8fa84d549aa8708fcd062372bf8ec6e849de39016ab921067d21bde367"
 dependencies = [
  "cfg-if",
  "convert_case 0.6.0",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.51"
+version = "1.0.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a83afae5b4ba6f98ed6e33a52da343fdeb66474f1162a38cde5a3d46eb054e7"
+checksum = "20bbc7c69168d06a848f925ec5f0e0997f98e8c8d4f2cc30157f0da51c009e17"
 dependencies = [
  "convert_case 0.6.0",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
  "semver",
@@ -853,14 +841,15 @@
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
+ "rand",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
@@ -886,31 +875,25 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
-name = "os_str_bytes"
-version = "6.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1024,17 +1007,17 @@
 checksum = "1d6ea3c4595b96363c13943497db34af4460fb474a95c43f4446ad341b8c9785"
 dependencies = [
  "toml",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1125,22 +1108,28 @@
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
@@ -1195,57 +1184,60 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rend"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "581008d2099240d37fb08d77ad713bcaec2c4d89d50b5b21a8bb1996bbab68ab"
 dependencies = [
  "bytecheck",
 ]
 
 [[package]]
 name = "rkyv"
-version = "0.7.41"
+version = "0.7.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21499ed91807f07ae081880aabb2ccc0235e9d88011867d984525e9a4c3cfa3e"
+checksum = "0200c8230b013893c0b2d6213d6ec64ed2b9be2e0e016682b7224ff82cff5c58"
 dependencies = [
+ "bitvec",
  "bytecheck",
  "hashbrown 0.12.3",
  "ptr_meta",
  "rend",
  "rkyv_derive",
  "seahash",
+ "tinyvec",
+ "uuid",
 ]
 
 [[package]]
 name = "rkyv_derive"
-version = "0.7.41"
+version = "0.7.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac1c672430eb41556291981f45ca900a0239ad007242d1cb4b4167af842db666"
+checksum = "b2e06b915b5c230a17d7a736d1e2e63ee753c256a8614ef3f5147b13a4f5541d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -1282,14 +1274,28 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.37.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+dependencies = [
+ "bitflags 1.3.2",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
@@ -1303,36 +1309,30 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
-
-[[package]]
 name = "seahash"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
 
 [[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.9"
@@ -1340,21 +1340,21 @@
 checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -1362,24 +1362,25 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_v8"
-version = "0.88.0"
+version = "0.100.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b163edac8a2f2536ae7b52f839a33aba7892c04d0cf21e1bf8213ecfc905ebcc"
+checksum = "1e66031ca2e6c4b682cf0377633992f3c0ec3fda65701ff14fee99d6ff5eeeeb"
 dependencies = [
  "bytes",
  "derive_more",
  "num-bigint",
  "serde",
  "serde_bytes",
  "smallvec",
+ "thiserror",
  "v8",
 ]
 
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1415,43 +1416,34 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
-
-[[package]]
-name = "termcolor"
-version = "1.2.0"
+name = "tap"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
-dependencies = [
- "winapi-util",
-]
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
-name = "textwrap"
-version = "0.16.0"
+name = "target-lexicon"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
@@ -1462,15 +1454,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -1487,18 +1479,33 @@
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
 name = "tokio"
-version = "1.28.0"
+version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "num_cpus",
  "pin-project-lite",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
@@ -1507,59 +1514,59 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
-
-[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "uuid"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
+
+[[package]]
 name = "v8"
-version = "0.66.0"
+version = "0.73.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8ab8597b885c17b3761f6ffc29b7a62758612c409285a9271c6dacd17bb745"
+checksum = "e1bd3f04ba5065795dae6e3db668ff0b628920fbd2e39c1755e9b62d93660c3c"
 dependencies = [
  "bitflags 1.3.2",
  "fslock",
- "lazy_static",
+ "once_cell",
  "which",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1591,71 +1598,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.85"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b6cb788c4e39112fbe1822277ef6fb3c55cd86b95cb3d3c4c1c9597e4ac74b4"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.85"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35e522ed4105a9d626d885b35d62501b30d9666283a5c8be12c14a8bdafe7822"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.85"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "358a79a0cb89d21db8120cbfb91392335913e4890665b1a7981d9e956903b434"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.85"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4783ce29f09b9d93134d41297aded3a712b7b979e9c6f28c32cb88c973a94869"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.85"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a901d592cafaa4d711bc324edfaff879ac700b19c3dfd60058d2b445be2691eb"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.62"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b5f940c7edfdc6d12126d98c9ef4d1b3d470011c47c76a6581df47ad9ba721"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "which"
@@ -1837,16 +1844,25 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
-name = "zen-engine"
+name = "wyz"
 version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+dependencies = [
+ "tap",
+]
+
+[[package]]
+name = "zen-engine"
+version = "0.5.2"
 dependencies = [
  "anyhow",
  "async-recursion",
  "async-trait",
  "bincode",
  "criterion",
  "futures",
@@ -1858,15 +1874,15 @@
  "tokio",
  "v8",
  "zen-expression",
 ]
 
 [[package]]
 name = "zen-expression"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "ahash 0.8.3",
  "bumpalo",
  "chrono",
  "criterion",
  "fastrand",
  "hashbrown 0.13.2",
@@ -1890,15 +1906,15 @@
  "napi-derive",
  "serde_json",
  "zen-engine",
 ]
 
 [[package]]
 name = "zen-python"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "anyhow",
  "async-trait",
  "futures",
  "pyo3",
  "pythonize",
  "serde",
```

### Comparing `zen_engine-0.6.0/PKG-INFO` & `zen_engine-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-engine
-Version: 0.6.0
+Version: 0.6.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

