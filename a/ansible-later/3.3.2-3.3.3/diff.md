# Comparing `tmp/ansible_later-3.3.2.tar.gz` & `tmp/ansible_later-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_later-3.3.2.tar", max compression
+gzip compressed data, was "ansible_later-3.3.3.tar", max compression
```

## Comparing `ansible_later-3.3.2.tar` & `ansible_later-3.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1123 2023-05-29 20:03:20.035422 ansible_later-3.3.2/LICENSE
--rw-r--r--   0        0        0     3173 2023-05-29 20:03:20.035422 ansible_later-3.3.2/README.md
--rw-r--r--   0        0        0      120 2023-05-29 20:03:42.607103 ansible_later-3.3.2/ansiblelater/__init__.py
--rwxr-xr-x   0        0        0     2892 2023-05-29 20:03:20.035422 ansible_later-3.3.2/ansiblelater/__main__.py
--rw-r--r--   0        0        0     9843 2023-05-29 20:03:20.035422 ansible_later-3.3.2/ansiblelater/candidate.py
--rw-r--r--   0        0        0      666 2023-05-29 20:03:20.035422 ansible_later-3.3.2/ansiblelater/exceptions.py
--rw-r--r--   0        0        0     5180 2023-05-29 20:03:20.035422 ansible_later-3.3.2/ansiblelater/logger.py
--rw-r--r--   0        0        0      834 2023-05-29 20:03:20.039422 ansible_later-3.3.2/ansiblelater/rules/CheckBecomeUser.py
--rw-r--r--   0        0        0     1636 2023-05-29 20:03:20.039422 ansible_later-3.3.2/ansiblelater/rules/CheckBracesSpaces.py
--rw-r--r--   0        0        0     2346 2023-05-29 20:03:20.039422 ansible_later-3.3.2/ansiblelater/rules/CheckChangedInWhen.py
--rw-r--r--   0        0        0     1079 2023-05-29 20:03:20.039422 ansible_later-3.3.2/ansiblelater/rules/CheckCommandHasChanges.py
--rw-r--r--   0        0        0     2650 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckCommandInsteadOfArgument.py
--rw-r--r--   0        0        0     2031 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckCommandInsteadOfModule.py
--rw-r--r--   0        0        0     1227 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckCompareToEmptyString.py
--rw-r--r--   0        0        0     1229 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckCompareToLiteralBool.py
--rw-r--r--   0        0        0      952 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckDeprecated.py
--rw-r--r--   0        0        0     3822 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckDeprecatedBareVars.py
--rw-r--r--   0        0        0     3764 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckFilePermissionMissing.py
--rw-r--r--   0        0        0     3106 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckFilePermissionOctal.py
--rw-r--r--   0        0        0     1156 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckFilterSeparation.py
--rw-r--r--   0        0        0     1921 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckGitHasVersion.py
--rw-r--r--   0        0        0     1162 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckInstallUseLatest.py
--rw-r--r--   0        0        0      941 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckLiteralBoolFormat.py
--rw-r--r--   0        0        0      737 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckLocalAction.py
--rw-r--r--   0        0        0     1182 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckMetaChangeFromDefault.py
--rw-r--r--   0        0        0     1201 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckMetaMain.py
--rw-r--r--   0        0        0      892 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckNameFormat.py
--rw-r--r--   0        0        0      897 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckNamedTask.py
--rw-r--r--   0        0        0     1679 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckNativeYaml.py
--rw-r--r--   0        0        0     2179 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckNestedJinja.py
--rw-r--r--   0        0        0     1235 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckRelativeRolePaths.py
--rw-r--r--   0        0        0      786 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckScmInSrc.py
--rw-r--r--   0        0        0     1064 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckShellInsteadCommand.py
--rw-r--r--   0        0        0     1601 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckTaskSeparation.py
--rw-r--r--   0        0        0      904 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckUniqueNamedTask.py
--rw-r--r--   0        0        0      590 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckVersion.py
--rw-r--r--   0        0        0      891 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckWhenFormat.py
--rw-r--r--   0        0        0      518 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlColons.py
--rw-r--r--   0        0        0      517 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlDocumentEnd.py
--rw-r--r--   0        0        0      525 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlDocumentStart.py
--rw-r--r--   0        0        0      524 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlEmptyLines.py
--rw-r--r--   0        0        0      684 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlFile.py
--rw-r--r--   0        0        0      627 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlHasContent.py
--rw-r--r--   0        0        0      521 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlHyphens.py
--rw-r--r--   0        0        0      526 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/rules/CheckYamlIndent.py
--rw-r--r--   0        0        0     7899 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/settings.py
--rw-r--r--   0        0        0    11940 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/standard.py
--rw-r--r--   0        0        0        0 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/test/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/test/unit/__init__.py
--rw-r--r--   0        0        0     2337 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/test/unit/test_logger.py
--rw-r--r--   0        0        0      527 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/test/unit/test_settings.py
--rw-r--r--   0        0        0     2909 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/utils/__init__.py
--rw-r--r--   0        0        0    19003 2023-05-29 20:03:20.051422 ansible_later-3.3.2/ansiblelater/utils/yamlhelper.py
--rw-r--r--   0        0        0     3475 2023-05-29 20:03:42.607103 ansible_later-3.3.2/pyproject.toml
--rw-r--r--   0        0        0     4876 1970-01-01 00:00:00.000000 ansible_later-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-05-31 09:54:48.243787 ansible_later-3.3.3/LICENSE
+-rw-r--r--   0        0        0     3173 2023-05-31 09:54:48.243787 ansible_later-3.3.3/README.md
+-rw-r--r--   0        0        0      120 2023-05-31 09:55:02.443829 ansible_later-3.3.3/ansiblelater/__init__.py
+-rwxr-xr-x   0        0        0     2892 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/__main__.py
+-rw-r--r--   0        0        0     9843 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/candidate.py
+-rw-r--r--   0        0        0      666 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/exceptions.py
+-rw-r--r--   0        0        0     5180 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/logger.py
+-rw-r--r--   0        0        0      834 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckBecomeUser.py
+-rw-r--r--   0        0        0     1636 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckBracesSpaces.py
+-rw-r--r--   0        0        0     2346 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckChangedInWhen.py
+-rw-r--r--   0        0        0     1079 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckCommandHasChanges.py
+-rw-r--r--   0        0        0     2650 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py
+-rw-r--r--   0        0        0     2031 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckCommandInsteadOfModule.py
+-rw-r--r--   0        0        0     1227 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckCompareToEmptyString.py
+-rw-r--r--   0        0        0     1229 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckCompareToLiteralBool.py
+-rw-r--r--   0        0        0      952 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckDeprecated.py
+-rw-r--r--   0        0        0     3822 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckDeprecatedBareVars.py
+-rw-r--r--   0        0        0     3764 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckFilePermissionMissing.py
+-rw-r--r--   0        0        0     3106 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckFilePermissionOctal.py
+-rw-r--r--   0        0        0     1156 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckFilterSeparation.py
+-rw-r--r--   0        0        0     1921 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckGitHasVersion.py
+-rw-r--r--   0        0        0     1162 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckInstallUseLatest.py
+-rw-r--r--   0        0        0      941 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckLiteralBoolFormat.py
+-rw-r--r--   0        0        0      737 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckLocalAction.py
+-rw-r--r--   0        0        0     1182 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckMetaChangeFromDefault.py
+-rw-r--r--   0        0        0     1201 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckMetaMain.py
+-rw-r--r--   0        0        0      892 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckNameFormat.py
+-rw-r--r--   0        0        0      897 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckNamedTask.py
+-rw-r--r--   0        0        0     1679 2023-05-31 09:54:48.243787 ansible_later-3.3.3/ansiblelater/rules/CheckNativeYaml.py
+-rw-r--r--   0        0        0     2179 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckNestedJinja.py
+-rw-r--r--   0        0        0     1235 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckRelativeRolePaths.py
+-rw-r--r--   0        0        0      786 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckScmInSrc.py
+-rw-r--r--   0        0        0     1064 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckShellInsteadCommand.py
+-rw-r--r--   0        0        0     1601 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckTaskSeparation.py
+-rw-r--r--   0        0        0      904 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckUniqueNamedTask.py
+-rw-r--r--   0        0        0      590 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckVersion.py
+-rw-r--r--   0        0        0      891 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckWhenFormat.py
+-rw-r--r--   0        0        0      518 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlColons.py
+-rw-r--r--   0        0        0      517 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlDocumentEnd.py
+-rw-r--r--   0        0        0      525 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlDocumentStart.py
+-rw-r--r--   0        0        0      524 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlEmptyLines.py
+-rw-r--r--   0        0        0      684 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlFile.py
+-rw-r--r--   0        0        0      627 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlHasContent.py
+-rw-r--r--   0        0        0      521 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlHyphens.py
+-rw-r--r--   0        0        0      526 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/rules/CheckYamlIndent.py
+-rw-r--r--   0        0        0     7899 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/settings.py
+-rw-r--r--   0        0        0    11940 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/standard.py
+-rw-r--r--   0        0        0        0 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/test/unit/__init__.py
+-rw-r--r--   0        0        0     2337 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/test/unit/test_logger.py
+-rw-r--r--   0        0        0      527 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/test/unit/test_settings.py
+-rw-r--r--   0        0        0     2909 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/utils/__init__.py
+-rw-r--r--   0        0        0    19032 2023-05-31 09:54:48.247787 ansible_later-3.3.3/ansiblelater/utils/yamlhelper.py
+-rw-r--r--   0        0        0     3475 2023-05-31 09:55:02.443829 ansible_later-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4876 1970-01-01 00:00:00.000000 ansible_later-3.3.3/PKG-INFO
```

### Comparing `ansible_later-3.3.2/LICENSE` & `ansible_later-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/README.md` & `ansible_later-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/__main__.py` & `ansible_later-3.3.3/ansiblelater/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/candidate.py` & `ansible_later-3.3.3/ansiblelater/candidate.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/exceptions.py` & `ansible_later-3.3.3/ansiblelater/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/logger.py` & `ansible_later-3.3.3/ansiblelater/logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckBecomeUser.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckBecomeUser.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckBracesSpaces.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckBracesSpaces.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckChangedInWhen.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckChangedInWhen.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckCommandHasChanges.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckCommandHasChanges.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckCommandInsteadOfArgument.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckCommandInsteadOfArgument.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckCommandInsteadOfModule.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckCommandInsteadOfModule.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckCompareToEmptyString.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckCompareToEmptyString.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckCompareToLiteralBool.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckCompareToLiteralBool.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckDeprecated.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckDeprecated.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckDeprecatedBareVars.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckDeprecatedBareVars.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckFilePermissionMissing.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckFilePermissionMissing.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckFilePermissionOctal.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckFilePermissionOctal.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckFilterSeparation.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckFilterSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckGitHasVersion.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckGitHasVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckInstallUseLatest.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckInstallUseLatest.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckLiteralBoolFormat.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckLiteralBoolFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckLocalAction.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckLocalAction.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckMetaChangeFromDefault.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckMetaChangeFromDefault.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckMetaMain.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckMetaMain.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckNameFormat.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckNameFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckNamedTask.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckNativeYaml.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckNativeYaml.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckNestedJinja.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckNestedJinja.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckRelativeRolePaths.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckRelativeRolePaths.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckScmInSrc.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckScmInSrc.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckShellInsteadCommand.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckShellInsteadCommand.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckTaskSeparation.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckTaskSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckUniqueNamedTask.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckUniqueNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckVersion.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckWhenFormat.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckWhenFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlColons.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlColons.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlDocumentEnd.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlDocumentEnd.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlDocumentStart.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlDocumentStart.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlEmptyLines.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlEmptyLines.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlFile.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlFile.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlHasContent.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlHasContent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlHyphens.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlHyphens.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/rules/CheckYamlIndent.py` & `ansible_later-3.3.3/ansiblelater/rules/CheckYamlIndent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/settings.py` & `ansible_later-3.3.3/ansiblelater/settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/standard.py` & `ansible_later-3.3.3/ansiblelater/standard.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/test/unit/test_logger.py` & `ansible_later-3.3.3/ansiblelater/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/test/unit/test_settings.py` & `ansible_later-3.3.3/ansiblelater/test/unit/test_settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/utils/__init__.py` & `ansible_later-3.3.3/ansiblelater/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.2/ansiblelater/utils/yamlhelper.py` & `ansible_later-3.3.3/ansiblelater/utils/yamlhelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     templar = Templar(dl, variables=templatevars)
     return templar.template(varname, **kwargs)
 
 
 try:
     from ansible.plugins import module_loader
 except ImportError:
