# Comparing `tmp/step_pipeline-0.2.2.tar.gz` & `tmp/step_pipeline-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/step_pipeline-0.2.2.tar", last modified: Wed Apr 20 11:17:45 2022, max compression
+gzip compressed data, was "dist/step_pipeline-0.2.4.tar", last modified: Thu Jun  1 18:51:32 2023, max compression
```

## Comparing `step_pipeline-0.2.2.tar` & `step_pipeline-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/
--rw-r--r--   0 root         (0) staff       (20)     1060 2021-05-21 18:58:34.000000 step_pipeline-0.2.2/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     2648 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1445 2022-03-18 01:37:01.000000 step_pipeline-0.2.2/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2109 2022-04-20 11:17:39.000000 step_pipeline-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/step_pipeline/
--rw-r--r--   0 root         (0) staff       (20)      105 2022-03-13 00:46:39.000000 step_pipeline-0.2.2/step_pipeline/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    38064 2022-04-20 11:09:20.000000 step_pipeline-0.2.2/step_pipeline/batch.py
--rw-r--r--   0 root         (0) staff       (20)      223 2022-03-16 16:43:41.000000 step_pipeline-0.2.2/step_pipeline/constants.py
--rw-r--r--   0 root         (0) staff       (20)    12336 2022-04-20 11:09:20.000000 step_pipeline-0.2.2/step_pipeline/io.py
--rw-r--r--   0 root         (0) staff       (20)     2278 2022-03-16 17:33:05.000000 step_pipeline-0.2.2/step_pipeline/main.py
--rw-r--r--   0 root         (0) staff       (20)    41338 2022-04-20 11:09:20.000000 step_pipeline-0.2.2/step_pipeline/pipeline.py
--rw-r--r--   0 root         (0) staff       (20)    13193 2022-04-20 11:09:39.000000 step_pipeline-0.2.2/step_pipeline/utils.py
--rw-r--r--   0 root         (0) staff       (20)    14707 2022-04-20 11:09:20.000000 step_pipeline-0.2.2/step_pipeline/wdl.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/step_pipeline.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     2648 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/step_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      467 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/step_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/step_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      100 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/step_pipeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       20 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/step_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-04-20 11:17:45.000000 step_pipeline-0.2.2/tests/
--rw-r--r--   0 root         (0) staff       (20)        0 2021-05-21 03:13:52.000000 step_pipeline-0.2.2/tests/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    10957 2022-04-20 11:09:39.000000 step_pipeline-0.2.2/tests/utils_tests.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/
+-rw-r--r--   0 weisburd   (502) staff       (20)     1060 2021-05-21 18:58:34.000000 step_pipeline-0.2.4/LICENSE
+-rw-r--r--   0 weisburd   (502) staff       (20)     2368 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)     1445 2022-03-18 01:37:01.000000 step_pipeline-0.2.4/README.md
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/integration_tests/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2022-05-24 22:25:36.000000 step_pipeline-0.2.4/integration_tests/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      553 2022-10-12 17:27:55.000000 step_pipeline-0.2.4/integration_tests/batch_pipeline1.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      450 2022-03-03 16:33:56.000000 step_pipeline-0.2.4/integration_tests/integration_test1.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1062 2022-05-24 22:58:13.000000 step_pipeline-0.2.4/integration_tests/integration_test2.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1387 2022-05-24 23:01:47.000000 step_pipeline-0.2.4/integration_tests/integration_test3.py
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/setup.cfg
+-rw-r--r--   0 weisburd   (502) staff       (20)     2109 2023-06-01 18:51:10.000000 step_pipeline-0.2.4/setup.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline/
+-rw-r--r--   0 weisburd   (502) staff       (20)      267 2023-05-17 16:33:11.000000 step_pipeline-0.2.4/step_pipeline/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    43539 2023-05-17 19:22:29.000000 step_pipeline-0.2.4/step_pipeline/batch.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      223 2022-03-16 16:43:41.000000 step_pipeline-0.2.4/step_pipeline/constants.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    13598 2022-10-10 22:13:19.000000 step_pipeline-0.2.4/step_pipeline/io.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2278 2022-03-16 17:33:05.000000 step_pipeline-0.2.4/step_pipeline/main.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    50464 2023-05-31 13:10:30.000000 step_pipeline-0.2.4/step_pipeline/pipeline.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    14717 2023-05-25 22:02:37.000000 step_pipeline-0.2.4/step_pipeline/utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    14714 2022-07-04 19:59:27.000000 step_pipeline-0.2.4/step_pipeline/wdl.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/
+-rw-r--r--   0 weisburd   (502) staff       (20)     2368 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)      661 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)        1 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)      100 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/requires.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/tests/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-05-21 03:13:52.000000 step_pipeline-0.2.4/tests/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    10927 2022-07-04 19:59:27.000000 step_pipeline-0.2.4/tests/utils_tests.py
```

### Comparing `step_pipeline-0.2.2/LICENSE` & `step_pipeline-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.2/README.md` & `step_pipeline-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.2/setup.py` & `step_pipeline-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system("rm -rf dist")
         os.system("python3.7 setup.py sdist"
                   "&& python3.7 setup.py bdist_wheel"
                   "&& python3.7 -m twine upload dist/*whl dist/*gz")
 
 setup(
     name='step_pipeline',
-    version="0.2.2",
+    version="0.2.4",
     description="Pipeline library that simplifies creation of pipelines that run on top of hail Batch and other compute enviornments",
     install_requires=install_requires,
     cmdclass={
         'coverage': CoverageCommand,
         'publish': PublishCommand,
     },
     long_description_content_type="text/markdown",
```

### Comparing `step_pipeline-0.2.2/step_pipeline/batch.py` & `step_pipeline-0.2.4/step_pipeline/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,25 +50,27 @@
             env_var="BATCH_REMOTE_TMPDIR",
             help="Batch requires a temp cloud storage path that it can use to store intermediate files. The Batch "
                  "service account must have Admin access to this directory. To get the name of your Batch "
                  "service account, go to https://auth.hail.is/user. Then, to grant Admin permissions, run "
                  "gsutil iam ch serviceAccount:[SERVICE_ACCOUNT_NAME]:objectAdmin gs://[BUCKET_NAME]"
         )
 
-        args = self.parse_args()
+        args = self.parse_known_args()
 
         self._backend = backend
         self._gcloud_project = args.gcloud_project
         self._cancel_after_n_failures = None
         self._default_image = DEFAULT_BASH_IMAGE
         self._default_python_image = DEFAULT_PYTHON_IMAGE
         self._default_memory = None
         self._default_cpu = None
         self._default_storage = None
         self._default_timeout = None
+        self._default_custom_machine_type = None
+        self._default_custom_machine_is_preemptible = None
         self._backend_obj = None
 
     @property
     def backend(self):
         """Returns either Backend.HAIL_BATCH_SERVICE or Backend.HAIL_BATCH_LOCAL"""
         return self._backend
 
@@ -225,20 +227,38 @@
         self._default_storage = default_storage
         return self
 
     def default_timeout(self, default_timeout):
         """Set the default job timeout duration.
 
         Args:
-            default_timeout: Maximum time in seconds for a job to run before being killed. Only applicable for the
+            default_timeout (int): Maximum time in seconds for a job to run before being killed. Only applicable for the
                 ServiceBackend. If None, there is no timeout.
         """
         self._default_timeout = default_timeout
         return self
 
+    def default_custom_machine_type(self, default_custom_machine_type):
+        """Set the default custom machine type.
+
+        Args:
+            default_custom_machine_type (str): Cloud machine type, eg. 'n1-highmem-32'
+        """
+        self._default_custom_machine_type = default_custom_machine_type
+        return self
+
+    def default_custom_machine_is_preemptible(self, default_custom_machine_is_preemptible):
+        """Set whether the custom machine should be preemptible.
+
+        Args:
+            default_custom_machine_is_preemptible (bool): Whether the custom machine is preemptible.
+        """
+        self._default_custom_machine_is_preemptible = default_custom_machine_is_preemptible
+        return self
+
     def run(self):
         """Batch-specific code for submitting the pipeline to the Hail Batch backend"""
         print(f"Starting {self.name or ''} pipeline:")
 
         super().run()
 
         try:
@@ -259,15 +279,15 @@
     def _get_localization_root_dir(self, localize_by):
         """Return the top-level root directory where localized files will be copied"""
         return "/io"
 
     def _create_batch_obj(self):
         """Instantiate the Hail Batch Backend."""
 
-        args = self.parse_args()
+        args = self.parse_known_args()
 
         if self._backend == Backend.HAIL_BATCH_LOCAL:
             self._backend_obj = hb.LocalBackend()
         elif self._backend == Backend.HAIL_BATCH_SERVICE:
             if not args.batch_billing_project:
                 raise ValueError("--batch-billing-project must be set when --cluster is used")
             if not args.batch_remote_tmpdir:
@@ -299,15 +319,15 @@
 
         if self._backend == Backend.HAIL_BATCH_LOCAL:
             # Hail Batch LocalBackend mode doesn't support some of the args suported by ServiceBackend
             result = self._batch.run(dry_run=args.dry_run, verbose=args.verbose)
         elif self._backend == Backend.HAIL_BATCH_SERVICE:
             result = self._batch.run(
                 dry_run=args.dry_run,
-                verbose=args.verbose,
+                verbose=False,  # always set to False since hail verbose output is too detailed
                 delete_scratch_on_exit=None,  # If True, delete temporary directories with intermediate files
                 wait=True,  # If True, wait for the batch to finish executing before returning
                 open=False,  # If True, open the UI page for the batch
                 disable_progress_bar=False,  # If True, disable the progress bar.
                 callback=None,  # If not None, a URL that will receive at most one POST request after the entire batch completes.
             )
         else:
