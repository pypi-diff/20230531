# Comparing `tmp/molecule-qemu-0.4.0rc0.tar.gz` & `tmp/molecule-qemu-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.0rc0.tar", last modified: Tue May 30 09:14:41 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.0rc1.tar", last modified: Tue May 30 15:37:50 2023, max compression
```

## Comparing `molecule-qemu-0.4.0rc0.tar` & `molecule-qemu-0.4.0rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.383756 molecule-qemu-0.4.0rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.383756 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:14:41.387757 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 09:14:41.000000 molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 09:14:29.000000 molecule-qemu-0.4.0rc0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 09:14:41.391757 molecule-qemu-0.4.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/setup.cfg
```

### Comparing `molecule-qemu-0.4.0rc0/.github/workflows/python-publish.yml` & `molecule-qemu-0.4.0rc1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/.github/workflows/release.yml` & `molecule-qemu-0.4.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/.gitignore` & `molecule-qemu-0.4.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/LICENSE` & `molecule-qemu-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/Makefile` & `molecule-qemu-0.4.0rc1/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/PKG-INFO` & `molecule-qemu-0.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.0rc0
+Version: 0.4.0rc1
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.0rc0/README.md` & `molecule-qemu-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/molecule_qemu/driver.py` & `molecule-qemu-0.4.0rc1/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/create.yml`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     molecule_scenario_name: "{{ lookup('env', 'MOLECULE_SCENARIO_NAME') }}"
     molecule_project_name: "{{ lookup('env', 'MOLECULE_PROJECT_DIRECTORY') | basename }}"
     qemu_cap_hvf: false
     qemu_vm_image_arch: "x86_64"
     qemu_vm_image_format: "qcow2"
     qemu_vm_memory: "1024"
     qemu_vm_cpus: "2"
+    qemu_vm_disk: "4G"
 
   tasks:
     ### configuration #########################################################
     - name: Register VMs data
       ansible.builtin.set_fact:
         instance: {
           "instance": "molecule-{{ molecule_project_name }}-{{ molecule_scenario_name }}-{{ item.name }}",
@@ -30,14 +31,15 @@
 
           "ssh_host": "{{ item.ssh_host | default('127.0.0.1') }}",
           "ssh_port": "{{ item.ssh_port | default(10022) }}",
           "ssh_user": "{{ item.ssh_user }}",
 
           "vm_cpus": "{{ item.vm_cpus | default(qemu_vm_cpus) }}",
           "vm_memory": "{{ item.vm_memory | default(qemu_vm_memory) }}",
+          "vm_disk": "{{ item.vm_disk | default(qemu_vm_disk) }}",
 
           "path_disk": "{{ molecule_ephemeral_directory }}/run/{{ item.name }}.qcow2",
           "path_pid": "{{ molecule_ephemeral_directory }}/run/{{ item.name }}.pid",
         }
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "{{ item.name }}"
@@ -183,14 +185,15 @@
     ### qemu ##################################################################
     - name: Create VMs disks
       ansible.builtin.command: >
         qemu-img create
         -f qcow2
         -o backing_file={{ images_cache[item.image] }},backing_fmt={{ item.image_format }}
         {{ item.path_disk }}
+        {{ item.vm_disk }}
       args:
         creates: "{{ item.path_disk }}"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Launch VMs
```

### Comparing `molecule-qemu-0.4.0rc0/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.0rc0
+Version: 0.4.0rc1
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.0rc0/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc0/pyproject.toml` & `molecule-qemu-0.4.0rc1/pyproject.toml`

 * *Files identical despite different names*

