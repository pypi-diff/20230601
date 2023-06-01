# Comparing `tmp/molecule-qemu-0.4.0rc1.tar.gz` & `tmp/molecule-qemu-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.0rc1.tar", last modified: Tue May 30 15:37:50 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.1.tar", last modified: Thu Jun  1 10:08:46 2023, max compression
```

## Comparing `molecule-qemu-0.4.0rc1.tar` & `molecule-qemu-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/pycodestyle.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.119592 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 15:37:50.000000 molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 15:37:40.000000 molecule-qemu-0.4.0rc1/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 15:37:50.123592 molecule-qemu-0.4.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.917879 molecule-qemu-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.917879 molecule-qemu-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.917879 molecule-qemu-0.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.917879 molecule-qemu-0.4.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-01 10:08:46.000000 molecule-qemu-0.4.1/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-01 10:08:46.000000 molecule-qemu-0.4.1/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:08:46.000000 molecule-qemu-0.4.1/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 10:08:46.000000 molecule-qemu-0.4.1/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 10:08:46.000000 molecule-qemu-0.4.1/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 10:08:46.000000 molecule-qemu-0.4.1/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 10:08:37.000000 molecule-qemu-0.4.1/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 10:08:46.921879 molecule-qemu-0.4.1/setup.cfg
```

### Comparing `molecule-qemu-0.4.0rc1/.github/workflows/python-publish.yml` & `molecule-qemu-0.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc1/.github/workflows/release.yml` & `molecule-qemu-0.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc1/.gitignore` & `molecule-qemu-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc1/LICENSE` & `molecule-qemu-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc1/Makefile` & `molecule-qemu-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc1/molecule_qemu/driver.py` & `molecule-qemu-0.4.1/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.0rc1/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.1/molecule_qemu/playbooks/destroy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -20,22 +20,24 @@
         pid: "{{ lookup('file', item.pidfile) }}"
       loop: "{{ instance_conf }}"
       loop_control:
         label: "{{ item.name }}"
       register: qemu_processes
 
     - name: Destroy running VMs
+      become: "{{ item.item.privileged | default(false) }}"
       ansible.builtin.command: >
         kill {{ item.ansible_facts.pid }}
       changed_when: false
       loop: "{{ qemu_processes.results }}"
       loop_control:
         label: "{{ item.item.name }}"
 
     - name: Delete PID files
+      become: "{{ item.item.privileged | default(false) }}"
       ansible.builtin.file:
         path: "{{ item.pidfile }}"
         state: absent
       loop: "{{ instance_conf }}"
       loop_control:
         label: "{{ item.name }}"
```

### Comparing `molecule-qemu-0.4.0rc1/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.1/molecule_qemu.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.yamllint
 LICENSE
 Makefile
 README.md
 pyproject.toml
 requirements.yml
 setup.cfg
 .github/workflows/ansible-lint.yml
```

### Comparing `molecule-qemu-0.4.0rc1/pyproject.toml` & `molecule-qemu-0.4.1/pyproject.toml`

 * *Files identical despite different names*