@@ -322,15 +342,15 @@
         user-defined Steps and decides which steps can be skipped, and which should be executed (ie. transferred to
         the execution backend).
         """
 
         num_steps_transferred = super()._transfer_all_steps()
 
         # handle --slack-when-done by adding an always-run job
-        args = self.parse_args()
+        args = self.parse_known_args()
         if args.slack_when_done and num_steps_transferred > 0:
             post_to_slack_job = self._batch.new_job(name="post to slack when done")
             for step in self._all_steps:
                 if step._job:
                     post_to_slack_job.depends_on(step._job)
             post_to_slack_job.always_run()
             post_to_slack_job.cpu(0.25)
@@ -352,14 +372,16 @@
         arg_suffix=None,
         image=None,
         cpu=None,
         memory=None,
         storage=None,
         always_run=False,
         timeout=None,
+        custom_machine_type=None,
+        custom_machine_is_preemptible=None,
         output_dir=None,
         reuse_job_from_previous_step=None,
         localize_by=Localize.COPY,
         delocalize_by=Delocalize.COPY,
     ):
         """Step constructor.
 
@@ -384,14 +406,16 @@
                 If you need additional storage, you can explicitly request more storage using this method and the extra
                 storage space will be mounted at /io. Batch automatically writes all ResourceFile to /io.
                 The default storage size is 0 Gi. The minimum storage size is 0 Gi and the maximum storage size is
                 64 Ti. If storage is set to a value between 0 Gi and 10 Gi, the storage request is rounded up to 10 Gi.
                 All values are rounded up to the nearest Gi.
             always_run (bool): Set the Step to always run, even if dependencies fail.
             timeout (float, int): Set the maximum amount of time this job can run for before being killed.
+            custom_machine_type (str):
+            custom_machine_is_preemptible (bool):
             output_dir (str): Optional default output directory for Step outputs.
             reuse_job_from_previous_step (Step): Optionally, reuse the batch.Job object from this other upstream Step.
             localize_by (Localize): If specified, this will be the default Localize approach used by Step inputs.
             delocalize_by (Delocalize): If specified, this will be the default Delocalize approach used by Step outputs.
         """
         super().__init__(
             pipeline,
@@ -405,25 +429,38 @@
 
         self._image = image
         self._cpu = cpu
         self._memory = memory
         self._storage = storage
         self._always_run = always_run
         self._timeout = timeout
+        self._custom_machine_type = custom_machine_type
+        self._custom_machine_is_preemptible = custom_machine_is_preemptible
         self._reuse_job_from_previous_step = reuse_job_from_previous_step
 
         self._job = None
         self._output_file_counter = 0
 
         self._paths_localized_via_temp_bucket = set()
-        self._buckets_mounted_via_gcsfuse = set()
+        self._buckets_mounted_via_cloudfuse = set()
 
         self._step_type = BatchStepType.BASH
         self._write_commands_to_script = False
 
+        self._regions = None
+        self._localize_by_copy_already_created_dirs_set = set()
+
+    def regions(self, *region):
+        """Set one or more compute regions.
+
+        Args:
+            region (str): eg. "us-central1".
+        """
+        self._regions = region
+
     def cpu(self, cpu):
         """Set the CPU requirement for this Step.
 
         Args:
             cpu (str, float, int): CPU requirements. Units are in cpu if cores is numeric.
         """
         self._cpu = cpu
@@ -475,17 +512,36 @@
 
         Args:
             timeout (float, int): Set the maximum amount of time this job can run for before being killed.
         """
         self._timeout = timeout
         return self
 
+    def custom_machine_type(self, custom_machine_type):
+        """Set a custom machine type.
+
+        Args:
+            custom_machine_type (str): Cloud machine type, eg. 'n1-highmem-32'
+        """
+        self._custom_machine_type = custom_machine_type
+        return self
+
+    def custom_machine_is_preemptible(self, custom_machine_is_preemptible):
+        """Set whether the custom machine should be preemptible.
+
+        Args:
+            custom_machine_is_preemptible (bool): Whether the custom machine is preemptible.
+        """
+        self._custom_machine_is_preemptible = custom_machine_is_preemptible
+        return self
+
     def _transfer_step(self):
         """Submit this Step to the Batch backend. This method is only called if the Step isn't skipped."""
         # create Batch Job object
+
         batch = self._pipeline._batch
         if self._reuse_job_from_previous_step:
             # reuse previous Job
             if self._reuse_job_from_previous_step._job is None:
                 raise Exception(f"self._reuse_job_from_previous_step._job object is None")
 
             self._job = self._reuse_job_from_previous_step._job
@@ -494,21 +550,24 @@
             if self._step_type == BatchStepType.PYTHON:
                 self._job = batch.new_python_job(name=self.name)
             elif self._step_type == BatchStepType.BASH:
                 self._job = batch.new_bash_job(name=self.name)
             else:
                 raise ValueError(f"Unexpected BatchStepType: {self._step_type}")
 
-        self._unique_batch_id = abs(hash(batch)) % 10**9
-        self._unique_job_id = abs(hash(self._job)) % 10**9
-
         # set execution parameters
         if self._image:
             self._job.image(self._image)
 
+        if self._regions is not None:
+            self._job.regions(self._regions)
+        else:
+            # set the default region to us-central1 to avoid random egress charges
+            self._job.regions(["us-central1"])
+
         if self._cpu is not None:
             if self._cpu < 0.25 or self._cpu > 16:
                 raise ValueError(f"CPU arg is {self._cpu}. This is outside the range of 0.25 to 16 CPUs")
 
             self._job.cpu(self._cpu)  # Batch default is 1
 
         if self._memory is not None:
@@ -518,14 +577,26 @@
 
                 self._job.memory(f"{self._memory}Gi")  # Batch default is 3.75G
             elif isinstance(self._memory, str):
                 self._job.memory(self._memory)
             else:
                 raise ValueError(f"Unexpected memory arg type: {type(self._memory)}")
 
+        custom_machine_type_requested = any(p is not None for p in [
+            self._custom_machine_type, self._custom_machine_is_preemptible,
+            self._pipeline._default_custom_machine_type, self._pipeline._default_custom_machine_is_preemptible,
+        ])
+        if custom_machine_type_requested:
+            if self._cpu or self._memory:
+                raise ValueError("Both a custom_machine_type or custom_machine_is_preemptible as well as cpu or memory "
+                                 "arguments were specified. Only one or the other should be provided.")
+            self.job._machine_type = self._custom_machine_type or self._pipeline._default_custom_machine_type
+            #if self._custom_machine_is_preemptible is not None or self._default_custom_machine_is_preemptible is not None:
+            self.job._preemptible = self._custom_machine_is_preemptible or self._pipeline._default_custom_machine_is_preemptible
+
         if self._storage:
             self._job.storage(self._storage)
 
         if self._timeout is not None:
             self._job.timeout(self._timeout)
 
         if self._always_run:
@@ -534,46 +605,41 @@
         # transfer job dependencies
         for upstream_step in self._upstream_steps:
             if upstream_step._job:
                 self._job.depends_on(upstream_step._job)
 
         # transfer inputs
         for input_spec in self._input_specs:
-            print(" "*4 + f"Input: {input_spec.source_path}  ({input_spec.localize_by})")
+            print(" "*4 + f"Input: {input_spec.original_source_path}  ({input_spec.localize_by})")
             self._transfer_input_spec(input_spec)
 
         # transfer commands
-        if self._write_commands_to_script:
-            # write to script
+        if self._write_commands_to_script or len(" ".join(self._commands)) > 5*10**4:
             args = self._pipeline.parse_args()
 
-            script_lines = []
-            # set bash options for easier debugging and to make command execution more robust
-            script_lines.append("set -euxo pipefail")
-            for command in self._commands:
-                script_lines.append(command)
-
+            # write script to a temp file
             script_file = tempfile.NamedTemporaryFile("wt", prefix="script_", suffix=".sh", encoding="UTF-8", delete=True)
-            script_file.writelines(script_lines)
+            for command in self._commands:
+                script_file.write(f"{command}\n")
             script_file.flush()
 
             # upload script to the temp bucket or output dir
             script_temp_gcloud_path = os.path.join(
                 args.batch_remote_tmpdir,
-                f"batch_{self._unique_batch_id}/job_{self._unique_job_id}",
+                f"pipeline_{self._pipeline._unique_pipeline_instance_id}/step_{self._unique_step_instance_id}",
                 os.path.basename(script_file.name))
 
             os.chmod(script_file.name, mode=stat.S_IREAD | stat.S_IEXEC)
-            script_file_upload_command = self._generate_gsutil_copy_command(script_file.name, script_temp_gcloud_path)
+            script_file_upload_command = self._generate_gsutil_copy_command(
+                script_file.name, output_dir=os.path.dirname(script_temp_gcloud_path))
             os.system(script_file_upload_command)
             script_file.close()
-
-            script_input_spec = self.input(script_temp_gcloud_path)
-            self._transfer_input_spec(script_input_spec)
-            self._job.command(f"bash -c '{script_input_spec.local_path}'")
+            print(" "*4 + f"Will run commands from: {script_temp_gcloud_path}")
+            script_input_obj = self._job._batch.read_input(script_temp_gcloud_path)
+            self._job.command(f"bash -c 'source {script_input_obj}'")
         else:
             for command in self._commands:
                 command_summary = command
                 command_summary_line_count = len(command_summary.split("\n"))
                 if command_summary_line_count > 5:
                     command_summary = "\n".join(command_summary.split("\n")[:5]) + f"\n...  {command_summary_line_count-5} more line(s)"
                 print(" "*4 + f"Adding command: {command_summary}")
@@ -582,32 +648,35 @@
         # transfer outputs
         for output_spec in self._output_specs:
             self._transfer_output_spec(output_spec)
             print(" "*4 + f"Output: {output_spec}  ({output_spec.delocalize_by})")
 
         # clean up any files that were copied to the temp bucket
         if self._paths_localized_via_temp_bucket:
-            cleanup_job_name = f"cleanup {len(self._paths_localized_via_temp_bucket)} files"
+            cleanup_job_name = f"clean up {len(self._paths_localized_via_temp_bucket)} files"
             if self.name:
