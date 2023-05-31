# Comparing `tmp/polyglot_piranha-0.3.5.tar.gz` & `tmp/polyglot_piranha-0.3.7.tar.gz`

## Comparing `polyglot_piranha-0.3.5.tar` & `polyglot_piranha-0.3.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.5/Cargo.toml
--rw-r--r--   0     1001      123    35640 2023-05-30 17:34:13.000000 polyglot_piranha-0.3.5/Cargo.lock
--rw-r--r--   0     1001      123    11359 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/LICENSE
--rw-r--r--   0     1001      123     3091 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/README.md
--rw-r--r--   0     1001      123     1373 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
--rw-r--r--   0     1001      123      994 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
--rw-r--r--   0     1001      123     5517 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
--rw-r--r--   0     1001      123     5621 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
--rw-r--r--   0     1001      123    66915 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
--rw-r--r--   0     1001      123    21518 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
--rw-r--r--   0     1001      123     5106 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
--rw-r--r--   0     1001      123      377 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
--rw-r--r--   0     1001      123     3615 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
--rw-r--r--   0     1001      123     5039 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
--rw-r--r--   0     1001      123     2584 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
--rw-r--r--   0     1001      123     2605 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
--rw-r--r--   0     1001      123      550 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
--rw-r--r--   0     1001      123     2456 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
--rw-r--r--   0     1001      123    13106 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
--rw-r--r--   0     1001      123     5875 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
--rw-r--r--   0     1001      123    85120 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
--rw-r--r--   0     1001      123    55188 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
--rw-r--r--   0     1001      123    48474 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
--rw-r--r--   0     1001      123     2304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
--rw-r--r--   0     1001      123    33367 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
--rw-r--r--   0     1001      123     6780 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
--rw-r--r--   0     1001      123     3480 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
--rw-r--r--   0     1001      123     8540 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
--rw-r--r--   0     1001      123     4153 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
--rw-r--r--   0     1001      123     4326 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
--rw-r--r--   0     1001      123     2555 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
--rw-r--r--   0     1001      123     1490 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
--rw-r--r--   0     1001      123     2091 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
--rw-r--r--   0     1001      123     2194 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
--rw-r--r--   0     1001      123     1550 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
--rw-r--r--   0     1001      123     1618 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
--rw-r--r--   0     1001      123     1573 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
--rw-r--r--   0     1001      123       75 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
--rw-r--r--   0     1001      123      109 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
--rw-r--r--   0     1001      123      175 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
--rw-r--r--   0     1001      123      103 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
--rw-r--r--   0     1001      123      154 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
--rw-r--r--   0     1001      123      155 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
--rw-r--r--   0     1001      123      160 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
--rw-r--r--   0     1001      123      122 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
--rw-r--r--   0     1001      123      229 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
--rw-r--r--   0     1001      123       97 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
--rw-r--r--   0     1001      123      202 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
--rw-r--r--   0     1001      123      213 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
--rw-r--r--   0     1001      123      216 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
--rw-r--r--   0     1001      123      361 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
--rw-r--r--   0     1001      123      525 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
--rw-r--r--   0     1001      123      526 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
--rw-r--r--   0     1001      123      488 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
--rw-r--r--   0     1001      123      489 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
--rw-r--r--   0     1001      123      526 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
--rw-r--r--   0     1001      123      704 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
--rw-r--r--   0     1001      123     1332 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
--rw-r--r--   0     1001      123      192 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
--rw-r--r--   0     1001      123      739 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
--rw-r--r--   0     1001      123      652 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
--rw-r--r--   0     1001      123     1896 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
--rw-r--r--   0     1001      123      844 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return.json
--rw-r--r--   0     1001      123     1776 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
--rw-r--r--   0     1001      123     1932 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
--rw-r--r--   0     1001      123     4525 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
--rw-r--r--   0     1001      123      251 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
--rw-r--r--   0     1001      123      246 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
--rw-r--r--   0     1001      123      142 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
--rw-r--r--   0     1001      123     1637 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
--rw-r--r--   0     1001      123     1304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
--rw-r--r--   0     1001      123     1304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
--rw-r--r--   0     1001      123     1107 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
--rw-r--r--   0     1001      123     2565 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/config_checker.js
--rw-r--r--   0     1001      123     4304 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/piranha.js
--rw-r--r--   0     1001      123    27988 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/refactor.js
--rw-r--r--   0     1001      123     1445 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/javascript/src/source_checker.js
--rw-r--r--   0     1001      123      646 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
--rw-r--r--   0     1001      123     1064 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/README.txt
--rw-r--r--   0     1001      123    26229 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
--rw-r--r--   0     1001      123        0 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
--rw-r--r--   0     1001      123      793 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/pyproject.toml
--rw-r--r--   0     1001      123     2043 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/go/edges.toml
--rw-r--r--   0     1001      123    11039 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/go/rules.toml
--rw-r--r--   0     1001      123     1466 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/go/scope_config.toml
--rwxr-xr-x   0     1001      123     2241 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/java/edges.toml
--rwxr-xr-x   0     1001      123    17674 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/java/rules.toml
--rwxr-xr-x   0     1001      123     3580 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/java/scope_config.toml
--rwxr-xr-x   0     1001      123     2251 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/kt/edges.toml
--rwxr-xr-x   0     1001      123    19368 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/kt/rules.toml
--rwxr-xr-x   0     1001      123     2142 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/kt/scope_config.toml
--rw-r--r--   0     1001      123     2316 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/swift/edges.toml
--rw-r--r--   0     1001      123    27137 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/swift/rules.toml
--rw-r--r--   0     1001      123     1684 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/cleanup_rules/swift/scope_config.toml
--rw-r--r--   0     1001      123     7391 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/lib.rs
--rw-r--r--   0     1001      123     1679 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/main.rs
--rw-r--r--   0     1001      123     3583 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/default_configs.rs
--rw-r--r--   0     1001      123     4915 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/edit.rs
--rw-r--r--   0     1001      123    11028 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/filter.rs
--rw-r--r--   0     1001      123     7097 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/language.rs
--rw-r--r--   0     1001      123    11128 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/matches.rs
--rw-r--r--   0     1001      123      924 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/mod.rs
--rw-r--r--   0     1001      123     1987 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/outgoing_edges.rs
--rw-r--r--   0     1001      123    14245 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/piranha_arguments.rs
--rw-r--r--   0     1001      123     2091 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/piranha_output.rs
--rw-r--r--   0     1001      123     7801 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/rule.rs
--rw-r--r--   0     1001      123     6286 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/rule_graph.rs
--rw-r--r--   0     1001      123     6288 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/rule_store.rs
--rw-r--r--   0     1001      123     3402 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/scopes.rs
--rw-r--r--   0     1001      123    14473 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/source_code_unit.rs
--rw-r--r--   0     1001      123     1661 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/piranha_arguments_test.rs
--rw-r--r--   0     1001      123     8344 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/rule_test.rs
--rw-r--r--   0     1001      123     6067 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/scopes_test.rs
--rw-r--r--   0     1001      123    13356 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/models/unit_tests/source_code_unit_test.rs
--rw-r--r--   0     1001      123     8260 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/mod.rs
--rw-r--r--   0     1001      123     1647 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_go.rs
--rw-r--r--   0     1001      123    12953 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_java.rs
--rw-r--r--   0     1001      123     1862 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_kt.rs
--rw-r--r--   0     1001      123     2423 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_python.rs
--rw-r--r--   0     1001      123     3532 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_swift.rs
--rw-r--r--   0     1001      123      770 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_thrift.rs
--rw-r--r--   0     1001      123     1138 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_ts.rs
--rw-r--r--   0     1001      123     1281 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/tests/test_piranha_tsx.rs
--rw-r--r--   0     1001      123     5629 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/mod.rs
--rw-r--r--   0     1001      123    12743 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/tree_sitter_utilities.rs
--rw-r--r--   0     1001      123     3681 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/unit_tests/tree_sitter_utilities_test.rs
--rw-r--r--   0     1001      123     2237 2023-05-30 17:31:22.000000 polyglot_piranha-0.3.5/src/utilities/unit_tests/utilities_test.rs
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.7/Cargo.toml
+-rw-r--r--   0     1001      123    35640 2023-05-31 21:26:20.000000 polyglot_piranha-0.3.7/Cargo.lock
+-rw-r--r--   0     1001      123    11359 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/LICENSE
+-rw-r--r--   0     1001      123     3091 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/README.md
+-rw-r--r--   0     1001      123     1373 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
+-rw-r--r--   0     1001      123      994 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
+-rw-r--r--   0     1001      123     5517 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
+-rw-r--r--   0     1001      123     5621 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
+-rw-r--r--   0     1001      123    66915 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
+-rw-r--r--   0     1001      123    21518 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
+-rw-r--r--   0     1001      123     5106 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
+-rw-r--r--   0     1001      123      377 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
+-rw-r--r--   0     1001      123     3615 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
+-rw-r--r--   0     1001      123     5039 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
+-rw-r--r--   0     1001      123     2584 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
+-rw-r--r--   0     1001      123     2605 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
+-rw-r--r--   0     1001      123      550 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
+-rw-r--r--   0     1001      123     2456 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
+-rw-r--r--   0     1001      123    13106 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
+-rw-r--r--   0     1001      123     5875 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
+-rw-r--r--   0     1001      123    85120 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
+-rw-r--r--   0     1001      123    55188 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
+-rw-r--r--   0     1001      123    48474 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
+-rw-r--r--   0     1001      123     2304 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
+-rw-r--r--   0     1001      123    33367 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
+-rw-r--r--   0     1001      123     6780 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
+-rw-r--r--   0     1001      123     3480 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
+-rw-r--r--   0     1001      123     8540 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
+-rw-r--r--   0     1001      123     4153 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
+-rw-r--r--   0     1001      123     4326 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
+-rw-r--r--   0     1001      123     2555 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
+-rw-r--r--   0     1001      123     1490 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
+-rw-r--r--   0     1001      123     2091 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
+-rw-r--r--   0     1001      123     2194 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
+-rw-r--r--   0     1001      123     1550 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
+-rw-r--r--   0     1001      123     1618 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
+-rw-r--r--   0     1001      123     1573 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
+-rw-r--r--   0     1001      123       75 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
+-rw-r--r--   0     1001      123      109 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
+-rw-r--r--   0     1001      123      175 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
+-rw-r--r--   0     1001      123      103 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
+-rw-r--r--   0     1001      123      154 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
+-rw-r--r--   0     1001      123      155 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
+-rw-r--r--   0     1001      123      160 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
+-rw-r--r--   0     1001      123      122 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
+-rw-r--r--   0     1001      123      229 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
+-rw-r--r--   0     1001      123       97 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
+-rw-r--r--   0     1001      123      202 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
+-rw-r--r--   0     1001      123      213 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
+-rw-r--r--   0     1001      123      216 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
+-rw-r--r--   0     1001      123      361 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
+-rw-r--r--   0     1001      123      525 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
+-rw-r--r--   0     1001      123      526 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
+-rw-r--r--   0     1001      123      488 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
+-rw-r--r--   0     1001      123      489 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
+-rw-r--r--   0     1001      123      526 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
+-rw-r--r--   0     1001      123      704 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
+-rw-r--r--   0     1001      123     1332 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
+-rw-r--r--   0     1001      123      192 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
+-rw-r--r--   0     1001      123      739 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
+-rw-r--r--   0     1001      123      652 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
+-rw-r--r--   0     1001      123     1896 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
+-rw-r--r--   0     1001      123      844 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return.json
+-rw-r--r--   0     1001      123     1776 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
+-rw-r--r--   0     1001      123     1932 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
+-rw-r--r--   0     1001      123     4525 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
+-rw-r--r--   0     1001      123      251 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
+-rw-r--r--   0     1001      123      246 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
+-rw-r--r--   0     1001      123      142 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
+-rw-r--r--   0     1001      123     1637 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
+-rw-r--r--   0     1001      123     1304 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
+-rw-r--r--   0     1001      123     1304 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
+-rw-r--r--   0     1001      123     1107 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
+-rw-r--r--   0     1001      123     2565 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/javascript/src/config_checker.js
+-rw-r--r--   0     1001      123     4304 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/javascript/src/piranha.js
+-rw-r--r--   0     1001      123    27988 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/javascript/src/refactor.js
+-rw-r--r--   0     1001      123     1445 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/javascript/src/source_checker.js
+-rw-r--r--   0     1001      123      646 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
+-rw-r--r--   0     1001      123     1064 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/objc/src/XPFlagRefactoring/README.txt
+-rw-r--r--   0     1001      123    26229 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
+-rw-r--r--   0     1001      123        0 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
+-rw-r--r--   0     1001      123      793 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/pyproject.toml
+-rw-r--r--   0     1001      123     2366 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/go/edges.toml
+-rw-r--r--   0     1001      123    12895 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/go/rules.toml
+-rw-r--r--   0     1001      123     1466 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/go/scope_config.toml
+-rwxr-xr-x   0     1001      123     2241 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/java/edges.toml
+-rwxr-xr-x   0     1001      123    17674 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/java/rules.toml
+-rwxr-xr-x   0     1001      123     3580 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/java/scope_config.toml
+-rwxr-xr-x   0     1001      123     2251 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/kt/edges.toml
+-rwxr-xr-x   0     1001      123    19368 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/kt/rules.toml
+-rwxr-xr-x   0     1001      123     2142 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/kt/scope_config.toml
+-rw-r--r--   0     1001      123     2316 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/swift/edges.toml
+-rw-r--r--   0     1001      123    27137 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/swift/rules.toml
+-rw-r--r--   0     1001      123     1684 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/cleanup_rules/swift/scope_config.toml
+-rw-r--r--   0     1001      123     7391 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/lib.rs
+-rw-r--r--   0     1001      123     1679 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/main.rs
+-rw-r--r--   0     1001      123     3619 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/default_configs.rs
+-rw-r--r--   0     1001      123     4915 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/edit.rs
+-rw-r--r--   0     1001      123    13503 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/filter.rs
+-rw-r--r--   0     1001      123     7097 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/language.rs
+-rw-r--r--   0     1001      123    11128 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/matches.rs
+-rw-r--r--   0     1001      123      924 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/mod.rs
+-rw-r--r--   0     1001      123     1987 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/outgoing_edges.rs
+-rw-r--r--   0     1001      123    14245 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/piranha_arguments.rs
+-rw-r--r--   0     1001      123     2091 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/piranha_output.rs
+-rw-r--r--   0     1001      123     7801 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/rule.rs
+-rw-r--r--   0     1001      123     6286 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/rule_graph.rs
+-rw-r--r--   0     1001      123     6288 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/rule_store.rs
+-rw-r--r--   0     1001      123     3402 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/scopes.rs
+-rw-r--r--   0     1001      123    14473 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/source_code_unit.rs
+-rw-r--r--   0     1001      123     1661 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/unit_tests/piranha_arguments_test.rs
+-rw-r--r--   0     1001      123     8344 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/unit_tests/rule_test.rs
+-rw-r--r--   0     1001      123     6067 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/unit_tests/scopes_test.rs
+-rw-r--r--   0     1001      123    16601 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/models/unit_tests/source_code_unit_test.rs
+-rw-r--r--   0     1001      123     8260 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1647 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_go.rs
+-rw-r--r--   0     1001      123    12953 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_java.rs
+-rw-r--r--   0     1001      123     1862 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_kt.rs
+-rw-r--r--   0     1001      123     2423 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_python.rs
+-rw-r--r--   0     1001      123     3532 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_swift.rs
+-rw-r--r--   0     1001      123      770 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_thrift.rs
+-rw-r--r--   0     1001      123     1138 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_ts.rs
+-rw-r--r--   0     1001      123     1281 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/tests/test_piranha_tsx.rs
+-rw-r--r--   0     1001      123     5629 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/utilities/mod.rs
+-rw-r--r--   0     1001      123    12743 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/utilities/tree_sitter_utilities.rs
+-rw-r--r--   0     1001      123     3681 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/utilities/unit_tests/tree_sitter_utilities_test.rs
+-rw-r--r--   0     1001      123     2237 2023-05-31 21:23:26.000000 polyglot_piranha-0.3.7/src/utilities/unit_tests/utilities_test.rs
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.7/PKG-INFO
```

### Comparing `polyglot_piranha-0.3.5/Cargo.toml` & `polyglot_piranha-0.3.7/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "Ameya Ketkar <ketkara@uber.com>",
   "Lazaro Clapp <lazaro@uber.com>",
   "Murali Krishna Ramanathan",
   "Uber Technologies Inc.",
 ]
 name = "piranha"
 description = "Polyglot Piranha is a library for performing structural find and replace with deep cleanup."