-    from ansible.plugins.loader import module_loader
+    from ansible.plugins.loader import init_plugin_loader, module_loader
+    init_plugin_loader()
 
 LINE_NUMBER_KEY = "__line__"
 FILENAME_KEY = "__file__"
 
 VALID_KEYS = [
     "name",
     "action",
@@ -407,15 +408,15 @@
     builtin = list(set(builtin + custom_modules))
     ansible.parsing.mod_args.BUILTIN_TASKS = frozenset(builtin)
     mod_arg_parser = ModuleArgsParser(task)
 
     try:
         action, arguments, normalized["delegate_to"] = mod_arg_parser.parse()
     except AnsibleParserError as e:
-        raise LaterAnsibleError("syntax error", e) from e
+        raise LaterAnsibleError(e) from e
 
     # denormalize shell -> command conversion
     if "_uses_shell" in arguments:
         action = "shell"
         del (arguments["_uses_shell"])
 
     for (k, v) in list(task.items()):
```

### Comparing `ansible_later-3.3.2/pyproject.toml` & `ansible_later-3.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 license = "MIT"
 name = "ansible-later"
 packages = [
   {include = "ansiblelater"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-later/"
-version = "3.3.2"
+version = "3.3.3"
 
 [tool.poetry.dependencies]
 PyYAML = "6.0"
-ansible = {version = "7.6.0", optional = true}
-ansible-core = {version = "2.14.6", optional = true}
+ansible = {version = "8.0.0", optional = true}
+ansible-core = {version = "2.15.0", optional = true}
 anyconfig = "0.13.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 jsonschema = "4.17.3"
 nested-lookup = "0.2.25"
 pathspec = "0.11.1"
 python = "^3.9.0"
```

### Comparing `ansible_later-3.3.2/PKG-INFO` & `ansible_later-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-later
-Version: 3.3.2
+Version: 3.3.3
 Summary: Reviews ansible playbooks, roles and inventories and suggests improvements.
 Home-page: https://ansible-later.geekdocs.de/
 License: MIT
 Keywords: ansible,code,review
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Provides-Extra: ansible
 Provides-Extra: ansible-core
 Requires-Dist: PyYAML (==6.0)
-Requires-Dist: ansible (==7.6.0) ; extra == "ansible"
-Requires-Dist: ansible-core (==2.14.6) ; extra == "ansible-core"
+Requires-Dist: ansible (==8.0.0) ; extra == "ansible"
+Requires-Dist: ansible-core (==2.15.0) ; extra == "ansible-core"
 Requires-Dist: anyconfig (==0.13.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.11.1)
 Requires-Dist: python-json-logger (==2.0.7)
```