-                cleanup_job_name += self.name
+                cleanup_job_name += f" from {self.name}"
             cleanup_job = self._pipeline._batch.new_job(name=cleanup_job_name)
+            cleanup_job.image("docker.io/hailgenetics/genetics:0.2.77")
             cleanup_job.depends_on(self._job)
             cleanup_job.always_run()
+            cleanup_job.command("set -x")
+            cleanup_job.command(f"gcloud auth activate-service-account --key-file /gsa-key/key.json")
             for temp_file_path in self._paths_localized_via_temp_bucket:
                 cleanup_job.command(f"gsutil -m rm -r {temp_file_path}")
             self._paths_localized_via_temp_bucket = set()
 
     def _get_supported_localize_by_choices(self):
         """Returns the set of Localize options supported by BatchStep"""
 
         return super()._get_supported_localize_by_choices() | {
             Localize.COPY,
             Localize.GSUTIL_COPY,
-            Localize.HAIL_BATCH_GCSFUSE,
-            Localize.HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET,
+            Localize.HAIL_BATCH_CLOUDFUSE,
+            #Localize.HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET,
         }
 
     def _get_supported_delocalize_by_choices(self):
         """Returns the set of Delocalize options supported by BatchStep"""
 
         return super()._get_supported_delocalize_by_choices() | {
             Delocalize.COPY,
@@ -619,120 +688,153 @@
         the Step runs or not. It validates the input_spec's localize_by value and adds any commands to the
         Step necessary for performing this localization.
 
         Args:
             input_spec (InputSpec): The input to localize.
         """
 
-        super()._preprocess_input_spec(input_spec)
+        input_spec = super()._preprocess_input_spec(input_spec)
 
         if input_spec.localize_by == Localize.GSUTIL_COPY:
-            if not input_spec.source_path.startswith("gs://"):
+            if not input_spec.original_source_path.startswith("gs://"):
                 raise ValueError(f"Expected gs:// path but instead found '{input_spec.local_dir}'")
             self.command(f"mkdir -p '{input_spec.local_dir}'")
-            self.command(self._generate_gsutil_copy_command(input_spec.source_path, input_spec.local_dir))
+            self.command(self._generate_gsutil_copy_command(
+                input_spec.original_source_path, output_dir=input_spec.local_dir))
             self.command(f"ls -lh '{input_spec.local_path}'")   # check that file was copied successfully
 
         elif input_spec.localize_by in (
                 Localize.COPY,
-                Localize.HAIL_BATCH_GCSFUSE,
-                Localize.HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET):
+                Localize.HAIL_BATCH_CLOUDFUSE):
             pass  # these will be handled in _transfer_input_spec(..)
+        elif input_spec.localize_by == Localize.HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET:
+            raise ValueError("Localize.HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET is no longer supported due to changes in gcloud egress charges")
+
+            args = self._pipeline.parse_known_args()
+            source_path = input_spec.source_path
+            source_path_without_protocol = input_spec.source_path_without_protocol
+
+            if not args.batch_remote_tmpdir:
+                raise ValueError("--batch-remote-tmpdir not specified.")
+
+            temp_dir = os.path.join(
+                args.batch_remote_tmpdir,
+                f"pipeline_{self._pipeline._unique_pipeline_instance_id}/step_{self._unique_step_instance_id}",
+                os.path.dirname(source_path_without_protocol).strip("/")+"/")
+            temp_file_path = os.path.join(temp_dir, input_spec.filename)
+
+            if temp_file_path in self._paths_localized_via_temp_bucket:
+                raise ValueError(f"{source_path} has already been localized via temp bucket.")
+            self._paths_localized_via_temp_bucket.add(temp_file_path)
+
+            # copy file to temp bucket
+            gsutil_command = self._generate_gsutil_copy_command(source_path, output_dir=temp_dir)
+            self.command(gsutil_command)
+
+            # create an InputSpec with the updated source path
+            input_spec = InputSpec(
+                source_path=temp_file_path,
+                name=input_spec.name,
+                localize_by=input_spec.localize_by,
+                localization_root_dir=input_spec.localization_root_dir,
+                original_source_path=input_spec.source_path,
+            )
+
         elif input_spec.localize_by not in super()._get_supported_localize_by_choices():
             raise ValueError(
                 f"The hail Batch backend doesn't support input_spec.localize_by={input_spec.localize_by}")
 
+        return input_spec
+
     def _transfer_input_spec(self, input_spec):
         """When a Step isn't skipped and is being transferred to the execution backend, this method is called for
-        each input to the Step. It performs the Steps necessary for localizing this input.
+        each input to the Step. It performs the steps necessary to localize this input.
 
         Args:
             input_spec (InputSpec): The input to localize.
         """
         super()._transfer_input_spec(input_spec)
 
-        args = self._pipeline.parse_args()
+        args = self._pipeline.parse_known_args()
         if args.acceptable_storage_regions:
             check_gcloud_storage_region(
                 input_spec.source_path,
                 expected_regions=args.acceptable_storage_regions,
                 gcloud_project=args.gcloud_project,
                 verbose=args.verbose)
 
         if input_spec.localize_by == Localize.GSUTIL_COPY:
             pass  # All necessary steps for this option were already handled by self._preprocess_input(..)
         elif input_spec.localize_by == Localize.COPY:
             input_spec.read_input_obj = self._job._batch.read_input(input_spec.source_path)
             if self._step_type == BatchStepType.BASH:
-                self._job.command(f"mkdir -p '{input_spec.local_dir}'")
-                self._job.command(f"ln -s {input_spec.read_input_obj} {input_spec.local_path}")
+                self._job.command(f"touch {input_spec.read_input_obj}")   # needed to trigger download
+
+                echo_done_command = 'echo "Done localizing files via COPY"'
+                commands_to_set_up_path = []
+                if not input_spec.local_dir in self._localize_by_copy_already_created_dirs_set:
+                    commands_to_set_up_path.append(f"mkdir -p '{input_spec.local_dir}'")
+                    self._localize_by_copy_already_created_dirs_set.add(input_spec.local_dir)
+                commands_to_set_up_path.append(f"ln -s {input_spec.read_input_obj} {input_spec.local_path}")
+
+                try:
+                    echo_done_command_index = self._commands.index(echo_done_command)
+                except ValueError:
+                    echo_done_command_index = 0
+                    commands_to_set_up_path.append(echo_done_command)
+
+                for command_to_set_up_path in commands_to_set_up_path[::-1]:
+                    self._commands.insert(echo_done_command_index, command_to_set_up_path)
+                
         elif input_spec.localize_by in (
-            Localize.HAIL_BATCH_GCSFUSE,
-            Localize.HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET):
-            self._handle_input_transfer_using_gcsfuse(input_spec)
+            Localize.HAIL_BATCH_CLOUDFUSE,
+            Localize.HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET):
+            self._handle_input_transfer_using_cloudfuse(input_spec)
         elif input_spec.localize_by == Localize.HAIL_HADOOP_COPY:
             self._add_commands_for_hail_hadoop_copy(input_spec.source_path, input_spec.local_dir)
 
-    def _generate_gsutil_copy_command(self, source_path, output_dir):
-        """Utility method that puts together the gsutil command for copying the given source path to an output directory.
+    def _generate_gsutil_copy_command(self, source_path, output_dir=None, output_path=None):
+        """Utility method that puts together the gsutil command for copying the given source path to an output path
+        or directory. Either the output path or the output directory must be provided.
 
         Args:
             source_path (str): The source path.
             output_dir (str): Output directory.
-
+            output_path (str): Output file path.
         Return:
             str: gsutil command string
         """
-        args = self._pipeline.parse_args()
+        args = self._pipeline.parse_known_args()
         gsutil_command = f"gsutil"
         if args.gcloud_project:
             gsutil_command += f" -u {args.gcloud_project}"
 
-        output_dir = output_dir.rstrip("/") + "/"
-        return f"time {gsutil_command} -m cp -r '{source_path}' '{output_dir}'"
+        if output_path:
+            destination = output_path
+        elif output_dir:
+            destination = output_dir.rstrip("/") + "/"
+        else:
+            raise ValueError("Neither output_path nor output_dir arg was specified")
+
+        return f"time {gsutil_command} -m cp -r '{source_path}' '{destination}'"
 
-    def _handle_input_transfer_using_gcsfuse(self, input_spec):
-        """Utility method that implements localizing an input via gcsfuse.
+    def _handle_input_transfer_using_cloudfuse(self, input_spec):
+        """Utility method that implements localizing an input via cloudfuse.
 
         Args:
             input_spec (InputSpec): The input to localize.
         """
-        args = self._pipeline.parse_args()
-
-        source_path = input_spec.source_path
-        source_path_without_protocol = input_spec.source_path_without_protocol
-
         localize_by = input_spec.localize_by
-        if localize_by == Localize.HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET:
-            if not args.batch_remote_tmpdir:
-                raise ValueError("--batch-remote-tmpdir not specified.")
-
-            temp_dir = os.path.join(
-                args.batch_remote_tmpdir,
-                f"batch_{self._unique_batch_id}/job_{self._unique_job_id}",
-                source_path_without_protocol.strip("/")+"/")
-            temp_file_path = os.path.join(temp_dir, input_spec.filename)
-
-            if temp_file_path in self._paths_localized_via_temp_bucket:
-                raise ValueError(f"{source_path} has already been localized via temp bucket.")
-            self._paths_localized_via_temp_bucket.add(temp_file_path)
-
-            # copy file to temp bucket
-            gsutil_command = self._generate_gsutil_copy_command(source_path, temp_dir)
-            print("Running: ", gsutil_command)
-            self._job.command(gsutil_command)
-
-        subdir = localize_by.get_subdir_name()
         source_bucket = input_spec.source_bucket
         local_root_dir = self._pipeline._get_localization_root_dir(localize_by)
-        local_mount_dir = os.path.join(local_root_dir, subdir, source_bucket)
-        if source_bucket not in self._buckets_mounted_via_gcsfuse:
+        local_mount_dir = os.path.join(local_root_dir, localize_by.get_subdir_name(), source_bucket)
+        if source_bucket not in self._buckets_mounted_via_cloudfuse:
             self._job.command(f"mkdir -p {local_mount_dir}")
             self._job.cloudfuse(source_bucket, local_mount_dir, read_only=True)
-            self._buckets_mounted_via_gcsfuse.add(source_bucket)
+            self._buckets_mounted_via_cloudfuse.add(source_bucket)
 
     def _add_commands_for_hail_hadoop_copy(self, source_path, output_dir):
         """Utility method that implements localizing an input via hl.hadoop_copy.
 
         Args:
             source_path (str): The source path.
             output_dir (str): Output directory.
@@ -757,24 +859,29 @@
         Args:
             output_spec (OutputSpec): The output to preprocess.
         """
         if output_spec.delocalize_by not in self._get_supported_delocalize_by_choices():
             raise ValueError(f"Unexpected output_spec.delocalize_by value: {output_spec.delocalize_by}")
 
         super()._preprocess_output_spec(output_spec)
-        if not output_spec.output_dir.startswith("gs://"):
-            raise ValueError(f"{output_spec.output_dir} Destination path must start with gs://")
         if output_spec.delocalize_by == Delocalize.COPY:
             # validate path since Batch delocalization doesn't work for gs:// paths with a Local backend.
-            if output_spec.output_path.startswith("gs://") and self._pipeline.backend == Backend.HAIL_BATCH_LOCAL:
-                raise ValueError("The hail Batch Local backend doesn't support Delocalize.COPY for gs:// paths")
+            if self._pipeline.backend == Backend.HAIL_BATCH_LOCAL and any(
+                    output_spec.output_path.startswith(s) for s in ("gs://", "hail-az://")):
+                raise ValueError("The hail Batch Local backend doesn't support Delocalize.COPY for non-local path: "
+                                 f"{output_spec.output_path}")
             if not output_spec.filename:
                 raise ValueError(f"{output_spec} filename isn't specified. It is required for Delocalize.COPY")
         elif output_spec.delocalize_by == Delocalize.GSUTIL_COPY:
-            self.command(self._generate_gsutil_copy_command(output_spec.local_path, output_spec.output_dir))
+            if not output_spec.output_path.startswith("gs://"):
+                raise ValueError(f"{output_spec.output_path} Destination path must start with gs://")
+
+            if not hasattr(self, "_switched_gcloud_auth_to_user_account"):
+                self.gcloud_auth_activate_service_account()
+            self.command(self._generate_gsutil_copy_command(output_spec.local_path, output_path=output_spec.output_path))
 
     def _transfer_output_spec(self, output_spec):
         """When a Step isn't skipped and is being transferred to the execution backend, this method is called for
         each output of the Step. It performs the steps necessary to delocalize the output using the approach requested
         by the user via the delocalize_by parameter.
 
         Args:
```

### Comparing `step_pipeline-0.2.2/step_pipeline/io.py` & `step_pipeline-0.2.4/step_pipeline/io.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     """
 
     HAIL_HADOOP_COPY = ("hail_hadoop_copy", "local_copy")
     """HAIL_HADOOP_COPY uses the Hail hadoop API to copy file(s) from a google bucket path. This requires python3 and 
     Hail to be installed inside the execution container.
     """
 
-    HAIL_BATCH_GCSFUSE = ("hail_batch_gcsfuse", "gcsfuse")
-    """HAIL_BATCH_GCSFUSE use the Hail Batch gcsfuse function to mount a google bucket into the execution container 
+    HAIL_BATCH_CLOUDFUSE = ("hail_batch_cloudfuse", "cloudfuse")
+    """HAIL_BATCH_CLOUDFUSE use the Hail Batch cloudfuse function to mount a google bucket into the execution container 
     as a network drive, without copying the files. This Hail Batch service account must have read access to the bucket.
     """
 
-    HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET = ("hail_batch_gcsfuse_via_temp_bucket", "gcsfuse")
-    """HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET is useful for situations where you'd like to use gcsfuse to localize files and 
+    HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET = ("hail_batch_cloudfuse_via_temp_bucket", "cloudfuse")
+    """HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET is useful for situations where you'd like to use cloudfuse to localize files and 
     your personal gcloud account has read access to the source bucket, but the Hail Batch service account cannot be 
     granted read access to that bucket. Since it's possible to run 'gsutil cp' under your personal credentials within
-    the execution container, but Hail Batch gcsfuse always runs under the Hail Batch service account credentials, this 
+    the execution container, but Hail Batch cloudfuse always runs under the Hail Batch service account credentials, this 
     workaround 1) runs 'gsutil cp' under your personal credentials to copy the source files to a temporary bucket that 