-version = "0.3.5"
+version = "0.3.7"
 edition = "2021"
 include = ["pyproject.toml", "src/"]
 exclude = ["legacy"]
 license-file = "LICENSE"
 categories = [
   "structural find-replace",
   "find-replace",
```

### Comparing `polyglot_piranha-0.3.5/Cargo.lock` & `polyglot_piranha-0.3.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "piranha"
-version = "0.3.5"
+version = "0.3.7"
 dependencies = [
  "assert_cmd",
  "cc",
  "clap",
  "colored",
  "derive_builder",
  "env_logger",
```

### Comparing `polyglot_piranha-0.3.5/LICENSE` & `polyglot_piranha-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/README.md` & `polyglot_piranha-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_argument.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json` & `polyglot_piranha-0.3.7/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java` & `polyglot_piranha-0.3.7/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak` & `polyglot_piranha-0.3.7/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect` & `polyglot_piranha-0.3.7/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/javascript/src/config_checker.js` & `polyglot_piranha-0.3.7/legacy/javascript/src/config_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/javascript/src/piranha.js` & `polyglot_piranha-0.3.7/legacy/javascript/src/piranha.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/javascript/src/refactor.js` & `polyglot_piranha-0.3.7/legacy/javascript/src/refactor.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/javascript/src/source_checker.js` & `polyglot_piranha-0.3.7/legacy/javascript/src/source_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt` & `polyglot_piranha-0.3.7/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/README.txt` & `polyglot_piranha-0.3.7/legacy/objc/src/XPFlagRefactoring/README.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp` & `polyglot_piranha-0.3.7/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/pyproject.toml` & `polyglot_piranha-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/go/edges.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/go/edges.toml`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,26 @@
 from = "statement_cleanup"
 to = ["if_cleanup"]
 
 ### statement_cleanup
 [[edges]]
 scope = "Function-Method"
 from = "statement_cleanup"
-to = ["delete_variable_declaration"]
+to = ["delete_variable_declaration", "delete_variable_declaration_with_nil"]
+
+[[edges]]
+scope = "Function-Method"
+from = "delete_variable_declaration_with_nil"
+to = ["replace_identifier_with_value", "replace_identifier_with_nil"]
+
+[[edges]]
+scope = "Parent"
+from = "replace_identifier_with_nil"
+to = ["simplify_identity_equal", "simplify_identity_not_equal"]
+
 
 [[edges]]
 scope = "Function-Method"
 from = "delete_variable_declaration"
 to = ["replace_identifier_with_value"]
 
 [[edges]]
```

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/go/rules.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/go/rules.toml`

 * *Files 6% similar despite different names*

```diff
@@ -466,14 +466,63 @@
         )
     ) @assignment
     (#eq? @a.lhs "@variable_name")
     (#not-eq? @a.rhs "@value")
 )
 """]
 
+# Before: 
+# enabled, err = true, nil 
+
+# After: 
+# <>
+[[rules]]
+name = "delete_variable_declaration_with_nil"
+query = """
+(
+    (
+        (short_var_declaration
+            left: (expression_list
+                (identifier) @variable_name
+                (identifier) @err
+            )
+            right: (expression_list
+                ([
+                    (true)
+                    (false)
+                ]) @value
+                (nil) @nil
+            )
+        )
+    ) @short_v_decl
+)
+"""
+replace = ""
+replace_node = "short_v_decl"
+is_seed_rule = false
+# Check if there is an assignment to @variable_name with a value other than @value
+# Note that the query is against a short_var_declaration while
+# the filter is against an assigment_statement
+[[rules.filters]]
+enclosing_node = "(block) @block"
+not_contains = ["""
+(
+    (assignment_statement
+        left: (expression_list
+            (identifier) @a.lhs
+        )
+        right: (expression_list
+            (_) @a.rhs
+        )
+    ) @assignment
+    (#eq? @a.lhs "@variable_name")
+    (#not-eq? @a.rhs "@value")
+)
+"""]
+
 [[rules]]
 name = "replace_identifier_with_value"
 query = """
 (
     (identifier) @identifier
     (#eq? @identifier "@variable_name")
 )
@@ -502,7 +551,49 @@
                 (identifier) @vn
             )
         ) @assignment
     ]
     (#eq? @vn "@variable_name")
 )
 """]
+
+# for @err = "err"
+# Before: 
+# err 
+# After :
+# nil
+[[rules]]
+name = "replace_identifier_with_nil"
+query = """
+(
+    (identifier) @identifier
+    (#eq? @identifier "@err")
+)
+"""
+replace = "nil"
+replace_node = "identifier"
+holes = ["err"]
+is_seed_rule = false
+[[rules.filters]]
+enclosing_node = "(block) @block"
+not_contains = ["""
+(
+    [
+        (short_var_declaration
+            left: (expression_list
+                (identifier) @vn
+            )
+        ) @assignment
+        (var_declaration
+            (var_spec
+                name: (identifier) @vn
+            )
+        ) @assignment
+        (assignment_statement
+            left: (expression_list
+                (identifier) @vn
+            )
+        ) @assignment
+    ]
+    (#eq? @vn "@err")
+)
+"""]
```

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/go/scope_config.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/go/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/java/edges.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/java/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/java/rules.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/java/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/java/scope_config.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/java/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/kt/edges.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/kt/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/kt/rules.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/kt/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/kt/scope_config.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/kt/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/swift/edges.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/swift/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/swift/rules.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/swift/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/cleanup_rules/swift/scope_config.toml` & `polyglot_piranha-0.3.7/src/cleanup_rules/swift/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/lib.rs` & `polyglot_piranha-0.3.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/main.rs` & `polyglot_piranha-0.3.7/src/main.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/default_configs.rs` & `polyglot_piranha-0.3.7/src/models/default_configs.rs`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 pub const TYPESCRIPT: &str = "ts";
 pub const TSX: &str = "tsx";
 pub const THRIFT: &str = "thrift";
 
 #[cfg(test)]
 //FIXME: Remove this  hack by not passing PiranhaArguments to SourceCodeUnit
 pub(crate) const UNUSED_CODE_PATH: &str = "/dev/null";
-pub(crate) const DEFAULT_ENCLOSING_QUERY: &str = "";
 
 pub fn default_number_of_ancestors_in_parent_scope() -> u8 {
   4
 }
 
 pub fn default_language() -> String {
   JAVA.to_string()
@@ -151,14 +150,18 @@
   u32::MAX
 }
 
 pub(crate) fn default_enclosing_node() -> TSQuery {
   TSQuery::new(String::new())
 }
 
+pub(crate) fn default_not_enclosing_node() -> TSQuery {
+  TSQuery::new(String::new())
+}
+
 pub(crate) fn default_rule_name() -> String {
   String::new()
 }
 
 pub(crate) fn default_rule_graph() -> RuleGraph {
   RuleGraph::default()
 }
```

### Comparing `polyglot_piranha-0.3.5/src/models/edit.rs` & `polyglot_piranha-0.3.7/src/models/edit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/filter.rs` & `polyglot_piranha-0.3.7/src/models/filter.rs`

 * *Files 22% similar despite different names*

```diff
@@ -28,133 +28,192 @@
 
 use super::{rule::InstantiatedRule, rule_store::RuleStore, source_code_unit::SourceCodeUnit};
 
 use crate::utilities::{tree_sitter_utilities::TSQuery, Instantiate};
 
 use super::default_configs::{
   default_contains_at_least, default_contains_at_most, default_contains_query,
-  default_enclosing_node, default_not_contains_queries, DEFAULT_ENCLOSING_QUERY,
+  default_enclosing_node, default_not_contains_queries, default_not_enclosing_node,
 };
 
 #[derive(Deserialize, Debug, Clone, Hash, PartialEq, Eq, Getters, Builder)]
 #[pyclass]
+#[builder(build_fn(name = "create"))]
 pub struct Filter {
-  /// AST patterns that some ancestor node of the primary match should comply
+  /// AST patterns that some ancestor node of the primary match should match
   #[builder(default = "default_enclosing_node()")]
   #[get = "pub"]
   #[serde(default = "default_enclosing_node")]
   #[pyo3(get)]
   enclosing_node: TSQuery,
+  /// AST patterns NO ancestor node of the primary match should match
+  #[builder(default = "default_not_enclosing_node()")]
+  #[get = "pub"]
+  #[serde(default = "default_not_enclosing_node")]
+  #[pyo3(get)]
+  not_enclosing_node: TSQuery,
   /// AST patterns that should not match any subtree of node matching `enclosing_node` pattern
   #[builder(default = "default_not_contains_queries()")]
   #[get = "pub"]
   #[serde(default = "default_not_contains_queries")]
   #[pyo3(get)]
   not_contains: Vec<TSQuery>,
   /// AST patterns that should match any subtree of node matching `enclosing_node` pattern
   #[builder(default = "default_contains_query()")]
   #[get = "pub"]
   #[serde(default = "default_contains_query")]
   #[pyo3(get)]
   contains: TSQuery,
-
   /// Least number of matches we should find for the contains query
   #[builder(default = "default_contains_at_least()")]
   #[get = "pub"]
   #[serde(default = "default_contains_at_least")]
   #[pyo3(get)]
   at_least: u32,
-
   /// Most number of matches we should find for the contains query
   #[builder(default = "default_contains_at_most()")]
   #[get = "pub"]
   #[serde(default = "default_contains_at_most")]
   #[pyo3(get)]
   at_most: u32,
 }
 
 #[pymethods]
 impl Filter {
   #[new]
   fn py_new(
-    enclosing_node: Option<String>, not_contains: Option<Vec<String>>, contains: Option<String>,
-    at_least: Option<u32>, at_most: Option<u32>,
+    enclosing_node: Option<String>, not_enclosing_node: Option<String>,
+    not_contains: Option<Vec<String>>, contains: Option<String>, at_least: Option<u32>,
+    at_most: Option<u32>,
   ) -> Self {
     FilterBuilder::default()
       .enclosing_node(TSQuery::new(enclosing_node.unwrap_or_default()))
+      .not_enclosing_node(TSQuery::new(not_enclosing_node.unwrap_or_default()))
       .not_contains(
         not_contains
           .unwrap_or_default()
           .iter()
           .map(|x| TSQuery::new(x.to_string()))
           .collect_vec(),
       )
       .contains(TSQuery::new(contains.unwrap_or_default()))
       .at_least(at_least.unwrap_or(default_contains_at_least()))
       .at_most(at_most.unwrap_or(default_contains_at_most()))
       .build()
-      .unwrap()
   }
   gen_py_str_methods!();
 }
 
+impl FilterBuilder {
+  /// Builds Filter from FilterBuilder
+  /// * create Filter from the builder
+  /// * validates new argument combinations
+  pub fn build(&self) -> Filter {
+    match &self._validate() {
+      Ok(filter) => filter.clone(),
+      Err(e) => panic!("Invalid filter - {}", e),
+    }
+  }
+
+  fn _validate(&self) -> Result<Filter, String> {
+    let _filter: Filter = self.create().unwrap();
+
+    // Only allow users to set either contains or not_contains, but not both
+    if !_filter.contains().get_query().is_empty() && !_filter.not_contains().is_empty() {
+      return Err(
+        "Invalid Filter Argument. `contains` and `not_contains` cannot be set at the same time !!! Please use two filters instead."
+          .to_string(),
+      );
+    }
+
+    if _filter.at_least > _filter.at_most {
+      return Err(
+        "Invalid Filter Argument. `at_least` should be less than or equal to `at_most` !!!"
+          .to_string(),
+      );
+    }
+
+    // If the user set `at_least` or `at_most`, then the contains query cannot be empty
+    if (_filter.at_least != default_contains_at_least()
+      || _filter.at_most != default_contains_at_most())
+      && _filter.contains().get_query().is_empty()
+    {
+      return Err(
+        "Invalid Filter Argument. `at_least` or `at_most` is set, but `contains` is empty !!!"
+          .to_string(),
+      );
+    }
+
+    Ok(_filter)
+  }
+}
+
 #[macro_export]
 /// This macro constructs a FilterBuilder for creating filter queries. It provides a more "dynamic" way to use the builder pattern.
 ///
-/// 'enclosing_node' is a required parameter that specifies the node to be inspected.
+/// 'enclosing_node' is an optional parameter that specifies the node to be inspected. If it is not provided
+/// piranha will check the filters against the matched node
+///
+/// 'not_enclosing_node' is an optional parameter that specifies the nodes that should not enclose the matched node
 ///
 /// 'not_contains' and 'contains' are optional parameters, accepting a list of queries that should not and should match
 /// within the 'enclosing_node' respectively.
 ///
 /// 'at_least' and 'at_most' specify the inclusive range for the count of matches 'contains' queries should find within
 /// the 'enclosing_node'. These parameters provide control over the desired quantity of matches.
 ///
 /// Usage:
 ///
 /// ```
 /// filter! {
 ///   enclosing_node = "(method_declaration) @md",
+///   not_enclosing_node = "(while_statement) @wt",
 ///   not_contains= ["(method_invocation name: (_) @name)"],
 ///   contains= ["(parameter_list)"],
 ///   at_least = 1,
 ///   at_most = 10
 /// }
 /// ```
 ///
 /// expands to
 ///
 /// ```
 /// FilterBuilder::default()
 ///      .enclosing_node(TSQuery::new("(method_declaration) @md"))
+///      .not_enclosing_node(TSQuery::new("(while_statement) @wt"))
 ///      .not_contains(vec![TSQuery::new("(method_invocation name: (_) @name)")])
 ///      .contains(TSQuery::new("(parameter_list)"))
 ///      .at_least(1)
 ///      .at_most(10)
 ///      .build().unwrap()
 /// ```
 ///
 macro_rules! filter {
-  ($(enclosing_node = $enclosing_node:expr)? $(, not_contains= [$($q:expr,)*])? $(, contains= $p:expr)? $(, at_least=$min:expr)? $(, at_most=$max:expr)?) => {
+  ($(enclosing_node = $enclosing_node:expr)? $(, not_enclosing_node=$not_enclosing_node:expr)? $(, not_contains= [$($q:expr,)*])? $(, contains= $p:expr)? $(, at_least=$min:expr)? $(, at_most=$max:expr)?) => {
     $crate::models::filter::FilterBuilder::default()
       $(.enclosing_node($crate::utilities::tree_sitter_utilities::TSQuery::new($enclosing_node.to_string())))?
+      $(.not_enclosing_node($crate::utilities::tree_sitter_utilities::TSQuery::new($not_enclosing_node.to_string())))?
       $(.not_contains(vec![$($crate::utilities::tree_sitter_utilities::TSQuery::new($q.to_string()),)*]))?
       $(.contains($crate::utilities::tree_sitter_utilities::TSQuery::new($p.to_string())))?
       $(.at_least($min))?
       $(.at_most($max))?
-      .build().unwrap()
+      .build()
   };
 }
 
 pub use filter;
 
 impl Instantiate for Filter {
-  /// Create a new query from `self` by updating the `query` and `replace` based on the substitutions.
+  /// Create a new filter from `self` by updating the all queries (i.e., `enclosing_node`, `not_enclosing_node`, `contains`, `not_contains`) based on the substitutions.
   fn instantiate(&self, substitutions_for_holes: &HashMap<String, String>) -> Filter {
     Filter {
       enclosing_node: self.enclosing_node().instantiate(substitutions_for_holes),
+      not_enclosing_node: self
+        .not_enclosing_node()
+        .instantiate(substitutions_for_holes),
       not_contains: self
         .not_contains()
         .iter()
         .map(|x| x.instantiate(substitutions_for_holes))
         .collect_vec(),
       contains: self.contains().instantiate(substitutions_for_holes),
       at_least: self.at_least,
@@ -177,116 +236,124 @@
       .all(|filter| self._check(filter.clone(), node, rule_store, &updated_substitutions))
   }
 
   /// Determines if the given `node` meets the conditions specified by the `filter`.
   ///
   /// The `filter` is composed of:
   /// (i) `enclosing_node`, the node to inspect, optional. If not provided we check whether the contains or non_contains are satisfied in the current node.
-  /// (ii) `not_contains` and `contains`, optional queries that should not and should match within the `enclosing_node`,
-  /// (iii) `at_least` and `at_most`, optional parameters indicating the acceptable range of matches for `contains` within the `enclosing_node`.
+  /// (ii) `not_enclosing_node`, optionalquery that no ancestor of the primary match should match,
+  /// (iii) `not_contains` and `contains`, optional queries that should not and should match within the `enclosing_node`,
+  /// (iv) `at_least` and `at_most`, optional parameters indicating the acceptable range of matches for `contains` within the `enclosing_node`.
   ///
   /// The function identifies the `enclosing_node` by traversing the ancestors of the `node`. Within this node:
   /// (i) if `not_contains` is provided, it ensures no sub-tree matches any of these queries,
   /// (ii) if `contains` is provided, it ensures the number sub-trees matching `contains` fall within the specified range.
   ///
   /// If these conditions hold, the function returns true, indicating the `node` meets the `filter`'s criteria.
   fn _check(
     &self, filter: Filter, node: Node, rule_store: &mut RuleStore,
     substitutions: &HashMap<String, String>,
   ) -> bool {
-    // This ensures that the below while loop considers the current node too when checking for filters.
-    // It does not make sense to check for filter if current node is a "leaf" node.
-    let mut initial_node = node;
+    let mut node_to_check = node;
+    let instantiated_filter = filter.instantiate(substitutions);
 
-    // No enclosing node is provided
-    if filter.enclosing_node().get_query().as_str() == DEFAULT_ENCLOSING_QUERY {
-      // Get the enclosing node matching the pattern specified in the filter (`filter.enclosing_node`)
-      self._check_current_node(filter, rule_store, substitutions, initial_node)
-    } else {
-      if node.child_count() > 0 {
-        initial_node = node.child(0).unwrap();
+    // Check if no ancestor matches the query for not_enclosing_node
+    if !self._check_not_enclosing_node(rule_store, node_to_check, &instantiated_filter) {
+      return false;
+    }
+    // If an enclosing node is provided
+    let query = instantiated_filter.enclosing_node();
+    if !query.get_query().is_empty() {
+      if let Some(result) = self._match_ancestor(rule_store, node_to_check, query) {
+        node_to_check = result;
+      } else {
+        return false;
       }
-      self._check_enclosing_node(filter, rule_store, substitutions, initial_node)
     }
+
+    self._check_filter_not_contains(&instantiated_filter, rule_store, &node_to_check)
+      && self._check_filter_contains(&instantiated_filter, rule_store, &node_to_check)
   }
 
-  fn _check_current_node(
-    &self, filter: Filter, rule_store: &mut RuleStore, substitutions: &HashMap<String, String>,
-    node: Node,
+  /// Check if the `node` does not have any ancestor that matches the `not_enclosing_node` query
+  fn _check_not_enclosing_node(
+    &self, rule_store: &mut RuleStore, node_to_check: Node, instantiated_filter: &Filter,
   ) -> bool {
-    if !self._filter_contains(&filter, rule_store, substitutions, &node) {
-      return false;
-    }
-    if !self._filter_not_contains(&filter, rule_store, substitutions, &node) {
-      return false;
+    let query = instantiated_filter.not_enclosing_node();
+    if !query.get_query().is_empty() {
+      // No ancestor should match with it
+      if self
+        ._match_ancestor(rule_store, node_to_check, query)
+        .is_some()
+      {
+        return false;
+      }
     }
     true
   }
 
-  /// This function checks for the contains
-  fn _check_enclosing_node(
-    &self, filter: Filter, rule_store: &mut RuleStore, substitutions: &HashMap<String, String>,
-    initial: Node,
-  ) -> bool {
-    let mut matched_enclosing_node = false;
-    let mut current_node = initial;
+  /// Search for any ancestor of `node` (including itself) that matches `query_str`
+  fn _match_ancestor(
+    &self, rule_store: &mut RuleStore, node: Node, ts_query: &TSQuery,
+  ) -> Option<Node> {
+    let mut current_node = node;
+    // This ensures that the below while loop considers the current node too when checking for filters.
+    if current_node.child_count() > 0 {
+      current_node = current_node.child(0).unwrap();
+    }
+
     while let Some(parent) = current_node.parent() {
-      let instantiated_filter = filter.instantiate(substitutions);
-      let enclosing_node_query_str = instantiated_filter.enclosing_node();
-      if let Some(p_match) = get_match_for_query(
-        &parent,
-        self.code(),
-        rule_store.query(enclosing_node_query_str),
-        false,
-      ) {
-        matched_enclosing_node = true;
-        let scope_node = get_node_for_range(
+      if let Some(p_match) =
+        get_match_for_query(&parent, self.code(), rule_store.query(ts_query), false)
+      {
+        let matched_ancestor = get_node_for_range(
           self.root_node(),
           p_match.range().start_byte,
           p_match.range().end_byte,
         );
-        if !self._filter_contains(&filter, rule_store, substitutions, &scope_node) {
-          return false;
-        }
-        if !self._filter_not_contains(&filter, rule_store, substitutions, &scope_node) {
-          return false;
-        }
-        break;
+        return Some(matched_ancestor);
       }
       current_node = parent;
     }
-    matched_enclosing_node
+    None
   }
 
-  fn _filter_contains(
-    &self, filter: &Filter, rule_store: &mut RuleStore, substitutions: &HashMap<String, String>,
-    scope_node: &Node,
+  /// Check if the contains filter is satisfied by ancestor or any of its descendants
+  fn _check_filter_contains(
+    &self, filter: &Filter, rule_store: &mut RuleStore, ancestor: &Node,
   ) -> bool {
-    let query_with_holes = filter.contains();
-    if query_with_holes.get_query().is_empty() {
+    // If the query is empty
+    let ts_query = filter.contains();
+    if ts_query.get_query().is_empty() {
       return true;
     }
-    // Instantiate the query and retrieve all matches within the scope node
-    let query = &rule_store.query(&query_with_holes.instantiate(substitutions));
-    let matches = get_all_matches_for_query(scope_node, self.code().to_string(), query, true, None);
+
+    // Retrieve all matches within the ancestor node
+    let contains_query = &rule_store.query(filter.contains());
+    let matches = get_all_matches_for_query(
+      ancestor,
+      self.code().to_string(),
+      contains_query,
+      true,
+      None,
+    );
     let at_least = filter.at_least as usize;
     let at_most = filter.at_most as usize;
     // Validate if the count of matches falls within the expected range
     at_least <= matches.len() && matches.len() <= at_most
   }
 
-  fn _filter_not_contains(
-    &self, filter: &Filter, rule_store: &mut RuleStore, substitutions: &HashMap<String, String>,
-    scope_node: &Node,
+  /// Check if the not_contains filter is satisfied by ancestor or any of its descendants
+  fn _check_filter_not_contains(
+    &self, filter: &Filter, rule_store: &mut RuleStore, ancestor: &Node,
   ) -> bool {
-    for query_with_holes in filter.not_contains() {
-      // Instantiate the query and check if there's a match within the scope node
-      // If there is the filter is not satisfied
-      let query = &rule_store.query(&query_with_holes.instantiate(substitutions));
-
-      if get_match_for_query(scope_node, self.code(), query, true).is_some() {
+    for ts_query in filter.not_contains() {
+      // Check if there's a match within the scope node
+      // If one of the filters is not satisfied, return false
+      let query = &rule_store.query(ts_query);
+      if get_match_for_query(ancestor, self.code(), query, true).is_some() {
         return false;
       }
     }
     true
   }
 }
```

### Comparing `polyglot_piranha-0.3.5/src/models/language.rs` & `polyglot_piranha-0.3.7/src/models/language.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/matches.rs` & `polyglot_piranha-0.3.7/src/models/matches.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/mod.rs` & `polyglot_piranha-0.3.7/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/outgoing_edges.rs` & `polyglot_piranha-0.3.7/src/models/outgoing_edges.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/piranha_arguments.rs` & `polyglot_piranha-0.3.7/src/models/piranha_arguments.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/piranha_output.rs` & `polyglot_piranha-0.3.7/src/models/piranha_output.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/rule.rs` & `polyglot_piranha-0.3.7/src/models/rule.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/rule_graph.rs` & `polyglot_piranha-0.3.7/src/models/rule_graph.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/rule_store.rs` & `polyglot_piranha-0.3.7/src/models/rule_store.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/scopes.rs` & `polyglot_piranha-0.3.7/src/models/scopes.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/source_code_unit.rs` & `polyglot_piranha-0.3.7/src/models/source_code_unit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/unit_tests/piranha_arguments_test.rs` & `polyglot_piranha-0.3.7/src/models/unit_tests/piranha_arguments_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/unit_tests/rule_test.rs` & `polyglot_piranha-0.3.7/src/models/unit_tests/rule_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/unit_tests/scopes_test.rs` & `polyglot_piranha-0.3.7/src/models/unit_tests/scopes_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/models/unit_tests/source_code_unit_test.rs` & `polyglot_piranha-0.3.7/src/models/unit_tests/source_code_unit_test.rs`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
 use tree_sitter::{Parser, Point};
 
+use crate::models::filter::FilterBuilder;
+use crate::utilities::tree_sitter_utilities::TSQuery;
 use crate::{
   filter,
   models::{
     default_configs::{JAVA, UNUSED_CODE_PATH},
     filter::Filter,
     language::PiranhaLanguage,
     piranha_arguments::PiranhaArgumentsBuilder,
@@ -125,15 +127,15 @@
 }
 
 /// Tests for contains, at_least, and at_most
 
 fn run_test_satisfies_filters(
   filter: Filter, // Replace with the filter to test
   assertion: fn(bool) -> bool,
-) {
+) -> bool {
   let _rule = piranha_rule! {
       name= "test",
       query= "(
             ((local_variable_declaration
                             declarator: (variable_declarator
                                             name: (_) @variable_name
                                             value: [(true)] @init)) @variable_declaration)
@@ -168,23 +170,25 @@
   );
 
   let node = &source_code_unit
     .root_node()
     .descendant_for_byte_range(50, 72)
     .unwrap();
 
-  assert!(assertion(source_code_unit.is_satisfied(
+  let satisfied = source_code_unit.is_satisfied(
     *node,
     &rule,
     &HashMap::from([
       ("variable_name".to_string(), "isFlagTreated".to_string()),
-      ("init".to_string(), "true".to_string())
+      ("init".to_string(), "true".to_string()),
     ]),
     &mut rule_store,
-  )));
+  );
+  assert!(assertion(satisfied));
+  satisfied
 }
 
 #[test]
 fn test_satisfies_filters_contains_positive() {
   run_test_satisfies_filters(
     filter! {
         enclosing_node= "(method_declaration) @md",
@@ -485,7 +489,121 @@
                       name: (identifier) @inv) @md
                    (#eq? @inv \"@method_name\")
                       )",
     at_least =2},
     |result| result,
   );
 }
+
+// Tests for not_enclosing_node
+fn run_test_satisfies_filters_not_enclosing_node(
+  filter: Filter, // Replace with the filter to test
+  assertion: fn(bool) -> bool,
+) {
+  let _rule = piranha_rule! {
+    name= "test",
+    query= "(
+      ((local_variable_declaration
+                      declarator: (variable_declarator
+                                          name: (_) @variable_name
+                                          )) @variable_declaration)
+      )",
+    replace_node= "variable_declaration",
+    replace= "",
+    filters= [filter,]
+  };
+  let rule = InstantiatedRule::new(&_rule, &HashMap::new());
+  let source_code = "class Test {
+      public void foobar(){
+        if (isFlagTreated) {
+          int testNumber = 0;
+        }
+       }
+      }";
+
+  let mut rule_store = RuleStore::default();
+  let java = get_java_tree_sitter_language();
+  let mut parser = java.parser();
+  let piranha_args = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(UNUSED_CODE_PATH.to_string())
+    .language(java)
+    .build();
+  let source_code_unit = SourceCodeUnit::new(
+    &mut parser,
+    source_code.to_string(),
+    &HashMap::new(),
+    PathBuf::new().as_path(),
+    &piranha_args,
+  );
+
+  let start = Point::new(3, 10);
+  let end = Point::new(3, 29);
+  let node = &source_code_unit
+    .root_node()
+    .descendant_for_point_range(start, end)
+    .unwrap();
+
+  let map: HashMap<String, String> = HashMap::new();
+  assert!(assertion(source_code_unit.is_satisfied(
+    *node,
+    &rule,
+    &map,
+    &mut rule_store,
+  )));
+}
+
+#[test]
+fn test_satisfies_filter_not_enclosing_node_positive() {
+  run_test_satisfies_filters_not_enclosing_node(
+    filter! {,
+    not_enclosing_node = "(if_statement) @if_stmt"},
+    |result| !result,
+  );
+}
+
+#[test]
+fn test_satisfies_filter_not_enclosing_node_negative() {
+  run_test_satisfies_filters_not_enclosing_node(
+    filter! {,
+    not_enclosing_node = "(while_statement ) @while"},
+    |result| result,
+  );
+}
+
+#[test]
+#[should_panic(
+  expected = "Invalid Filter Argument. `at_least` or `at_most` is set, but `contains` is empty !!!"
+)]
+fn test_filter_bad_arg_at_least() {
+  FilterBuilder::default().at_least(2).build();
+}
+
+#[test]
+#[should_panic(
+  expected = "Invalid Filter Argument. `at_least` or `at_most` is set, but `contains` is empty !!!"
+)]
+fn test_filter_bad_arg_at_most() {
+  FilterBuilder::default().at_least(5).build();
+}
+
+#[test]
+#[should_panic(
+  expected = "Invalid Filter Argument. `contains` and `not_contains` cannot be set at the same time !!! Please use two filters instead."
+)]
+fn test_filter_bad_arguments_contains_not_contains() {
+  FilterBuilder::default()
+    .contains(TSQuery::new(String::from("(if_statement) @if_stmt")))
+    .not_contains(vec![TSQuery::new(String::from("(for_statement) @for"))])
+    .build();
+}
+
+#[test]
+#[should_panic(
+  expected = "Invalid Filter Argument. `at_least` should be less than or equal to `at_most` !!!"
+)]
+fn test_filter_bad_range() {
+  FilterBuilder::default()
+    .contains(TSQuery::new(String::from("(if_statement) @if_stmt")))
+    .at_least(5)
+    .at_most(4)
+    .build();
+}
```

### Comparing `polyglot_piranha-0.3.5/src/tests/mod.rs` & `polyglot_piranha-0.3.7/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_go.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_go.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_java.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_java.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_kt.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_kt.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_python.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_python.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_swift.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_swift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_thrift.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_thrift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_ts.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_ts.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/tests/test_piranha_tsx.rs` & `polyglot_piranha-0.3.7/src/tests/test_piranha_tsx.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/utilities/mod.rs` & `polyglot_piranha-0.3.7/src/utilities/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/utilities/tree_sitter_utilities.rs` & `polyglot_piranha-0.3.7/src/utilities/tree_sitter_utilities.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/utilities/unit_tests/tree_sitter_utilities_test.rs` & `polyglot_piranha-0.3.7/src/utilities/unit_tests/tree_sitter_utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/src/utilities/unit_tests/utilities_test.rs` & `polyglot_piranha-0.3.7/src/utilities/unit_tests/utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.5/PKG-INFO` & `polyglot_piranha-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyglot_piranha
-Version: 0.3.5
+Version: 0.3.7
 License-File: LICENSE
 License-File: LICENSE
 License-File: NOTICE
 Summary: Polyglot Piranha is a library for performing structural find and replace with deep cleanup.
 Keywords: refactoring,code update,structural find-replace,structural search and replace,structural search
 Author: Uber Technologies Inc.
 Author-email: Ameya Ketkar <ketkara@uber.com>, Lazaro Clapp <lazaro@uber.com>
```