-    you control, and where you have granted read access to the Hail Batch service account 2) uses gcsfuse to mount the 
+    you control, and where you have granted read access to the Hail Batch service account 2) uses cloudfuse to mount the 
     temporary bucket 3) performs computational steps on the mounted data 4) deletes the source files from the temporary 
     bucket when the Batch job completes.
     
     This localization approach may be useful for situations where you need a large number of jobs and each job processes 
     a very small piece of a large data file (eg. a few loci in a cram file). 
     
     Copying the large file(s) from the source bucket to a temp bucket in the same region is fast and inexpensive, and 
@@ -171,41 +171,54 @@
     """An InputSpec stores metadata about an input file or directory"""
 
     def __init__(
             self,
             source_path=None,
             name=None,
             localize_by=None,
-            localization_root_dir=None):
+            localization_root_dir=None,
+            original_source_path=None,
+    ):
         """InputSpec constructor
 
         Args:
             source_path (str): Source file or directory to localize. It can be a gs://, http(s)://, or a filesystem path.
                 The path can include * wildcards where appropriate.
             name (str): Optional name for this input.
             localize_by (Localize): Approach to use to localize this path.
             localization_root_dir (str): This input will be localized to this directory within the container filesystem.
+            original_source_path (str): Sometimes the file is copied to a different cloud location as part of
+                localization. This is an optional arg to records its original location.
         """
 
         super().__init__(name=name)
 
         self._source_path = source_path
         self._localize_by = localize_by
+        self._localization_root_dir = localization_root_dir
+        self._original_source_path = original_source_path or source_path
 
         # these fields are computed based on the source_path
         self._source_bucket = None
         self._source_path_without_protocol = None
         self._source_dir = None
         self._filename = None
         self._local_dir = None
         self._local_path = None
 
+        if localize_by and not isinstance(localize_by, Localize):
+            raise ValueError(f"localize_by arg: {localize_by} is not an instance of the Localize enum")
+
+        if localization_root_dir and not isinstance(localization_root_dir, str):
+            raise ValueError(f"localization_root_dir arg: {localization_root_dir} is not a string")
+
         if source_path is not None:
-            if source_path.startswith("gs://"):
-                self._source_path_without_protocol = re.sub("^gs://", "", source_path)
+            match = re.match("^([a-zA-Z-_]+)://(.*)", source_path)
+            if match:
+                self._source_path_without_protocol = match.group(2)
                 self._source_bucket = self._source_path_without_protocol.split("/")[0]
             elif source_path.startswith("http://") or source_path.startswith("https://"):
                 self._source_path_without_protocol = re.sub("^http[s]?://", "", source_path).split("?")[0]
             else:
                 self._source_path_without_protocol = source_path
 
             self._source_dir = os.path.dirname(self._source_path_without_protocol)
@@ -229,14 +242,20 @@
     @property
     def source_path(self):
         if self._source_path is None:
             raise ValueError("source_path not available for this input")
         return self._source_path
 
     @property
+    def original_source_path(self):
+        if self._original_source_path is None:
+            raise ValueError("original_source_path not available for this input")
+        return self._original_source_path
+
+    @property
     def source_bucket(self):
         if self._source_bucket is None:
             raise ValueError("source_path not available for this input")
         return self._source_bucket
 
     @property
     def source_path_without_protocol(self):
@@ -268,14 +287,18 @@
             raise ValueError("source_path not available for this input")
         return self._local_dir
 
     @property
     def localize_by(self):
         return self._localize_by
 
+    @property
+    def localization_root_dir(self):
+        return self._localization_root_dir
+
 
 class OutputSpec:
     """An OutputSpec stores metadata about an output file or directory from a Step"""
 
     def __init__(
             self,
             local_path=None,
@@ -294,38 +317,41 @@
             delocalize_by (Delocalize): Approach to use to delocalize this path.
         """
         self._local_path = local_path
         self._local_dir = os.path.dirname(local_path)
         self._name = name
         self._delocalize_by = delocalize_by
 
+        if delocalize_by and not isinstance(delocalize_by, Delocalize):
+            raise ValueError(f"localize_by arg: {delocalize_by} is not an instance of the Delocalize enum")
+
         # define self._output_filename
         if output_path:
             self._output_filename = os.path.basename(output_path)
         elif "*" not in local_path:
             self._output_filename = os.path.basename(local_path)
         else:
             self._output_filename = None
 
         # define self._output_path and self._output_dir
-        if output_dir:
+        if output_path:
+            self._output_path = output_path
+            self._output_dir = os.path.dirname(self._output_path)
+        elif output_dir:
             self._output_dir = output_dir
             if output_path:
-                if os.path.isabs(output_path) or output_path.startswith("gs://"):
+                if os.path.isabs(output_path) or "://" in output_path:
                     self._output_path = output_path
                 else:
                     self._output_path = os.path.join(output_dir, output_path)
             elif self._output_filename:
                 self._output_path = os.path.join(output_dir, self._output_filename)
             else:
                 self._output_path = output_dir
 
-        elif output_path:
-            self._output_path = output_path
-            self._output_dir = os.path.dirname(self._output_path)
         else:
             raise ValueError("Neither output_dir nor output_path were specified.")
 
         if "*" in self._output_path:
             raise ValueError(f"output path ({output_path}) cannot contain wildcards (*)")
 
     def __str__(self):
```

### Comparing `step_pipeline-0.2.2/step_pipeline/main.py` & `step_pipeline-0.2.4/step_pipeline/main.py`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.2/step_pipeline/pipeline.py` & `step_pipeline-0.2.4/step_pipeline/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+import collections
 from abc import ABC, abstractmethod
 
 import configargparse
 import os
+import random
 import re
 import sys
 
 from step_pipeline.utils import _file_stat__cached
-from .utils import are_any_inputs_missing, are_outputs_up_to_date
+from .utils import are_any_inputs_missing, are_outputs_up_to_date, all_outputs_exist
 from .io import Localize, Delocalize, InputSpec, InputValueSpec, OutputSpec
 
+TOO_MANY_COMMAND_LINE_ARGS_ERROR_THRESHOLD = 500
+TOO_MANY_COMMAND_LINE_ARGS_WARNING_THRESHOLD = 500
+
 
 class Pipeline(ABC):
     """Pipeline represents the execution pipeline. This base class contains only generalized code that is not specific
     to any particular execution backend. It has public methods for creating Steps, as well as some private methods that
     implement the general aspects of traversing the execution graph (DAG) and transferring all steps to a specific
     execution backend.
     """
@@ -37,20 +42,26 @@
 
         self._argument_parser = config_arg_parser
 
         self.name = name
         self._config_arg_parser = config_arg_parser
         self._default_output_dir = None
         self._all_steps = []
+        self._unique_pipeline_instance_id = str(random.randint(10**10, 10**11))
 
         config_arg_parser.add_argument("-v", "--verbose", action='count', default=0, help="Print more info")
         config_arg_parser.add_argument("-c", "--config-file", help="YAML config file path", is_config_file_arg=True)
         config_arg_parser.add_argument("--dry-run", action="store_true", help="Don't run commands, just print them.")
         config_arg_parser.add_argument("-f", "--force", action="store_true", help="Force execution of all steps.")
-
+        config_arg_parser.add_argument(
+            "--check-file-last-modified-times",
+            action="store_true",
+            help="When deciding whether a Step can be skipped, instead of only checking whether all output files "
+                 "already exist, also check input and output file last-modified times to make sure that all output "
+                 "files are newer than all input files.")
         config_arg_parser.add_argument(
             "--skip-steps-with-missing-inputs",
             action="store_true",
             help="When a Step is ready to run but has missing input file(s), the default behavior is to print an error "
                  "and exit. This arg instead causes the Step to be skipped with a warning.")
 
         config_arg_parser.add_argument("--export-pipeline-graph", action="store_true",
@@ -82,40 +93,74 @@
             nargs="*",
             default=("US", "US-CENTRAL1"),
             help="If specified, the pipeline will confirm that input buckets are in one of these regions "
                  "to avoid egress charges",
         )
 
         # validate the command-line args defined so far
-        args = self.parse_args()
+        args = self.parse_known_args()
         if args.slack_when_done and (not args.slack_token or not args.slack_channel):
             config_arg_parser.error(
                 "Both --slack-token and --slack-channel must be specified when --slack-when-done is used")
 
+    def set_name(self, name):
+        """Update the pipeline name"""
+
+        self.name = name
+
     def get_config_arg_parser(self):
         """Returns the configargparse.ArgumentParser object used by the Pipeline to define command-line args.
         This is a drop-in replacement for argparse.ArgumentParser with some extra features such as support for
         config files and environment variables. See https://github.com/bw2/ConfigArgParse for more details.
         You can use this to add and parse your own command-line arguments the same way you would using argparse. For
         example:
 
         p = pipeline.get_config_arg_parser()
         p.add_argument("--my-arg")
         args = pipeline.parse_args()
         """
         return self._config_arg_parser
 
     def parse_args(self):
+        """Parse command line args.
+
+        Return:
+            argparse args object.
+        """
+        return self._config_arg_parser.parse_args()
+
+    def parse_known_args(self):
         """Parse command line args defined up to this point. This method can be called more than once.
 
         Return:
             argparse args object.
         """
-        args, _ = self._config_arg_parser.parse_known_args(ignore_help_args=True)
-        return args
+        global TOO_MANY_COMMAND_LINE_ARGS_WARNING_THRESHOLD
+
+        current_num_args = len(self._config_arg_parser._actions)
+        shared_message_text = (
+            "To avoid this, you can use the my_pipeline.new_step(arg_suffix=..) argument to specify a single common "
+            "command-line arg suffix for Steps that run in parallel (eg. arg_suffix='step2'), while still specifying "
+            "a unique Step name (such as a sample id) for each individual parallel Step.")
+        if current_num_args > TOO_MANY_COMMAND_LINE_ARGS_ERROR_THRESHOLD:
+            raise ValueError(
+                f"The pipeline now has more than {TOO_MANY_COMMAND_LINE_ARGS_ERROR_THRESHOLD} command-line args. "
+                f"{shared_message_text}")
+        elif current_num_args > TOO_MANY_COMMAND_LINE_ARGS_WARNING_THRESHOLD:
+            print(f"WARNING: The pipeline now has more than {TOO_MANY_COMMAND_LINE_ARGS_WARNING_THRESHOLD} "
+                  f"command-line args. {shared_message_text}")
+            TOO_MANY_COMMAND_LINE_ARGS_WARNING_THRESHOLD = 10**10
+
+        # speed up this method by caching the results of parse_known_args(..) until the number of args changes
+        if not hasattr(self, "_num_args") or self._num_args != current_num_args:
+            args, _ = self._config_arg_parser.parse_known_args(ignore_help_args=True)
+            self._cached_args = args
+            self._num_args = current_num_args
+
+        return self._cached_args
 
     @abstractmethod
     def new_step(self, name, step_number=None):
         """Creates a new pipeline Step. Subclasses must implement this method.
 
         Args:
             name (str): A short name for the step.
@@ -157,16 +202,16 @@
 
     @abstractmethod
     def run(self):
         """Submits a pipeline to an execution engine such as Hail Batch. Subclasses must implement this method.
         They should use this method to perform initialization of the specific execution backend and then call
         self._transfer_all_steps(..).
         """
-        # run parse_args(..) instead of self.parse_args() for the 1st time to confirm that all required command-line
-        # args were provided
+        # run self.parse_args(..) instead of self.parse_known_args() for the 1st time to confirm that all required
+        # command-line args were provided
         self._argument_parser.parse_args()
 
         args = self.parse_args()
         if args.export_pipeline_graph:
             output_filename_prefix = re.sub("[:, ]", "_", self.name)
             output_svg_path = f"{output_filename_prefix}.pipeline_diagram.svg"
             self.export_pipeline_graph(output_svg_path=output_svg_path)
@@ -192,14 +237,39 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """This method runs at the completion of a 'with' block, and is used to launch the pipeline after all Steps
          have been defined."""
 
         self.run()
 
+    def _check_step_graph_for_cycles(self, start_with_step=None):
+        """TODO test implementation"""
+
+        if start_with_step is None:
+            for step in self._all_steps:
+                # initialize variables to keep track of DAG traversal
+                step.dag_traversal_all_descendents_already_visited = False
+                step.dag_traversal_step_visit_count = 0
+
+            steps = [s for s in self._all_steps if not s.has_upstream_steps()]
+        else:
+            steps = [start_with_step]
+
+        for step in steps:
+            step.dag_traversal_step_visit_count += 1
+            if not step.dag_traversal_all_descendents_already_visited and step.dag_traversal_step_visit_count > 1:
+                raise ValueError(f"Cycle detected. {next_step} was already visited")
+
+            # push child steps
+            for next_step in step._downstream_steps:
+                if not next_step.dag_traversal_all_descendents_already_visited:
+                    self._check_step_graph_for_cycles(start_with_step=next_step)
+
+            step.dag_traversal_all_descendents_already_visited = True
+
     def _transfer_all_steps(self):
         """This method performs the core task of executing a pipeline. It traverses the execution graph (DAG) of
         user-defined Steps and decides which steps can be skipped, and which should be executed (ie. transferred to
         the execution backend).
 
         To decide whether a Step needs to run, this method takes into account any --skip-* command-line args,
         --force-* command-line args, whether the Step's output files already exist and are newer than all input files,
@@ -210,74 +280,120 @@
 
         Return:
             int: number of transferred steps
         """
 
         args = self.parse_args()
 
+        self._check_step_graph_for_cycles()
+
+        step_counters = collections.defaultdict(int)  # count steps seen (by name)
+        step_run_counters = collections.defaultdict(int) # count steps run (by name)
         current_steps = [s for s in self._all_steps if not s.has_upstream_steps()]
         num_steps_transferred = 0
+
+        # set up 'visited' boolean to track whether a Step has already been visited by the DAG traversal
+        for step in self._all_steps:
+            step.visited = False
+
+        # begin traversal of DAG
         while current_steps:
-            #print("Next steps: ", current_steps)
             for step in current_steps:
+                step.visited = True
+
                 if not step._commands:
                     print(f"WARNING: No commands specified for step [{step}]. Skipping...")
                     continue
 
+                step_counters[step.name] += 1
+
                 # decide whether this step needs to run
                 decided_this_step_needs_to_run = False
 
                 skip_requested = any(
                     getattr(args, skip_arg_name.replace("-", "_")) for skip_arg_name in step._skip_this_step_arg_names
                 )
+                skip_requested |= any(
+                    (getattr(args, run_n_arg_name.replace("-", "_")) or 10**9) < step_run_counters[step.name]
+                    for run_n_arg_name in step._run_n_arg_names
+                )
+                skip_requested |= any(
+                    (getattr(args, run_offset_arg_name.replace("-", "_")) or 0) > step_counters[step.name]
+                    for run_offset_arg_name in step._run_offset_arg_names
+                )
 
                 if skip_requested:
                     print(f"Skipping {step} as requested")
                 else:
                     is_being_forced = args.force or any(
                         getattr(args, force_arg_name.replace("-", "_")) for force_arg_name in step._force_this_step_arg_names
                     )
                     if is_being_forced:
                         decided_this_step_needs_to_run = True
 
                     if not decided_this_step_needs_to_run:
                         all_upstream_steps_skipped = all(s._is_being_skipped for s in step._upstream_steps)
                         if not all_upstream_steps_skipped:
+                            if args.verbose:
+                                print(f"Running {step} because upstream step is going to run.")
                             decided_this_step_needs_to_run = True
-
-                    if not decided_this_step_needs_to_run:
-                        # only do this check if upstream steps are being skipped. Otherwise, input files may not exist yet.
-                        if args.skip_steps_with_missing_inputs and are_any_inputs_missing(step, verbose=args.verbose):
+                        elif args.skip_steps_with_missing_inputs and are_any_inputs_missing(step, verbose=args.verbose):
+                            # only do this check if upstream steps are being skipped. Otherwise, input files may not exist yet.
                             continue  # skip this step
 
-                        outputs_are_up_to_date = are_outputs_up_to_date(step, verbose=args.verbose)
-                        if not outputs_are_up_to_date:
-                            decided_this_step_needs_to_run = True
+                    if not decided_this_step_needs_to_run:
+                        if not args.check_file_last_modified_times:
+                            if len(step._output_specs) == 0:
+                                if args.verbose:
+                                    print(f"Running {step}. No outputs specified.")
+                                decided_this_step_needs_to_run = True
+                            elif not all_outputs_exist(step, verbose=args.verbose):
+                                if args.verbose:
+                                    print(f"Running {step} because some output(s) don't exist yet.")
+                                decided_this_step_needs_to_run = True
                         else:
-                            print(f"Skipping {step}. The {len(step._output_specs)} output(s) already exist and are up-to-date.")
-                            if args.verbose > 0:
-                                print(f"Outputs:")
-                                for o in step._output_specs:
-                                    print(f"       {o}")
+                            if not are_outputs_up_to_date(step, verbose=args.verbose):
+                                if args.verbose:
+                                    print(f"Running {step} because some output(s) don't exist yet or are not up-to-date.")
+
+                                decided_this_step_needs_to_run = True
+
+                    if not decided_this_step_needs_to_run:
+                        print(f"Skipping {step}. The {len(step._output_specs)} output" +
+                              ("s already exist" if len(step._output_specs) > 1 else " already exists") +
+                              ("." if args.check_file_last_modified_times else
+                               " and are up-to-date." if len(step._output_specs) > 1 else " and is up-to-date"))
+                        if args.verbose > 0:
+                            print(f"Outputs:")
+                            for o in step._output_specs:
+                                print(f"       {o}")
 
                 if decided_this_step_needs_to_run:
                     print(f"==> Running {step}")
                     step._is_being_skipped = False
                     step._transfer_step()
+
+                    step_run_counters[step.name] += 1
                     num_steps_transferred += 1
                 else:
                     step._is_being_skipped = True
 
             # next, process all steps that depend on the previously-completed steps
             next_steps = []
             for step in current_steps:
                 for downstream_step in step._downstream_steps:
-                    # if multiple current steps share the same downstream step, avoid adding it multiple times
-                    if downstream_step not in next_steps:
-                        next_steps.append(downstream_step)
+                    if downstream_step in next_steps:
+                        # when multiple current steps share the same downstream step, avoid adding it multiple times
+                        continue
+
+                    if any(not s.visited for s in downstream_step._upstream_steps):
+                        # if any of the steps this downstream step depends on haven't been processed yet, wait for that
+                        continue
+                    next_steps.append(downstream_step)
+
             current_steps = next_steps
 
         return num_steps_transferred
 
     def _generate_post_to_slack_command(self, message, channel=None, slack_token=None):
         """Generates the command which posts to Slack
 
@@ -286,29 +402,35 @@
             channel (str): The Slack channel to post to.
             slack_token (str): Slack auth token.
 
         Return:
             str: command that posts the given message to Slack
         """
 
-        args = self.parse_args()
+        args = self.parse_known_args()
         slack_token = slack_token or args.slack_token
         if not slack_token:
             raise ValueError("slack token not provided")
         channel = channel or args.slack_channel
         if not channel:
             raise ValueError("slack channel not specified")
 
         return f"""python3 <<EOF
 from slacker import Slacker
 slack = Slacker("{slack_token}")
 response = slack.chat.post_message("{channel}", "{message}", as_user=False, icon_emoji=":bell:", username="step-pipeline-bot")
 print(response.raw)
 EOF"""
 
+    def precache_file_paths(self, glob_path):
+        """This method is an alias for the check_input_glob(..) method"""
+
+        return self.check_input_glob(glob_path)
+
+
     def check_input_glob(self, glob_path):
         """This method is useful for checking the existence of multiple input files and caching the results.
         Input file(s) to this Step using glob syntax (ie. using wildcards as in `gs://bucket/**/sample*.cram`)
 
         Args:
             path (str): local file path or gs:// Google Storage path. The path can contain wildcards (*).
 
@@ -320,16 +442,18 @@
                     'path': 'gs://bucket/dir/file.bam.bai',
                     'size_bytes': 2784,
                     'modification_time': 'Wed May 20 12:52:01 EDT 2020',
                 },
             ]
 
         """
-
-        return _file_stat__cached(glob_path)
+        try:
+            return _file_stat__cached(glob_path)
+        except FileNotFoundError as e:
+            return []
 
     def export_pipeline_graph(self, output_svg_path=None):
         """Renders the pipeline execution graph diagram based on the Steps defined so far.
 
         Args:
             output_svg_path (str): Path where to write the SVG image with the execution graph diagram. If not specified,
                 it will be based on the pipeline name.
@@ -393,40 +517,46 @@
     skipped if the output files already exist (and are newer than any input files unless a --force arg is used).
     A Step's input and output files must be stored in some persistant location, like a local disk or GCS.
 
     Using Hail Batch as an example, a Step typically corresponds to a single Hail Batch Job. Sometimes a Job can be
     reused to run multiple steps (for example, where step 1 creates a VCF and step 2 tabixes it).
     """
     _STEP_ID_COUNTER = 0
-    _USED_ARG_SUFFIXES = set()
+    _USED_FORCE_ARG_SUFFIXES = set()
+    _USED_SKIP_ARG_SUFFIXES = set()
+    _USED_RUN_SUBSET_ARG_SUFFIXES = set()
 
     def __init__(self,
                  pipeline,
                  name,
                  step_number=None,
                  arg_suffix=None,
                  output_dir=None,
                  localize_by=None,
                  delocalize_by=None,
                  add_force_command_line_args=True,
-                 add_skip_command_line_args=True):
+                 add_skip_command_line_args=True,
+                 add_run_subset_command_line_args=True,
+        ):
         """Step constructor
 
         Args:
             pipeline (Pipeline): The Pipeline object representing the current pipeline.
             name (str): A short name for this step
             step_number (int): If specified, --skip-step{step_number} and --force-step{step_number} command-line args
                 will be created.
             arg_suffix (str): If specified, --skip-{arg_suffix} and --force-{arg_suffix} command-line args will be
                 created.
             output_dir (str): If specified, this will be the default output directory used by Step outputs.
             localize_by (Localize): If specified, this will be the default Localize approach used by Step inputs.
             delocalize_by (Delocalize): If specified, this will be the default Delocalize approach used by Step outputs.
             add_force_command_line_args (bool): Whether to add command line args for forcing execution of this Step.
             add_skip_command_line_args (bool): Whether to add command line args for skipping execution of this Step.
+            add_run_subset_command_line_args (bool): Whether to add command line args for running a subset of
+                parallel jobs from this Step (--run-n-step1, --run-offset-step1).
         """
         self._pipeline = pipeline
         self.name = name
         self.step_number = step_number
         self.arg_suffix = arg_suffix
         self._output_dir = output_dir
 
@@ -445,50 +575,86 @@
         self._upstream_steps = []  # this Step depends on these Steps
         self._downstream_steps = []  # Steps that depend on this Step
 
         self._is_being_skipped = False  # records whether this Step is being skipped
 
         self._force_this_step_arg_names = []
         self._skip_this_step_arg_names = []
+        self._run_n_arg_names = []
+        self._run_offset_arg_names = []
 
         Step._STEP_ID_COUNTER += 1
         self._step_id = Step._STEP_ID_COUNTER  # this id is unique to each Step object
 
+        self._unique_step_instance_id = str(random.randint(10**10, 10**11))
+
         # define command line args for skipping or forcing execution of this step
         argument_parser = pipeline.get_config_arg_parser()
 
-        command_line_arg_suffixes = []
+        command_line_arg_suffixes = set()
+        def cleanup_arg_suffix(suffix):
+            return suffix.replace(" ", "-").replace(":", "").replace("_", "-")
+
         if arg_suffix:
-            command_line_arg_suffixes.append(arg_suffix)
+            command_line_arg_suffixes.add(cleanup_arg_suffix(arg_suffix))
         elif name:
-            command_line_arg_suffixes.append(name.replace(" ", "-").replace(":", ""))
+            command_line_arg_suffixes.add(cleanup_arg_suffix(name))
 
         if step_number is not None:
             if not isinstance(step_number, (int, float)):
                 raise ValueError(f"step_number must be an integer or a float rather than '{step_number}'")
-            command_line_arg_suffixes.append(f"step{step_number}")
+            command_line_arg_suffixes.add(f"step{step_number}")
 
         for suffix in command_line_arg_suffixes:
             if add_force_command_line_args:
                 self._force_this_step_arg_names.append(f"force_{suffix}")
-                if suffix not in Step._USED_ARG_SUFFIXES:
+                if suffix not in Step._USED_FORCE_ARG_SUFFIXES:
                     argument_parser.add_argument(
                         f"--force-{suffix}",
                         help=f"Force execution of '{name}'.",
                         action="store_true",
                     )
+                    Step._USED_FORCE_ARG_SUFFIXES.add(suffix)
+
             if add_skip_command_line_args:
                 self._skip_this_step_arg_names.append(f"skip_{suffix}")
-                if suffix not in Step._USED_ARG_SUFFIXES:
+                if suffix not in Step._USED_SKIP_ARG_SUFFIXES:
                     argument_parser.add_argument(
                         f"--skip-{suffix}",
                         help=f"Skip '{name}' even if --force is used.",
                         action="store_true",
                     )
-            Step._USED_ARG_SUFFIXES.add(suffix)
+                    Step._USED_SKIP_ARG_SUFFIXES.add(suffix)
+
+            if add_run_subset_command_line_args:
+                self._run_n_arg_names.append(f"run_n_{suffix}")
+                self._run_offset_arg_names.append(f"run_offset_{suffix}")
+                if suffix not in Step._USED_RUN_SUBSET_ARG_SUFFIXES:
+                    argument_parser.add_argument(
+                        f"--run-n-{suffix}",
+                        help=f"Run only this many parallel jobs for '{name}' even if --force is used. This can be "
+                             f"useful for test-running a pipeline.",
+                        type=int,
+                    )
+                    argument_parser.add_argument(
+                        f"--run-offset-{suffix}",
+                        help=f"Skip the first this many parallel jobs from '{name}' even if --force is used. This can "
+                             f"be useful for test-running a pipeline, especially when used with --run-n-..",
+                        type=int,
+                    )
+                    Step._USED_RUN_SUBSET_ARG_SUFFIXES.add(suffix)
+
+    def __eq__(self, other):
+        return isinstance(other, Step) and self._step_id == other._step_id
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __hash__(self):
+        return self._step_id
 
     def name(self, name):
         """Set the short name for this Step.
 
         Args:
             name (str): Name
         """
@@ -555,28 +721,35 @@
 
         Return:
             InputSpec: An object that describes the specified input file or directory.
         """
         localize_by = localize_by or self._localize_by
 
         # validate inputs
+        if source_path is not None and not isinstance(source_path, str):
+            raise ValueError(f"source_path '{source_path}' has type {type(source_path).__name__} instead of string")
+
         if not source_path.startswith("gs://") and localize_by in (
                 Localize.GSUTIL_COPY,
-                Localize.HAIL_BATCH_GCSFUSE,
-                Localize.HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET):
+        ):
             raise ValueError(f"source_path '{source_path}' doesn't start with gs://")
 
+        if not source_path.startswith("gs://") and not source_path.startswith("hail-az://") and localize_by in (
+                Localize.HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET,
+        ):
+            raise ValueError(f"source_path '{source_path}' doesn't start with gs:// or hail-az://")
+
         input_spec = InputSpec(
             source_path=source_path,
             name=name,
             localize_by=localize_by,
             localization_root_dir=self._pipeline._get_localization_root_dir(localize_by),
         )
 
-        self._preprocess_input_spec(input_spec)
+        input_spec = self._preprocess_input_spec(input_spec)
         self._input_specs.append(input_spec)
 
         return input_spec
 
     def inputs(self, source_path, *source_paths, name=None, localize_by=None):
         """Specifies one or more input file or directory paths.
 
@@ -743,22 +916,25 @@
         """Marks this Step as being downstream of another Step in the pipeline, meaning that this Step can only run
         after the upstream_step has completed successfully.
 
         Args:
             upstream_step (Step): The upstream Step this Step depends on.
         """
         if isinstance(upstream_step, Step):
-            self._upstream_steps.append(upstream_step)
-            upstream_step._downstream_steps.append(self)
+            if upstream_step not in self._upstream_steps:
+                self._upstream_steps.append(upstream_step)
+            if self not in upstream_step._downstream_steps:
+                upstream_step._downstream_steps.append(self)
 
         elif isinstance(upstream_step, list):
-            self._upstream_steps.extend(upstream_step)
             for _upstream_step in upstream_step:
-                _upstream_step._downstream_steps.append(self)
-
+                if _upstream_step not in self._upstream_steps:
+                    self._upstream_steps.append(_upstream_step)
+                if self not in _upstream_step._downstream_steps:
+                    _upstream_step._downstream_steps.append(self)
         else:
             raise ValueError(f"Unexpected step object type: {type(upstream_step)}")
 
     def has_upstream_steps(self):
         """Returns True if this Step has upstream Steps that must run before it runs (ie. that it depends on)"""
 
         return len(self._upstream_steps) > 0
@@ -787,14 +963,19 @@
         """
         if not hasattr(self, "_already_installed_slacker"):
             self.command("python3 -m pip install slacker")
             self._already_installed_slacker = True
 
         self.command(self._pipeline._generate_post_to_slack_command(message, channel=channel, slack_token=slack_token))
 
+    def gcloud_auth_activate_service_account(self):
+        """Utility method to active gcloud auth using the Hail Batch-provided service account"""
+
+        self.command(f"gcloud auth activate-service-account --key-file /gsa-key/key.json")
+
     def switch_gcloud_auth_to_user_account(self, gcloud_credentials_path=None, gcloud_user_account=None,
                                            gcloud_project=None, debug=False):
         """This method adds commands to this Step to switch gcloud auth from the Batch-provided service
         account to the user's personal account.
 
         This is useful if subsequent commands need to access google buckets that to which the user's personal account
         has access but to which the Batch service account cannot be granted access for whatever reason.
@@ -823,15 +1004,15 @@
             gcloud_credentials_path (str): Google bucket path that contains your gcloud auth .config folder.
             gcloud_user_account (str): The user account to activate (ie. "weisburd@broadinstitute.org").
             gcloud_project (str): This will be set as the default gcloud project within the container.
             debug (bool): Whether to add extra "gcloud auth list" commands that are helpful for troubleshooting issues
                 with the auth steps.
         """
 
-        args = self._pipeline.parse_args()
+        args = self._pipeline.parse_known_args()
         if not gcloud_credentials_path:
             gcloud_credentials_path = args.gcloud_credentials_path
             if not gcloud_credentials_path:
                 raise ValueError("gcloud_credentials_path not specified")
 
         if not gcloud_user_account:
             gcloud_user_account = args.gcloud_user_account
@@ -840,25 +1021,27 @@
 
         if not gcloud_project:
             gcloud_project = args.gcloud_project
 
         if debug:
             self.command(f"gcloud auth list")
         
-        self.command(f"gcloud auth activate-service-account --key-file /gsa-key/key.json")
+        self.gcloud_auth_activate_service_account()
         self.command(f"gsutil -m cp -r {os.path.join(gcloud_credentials_path, '.config')} /tmp/")
         self.command(f"rm -rf ~/.config")
         self.command(f"mv /tmp/.config ~/")
         self.command(f"gcloud config set account {gcloud_user_account}")
         if gcloud_project:
             self.command(f"gcloud config set project {gcloud_project}")
         
         if debug:
             self.command(f"gcloud auth list")  # print auth list again to check if 'gcloud config set account' succeeded
 
+        self._switched_gcloud_auth_to_user_account = True
+
     @abstractmethod
     def _get_supported_localize_by_choices(self):
         """Returns set of Localize options supported by this pipeline"""
         return set()
 
     @abstractmethod
     def _get_supported_delocalize_by_choices(self):
@@ -870,18 +1053,23 @@
         """This method is called by step.input(..) immediately when the input is first specified, regardless of whether
         the Step runs or not. It should perform simple checks of the input_spec that are fast and don't require a
         network connection, but that catch simple errors such as incorrect source path syntax.
         Step subclasses must implement this method.
 
         Args:
             input_spec (InputSpec): The input to preprocess.
+
+        Return:
+            input_spec (InputSpec): A potentially-updated input_spec.
         """
         if input_spec.localize_by not in self._get_supported_localize_by_choices():
             raise ValueError(f"Unexpected input_spec.localize_by value: {input_spec.localize_by}")
 
+        return input_spec
+
     @abstractmethod
     def _transfer_input_spec(self, input_spec):
         """When a Step isn't skipped and is being transferred to the execution backend, this method is called for
         each input to the Step. It should localize the input into the Step's execution container using the approach
         requested by the user via the localize_by parameter.
 
         Args:
```

### Comparing `step_pipeline-0.2.2/step_pipeline/utils.py` & `step_pipeline-0.2.4/step_pipeline/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 PATH_EXISTS_CACHE = {}
 PATH_STAT_CACHE = {}
 GSUTIL_PATH_TO_FILE_STAT_CACHE = {}
 BUCKET_LOCATION_CACHE = {}
 
 LOCAL_TIMEZONE = pytz.timezone("US/Eastern") #datetime.now(timezone.utc).astimezone().tzinfo
 
+DATE_STRFTIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 def _get_bucket_name(gs_path):
     """Get the Google bucket name from the given gs_path."""
 
     gs_path_tokens = gs_path.split("/")
     if not gs_path.startswith("gs://") or len(gs_path_tokens) < 3:
         raise ValueError(f"Invalid gs_path arg: {gs_path}")
@@ -68,27 +69,28 @@
         if any(phrase in e.output for phrase in (
             "One or more URLs matched no objects",
             "bucket does not exist.",
         )):
             return {}
         else:
             raise GoogleStorageException(e.output)
+
     # map path to file size in bytes and its last-modified date (eg. "2020-05-20T16:52:01Z")
     def parse_gsutil_date_string(date_string):
         #utc_date = datetime.strptime(date_string, "%Y-%m-%dT%H:%M:%SZ").replace(tzinfo=timezone.utc)
         utc_date = parser.parse(date_string).replace(tzinfo=timezone.utc)
         return utc_date.astimezone(LOCAL_TIMEZONE)
 
-    records = [r.strip().split("  ") for r in gsutil_output.strip().split("\n") if not r.startswith("TOTAL: ")]
+    records = [r.strip().split("  ") for r in gsutil_output.strip().split("\n") if r.startswith("   ") and "gs://" in r]
     try:
         path_to_file_stat_dict = {
             r[2]: (int(r[0]), parse_gsutil_date_string(r[1])) for r in records
         }
     except Exception as e:
-        raise Exception(f"Unable to parse gsutil output for {gs_path_with_wildcards}: {e}\n{gsutil_output}")
+        raise GoogleStorageException(f"Unable to parse gsutil output for {gs_path_with_wildcards}: {e}\n{gsutil_output}")
 
     print(f"Found {len(path_to_file_stat_dict)} matching paths")
 
     GSUTIL_PATH_TO_FILE_STAT_CACHE[gs_path_with_wildcards] = path_to_file_stat_dict
 
     return path_to_file_stat_dict
 
@@ -118,15 +120,18 @@
     else:
         if "*" in path:
             PATH_EXISTS_CACHE[path] = len(glob.glob(path)) > 0
         else:
             PATH_EXISTS_CACHE[path] = os.path.exists(path)
 
     if verbose:
-        print(f"Checked if exists: {path}   Result: ", PATH_EXISTS_CACHE[path])
+        if PATH_EXISTS_CACHE[path]:
+            print(f"Confirmed path exists: {path}")
+        else:
+            print(f"Missing path: {path}")
 
     return PATH_EXISTS_CACHE[path]
 
 
 def _file_stat__cached(path, verbose=False):
     """Takes a local file path or gs:// Google Storage path and returns a list of file stats including the size in bytes
     and the modification time.
@@ -189,27 +194,28 @@
                     stat_results["modification_time"]).replace(tzinfo=LOCAL_TIMEZONE)
             elif isinstance(stat_results["modification_time"], str):
                 try:
                     stat_results["modification_time"] = LOCAL_TIMEZONE.localize(
                         parser.parse(stat_results["modification_time"], ignoretz=True))
                 except Exception as e:
                     raise Exception(f"Unable to parse 'modification_time' from {stat_results}: {e}")
+            elif stat_results["modification_time"] == None:
+                raise GoogleStorageException(f"hl.stat returned modification_time == None for {path}")
             else:
-                raise Exception(f"Unexpected stat_results type: {type(stat_results)}: {stat_results}")
+                raise GoogleStorageException(f"Unexpected modification_time type: {type(stat_results['modification_time'])} in {stat_results}")
 
             PATH_STAT_CACHE[path] = [stat_results]
             PATH_EXISTS_CACHE[path] = True
 
     else:
         if "*" in path:
             local_paths = glob.glob(path)
         else:
             local_paths = [path]
 
-        print(f"Running stat on {local_paths}")
         for local_path in local_paths:
             stat = os.stat(local_path)
             if path not in PATH_STAT_CACHE:
                 PATH_STAT_CACHE[path] = []
             stat_results = {
                 "path": local_path,
                 "size_bytes": stat.st_size,
@@ -222,17 +228,16 @@
     if verbose:
         for stat_results in PATH_STAT_CACHE[path]:
             try:
                 file_size_str = "%0.1f Gb" % (int(stat_results["size_bytes"])/10**9)
             except Exception as e:
                 file_size_str = "%s bytes  (%s)" % (stat_results["size_bytes"], str(e))
 
-            print(f"Checked path stats: {path}   Result:",
-                  f"last-modified =", stat_results["modification_time"],
-                  " size =", file_size_str)
+            last_modified_time = stat_results['modification_time']
+            print(f"Checked path stats: {file_size_str:5}  {last_modified_time:15}   {path}")
 
     return PATH_STAT_CACHE[path]
 
 
 def are_any_inputs_missing(step, verbose=False):
     """Returns True if any of the Step's inputs don't exist"""
     for input_spec in step._input_specs:
@@ -240,49 +245,79 @@
         if not _path_exists__cached(input_path, verbose=verbose):
             print(f"WARNING: Input missing: {input_path}")
             return True
 
     return False
 
 
-def are_outputs_up_to_date(step, verbose=False):
-    """Returns True if all of the Step's outputs already exist and are newer than all inputs"""
+def all_outputs_exist(step, verbose=False):
+    """Returns True if all of the Step's output files already exist"""
+    return files_exist([output_spec.output_path for output_spec in step._output_specs], verbose=verbose)
+
+
+def files_exist(file_paths, verbose=False):
+    """Returns True if all of the files exist"""
+    for file_path in file_paths:
+        if not _path_exists__cached(file_path, verbose=verbose):
+            return False
+
+    return True
+
+
+def are_output_files_up_to_date(input_paths, output_paths, verbose=False):
+    """Returns True if all of the output files already exist and are newer than all the input files.
 
-    if len(step._output_specs) == 0:
+    input_paths (list): gs:// paths of input files
+    output_paths (list): gs:// paths of output files
+
+    Returns:
+        bool: True if all output files exist and are newer than all input files
+    """
+    if len(output_paths) == 0:
         return False
 
     latest_input_path = None
     latest_input_modified_date = datetime(2, 1, 1, tzinfo=LOCAL_TIMEZONE)
-    for input_spec in step._input_specs:
-        input_path = input_spec.source_path
+    for input_path in input_paths:
         if not _path_exists__cached(input_path, verbose=verbose):
             raise ValueError(f"Input path doesn't exist: {input_path}")
 
         stat_list = _file_stat__cached(input_path, verbose=verbose)
         for stat in stat_list:
-            latest_input_modified_date = max(latest_input_modified_date, stat["modification_time"])
-            latest_input_path = stat["path"]
+            if stat["modification_time"] > latest_input_modified_date:
+                latest_input_modified_date = stat["modification_time"]
+                latest_input_path = stat["path"]
 
     # check whether any outputs are missing
     oldest_output_path = None
-    oldest_output_modified_date = datetime.now(LOCAL_TIMEZONE)
-    for output_spec in step._output_specs:
-        if not _path_exists__cached(output_spec.output_path, verbose=verbose):
+    oldest_output_modified_date = None
+    for output_path in output_paths:
+        if not _path_exists__cached(output_path, verbose=verbose):
             return False
 
-        stat_list = _file_stat__cached(output_spec.output_path, verbose=verbose)
+        stat_list = _file_stat__cached(output_path, verbose=verbose)
         for stat in stat_list:
-            oldest_output_modified_date = min(oldest_output_modified_date, stat["modification_time"])
-            oldest_output_path = stat["path"]
+            if oldest_output_modified_date is None or stat["modification_time"] < oldest_output_modified_date:
+                oldest_output_modified_date = stat["modification_time"]
+                oldest_output_path = stat["path"]
 
     if verbose:
-        print(f"Oldest output ({oldest_output_modified_date}): {oldest_output_path},  "
-              f"newest input ({latest_input_modified_date}): {latest_input_path}")
+        print(f"Newest input    {latest_input_modified_date.strftime(DATE_STRFTIME_FORMAT):20}: {latest_input_path}")
+        print(f"Oldest output   {oldest_output_modified_date.strftime(DATE_STRFTIME_FORMAT) if oldest_output_modified_date else '':20}: {oldest_output_path}")
+
+    return oldest_output_modified_date is not None and latest_input_modified_date <= oldest_output_modified_date
+
+
+def are_outputs_up_to_date(step, verbose=False):
+    """Returns True if all of the Step's outputs already exist and are newer than all inputs"""
+
+    input_paths = [input_spec.original_source_path for input_spec in step._input_specs]
+    output_paths = [output_spec.output_path for output_spec in step._output_specs]
 
-    return latest_input_modified_date <= oldest_output_modified_date
+    return are_output_files_up_to_date(input_paths, output_paths, verbose=verbose)
 
 
 class GoogleStorageException(Exception):
     pass
 
 
 def check_gcloud_storage_region(gs_path, expected_regions=("US", "US-CENTRAL1"), gcloud_project=None,
@@ -318,13 +353,12 @@
             if not ignore_access_denied_exception or "access" not in str(e).lower():
                 raise GoogleStorageException(f"ERROR: Could not determine gs://{bucket_name} bucket region: {e}")
 
             print(f"WARNING: Unable to check bucket region for gs://{bucket_name}: {e}")
             return
 
     if location not in expected_regions:
-        #raise GoogleStorageException(
-        print(
+        raise GoogleStorageException(
             f"ERROR: gs://{bucket_name} is located in {location} which is not one of the "
             f"expected regions {expected_regions}")
     if verbose:
         print(f"Confirmed gs://{bucket_name} is in {location}")
```

### Comparing `step_pipeline-0.2.2/step_pipeline/wdl.py` & `step_pipeline-0.2.4/step_pipeline/wdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,15 @@
         the Step runs or not. It validates the input_spec's localize_by value and adds any commands to the
         Step necessary for performing this localization.
 
         Args:
             input_spec (InputSpec): The input to localize.
         """
 
-        super()._preprocess_input_spec(input_spec)
+        return super()._preprocess_input_spec(input_spec)
 
     def _transfer_input_spec(self, input_spec):
         """When a Step isn't skipped and is being transferred to the execution backend, this method is called for
         each input to the Step. It performs the Steps necessary for localizing this input.
 
         Args:
             input_spec (InputSpec): The input to localize.
```

### Comparing `step_pipeline-0.2.2/tests/utils_tests.py` & `step_pipeline-0.2.4/tests/utils_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     def _get_supported_delocalize_by_choices(self):
         return {
             Delocalize.COPY,
         }
 
     def _preprocess_input_spec(self, input_spec):
-        pass
+        return input_spec
 
     def _preprocess_output_spec(self, output_spec):
         pass
 
     def _transfer_input_spec(self, input_spec):
         pass
 
@@ -204,16 +204,15 @@
 
     def test_are_outputs_up_to_date(self):
         test_step = StepWithSupportForCopy(self._pipeline, "test_step")
         self.assertFalse(are_outputs_up_to_date(test_step))
 
         for localize_by in (
                 Localize.GSUTIL_COPY,
-                Localize.HAIL_BATCH_GCSFUSE,
-                Localize.HAIL_BATCH_GCSFUSE_VIA_TEMP_BUCKET):
+                Localize.HAIL_BATCH_CLOUDFUSE_VIA_TEMP_BUCKET):
             self.assertRaisesRegex(ValueError, "doesn't start with gs://", test_step.input,
                 "some_file.txt", localize_by=localize_by)
 
 
         # test missing input path
         test_step = StepWithSupportForCopy(self._pipeline, "test_step")
         test_step.input("gs://missing-bucket/test", localize_by=Localize.COPY)
```

