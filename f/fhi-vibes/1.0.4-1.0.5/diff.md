# Comparing `tmp/fhi-vibes-1.0.4.tar.gz` & `tmp/fhi-vibes-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhi-vibes-1.0.4.tar", max compression
+gzip compressed data, was "fhi-vibes-1.0.5.tar", max compression
```

## Comparing `fhi-vibes-1.0.4.tar` & `fhi-vibes-1.0.5.tar`

### file list

```diff
@@ -1,217 +1,216 @@
--rw-r--r--   0        0        0     1131 2022-08-16 07:15:02.365235 fhi-vibes-1.0.4/LICENSE
--rw-r--r--   0        0        0     3156 2022-08-16 09:33:43.871165 fhi-vibes-1.0.4/README.md
--rw-r--r--   0        0        0      452 2021-08-26 08:25:19.128640 fhi-vibes-1.0.4/build.py
--rw-r--r--   0        0        0     2088 2022-08-16 09:33:43.872435 fhi-vibes-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      338 2021-08-26 08:25:19.187214 fhi-vibes-1.0.4/vibes/__init__.py
--rw-r--r--   0        0        0      398 2021-08-26 08:25:19.187272 fhi-vibes-1.0.4/vibes/_defaults.py
--rw-r--r--   0        0        0     8331 2022-08-16 07:15:02.367954 fhi-vibes-1.0.4/vibes/anharmonicity_score.py
--rw-r--r--   0        0        0       46 2021-08-26 08:25:19.187436 fhi-vibes-1.0.4/vibes/ase/__init__.py
--rw-r--r--   0        0        0     3391 2022-08-16 07:15:02.368075 fhi-vibes-1.0.4/vibes/ase/calculators/fc.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.187565 fhi-vibes-1.0.4/vibes/ase/db/__init__.py
--rw-r--r--   0        0        0     2851 2021-08-26 08:25:19.187634 fhi-vibes-1.0.4/vibes/ase/db/dict_converters.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.187681 fhi-vibes-1.0.4/vibes/ase/md/__init__.py
--rw-r--r--   0        0        0     6085 2022-02-15 12:44:19.081232 fhi-vibes-1.0.4/vibes/ase/md/velocitydistribution.py
--rw-r--r--   0        0        0     7829 2021-12-06 13:19:16.099860 fhi-vibes-1.0.4/vibes/calculate.py
--rw-r--r--   0        0        0      130 2021-08-26 08:25:19.187939 fhi-vibes-1.0.4/vibes/calculator/__init__.py
--rw-r--r--   0        0        0      251 2021-08-26 08:25:19.188000 fhi-vibes-1.0.4/vibes/calculator/_defaults.py
--rw-r--r--   0        0        0     6936 2022-08-16 07:15:02.368210 fhi-vibes-1.0.4/vibes/calculator/aims.py
--rw-r--r--   0        0        0     3636 2021-08-26 08:25:19.188145 fhi-vibes-1.0.4/vibes/calculator/context.py
--rw-r--r--   0        0        0      880 2021-08-26 08:25:19.188195 fhi-vibes-1.0.4/vibes/calculator/setup.py
--rw-r--r--   0        0        0     2378 2022-06-25 16:27:33.163807 fhi-vibes-1.0.4/vibes/calculator/workflow.py
--rw-r--r--   0        0        0     2263 2021-08-26 08:25:19.188329 fhi-vibes-1.0.4/vibes/cli/__init__.py
--rw-r--r--   0        0        0      118 2021-08-26 08:25:19.188379 fhi-vibes-1.0.4/vibes/cli/cli_tracker.py
--rw-r--r--   0        0        0    14117 2022-08-16 07:15:02.368374 fhi-vibes-1.0.4/vibes/cli/info.py
--rw-r--r--   0        0        0     1677 2021-08-26 08:25:19.188520 fhi-vibes-1.0.4/vibes/cli/misc.py
--rw-r--r--   0        0        0     6454 2022-08-16 07:15:02.368518 fhi-vibes-1.0.4/vibes/cli/output.py
--rw-r--r--   0        0        0     3410 2021-08-26 08:25:19.188648 fhi-vibes-1.0.4/vibes/cli/run.py
--rw-r--r--   0        0        0       48 2021-08-26 08:25:19.188723 fhi-vibes-1.0.4/vibes/cli/scripts/__init__.py
--rwxr-xr-x   0        0        0     6386 2022-08-16 07:15:02.368823 fhi-vibes-1.0.4/vibes/cli/scripts/create_samples.py
--rw-r--r--   0        0        0     1387 2022-06-25 16:27:33.164500 fhi-vibes-1.0.4/vibes/cli/scripts/create_trajectory.py
--rwxr-xr-x   0        0        0      905 2022-08-16 07:15:02.368943 fhi-vibes-1.0.4/vibes/cli/scripts/geometry_info.py
--rwxr-xr-x   0        0        0     7558 2021-08-26 08:25:19.188996 fhi-vibes-1.0.4/vibes/cli/scripts/get_relaxation_info.py
--rw-r--r--   0        0        0      545 2022-06-25 16:27:33.165389 fhi-vibes-1.0.4/vibes/cli/scripts/hilde_run.py
--rwxr-xr-x   0        0        0     4166 2022-08-16 07:15:02.369232 fhi-vibes-1.0.4/vibes/cli/scripts/make_supercell.py
--rw-r--r--   0        0        0     5712 2022-06-25 16:27:33.165851 fhi-vibes-1.0.4/vibes/cli/scripts/md_sum.py
--rwxr-xr-x   0        0        0     4697 2022-08-16 07:15:02.369366 fhi-vibes-1.0.4/vibes/cli/scripts/refine_geometry.py
--rw-r--r--   0        0        0     1206 2021-08-26 08:25:19.189305 fhi-vibes-1.0.4/vibes/cli/scripts/remap_phonopy_forceconstants.py
--rwxr-xr-x   0        0        0     1120 2022-06-25 16:27:33.166880 fhi-vibes-1.0.4/vibes/cli/scripts/rewrite_geometry.py
--rw-r--r--   0        0        0      118 2021-08-26 08:25:19.189444 fhi-vibes-1.0.4/vibes/cli/scripts/run/md.py
--rw-r--r--   0        0        0       88 2021-08-26 08:25:19.189498 fhi-vibes-1.0.4/vibes/cli/scripts/run/phono3py.py
--rw-r--r--   0        0        0      102 2021-08-26 08:25:19.189548 fhi-vibes-1.0.4/vibes/cli/scripts/run/relaxation.py
--rw-r--r--   0        0        0      716 2021-08-26 08:25:19.189601 fhi-vibes-1.0.4/vibes/cli/scripts/run_thermal_conductivity.py
--rwxr-xr-x   0        0        0     1561 2022-06-25 16:27:33.167247 fhi-vibes-1.0.4/vibes/cli/scripts/suggest_k_grid.py
--rw-r--r--   0        0        0      555 2022-06-25 16:27:33.167534 fhi-vibes-1.0.4/vibes/cli/scripts/trajectory2tdep.py
--rw-r--r--   0        0        0      544 2022-06-25 16:27:33.167752 fhi-vibes-1.0.4/vibes/cli/scripts/trajectory2xyz.py
--rw-r--r--   0        0        0     1326 2022-06-25 16:27:33.168215 fhi-vibes-1.0.4/vibes/cli/scripts/update_md_trajectory.py
--rw-r--r--   0        0        0     4034 2022-06-25 16:27:33.168479 fhi-vibes-1.0.4/vibes/cli/scripts/vibes_phonopy.py
--rw-r--r--   0        0        0      803 2022-06-25 16:27:33.168702 fhi-vibes-1.0.4/vibes/cli/scripts/yaml2json.py
--rw-r--r--   0        0        0     1981 2021-08-26 08:25:19.189984 fhi-vibes-1.0.4/vibes/cli/submit.py
--rw-r--r--   0        0        0     2445 2021-08-26 08:25:19.190063 fhi-vibes-1.0.4/vibes/cli/template.py
--rw-r--r--   0        0        0    22340 2022-08-16 07:15:02.369557 fhi-vibes-1.0.4/vibes/cli/utils.py
--rw-r--r--   0        0        0     2927 2021-08-26 08:25:19.190274 fhi-vibes-1.0.4/vibes/context.py
--rw-r--r--   0        0        0     9053 2022-08-16 07:15:02.369906 fhi-vibes-1.0.4/vibes/correlation.py
--rw-r--r--   0        0        0      232 2022-08-16 07:15:02.370013 fhi-vibes-1.0.4/vibes/defaults.py
--rw-r--r--   0        0        0      524 2022-08-16 07:15:02.370125 fhi-vibes-1.0.4/vibes/dimensions.py
--rw-r--r--   0        0        0     1208 2022-08-16 07:15:02.370232 fhi-vibes-1.0.4/vibes/filenames.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.190594 fhi-vibes-1.0.4/vibes/fireworks/__init__.py
--rw-r--r--   0        0        0     1113 2021-08-26 08:25:19.190660 fhi-vibes-1.0.4/vibes/fireworks/_defaults.py
--rw-r--r--   0        0        0    23373 2022-04-19 07:43:02.276453 fhi-vibes-1.0.4/vibes/fireworks/cli/__init__.py
--rw-r--r--   0        0        0     6679 2021-08-26 08:25:19.190872 fhi-vibes-1.0.4/vibes/fireworks/cli/launch_utils.py
--rw-r--r--   0        0        0    15063 2021-08-26 08:25:19.191058 fhi-vibes-1.0.4/vibes/fireworks/combined_launcher.py
--rw-r--r--   0        0        0     3944 2021-12-23 12:08:02.437374 fhi-vibes-1.0.4/vibes/fireworks/launchpad.py
--rw-r--r--   0        0        0     7007 2021-08-26 08:25:19.191194 fhi-vibes-1.0.4/vibes/fireworks/qlaunch_remote.py
--rw-r--r--   0        0        0    23072 2022-06-25 16:27:33.171698 fhi-vibes-1.0.4/vibes/fireworks/queue_launcher.py
--rw-r--r--   0        0        0     6533 2021-08-26 08:25:19.191351 fhi-vibes-1.0.4/vibes/fireworks/rocket_launcher.py
--rw-r--r--   0        0        0       86 2021-08-26 08:25:19.191434 fhi-vibes-1.0.4/vibes/fireworks/tasks/__init__.py
--rw-r--r--   0        0        0     5998 2021-08-26 08:25:19.191510 fhi-vibes-1.0.4/vibes/fireworks/tasks/calculate_wrapper.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.191560 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/__init__.py
--rw-r--r--   0        0        0     3896 2022-04-19 07:43:02.276656 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/aims.py
--rw-r--r--   0        0        0     4183 2021-08-26 08:25:19.191719 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/calculate.py
--rw-r--r--   0        0        0     5283 2022-04-19 07:43:02.276757 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/check_conditionals.py
--rw-r--r--   0        0        0     2431 2021-08-26 08:25:19.191785 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/general.py
--rw-r--r--   0        0        0     1891 2022-04-19 07:43:02.276905 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/md.py
--rw-r--r--   0        0        0     2375 2021-08-26 08:25:19.191911 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/optimizations.py
--rw-r--r--   0        0        0    17406 2022-08-16 07:15:02.370437 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/phonons.py
--rw-r--r--   0        0        0     3270 2022-04-19 07:43:02.277335 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/relaxation.py
--rw-r--r--   0        0        0     2057 2022-08-16 07:15:02.370578 fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/statistical_sampling.py
--rw-r--r--   0        0        0     4865 2021-08-26 08:25:19.192224 fhi-vibes-1.0.4/vibes/fireworks/tasks/general_py_task.py
--rw-r--r--   0        0        0     6131 2022-08-16 07:15:02.370846 fhi-vibes-1.0.4/vibes/fireworks/tasks/md.py
--rw-r--r--   0        0        0    13514 2022-08-16 07:15:02.371011 fhi-vibes-1.0.4/vibes/fireworks/tasks/phonopy_phono3py_functions.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.192423 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/__init__.py
--rw-r--r--   0        0        0     3309 2022-04-19 07:43:02.278026 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/aims.py
--rw-r--r--   0        0        0     1197 2021-08-26 08:25:19.192546 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/calculate.py
--rw-r--r--   0        0        0      274 2021-08-26 08:25:19.192605 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/md.py
--rw-r--r--   0        0        0     1916 2021-08-26 08:25:19.192654 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/optimizations.py
--rw-r--r--   0        0        0    11937 2022-08-16 07:15:02.371161 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/phonons.py
--rw-r--r--   0        0        0      399 2021-08-26 08:25:19.192789 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/relaxation.py
--rw-r--r--   0        0        0     1673 2022-08-16 07:15:02.371273 fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/statistical_sampling.py
--rw-r--r--   0        0        0     2616 2021-08-26 08:25:19.192909 fhi-vibes-1.0.4/vibes/fireworks/tasks/relaxation.py
--rw-r--r--   0        0        0     7956 2022-08-16 07:15:02.371557 fhi-vibes-1.0.4/vibes/fireworks/tasks/statistical_sampling_wrappers.py
--rw-r--r--   0        0        0     3727 2021-08-26 08:25:19.193042 fhi-vibes-1.0.4/vibes/fireworks/tasks/task_spec.py
--rw-r--r--   0        0        0     3610 2021-08-26 08:25:19.193104 fhi-vibes-1.0.4/vibes/fireworks/tasks/utility_tasks.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.193160 fhi-vibes-1.0.4/vibes/fireworks/utils/__init__.py
--rw-r--r--   0        0        0     5512 2021-08-26 08:25:19.193245 fhi-vibes-1.0.4/vibes/fireworks/utils/converters.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.193302 fhi-vibes-1.0.4/vibes/fireworks/workflows/__init__.py
--rw-r--r--   0        0        0    29066 2022-04-19 07:43:02.278988 fhi-vibes-1.0.4/vibes/fireworks/workflows/firework_generator.py
--rw-r--r--   0        0        0     4692 2021-08-26 08:25:19.193511 fhi-vibes-1.0.4/vibes/fireworks/workflows/task_generator.py
--rw-r--r--   0        0        0    13867 2021-08-26 08:25:19.193611 fhi-vibes-1.0.4/vibes/fireworks/workflows/task_spec_generator.py
--rw-r--r--   0        0        0     9866 2022-04-19 07:43:02.279189 fhi-vibes-1.0.4/vibes/fireworks/workflows/workflow_generator.py
--rw-r--r--   0        0        0     5447 2022-08-16 07:15:02.371856 fhi-vibes-1.0.4/vibes/fourier.py
--rw-r--r--   0        0        0      221 2022-08-16 07:15:02.372129 fhi-vibes-1.0.4/vibes/green_kubo/README.md
--rw-r--r--   0        0        0     8604 2022-08-16 07:15:02.372278 fhi-vibes-1.0.4/vibes/green_kubo/__init__.py
--rw-r--r--   0        0        0     2997 2021-08-26 08:25:19.194010 fhi-vibes-1.0.4/vibes/green_kubo/analysis.snippets
--rw-r--r--   0        0        0     2799 2022-08-16 07:15:02.372404 fhi-vibes-1.0.4/vibes/green_kubo/velocities.py
--rw-r--r--   0        0        0      337 2022-08-16 07:15:02.372486 fhi-vibes-1.0.4/vibes/harmonic_analysis/__init__.py
--rw-r--r--   0        0        0     3791 2022-08-16 07:15:02.372573 fhi-vibes-1.0.4/vibes/harmonic_analysis/dynamical_matrix.py
--rw-r--r--   0        0        0     2229 2022-08-16 07:15:02.372649 fhi-vibes-1.0.4/vibes/harmonic_analysis/force_constants.py
--rw-r--r--   0        0        0    17557 2022-08-16 07:15:02.372821 fhi-vibes-1.0.4/vibes/harmonic_analysis/mode_projection.py
--rw-r--r--   0        0        0     8092 2022-08-16 07:15:02.372931 fhi-vibes-1.0.4/vibes/harmonic_analysis/normal_modes.py
--rw-r--r--   0        0        0     3110 2022-08-16 07:15:02.373009 fhi-vibes-1.0.4/vibes/harmonic_analysis/spectral_energy_density.py
--rw-r--r--   0        0        0      236 2021-08-26 08:25:19.194577 fhi-vibes-1.0.4/vibes/helpers/__init__.py
--rw-r--r--   0        0        0     1097 2021-08-26 08:25:19.194636 fhi-vibes-1.0.4/vibes/helpers/aims.py
--rw-r--r--   0        0        0     3294 2021-08-26 08:25:19.194689 fhi-vibes-1.0.4/vibes/helpers/backup.py
--rw-r--r--   0        0        0     3679 2022-08-16 07:15:02.373127 fhi-vibes-1.0.4/vibes/helpers/brillouinzone.py
--rw-r--r--   0        0        0    14649 2022-06-25 16:27:33.172767 fhi-vibes-1.0.4/vibes/helpers/converters.py
--rw-r--r--   0        0        0     1608 2022-06-25 16:27:33.173258 fhi-vibes-1.0.4/vibes/helpers/dict.py
--rw-r--r--   0        0        0     1781 2022-06-25 16:27:33.173613 fhi-vibes-1.0.4/vibes/helpers/displacements.py
--rw-r--r--   0        0        0       69 2021-08-26 08:25:19.194980 fhi-vibes-1.0.4/vibes/helpers/fileformats.py
--rw-r--r--   0        0        0     2375 2022-08-16 07:15:02.373256 fhi-vibes-1.0.4/vibes/helpers/filter.py
--rw-r--r--   0        0        0     3378 2022-08-16 07:15:02.373405 fhi-vibes-1.0.4/vibes/helpers/geometry.py
--rw-r--r--   0        0        0     4409 2021-08-26 08:25:19.195159 fhi-vibes-1.0.4/vibes/helpers/hash.py
--rw-r--r--   0        0        0     3900 2022-08-16 07:15:02.373541 fhi-vibes-1.0.4/vibes/helpers/k_grid.py
--rw-r--r--   0        0        0      380 2021-08-26 08:25:19.195280 fhi-vibes-1.0.4/vibes/helpers/latex.py
--rw-r--r--   0        0        0      495 2022-06-25 16:27:33.173897 fhi-vibes-1.0.4/vibes/helpers/lattice.py
--rw-r--r--   0        0        0     4919 2022-08-16 07:15:02.373753 fhi-vibes-1.0.4/vibes/helpers/lattice_points.py
--rw-r--r--   0        0        0      905 2021-08-26 08:25:19.195507 fhi-vibes-1.0.4/vibes/helpers/lists.py
--rw-r--r--   0        0        0      536 2021-08-26 08:25:19.195578 fhi-vibes-1.0.4/vibes/helpers/notifications.py
--rw-r--r--   0        0        0     1407 2021-08-26 08:25:19.195639 fhi-vibes-1.0.4/vibes/helpers/numerics.py
--rw-r--r--   0        0        0     2641 2021-08-26 08:25:19.195698 fhi-vibes-1.0.4/vibes/helpers/paths.py
--rw-r--r--   0        0        0     1016 2021-08-26 08:25:19.195771 fhi-vibes-1.0.4/vibes/helpers/pickle.py
--rw-r--r--   0        0        0      292 2022-08-16 07:15:02.373860 fhi-vibes-1.0.4/vibes/helpers/plotting.py
--rw-r--r--   0        0        0      580 2021-08-26 08:25:19.195906 fhi-vibes-1.0.4/vibes/helpers/properties.py
--rw-r--r--   0        0        0     1220 2022-06-25 16:27:33.174636 fhi-vibes-1.0.4/vibes/helpers/restarts.py
--rw-r--r--   0        0        0     4553 2021-08-26 08:25:19.196070 fhi-vibes-1.0.4/vibes/helpers/socketio.py
--rw-r--r--   0        0        0      758 2021-08-26 08:25:19.196141 fhi-vibes-1.0.4/vibes/helpers/stress.py
--rw-r--r--   0        0        0     2125 2021-08-26 08:25:19.196207 fhi-vibes-1.0.4/vibes/helpers/stresses.py
--rw-r--r--   0        0        0      523 2021-08-26 08:25:19.196263 fhi-vibes-1.0.4/vibes/helpers/structure.py
--rw-r--r--   0        0        0      224 2021-08-26 08:25:19.196363 fhi-vibes-1.0.4/vibes/helpers/supercell/Makefile
--rw-r--r--   0        0        0    11122 2022-08-16 07:15:02.374024 fhi-vibes-1.0.4/vibes/helpers/supercell/__init__.py
--rw-r--r--   0        0        0     1838 2022-08-16 07:15:02.374144 fhi-vibes-1.0.4/vibes/helpers/supercell/linalg.f90
--rw-r--r--   0        0        0    13980 2022-08-12 09:06:12.043207 fhi-vibes-1.0.4/vibes/helpers/supercell/make.log
--rw-r--r--   0        0        0      339 2021-08-26 08:25:19.196582 fhi-vibes-1.0.4/vibes/helpers/supercell/setup.py
--rw-r--r--   0        0        0     9307 2022-08-16 07:15:02.374362 fhi-vibes-1.0.4/vibes/helpers/supercell/supercell.f90
--rw-r--r--   0        0        0     7786 2022-08-16 07:15:02.374493 fhi-vibes-1.0.4/vibes/helpers/utils.py
--rw-r--r--   0        0        0     1624 2021-08-26 08:25:19.196804 fhi-vibes-1.0.4/vibes/helpers/virials.py
--rw-r--r--   0        0        0      935 2021-08-26 08:25:19.196860 fhi-vibes-1.0.4/vibes/helpers/warnings.py
--rw-r--r--   0        0        0     7697 2021-08-26 08:25:19.196945 fhi-vibes-1.0.4/vibes/helpers/watchdogs.py
--rw-r--r--   0        0        0      806 2021-08-26 08:25:19.197003 fhi-vibes-1.0.4/vibes/helpers/xarray.py
--rw-r--r--   0        0        0     2976 2022-08-16 07:15:02.374637 fhi-vibes-1.0.4/vibes/hiphive/__init__.py
--rw-r--r--   0        0        0     1989 2022-08-16 07:15:02.374825 fhi-vibes-1.0.4/vibes/integrate.py
--rw-r--r--   0        0        0     3572 2022-08-16 07:15:02.375130 fhi-vibes-1.0.4/vibes/io.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.197346 fhi-vibes-1.0.4/vibes/k_grid/__init__.py
--rw-r--r--   0        0        0     3579 2021-08-26 08:25:19.197434 fhi-vibes-1.0.4/vibes/k_grid/converge_kgrid.py
--rw-r--r--   0        0        0     3859 2022-06-25 16:27:33.175963 fhi-vibes-1.0.4/vibes/k_grid/kpointoptimizer.py
--rw-r--r--   0        0        0     3727 2022-08-16 07:15:02.375289 fhi-vibes-1.0.4/vibes/keys.py
--rw-r--r--   0        0        0      263 2022-08-16 07:15:02.375413 fhi-vibes-1.0.4/vibes/konstanten/__init__.py
--rw-r--r--   0        0        0     5417 2021-08-26 08:25:19.197749 fhi-vibes-1.0.4/vibes/konstanten/atomic_masses.py
--rw-r--r--   0        0        0     2044 2022-08-16 07:15:02.375502 fhi-vibes-1.0.4/vibes/konstanten/einheiten.py
--rw-r--r--   0        0        0      137 2021-08-26 08:25:19.197867 fhi-vibes-1.0.4/vibes/konstanten/numerics.py
--rw-r--r--   0        0        0       66 2021-08-26 08:25:19.197949 fhi-vibes-1.0.4/vibes/materials_fp/__init__.py
--rw-r--r--   0        0        0     6362 2021-08-26 08:25:19.198085 fhi-vibes-1.0.4/vibes/materials_fp/material_fingerprint.py
--rw-r--r--   0        0        0       69 2021-08-26 08:25:19.198175 fhi-vibes-1.0.4/vibes/molecular_dynamics/__init__.py
--rw-r--r--   0        0        0     1572 2021-08-26 08:25:19.198228 fhi-vibes-1.0.4/vibes/molecular_dynamics/_defaults.py
--rw-r--r--   0        0        0     6893 2021-08-26 08:25:19.198292 fhi-vibes-1.0.4/vibes/molecular_dynamics/context.py
--rw-r--r--   0        0        0     2100 2022-06-25 16:27:33.176382 fhi-vibes-1.0.4/vibes/molecular_dynamics/utils.py
--rw-r--r--   0        0        0     9194 2022-06-25 16:27:33.176797 fhi-vibes-1.0.4/vibes/molecular_dynamics/workflow.py
--rw-r--r--   0        0        0      127 2021-08-26 08:25:19.198510 fhi-vibes-1.0.4/vibes/phono3py/__init__.py
--rw-r--r--   0        0        0      637 2021-08-26 08:25:19.198557 fhi-vibes-1.0.4/vibes/phono3py/_defaults.py
--rw-r--r--   0        0        0      506 2021-08-26 08:25:19.198614 fhi-vibes-1.0.4/vibes/phono3py/context.py
--rw-r--r--   0        0        0     4026 2022-08-16 07:15:02.375846 fhi-vibes-1.0.4/vibes/phono3py/postprocess.py
--rw-r--r--   0        0        0     3856 2022-08-16 08:15:22.329677 fhi-vibes-1.0.4/vibes/phono3py/wrapper.py
--rw-r--r--   0        0        0      357 2021-08-26 08:25:19.198803 fhi-vibes-1.0.4/vibes/phonopy/__init__.py
--rw-r--r--   0        0        0      792 2021-08-26 08:25:19.198851 fhi-vibes-1.0.4/vibes/phonopy/_defaults.py
--rw-r--r--   0        0        0     3609 2022-08-16 09:33:43.872877 fhi-vibes-1.0.4/vibes/phonopy/context.py
--rw-r--r--   0        0        0    10917 2022-08-16 07:15:02.376596 fhi-vibes-1.0.4/vibes/phonopy/postprocess.py
--rw-r--r--   0        0        0    14149 2022-08-16 07:15:02.376922 fhi-vibes-1.0.4/vibes/phonopy/utils.py
--rw-r--r--   0        0        0     2888 2022-06-25 16:27:33.178427 fhi-vibes-1.0.4/vibes/phonopy/workflow.py
--rw-r--r--   0        0        0    14476 2022-08-16 09:33:43.873180 fhi-vibes-1.0.4/vibes/phonopy/wrapper.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.199242 fhi-vibes-1.0.4/vibes/relaxation/__init__.py
--rw-r--r--   0        0        0     1233 2021-08-26 08:25:19.199300 fhi-vibes-1.0.4/vibes/relaxation/_defaults.py
--rw-r--r--   0        0        0     5264 2021-08-26 08:25:19.199366 fhi-vibes-1.0.4/vibes/relaxation/context.py
--rw-r--r--   0        0        0     4092 2022-08-16 07:15:02.377497 fhi-vibes-1.0.4/vibes/relaxation/workflow.py
--rw-r--r--   0        0        0     6654 2022-06-25 16:27:33.179291 fhi-vibes-1.0.4/vibes/settings.py
--rw-r--r--   0        0        0      335 2021-08-26 08:25:19.199622 fhi-vibes-1.0.4/vibes/slurm/README.md
--rw-r--r--   0        0        0      135 2021-08-26 08:25:19.199666 fhi-vibes-1.0.4/vibes/slurm/__init__.py
--rw-r--r--   0        0        0      758 2021-08-26 08:25:19.199717 fhi-vibes-1.0.4/vibes/slurm/generate.py
--rw-r--r--   0        0        0      577 2021-08-26 08:25:19.199766 fhi-vibes-1.0.4/vibes/slurm/render.py
--rw-r--r--   0        0        0     1329 2021-08-26 08:25:19.199830 fhi-vibes-1.0.4/vibes/slurm/submit.py
--rw-r--r--   0        0        0      903 2021-08-26 08:25:19.199876 fhi-vibes-1.0.4/vibes/son.py
--rw-r--r--   0        0        0       35 2022-08-16 07:15:02.377570 fhi-vibes-1.0.4/vibes/spglib/__init__.py
--rw-r--r--   0        0        0     4966 2022-08-16 07:15:02.377672 fhi-vibes-1.0.4/vibes/spglib/q_mesh.py
--rw-r--r--   0        0        0     4192 2022-08-16 07:15:02.377756 fhi-vibes-1.0.4/vibes/spglib/wrapper.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.200111 fhi-vibes-1.0.4/vibes/structure/__init__.py
--rw-r--r--   0        0        0     2041 2021-08-26 08:25:19.200173 fhi-vibes-1.0.4/vibes/structure/convert.py
--rw-r--r--   0        0        0     7053 2022-08-16 07:15:02.377933 fhi-vibes-1.0.4/vibes/structure/io.py
--rw-r--r--   0        0        0     3400 2021-08-26 08:25:19.200314 fhi-vibes-1.0.4/vibes/structure/misc.py
--rw-r--r--   0        0        0       48 2021-08-26 08:25:19.200379 fhi-vibes-1.0.4/vibes/tdep/__init__.py
--rw-r--r--   0        0        0    11219 2022-08-16 07:15:02.378253 fhi-vibes-1.0.4/vibes/tdep/wrapper.py
--rw-r--r--   0        0        0       35 2021-08-26 08:25:19.200536 fhi-vibes-1.0.4/vibes/templates/__init__.py
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.200589 fhi-vibes-1.0.4/vibes/templates/config_files/__init__.py
--rw-r--r--   0        0        0      592 2021-08-26 08:25:19.200646 fhi-vibes-1.0.4/vibes/templates/config_files/fireworksrc.template
--rw-r--r--   0        0        0      165 2021-08-26 08:25:19.200700 fhi-vibes-1.0.4/vibes/templates/config_files/slurm.in
--rw-r--r--   0        0        0      391 2021-08-26 08:25:19.200746 fhi-vibes-1.0.4/vibes/templates/config_files/vibesrc.template
--rw-r--r--   0        0        0        0 2021-08-26 08:25:19.200799 fhi-vibes-1.0.4/vibes/templates/settings/__init__.py
--rw-r--r--   0        0        0      341 2022-08-16 07:15:02.378373 fhi-vibes-1.0.4/vibes/templates/settings/aims
--rw-r--r--   0        0        0      754 2021-08-26 08:25:19.200910 fhi-vibes-1.0.4/vibes/templates/settings/aims_full
--rw-r--r--   0        0        0      201 2021-08-26 08:25:19.200956 fhi-vibes-1.0.4/vibes/templates/settings/lj
--rw-r--r--   0        0        0      920 2021-08-26 08:25:19.201037 fhi-vibes-1.0.4/vibes/trajectory/README.md
--rw-r--r--   0        0        0      361 2021-08-26 08:25:19.201091 fhi-vibes-1.0.4/vibes/trajectory/__init__.py
--rw-r--r--   0        0        0     5096 2022-08-16 07:15:02.378514 fhi-vibes-1.0.4/vibes/trajectory/analysis.py
--rw-r--r--   0        0        0     6961 2022-08-16 07:15:02.378655 fhi-vibes-1.0.4/vibes/trajectory/dataset.py
--rw-r--r--   0        0        0     1567 2022-08-16 07:15:02.378733 fhi-vibes-1.0.4/vibes/trajectory/heat_flux.py
--rw-r--r--   0        0        0    13345 2022-08-16 07:15:02.378898 fhi-vibes-1.0.4/vibes/trajectory/io.py
--rw-r--r--   0        0        0     4669 2022-08-16 07:15:02.379043 fhi-vibes-1.0.4/vibes/trajectory/plotting.py
--rw-r--r--   0        0        0    24034 2022-08-16 07:15:02.379404 fhi-vibes-1.0.4/vibes/trajectory/trajectory.py
--rw-r--r--   0        0        0      873 2021-08-26 08:25:19.201618 fhi-vibes-1.0.4/vibes/trajectory/utils.py
--rw-r--r--   0        0        0     5756 2022-08-16 10:19:22.459626 fhi-vibes-1.0.4/setup.py
--rw-r--r--   0        0        0     5326 2022-08-16 10:19:22.460073 fhi-vibes-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-05-31 13:59:33.297455 fhi-vibes-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3165 2023-06-01 08:06:13.273085 fhi-vibes-1.0.5/README.md
+-rw-r--r--   0        0        0      452 2023-05-31 13:59:33.297578 fhi-vibes-1.0.5/build.py
+-rw-r--r--   0        0        0     2090 2023-06-01 08:05:41.517123 fhi-vibes-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      338 2023-05-31 13:59:33.346646 fhi-vibes-1.0.5/vibes/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-31 13:59:33.346697 fhi-vibes-1.0.5/vibes/_defaults.py
+-rw-r--r--   0        0        0     8331 2023-05-31 13:59:33.346799 fhi-vibes-1.0.5/vibes/anharmonicity_score.py
+-rw-r--r--   0        0        0       46 2023-05-31 13:59:33.346897 fhi-vibes-1.0.5/vibes/ase/__init__.py
+-rw-r--r--   0        0        0     3391 2023-05-31 13:59:33.346997 fhi-vibes-1.0.5/vibes/ase/calculators/fc.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.347051 fhi-vibes-1.0.5/vibes/ase/db/__init__.py
+-rw-r--r--   0        0        0     2851 2023-05-31 13:59:33.347117 fhi-vibes-1.0.5/vibes/ase/db/dict_converters.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.347177 fhi-vibes-1.0.5/vibes/ase/md/__init__.py
+-rw-r--r--   0        0        0     6085 2023-05-31 13:59:33.347291 fhi-vibes-1.0.5/vibes/ase/md/velocitydistribution.py
+-rw-r--r--   0        0        0     7829 2023-05-31 13:59:33.347391 fhi-vibes-1.0.5/vibes/calculate.py
+-rw-r--r--   0        0        0      130 2023-05-31 13:59:33.347471 fhi-vibes-1.0.5/vibes/calculator/__init__.py
+-rw-r--r--   0        0        0      251 2023-05-31 13:59:33.347540 fhi-vibes-1.0.5/vibes/calculator/_defaults.py
+-rw-r--r--   0        0        0     6936 2023-05-31 13:59:33.347615 fhi-vibes-1.0.5/vibes/calculator/aims.py
+-rw-r--r--   0        0        0     3636 2023-05-31 13:59:33.347689 fhi-vibes-1.0.5/vibes/calculator/context.py
+-rw-r--r--   0        0        0      880 2023-05-31 13:59:33.347747 fhi-vibes-1.0.5/vibes/calculator/setup.py
+-rw-r--r--   0        0        0     2378 2023-05-31 13:59:33.347824 fhi-vibes-1.0.5/vibes/calculator/workflow.py
+-rw-r--r--   0        0        0     2263 2023-05-31 13:59:33.347916 fhi-vibes-1.0.5/vibes/cli/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-31 13:59:33.347972 fhi-vibes-1.0.5/vibes/cli/cli_tracker.py
+-rw-r--r--   0        0        0    14117 2023-05-31 13:59:33.348059 fhi-vibes-1.0.5/vibes/cli/info.py
+-rw-r--r--   0        0        0     1677 2023-05-31 13:59:33.348127 fhi-vibes-1.0.5/vibes/cli/misc.py
+-rw-r--r--   0        0        0     6454 2023-05-31 13:59:33.348245 fhi-vibes-1.0.5/vibes/cli/output.py
+-rw-r--r--   0        0        0     3410 2023-05-31 13:59:33.348306 fhi-vibes-1.0.5/vibes/cli/run.py
+-rw-r--r--   0        0        0       48 2023-05-31 13:59:33.348383 fhi-vibes-1.0.5/vibes/cli/scripts/__init__.py
+-rwxr-xr-x   0        0        0     6386 2023-05-31 13:59:33.348486 fhi-vibes-1.0.5/vibes/cli/scripts/create_samples.py
+-rw-r--r--   0        0        0     1387 2023-05-31 13:59:33.348541 fhi-vibes-1.0.5/vibes/cli/scripts/create_trajectory.py
+-rwxr-xr-x   0        0        0      905 2023-05-31 13:59:33.348605 fhi-vibes-1.0.5/vibes/cli/scripts/geometry_info.py
+-rwxr-xr-x   0        0        0     7558 2023-05-31 13:59:33.348681 fhi-vibes-1.0.5/vibes/cli/scripts/get_relaxation_info.py
+-rw-r--r--   0        0        0      545 2023-05-31 13:59:33.348746 fhi-vibes-1.0.5/vibes/cli/scripts/hilde_run.py
+-rwxr-xr-x   0        0        0     4166 2023-05-31 13:59:33.348818 fhi-vibes-1.0.5/vibes/cli/scripts/make_supercell.py
+-rw-r--r--   0        0        0     5712 2023-05-31 13:59:33.348888 fhi-vibes-1.0.5/vibes/cli/scripts/md_sum.py
+-rwxr-xr-x   0        0        0     4697 2023-05-31 13:59:33.348957 fhi-vibes-1.0.5/vibes/cli/scripts/refine_geometry.py
+-rw-r--r--   0        0        0     1206 2023-05-31 13:59:33.349033 fhi-vibes-1.0.5/vibes/cli/scripts/remap_phonopy_forceconstants.py
+-rwxr-xr-x   0        0        0     1120 2023-05-31 13:59:33.349089 fhi-vibes-1.0.5/vibes/cli/scripts/rewrite_geometry.py
+-rw-r--r--   0        0        0      118 2023-05-31 13:59:33.349166 fhi-vibes-1.0.5/vibes/cli/scripts/run/md.py
+-rw-r--r--   0        0        0       88 2023-05-31 13:59:33.349216 fhi-vibes-1.0.5/vibes/cli/scripts/run/phono3py.py
+-rw-r--r--   0        0        0      102 2023-05-31 13:59:33.349273 fhi-vibes-1.0.5/vibes/cli/scripts/run/relaxation.py
+-rw-r--r--   0        0        0      716 2023-05-31 13:59:33.349331 fhi-vibes-1.0.5/vibes/cli/scripts/run_thermal_conductivity.py
+-rwxr-xr-x   0        0        0     1561 2023-05-31 13:59:33.349389 fhi-vibes-1.0.5/vibes/cli/scripts/suggest_k_grid.py
+-rw-r--r--   0        0        0      555 2023-05-31 13:59:33.349446 fhi-vibes-1.0.5/vibes/cli/scripts/trajectory2tdep.py
+-rw-r--r--   0        0        0      544 2023-05-31 13:59:33.349510 fhi-vibes-1.0.5/vibes/cli/scripts/trajectory2xyz.py
+-rw-r--r--   0        0        0     1326 2023-05-31 13:59:33.349563 fhi-vibes-1.0.5/vibes/cli/scripts/update_md_trajectory.py
+-rw-r--r--   0        0        0     4034 2023-05-31 13:59:33.349628 fhi-vibes-1.0.5/vibes/cli/scripts/vibes_phonopy.py
+-rw-r--r--   0        0        0      803 2023-05-31 13:59:33.349682 fhi-vibes-1.0.5/vibes/cli/scripts/yaml2json.py
+-rw-r--r--   0        0        0     1981 2023-05-31 13:59:33.349758 fhi-vibes-1.0.5/vibes/cli/submit.py
+-rw-r--r--   0        0        0     2445 2023-05-31 13:59:33.349839 fhi-vibes-1.0.5/vibes/cli/template.py
+-rw-r--r--   0        0        0    22373 2023-05-31 13:59:33.349947 fhi-vibes-1.0.5/vibes/cli/utils.py
+-rw-r--r--   0        0        0     2927 2023-05-31 13:59:33.350022 fhi-vibes-1.0.5/vibes/context.py
+-rw-r--r--   0        0        0     9053 2023-05-31 13:59:33.350134 fhi-vibes-1.0.5/vibes/correlation.py
+-rw-r--r--   0        0        0      232 2023-05-31 13:59:33.350186 fhi-vibes-1.0.5/vibes/defaults.py
+-rw-r--r--   0        0        0      524 2023-05-31 13:59:33.350235 fhi-vibes-1.0.5/vibes/dimensions.py
+-rw-r--r--   0        0        0     1208 2023-05-31 13:59:33.350291 fhi-vibes-1.0.5/vibes/filenames.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.350353 fhi-vibes-1.0.5/vibes/fireworks/__init__.py
+-rw-r--r--   0        0        0     1113 2023-05-31 13:59:33.350421 fhi-vibes-1.0.5/vibes/fireworks/_defaults.py
+-rw-r--r--   0        0        0    23373 2023-05-31 13:59:33.350563 fhi-vibes-1.0.5/vibes/fireworks/cli/__init__.py
+-rw-r--r--   0        0        0     6679 2023-05-31 13:59:33.350654 fhi-vibes-1.0.5/vibes/fireworks/cli/launch_utils.py
+-rw-r--r--   0        0        0    15063 2023-05-31 13:59:33.350848 fhi-vibes-1.0.5/vibes/fireworks/combined_launcher.py
+-rw-r--r--   0        0        0     3944 2023-05-31 13:59:33.350920 fhi-vibes-1.0.5/vibes/fireworks/launchpad.py
+-rw-r--r--   0        0        0     7007 2023-05-31 13:59:33.351138 fhi-vibes-1.0.5/vibes/fireworks/qlaunch_remote.py
+-rw-r--r--   0        0        0    23072 2023-05-31 13:59:33.351202 fhi-vibes-1.0.5/vibes/fireworks/queue_launcher.py
+-rw-r--r--   0        0        0     6533 2023-05-31 13:59:33.351308 fhi-vibes-1.0.5/vibes/fireworks/rocket_launcher.py
+-rw-r--r--   0        0        0       86 2023-05-31 13:59:33.351394 fhi-vibes-1.0.5/vibes/fireworks/tasks/__init__.py
+-rw-r--r--   0        0        0     5998 2023-05-31 13:59:33.351466 fhi-vibes-1.0.5/vibes/fireworks/tasks/calculate_wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.351519 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/__init__.py
+-rw-r--r--   0        0        0     3896 2023-05-31 13:59:33.351600 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/aims.py
+-rw-r--r--   0        0        0     4183 2023-05-31 13:59:33.351679 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/calculate.py
+-rw-r--r--   0        0        0     5283 2023-05-31 13:59:33.351746 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/check_conditionals.py
+-rw-r--r--   0        0        0     2431 2023-05-31 13:59:33.351807 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/general.py
+-rw-r--r--   0        0        0     1891 2023-05-31 13:59:33.351881 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/md.py
+-rw-r--r--   0        0        0     2375 2023-05-31 13:59:33.351950 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/optimizations.py
+-rw-r--r--   0        0        0    17406 2023-05-31 13:59:33.352052 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/phonons.py
+-rw-r--r--   0        0        0     3270 2023-05-31 13:59:33.352124 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/relaxation.py
+-rw-r--r--   0        0        0     2057 2023-05-31 13:59:33.352197 fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/statistical_sampling.py
+-rw-r--r--   0        0        0     4865 2023-05-31 13:59:33.352293 fhi-vibes-1.0.5/vibes/fireworks/tasks/general_py_task.py
+-rw-r--r--   0        0        0     6131 2023-05-31 13:59:33.352368 fhi-vibes-1.0.5/vibes/fireworks/tasks/md.py
+-rw-r--r--   0        0        0    13514 2023-05-31 13:59:33.352480 fhi-vibes-1.0.5/vibes/fireworks/tasks/phonopy_phono3py_functions.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.352547 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/__init__.py
+-rw-r--r--   0        0        0     3309 2023-05-31 13:59:33.352617 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/aims.py
+-rw-r--r--   0        0        0     1197 2023-05-31 13:59:33.352671 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/calculate.py
+-rw-r--r--   0        0        0      274 2023-05-31 13:59:33.352725 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/md.py
+-rw-r--r--   0        0        0     1916 2023-05-31 13:59:33.352799 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/optimizations.py
+-rw-r--r--   0        0        0    11925 2023-05-31 13:59:33.352883 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/phonons.py
+-rw-r--r--   0        0        0      399 2023-05-31 13:59:33.352932 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/relaxation.py
+-rw-r--r--   0        0        0     1673 2023-05-31 13:59:33.352988 fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/statistical_sampling.py
+-rw-r--r--   0        0        0     2616 2023-05-31 13:59:33.353061 fhi-vibes-1.0.5/vibes/fireworks/tasks/relaxation.py
+-rw-r--r--   0        0        0     7956 2023-05-31 13:59:33.353137 fhi-vibes-1.0.5/vibes/fireworks/tasks/statistical_sampling_wrappers.py
+-rw-r--r--   0        0        0     3727 2023-05-31 13:59:33.353194 fhi-vibes-1.0.5/vibes/fireworks/tasks/task_spec.py
+-rw-r--r--   0        0        0     3610 2023-05-31 13:59:33.353254 fhi-vibes-1.0.5/vibes/fireworks/tasks/utility_tasks.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.353319 fhi-vibes-1.0.5/vibes/fireworks/utils/__init__.py
+-rw-r--r--   0        0        0     5512 2023-05-31 13:59:33.353392 fhi-vibes-1.0.5/vibes/fireworks/utils/converters.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.353446 fhi-vibes-1.0.5/vibes/fireworks/workflows/__init__.py
+-rw-r--r--   0        0        0    29064 2023-05-31 13:59:33.353566 fhi-vibes-1.0.5/vibes/fireworks/workflows/firework_generator.py
+-rw-r--r--   0        0        0     4692 2023-05-31 13:59:33.353649 fhi-vibes-1.0.5/vibes/fireworks/workflows/task_generator.py
+-rw-r--r--   0        0        0    13867 2023-05-31 13:59:33.353727 fhi-vibes-1.0.5/vibes/fireworks/workflows/task_spec_generator.py
+-rw-r--r--   0        0        0     9866 2023-05-31 13:59:33.353828 fhi-vibes-1.0.5/vibes/fireworks/workflows/workflow_generator.py
+-rw-r--r--   0        0        0     5447 2023-05-31 13:59:33.353929 fhi-vibes-1.0.5/vibes/fourier.py
+-rw-r--r--   0        0        0      221 2023-05-31 13:59:33.354023 fhi-vibes-1.0.5/vibes/green_kubo/README.md
+-rw-r--r--   0        0        0     8727 2023-05-31 13:59:33.354096 fhi-vibes-1.0.5/vibes/green_kubo/__init__.py
+-rw-r--r--   0        0        0     2997 2023-05-31 13:59:33.354153 fhi-vibes-1.0.5/vibes/green_kubo/analysis.snippets
+-rw-r--r--   0        0        0     2799 2023-05-31 13:59:33.354209 fhi-vibes-1.0.5/vibes/green_kubo/velocities.py
+-rw-r--r--   0        0        0      337 2023-05-31 13:59:33.354303 fhi-vibes-1.0.5/vibes/harmonic_analysis/__init__.py
+-rw-r--r--   0        0        0     3791 2023-05-31 13:59:33.354364 fhi-vibes-1.0.5/vibes/harmonic_analysis/dynamical_matrix.py
+-rw-r--r--   0        0        0     2229 2023-05-31 13:59:33.354471 fhi-vibes-1.0.5/vibes/harmonic_analysis/force_constants.py
+-rw-r--r--   0        0        0    17557 2023-05-31 13:59:33.354579 fhi-vibes-1.0.5/vibes/harmonic_analysis/mode_projection.py
+-rw-r--r--   0        0        0     8092 2023-05-31 13:59:33.354674 fhi-vibes-1.0.5/vibes/harmonic_analysis/normal_modes.py
+-rw-r--r--   0        0        0     3110 2023-05-31 13:59:33.354733 fhi-vibes-1.0.5/vibes/harmonic_analysis/spectral_energy_density.py
+-rw-r--r--   0        0        0      236 2023-05-31 13:59:33.354822 fhi-vibes-1.0.5/vibes/helpers/__init__.py
+-rw-r--r--   0        0        0     1097 2023-05-31 13:59:33.354878 fhi-vibes-1.0.5/vibes/helpers/aims.py
+-rw-r--r--   0        0        0     3294 2023-05-31 13:59:33.354954 fhi-vibes-1.0.5/vibes/helpers/backup.py
+-rw-r--r--   0        0        0     3679 2023-05-31 13:59:33.355016 fhi-vibes-1.0.5/vibes/helpers/brillouinzone.py
+-rw-r--r--   0        0        0    14667 2023-05-31 13:59:33.355100 fhi-vibes-1.0.5/vibes/helpers/converters.py
+-rw-r--r--   0        0        0     1608 2023-05-31 13:59:33.355160 fhi-vibes-1.0.5/vibes/helpers/dict.py
+-rw-r--r--   0        0        0     1781 2023-05-31 13:59:33.355235 fhi-vibes-1.0.5/vibes/helpers/displacements.py
+-rw-r--r--   0        0        0       69 2023-05-31 13:59:33.355285 fhi-vibes-1.0.5/vibes/helpers/fileformats.py
+-rw-r--r--   0        0        0     2375 2023-05-31 13:59:33.355344 fhi-vibes-1.0.5/vibes/helpers/filter.py
+-rw-r--r--   0        0        0     3378 2023-05-31 13:59:33.355406 fhi-vibes-1.0.5/vibes/helpers/geometry.py
+-rw-r--r--   0        0        0     4409 2023-05-31 13:59:33.355496 fhi-vibes-1.0.5/vibes/helpers/hash.py
+-rw-r--r--   0        0        0     3900 2023-05-31 13:59:33.355574 fhi-vibes-1.0.5/vibes/helpers/k_grid.py
+-rw-r--r--   0        0        0      380 2023-05-31 13:59:33.355631 fhi-vibes-1.0.5/vibes/helpers/latex.py
+-rw-r--r--   0        0        0      495 2023-05-31 13:59:33.355692 fhi-vibes-1.0.5/vibes/helpers/lattice.py
+-rw-r--r--   0        0        0     4919 2023-05-31 13:59:33.355863 fhi-vibes-1.0.5/vibes/helpers/lattice_points.py
+-rw-r--r--   0        0        0      905 2023-05-31 13:59:33.355931 fhi-vibes-1.0.5/vibes/helpers/lists.py
+-rw-r--r--   0        0        0      536 2023-05-31 13:59:33.355996 fhi-vibes-1.0.5/vibes/helpers/notifications.py
+-rw-r--r--   0        0        0     1407 2023-05-31 13:59:33.356055 fhi-vibes-1.0.5/vibes/helpers/numerics.py
+-rw-r--r--   0        0        0     2641 2023-05-31 13:59:33.356130 fhi-vibes-1.0.5/vibes/helpers/paths.py
+-rw-r--r--   0        0        0     1016 2023-05-31 13:59:33.356193 fhi-vibes-1.0.5/vibes/helpers/pickle.py
+-rw-r--r--   0        0        0      292 2023-05-31 13:59:33.356252 fhi-vibes-1.0.5/vibes/helpers/plotting.py
+-rw-r--r--   0        0        0      580 2023-05-31 13:59:33.356310 fhi-vibes-1.0.5/vibes/helpers/properties.py
+-rw-r--r--   0        0        0     1220 2023-05-31 13:59:33.356384 fhi-vibes-1.0.5/vibes/helpers/restarts.py
+-rw-r--r--   0        0        0     4583 2023-05-31 13:59:33.356471 fhi-vibes-1.0.5/vibes/helpers/socketio.py
+-rw-r--r--   0        0        0      758 2023-05-31 13:59:33.356532 fhi-vibes-1.0.5/vibes/helpers/stress.py
+-rw-r--r--   0        0        0     2125 2023-05-31 13:59:33.356599 fhi-vibes-1.0.5/vibes/helpers/stresses.py
+-rw-r--r--   0        0        0      523 2023-05-31 13:59:33.356674 fhi-vibes-1.0.5/vibes/helpers/structure.py
+-rw-r--r--   0        0        0      224 2023-05-31 13:59:33.356775 fhi-vibes-1.0.5/vibes/helpers/supercell/Makefile
+-rw-r--r--   0        0        0    11161 2023-05-31 13:59:33.356876 fhi-vibes-1.0.5/vibes/helpers/supercell/__init__.py
+-rw-r--r--   0        0        0     1838 2023-05-31 13:59:33.356942 fhi-vibes-1.0.5/vibes/helpers/supercell/linalg.f90
+-rw-r--r--   0        0        0      339 2023-05-31 13:59:33.357011 fhi-vibes-1.0.5/vibes/helpers/supercell/setup.py
+-rw-r--r--   0        0        0     9307 2023-05-31 13:59:33.357094 fhi-vibes-1.0.5/vibes/helpers/supercell/supercell.f90
+-rw-r--r--   0        0        0     7786 2023-05-31 13:59:33.357179 fhi-vibes-1.0.5/vibes/helpers/utils.py
+-rw-r--r--   0        0        0     1624 2023-05-31 13:59:33.357241 fhi-vibes-1.0.5/vibes/helpers/virials.py
+-rw-r--r--   0        0        0      935 2023-05-31 13:59:33.357319 fhi-vibes-1.0.5/vibes/helpers/warnings.py
+-rw-r--r--   0        0        0     7697 2023-05-31 13:59:33.357401 fhi-vibes-1.0.5/vibes/helpers/watchdogs.py
+-rw-r--r--   0        0        0      806 2023-05-31 13:59:33.357458 fhi-vibes-1.0.5/vibes/helpers/xarray.py
+-rw-r--r--   0        0        0     2976 2023-05-31 13:59:33.357570 fhi-vibes-1.0.5/vibes/hiphive/__init__.py
+-rw-r--r--   0        0        0     1989 2023-05-31 13:59:33.357646 fhi-vibes-1.0.5/vibes/integrate.py
+-rw-r--r--   0        0        0     3572 2023-05-31 13:59:33.357720 fhi-vibes-1.0.5/vibes/io.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.357785 fhi-vibes-1.0.5/vibes/k_grid/__init__.py
+-rw-r--r--   0        0        0     3579 2023-05-31 13:59:33.357934 fhi-vibes-1.0.5/vibes/k_grid/converge_kgrid.py
+-rw-r--r--   0        0        0     3859 2023-05-31 13:59:33.358017 fhi-vibes-1.0.5/vibes/k_grid/kpointoptimizer.py
+-rw-r--r--   0        0        0     3727 2023-05-31 13:59:33.358096 fhi-vibes-1.0.5/vibes/keys.py
+-rw-r--r--   0        0        0      263 2023-05-31 13:59:33.358207 fhi-vibes-1.0.5/vibes/konstanten/__init__.py
+-rw-r--r--   0        0        0     5417 2023-05-31 13:59:33.358291 fhi-vibes-1.0.5/vibes/konstanten/atomic_masses.py
+-rw-r--r--   0        0        0     2044 2023-05-31 13:59:33.358368 fhi-vibes-1.0.5/vibes/konstanten/einheiten.py
+-rw-r--r--   0        0        0      137 2023-05-31 13:59:33.358424 fhi-vibes-1.0.5/vibes/konstanten/numerics.py
+-rw-r--r--   0        0        0       66 2023-05-31 13:59:33.358524 fhi-vibes-1.0.5/vibes/materials_fp/__init__.py
+-rw-r--r--   0        0        0     6360 2023-05-31 13:59:33.358608 fhi-vibes-1.0.5/vibes/materials_fp/material_fingerprint.py
+-rw-r--r--   0        0        0       69 2023-05-31 13:59:33.358716 fhi-vibes-1.0.5/vibes/molecular_dynamics/__init__.py
+-rw-r--r--   0        0        0     1572 2023-05-31 13:59:33.358781 fhi-vibes-1.0.5/vibes/molecular_dynamics/_defaults.py
+-rw-r--r--   0        0        0     6893 2023-05-31 13:59:33.358877 fhi-vibes-1.0.5/vibes/molecular_dynamics/context.py
+-rw-r--r--   0        0        0     2100 2023-05-31 13:59:33.358952 fhi-vibes-1.0.5/vibes/molecular_dynamics/utils.py
+-rw-r--r--   0        0        0     9194 2023-05-31 13:59:33.359048 fhi-vibes-1.0.5/vibes/molecular_dynamics/workflow.py
+-rw-r--r--   0        0        0      127 2023-05-31 13:59:33.359149 fhi-vibes-1.0.5/vibes/phono3py/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-31 13:59:33.359212 fhi-vibes-1.0.5/vibes/phono3py/_defaults.py
+-rw-r--r--   0        0        0      506 2023-05-31 13:59:33.359269 fhi-vibes-1.0.5/vibes/phono3py/context.py
+-rw-r--r--   0        0        0     4026 2023-05-31 13:59:33.359336 fhi-vibes-1.0.5/vibes/phono3py/postprocess.py
+-rw-r--r--   0        0        0     3856 2023-05-31 13:59:33.359414 fhi-vibes-1.0.5/vibes/phono3py/wrapper.py
+-rw-r--r--   0        0        0      357 2023-05-31 13:59:33.359512 fhi-vibes-1.0.5/vibes/phonopy/__init__.py
+-rw-r--r--   0        0        0      792 2023-05-31 13:59:33.359575 fhi-vibes-1.0.5/vibes/phonopy/_defaults.py
+-rw-r--r--   0        0        0     3609 2023-05-31 13:59:33.359659 fhi-vibes-1.0.5/vibes/phonopy/context.py
+-rw-r--r--   0        0        0    10917 2023-05-31 13:59:33.359763 fhi-vibes-1.0.5/vibes/phonopy/postprocess.py
+-rw-r--r--   0        0        0    14157 2023-05-31 13:59:33.359856 fhi-vibes-1.0.5/vibes/phonopy/utils.py
+-rw-r--r--   0        0        0     2888 2023-05-31 13:59:33.359943 fhi-vibes-1.0.5/vibes/phonopy/workflow.py
+-rw-r--r--   0        0        0    14476 2023-05-31 13:59:33.360054 fhi-vibes-1.0.5/vibes/phonopy/wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.360125 fhi-vibes-1.0.5/vibes/relaxation/__init__.py
+-rw-r--r--   0        0        0     1233 2023-05-31 13:59:33.360197 fhi-vibes-1.0.5/vibes/relaxation/_defaults.py
+-rw-r--r--   0        0        0     5264 2023-05-31 13:59:33.360285 fhi-vibes-1.0.5/vibes/relaxation/context.py
+-rw-r--r--   0        0        0     4092 2023-05-31 13:59:33.360351 fhi-vibes-1.0.5/vibes/relaxation/workflow.py
+-rw-r--r--   0        0        0     6654 2023-05-31 13:59:33.360480 fhi-vibes-1.0.5/vibes/settings.py
+-rw-r--r--   0        0        0      335 2023-05-31 13:59:33.360577 fhi-vibes-1.0.5/vibes/slurm/README.md
+-rw-r--r--   0        0        0      135 2023-05-31 13:59:33.360637 fhi-vibes-1.0.5/vibes/slurm/__init__.py
+-rw-r--r--   0        0        0      758 2023-05-31 13:59:33.360694 fhi-vibes-1.0.5/vibes/slurm/generate.py
+-rw-r--r--   0        0        0      577 2023-05-31 13:59:33.360756 fhi-vibes-1.0.5/vibes/slurm/render.py
+-rw-r--r--   0        0        0     1329 2023-05-31 13:59:33.360818 fhi-vibes-1.0.5/vibes/slurm/submit.py
+-rw-r--r--   0        0        0      903 2023-05-31 13:59:33.360884 fhi-vibes-1.0.5/vibes/son.py
+-rw-r--r--   0        0        0       35 2023-05-31 13:59:33.360973 fhi-vibes-1.0.5/vibes/spglib/__init__.py
+-rw-r--r--   0        0        0     4966 2023-05-31 13:59:33.361057 fhi-vibes-1.0.5/vibes/spglib/q_mesh.py
+-rw-r--r--   0        0        0     4192 2023-05-31 13:59:33.361141 fhi-vibes-1.0.5/vibes/spglib/wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.361209 fhi-vibes-1.0.5/vibes/structure/__init__.py
+-rw-r--r--   0        0        0     2041 2023-05-31 13:59:33.361283 fhi-vibes-1.0.5/vibes/structure/convert.py
+-rw-r--r--   0        0        0     7197 2023-05-31 13:59:33.361379 fhi-vibes-1.0.5/vibes/structure/io.py
+-rw-r--r--   0        0        0     3400 2023-05-31 13:59:33.361442 fhi-vibes-1.0.5/vibes/structure/misc.py
+-rw-r--r--   0        0        0       48 2023-05-31 13:59:33.361531 fhi-vibes-1.0.5/vibes/tdep/__init__.py
+-rw-r--r--   0        0        0    11219 2023-05-31 13:59:33.361621 fhi-vibes-1.0.5/vibes/tdep/wrapper.py
+-rw-r--r--   0        0        0       35 2023-05-31 13:59:33.361709 fhi-vibes-1.0.5/vibes/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.361775 fhi-vibes-1.0.5/vibes/templates/config_files/__init__.py
+-rw-r--r--   0        0        0      592 2023-05-31 13:59:33.361843 fhi-vibes-1.0.5/vibes/templates/config_files/fireworksrc.template
+-rw-r--r--   0        0        0      165 2023-05-31 13:59:33.361906 fhi-vibes-1.0.5/vibes/templates/config_files/slurm.in
+-rw-r--r--   0        0        0      391 2023-05-31 13:59:33.361964 fhi-vibes-1.0.5/vibes/templates/config_files/vibesrc.template
+-rw-r--r--   0        0        0        0 2023-05-31 13:59:33.362023 fhi-vibes-1.0.5/vibes/templates/settings/__init__.py
+-rw-r--r--   0        0        0      341 2023-05-31 13:59:33.362082 fhi-vibes-1.0.5/vibes/templates/settings/aims
+-rw-r--r--   0        0        0      754 2023-05-31 13:59:33.362140 fhi-vibes-1.0.5/vibes/templates/settings/aims_full
+-rw-r--r--   0        0        0      201 2023-05-31 13:59:33.362192 fhi-vibes-1.0.5/vibes/templates/settings/lj
+-rw-r--r--   0        0        0      920 2023-05-31 13:59:33.362270 fhi-vibes-1.0.5/vibes/trajectory/README.md
+-rw-r--r--   0        0        0      361 2023-05-31 13:59:33.362329 fhi-vibes-1.0.5/vibes/trajectory/__init__.py
+-rw-r--r--   0        0        0     5096 2023-05-31 13:59:33.362420 fhi-vibes-1.0.5/vibes/trajectory/analysis.py
+-rw-r--r--   0        0        0     6961 2023-05-31 13:59:33.362496 fhi-vibes-1.0.5/vibes/trajectory/dataset.py
+-rw-r--r--   0        0        0     1567 2023-05-31 13:59:33.362570 fhi-vibes-1.0.5/vibes/trajectory/heat_flux.py
+-rw-r--r--   0        0        0    13362 2023-05-31 13:59:33.362665 fhi-vibes-1.0.5/vibes/trajectory/io.py
+-rw-r--r--   0        0        0     4669 2023-05-31 13:59:33.362739 fhi-vibes-1.0.5/vibes/trajectory/plotting.py
+-rw-r--r--   0        0        0    24034 2023-05-31 13:59:33.362856 fhi-vibes-1.0.5/vibes/trajectory/trajectory.py
+-rw-r--r--   0        0        0      873 2023-05-31 13:59:33.362929 fhi-vibes-1.0.5/vibes/trajectory/utils.py
+-rw-r--r--   0        0        0     5765 2023-06-01 08:07:16.856752 fhi-vibes-1.0.5/setup.py
+-rw-r--r--   0        0        0     5336 2023-06-01 08:07:16.857152 fhi-vibes-1.0.5/PKG-INFO
```

### Comparing `fhi-vibes-1.0.4/LICENSE` & `fhi-vibes-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/README.md` & `fhi-vibes-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 - harmonic phonon calculations via [Phonopy](https://atztogo.github.io/phonopy/),
 - molecular dynamics simulations in [NVE](https://wiki.fysik.dtu.dk/ase/ase/md.html#constant-nve-simulations-the-microcanonical-ensemble), [NVT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.langevin), and [NPT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.nptberendsen) ensembles,
 - [harmonic sampling](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.96.115504), and
 - [anharmonicity quantification](https://journals.aps.org/prmaterials/abstract/10.1103/PhysRevMaterials.4.083809).
 
 Most of the functionality is high-throughput ready via [fireworks](https://materialsproject.github.io/fireworks/#).
 
+A reference implementation of the [ab initio Green Kubo method](https://arxiv.org/abs/2209.01139) is [available](https://gitlab.com/vibes-developers/vibes/-/merge_requests/57). However, we ask you to contact the developers before using this functionality as it requires extra instructions.
+
 ## Overview
 
 - [Installation](https://vibes-developers.gitlab.io/vibes/Installation)
 - [Tutorial](https://vibes-developers.gitlab.io/vibes/Tutorial/0_intro)
 - [Documentation](https://vibes-developers.gitlab.io/vibes/Documentation/0_intro)
 - [Credits](https://vibes-developers.gitlab.io/vibes/Credits)
 - [References](https://vibes-developers.gitlab.io/vibes/References)
 
+## Changelog
 
-## News
-
-- `FHI-vibes` got [published in JOSS](https://joss.theoj.org/papers/10.21105/joss.02671)!
-- [Our anharmonicity measure got published!](https://journals.aps.org/prmaterials/abstract/10.1103/PhysRevMaterials.4.083809)
-- [… the best is yet to come.](https://www.youtube.com/watch?v=B-Jq26BCwDs)
+#### v1.0.5
 
-## Changelog
+- bugfix
 
 #### v1.0.4
 
 - looser dependencies
 - [various bug fixes](https://gitlab.com/vibes-developers/vibes/-/merge_requests?scope=all&state=merged)
 
 #### v1.0.3
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fhi-vibes-1.0.4/pyproject.toml` & `fhi-vibes-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fhi-vibes"
-version = "1.0.4"
+version = "1.0.5"
 description = "Fritz Haber Institute Vibrational Simulations"
 authors = ["Florian Knoop <knoop@fhi-berlin.mpg.de>", "Thomas Purcell <purcell@fhi-berlin.mpg.de"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/vibes-developers/vibes"
 packages = [
     { include = "vibes" },
@@ -16,17 +16,17 @@
 
 [tool.poetry.dependencies]
 python = "^3.6.1, <4.0"
 numpy = "^1.17.5"
 scipy = "^1.1.1"
 matplotlib = "^3.1"
 son = "^0.4.1"
-spglib = "^1.12"
+spglib = ">=1.12"
 phonopy = "^2.6"
-ase = "^3.20.0,<3.23"
+ase = "^3.20.0"
 click = ">=8.0"
 attrs = ">=19.1"
 fireworks = {version = "^1.9",optional = true}
 phono3py = {version = "^1.21",optional = true}
 python-gssapi = {version = "^0.6.4",optional = true}
 pymongo = {version = "^3.8",optional = true}
 fabric = {version = "^2.4",optional = true}
@@ -36,15 +36,15 @@
 netCDF4 = ">=1.5"
 jinja2 = ">=2.10"
 hiphive = {version = "^0.5.0", optional = true}
 tables = "^3.5"
 click_aliases = ">=1.0"
 click_completion = ">=0.5.2"
 jconfigparser = "^0.1.2"
-pandas = ">=1.0"
+pandas = ">=1.0,<2.0"
 importlib_resources = { version = "*", python = "3.6.*" }
 dataclasses = { version = "*", python = "3.6.*" }
 seaborn = ">=0.11.0"
 requests = {version = "^2.25", optional=true}
 
 [tool.poetry.extras]
 fireworks = ["fireworks", "python-gssapi", "pymongo", "fabric", "paramiko", "requests"]
@@ -73,10 +73,10 @@
 target-version = ['py37']
 
 [tool.pytest.ini_options]
 addopts = "--import-mode=importlib"
 filterwarnings = ["ignore"]
 
 [build-system]
-requires = ["setuptools<=59.2.0", "wheel", "poetry>=0.12", "numpy"]
+requires = ["setuptools<=59.2.0", "wheel", "poetry<=1.1.12", "numpy"]
 build-backend = "poetry.masonry.api"
```

### Comparing `fhi-vibes-1.0.4/vibes/anharmonicity_score.py` & `fhi-vibes-1.0.5/vibes/anharmonicity_score.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/ase/calculators/fc.py` & `fhi-vibes-1.0.5/vibes/ase/calculators/fc.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/ase/db/dict_converters.py` & `fhi-vibes-1.0.5/vibes/ase/db/dict_converters.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/ase/md/velocitydistribution.py` & `fhi-vibes-1.0.5/vibes/ase/md/velocitydistribution.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/calculate.py` & `fhi-vibes-1.0.5/vibes/calculate.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/calculator/aims.py` & `fhi-vibes-1.0.5/vibes/calculator/aims.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/calculator/context.py` & `fhi-vibes-1.0.5/vibes/calculator/context.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/calculator/setup.py` & `fhi-vibes-1.0.5/vibes/calculator/setup.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/calculator/workflow.py` & `fhi-vibes-1.0.5/vibes/calculator/workflow.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/__init__.py` & `fhi-vibes-1.0.5/vibes/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/info.py` & `fhi-vibes-1.0.5/vibes/cli/info.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/misc.py` & `fhi-vibes-1.0.5/vibes/cli/misc.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/output.py` & `fhi-vibes-1.0.5/vibes/cli/output.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/run.py` & `fhi-vibes-1.0.5/vibes/cli/run.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/create_samples.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/create_samples.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/create_trajectory.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/create_trajectory.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/geometry_info.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/geometry_info.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/get_relaxation_info.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/get_relaxation_info.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/hilde_run.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/hilde_run.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/make_supercell.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/make_supercell.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/md_sum.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/md_sum.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/refine_geometry.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/refine_geometry.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/remap_phonopy_forceconstants.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/remap_phonopy_forceconstants.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/rewrite_geometry.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/rewrite_geometry.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/run_thermal_conductivity.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/run_thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/suggest_k_grid.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/suggest_k_grid.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/trajectory2tdep.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/trajectory2tdep.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/trajectory2xyz.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/trajectory2xyz.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/update_md_trajectory.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/update_md_trajectory.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/vibes_phonopy.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/vibes_phonopy.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/scripts/yaml2json.py` & `fhi-vibes-1.0.5/vibes/cli/scripts/yaml2json.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/submit.py` & `fhi-vibes-1.0.5/vibes/cli/submit.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/template.py` & `fhi-vibes-1.0.5/vibes/cli/template.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/cli/utils.py` & `fhi-vibes-1.0.5/vibes/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,14 +517,15 @@
     if uc:
         atoms = read(uc, format=format)
         traj.primitive = atoms
 
     if sc:
         atoms = read(sc, format=format)
         traj.supercell = atoms
+        traj.set_displacements()
 
     if rfc:
         fc = parse_force_constants(rfc)
         print(fc)
         traj.set_force_constants_remapped(fc)
 
     if not outfile:
```

### Comparing `fhi-vibes-1.0.4/vibes/context.py` & `fhi-vibes-1.0.5/vibes/context.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/correlation.py` & `fhi-vibes-1.0.5/vibes/correlation.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/dimensions.py` & `fhi-vibes-1.0.5/vibes/dimensions.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/filenames.py` & `fhi-vibes-1.0.5/vibes/filenames.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/_defaults.py` & `fhi-vibes-1.0.5/vibes/fireworks/_defaults.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/cli/__init__.py` & `fhi-vibes-1.0.5/vibes/fireworks/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/cli/launch_utils.py` & `fhi-vibes-1.0.5/vibes/fireworks/cli/launch_utils.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/combined_launcher.py` & `fhi-vibes-1.0.5/vibes/fireworks/combined_launcher.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/launchpad.py` & `fhi-vibes-1.0.5/vibes/fireworks/launchpad.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/qlaunch_remote.py` & `fhi-vibes-1.0.5/vibes/fireworks/qlaunch_remote.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/queue_launcher.py` & `fhi-vibes-1.0.5/vibes/fireworks/queue_launcher.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/rocket_launcher.py` & `fhi-vibes-1.0.5/vibes/fireworks/rocket_launcher.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/calculate_wrapper.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/calculate_wrapper.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/aims.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/aims.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/calculate.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/calculate.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/check_conditionals.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/check_conditionals.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/general.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/general.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/md.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/md.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/optimizations.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/optimizations.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/phonons.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/phonons.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/relaxation.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/relaxation.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/fw_out/statistical_sampling.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/fw_out/statistical_sampling.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/general_py_task.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/general_py_task.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/md.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/md.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/phonopy_phono3py_functions.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/phonopy_phono3py_functions.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/aims.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/aims.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/calculate.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/calculate.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/optimizations.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/optimizations.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/phonons.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/phonons.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,17 +272,17 @@
 
         phonon_small.run_mesh([45, 45, 45])
         phonon_small.run_total_dos(freq_pitch=0.01)
         n_bins = len(phonon_small.get_total_dos_dict()["frequency_points"])
         prev_dos_fp = get_phonon_dos_fp(phonon_small, nbins=n_bins)
 
     if prev_dos_fp:
-        de = prev_dos_fp[0][0][1] - prev_dos_fp[0][0][0]
-        min_f = prev_dos_fp[0][0][0] - 0.5 * de
-        max_f = prev_dos_fp[0][0][-1] + 0.5 * de
+        de = prev_dos_fp[0][1] - prev_dos_fp[0][0]
+        min_f = prev_dos_fp[0][0] - 0.5 * de
+        max_f = prev_dos_fp[0][-1] + 0.5 * de
         phonon.run_total_dos(freq_min=min_f, freq_max=max_f, freq_pitch=0.01)
     else:
         # If Not Converged update phonons
         phonon.run_total_dos(freq_pitch=0.01)
 
     # Get a phonon DOS Finger print to compare against the previous one
     n_bins = len(phonon.get_total_dos_dict()["frequency_points"])
```

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/postprocess/statistical_sampling.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/postprocess/statistical_sampling.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/relaxation.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/relaxation.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/statistical_sampling_wrappers.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/statistical_sampling_wrappers.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/task_spec.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/task_spec.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/tasks/utility_tasks.py` & `fhi-vibes-1.0.5/vibes/fireworks/tasks/utility_tasks.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/utils/converters.py` & `fhi-vibes-1.0.5/vibes/fireworks/utils/converters.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/workflows/firework_generator.py` & `fhi-vibes-1.0.5/vibes/fireworks/workflows/firework_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             chars, counts = np.unique(list(condition_split[0]), return_counts=True)
             op_check = [
                 (char, count)
                 for char, count in zip(chars, counts)
                 if char in ["(", ")"]
             ]
             if (len(op_check) not in [0, 2]) or (
-                not all([oc[1] == 1 for oc in op_check])
+                not all(oc[1] == 1 for oc in op_check)
             ):
                 raise ValueError(
                     f'Vector operation is not properly formatted in "{condition}".'
                 )
             elif len(op_check) == 0:
                 condition_list[:2] = [condition_split[0].strip(), ""]
             else:
```

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/workflows/task_generator.py` & `fhi-vibes-1.0.5/vibes/fireworks/workflows/task_generator.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/workflows/task_spec_generator.py` & `fhi-vibes-1.0.5/vibes/fireworks/workflows/task_spec_generator.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fireworks/workflows/workflow_generator.py` & `fhi-vibes-1.0.5/vibes/fireworks/workflows/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/fourier.py` & `fhi-vibes-1.0.5/vibes/fourier.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/green_kubo/__init__.py` & `fhi-vibes-1.0.5/vibes/green_kubo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         fs_factor (float): time * fs_factor = time in fs
 
     Returns:
         V / (k_B * T^2) * 1602
     """
     V = float(volume)
     T = float(temperature)
-    prefactor = 1 / units.kB / T ** 2 * 1.602 * V / fs_factor  # / 1000
+    prefactor = 1 / units.kB / T**2 * 1.602 * V / fs_factor  # / 1000
     msg = [
         f"Compute Prefactor:",
         f".. Volume:        {V:10.2f}  AA^3",
         f".. Temperature:   {T:10.2f}  K",
         f".. factor to fs.: {fs_factor:10.5f}",
         f"-> Prefactor:     {prefactor:10.2f}  W/mK / (eV/AA^/fs)",
     ]
@@ -56,33 +56,38 @@
 def get_gk_prefactor_from_dataset(dataset: xr.Dataset, verbose: bool = True) -> float:
     """get the GK prefactor for the dataset, wraps `gk_prefactor`"""
     volume = dataset.attrs[keys.volume]
     temperature = dataset[keys.temperature].mean()
     return gk_prefactor(volume=volume, temperature=temperature, verbose=verbose)
 
 
-def get_hf_data(flux: xr.DataArray, dropna_dim=keys.time) -> namedtuple:
+def get_hf_data(
+    flux: xr.DataArray, dropna_dim=keys.time, distribute=True
+) -> namedtuple:
     """Compute heat flux autocorrelation and integrated kappa from heat flux
 
     Args:
         flux [N_t, 3]: the heat flux in an xr.DataArray
         dropna_dim: drop nan values along this dimension (default: `time`)
+        bool: use multiprocessing to parallelize autocorrelation
 
     Returns:
         namedtuple: (heat flux autocorrelation function, integrated kappa)
 
     """
     # dropna
     flux = flux.dropna(dropna_dim)
 
     # compute the time mean flux of flux <J>
     flux_avg = flux.mean(axis=0)
 
     # compute heat flux autocorrelation function (HFACF) <J(t)J>
-    flux_corr = get_autocorrelationNd(flux - flux_avg, off_diagonal=True, verbose=False)
+    flux_corr = get_autocorrelationNd(
+        flux - flux_avg, off_diagonal=True, verbose=False, distribute=distribute
+    )
 
     # get integrated kappa
     kappa = get_cumtrapz(flux_corr)
 
     # return namedtuple w/ HFACF and integrated kappa
     cls = namedtuple(
         "gk_raw_data", (keys.heat_flux_autocorrelation, keys.kappa_cumulative)
```

### Comparing `fhi-vibes-1.0.4/vibes/green_kubo/analysis.snippets` & `fhi-vibes-1.0.5/vibes/green_kubo/analysis.snippets`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/green_kubo/velocities.py` & `fhi-vibes-1.0.5/vibes/green_kubo/velocities.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/harmonic_analysis/dynamical_matrix.py` & `fhi-vibes-1.0.5/vibes/harmonic_analysis/dynamical_matrix.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/harmonic_analysis/force_constants.py` & `fhi-vibes-1.0.5/vibes/harmonic_analysis/force_constants.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/harmonic_analysis/mode_projection.py` & `fhi-vibes-1.0.5/vibes/harmonic_analysis/mode_projection.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/harmonic_analysis/normal_modes.py` & `fhi-vibes-1.0.5/vibes/harmonic_analysis/normal_modes.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/harmonic_analysis/spectral_energy_density.py` & `fhi-vibes-1.0.5/vibes/harmonic_analysis/spectral_energy_density.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/aims.py` & `fhi-vibes-1.0.5/vibes/helpers/aims.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/backup.py` & `fhi-vibes-1.0.5/vibes/helpers/backup.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/brillouinzone.py` & `fhi-vibes-1.0.5/vibes/helpers/brillouinzone.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/converters.py` & `fhi-vibes-1.0.5/vibes/helpers/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 key_symbols = "symbols"
 key_masses = "masses"
 key_constraints = "constraint"
 
 
 class NumpyEncoder(json.JSONEncoder):
-    """ Decode numerical objects that json cannot parse by default"""
+    """Decode numerical objects that json cannot parse by default"""
 
     def default(self, obj) -> str:
         """Default JSON encoding"""
         if hasattr(obj, "tolist") and callable(obj.tolist):
             return obj.tolist()
         if isinstance(obj, (np.int32, np.int64)):
             return int(obj)
@@ -38,15 +38,17 @@
             return bool(obj)
         if isinstance(obj, PosixPath):
             return str(obj)
 
         return super().default(obj)
 
 
-def atoms2dict(atoms: Atoms, reduce: bool = True, add_constraints: bool = False) -> dict:
+def atoms2dict(
+    atoms: Atoms, reduce: bool = True, add_constraints: bool = False
+) -> dict:
     """Converts an Atoms object into a dict
 
     Args:
         atoms: The structure to be converted to a dict
         reduce: use reduced representation of `symbols` and `masses`
 
     Returns:
@@ -92,15 +94,15 @@
     """
 
     if calculator is None:
         return {}
     if isinstance(calculator, dict):
         return calculator
 
-    params = calculator.todict()
+    params = calculator.parameters
     for key, val in params.items():
         if isinstance(val, tuple):
             params[key] = list(val)
 
     calculator_dict = {
         "calculator": calculator.__class__.__name__,
         "calculator_parameters": params,
@@ -193,15 +195,15 @@
         if len(stresses[0]) == 6:
             calculator.results[keys.stresses] = voigt_6_to_full_3x3_stress(stresses)
 
     # convert numpy arrays into ordinary lists
     for key, val in calculator.results.items():
         if isinstance(val, np.ndarray):
             calculator_dict[key] = val.tolist()
-        elif isinstance(val, np.float):
+        elif isinstance(val, (float, np.double)):
             calculator_dict[key] = float(val)
         else:
             calculator_dict[key] = val
 
     if not calculator_dict:
         raise RuntimeError("calculator_dict is empty, was the calculation successful?")
 
@@ -322,15 +324,15 @@
     for key, val in dct.items():
         # convert np.ndarrays etc to lists
         if hasattr(val, "tolist") and callable(val.tolist):
             val = val.tolist()
 
         if isinstance(val, str):
             rep = f'"{val}"'
-        elif isinstance(val, (float, np.float)):
+        elif isinstance(val, (float, np.double)):
             rep = "{1: .{0}e}".format(n_yaml_digits, val)
         elif isinstance(val, dict):
             # recursive formatting
             rep = f"{{\n{dict2json(val, 2*(1 + indent // 2), False)}}}"
         elif val == []:  # empty list
             rep = json.dumps(val, cls=NumpyEncoder)
         elif (
```

### Comparing `fhi-vibes-1.0.4/vibes/helpers/dict.py` & `fhi-vibes-1.0.5/vibes/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/displacements.py` & `fhi-vibes-1.0.5/vibes/helpers/displacements.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/filter.py` & `fhi-vibes-1.0.5/vibes/helpers/filter.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/geometry.py` & `fhi-vibes-1.0.5/vibes/helpers/geometry.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/hash.py` & `fhi-vibes-1.0.5/vibes/helpers/hash.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/k_grid.py` & `fhi-vibes-1.0.5/vibes/helpers/k_grid.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/lattice_points.py` & `fhi-vibes-1.0.5/vibes/helpers/lattice_points.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/lists.py` & `fhi-vibes-1.0.5/vibes/helpers/lists.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/notifications.py` & `fhi-vibes-1.0.5/vibes/helpers/notifications.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/numerics.py` & `fhi-vibes-1.0.5/vibes/helpers/numerics.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/paths.py` & `fhi-vibes-1.0.5/vibes/helpers/paths.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/pickle.py` & `fhi-vibes-1.0.5/vibes/helpers/pickle.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/properties.py` & `fhi-vibes-1.0.5/vibes/helpers/properties.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/restarts.py` & `fhi-vibes-1.0.5/vibes/helpers/restarts.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/socketio.py` & `fhi-vibes-1.0.5/vibes/helpers/socketio.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,27 +101,27 @@
         unixsocket: get_unixsocket
     """
 
     port = None
     unixsocket = None
     if not hasattr(calculator, "parameters"):
         warn(f"{prefix} No parameters found in calculator {calculator.name}.", level=1)
-        return port
 
-    if "use_pimd_wrapper" in calculator.parameters:
-        port = calculator.parameters["use_pimd_wrapper"][1]
-        host = calculator.parameters["use_pimd_wrapper"][0]
-
-        if "UNIX:" in host:
-            unixsocket = calculator.parameters["use_pimd_wrapper"][0]
-            talk(f"Use SocketIO with unixsocket file {unixsocket}", prefix=prefix)
-        else:
-            talk(f"Use SocketIO with host {host} and port {port}", prefix=prefix)
     else:
-        talk(f"Socketio not used with calculator {calculator.name}", prefix=prefix)
+        if "use_pimd_wrapper" in calculator.parameters:
+            port = calculator.parameters["use_pimd_wrapper"][1]
+            host = calculator.parameters["use_pimd_wrapper"][0]
+
+            if "UNIX:" in host:
+                unixsocket = calculator.parameters["use_pimd_wrapper"][0]
+                talk(f"Use SocketIO with unixsocket file {unixsocket}", prefix=prefix)
+            else:
+                talk(f"Use SocketIO with host {host} and port {port}", prefix=prefix)
+        else:
+            talk(f"Socketio not used with calculator {calculator.name}", prefix=prefix)
 
     return port, unixsocket
 
 
 def get_stresses(atoms):
     """Use Socket to get intensive atomic stresses in eV/AA^3 in Nx3x3 shape.
     Raw stresses are supposed to be extensive and the volume is divided out.
```

### Comparing `fhi-vibes-1.0.4/vibes/helpers/stress.py` & `fhi-vibes-1.0.5/vibes/helpers/stress.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/stresses.py` & `fhi-vibes-1.0.5/vibes/helpers/stresses.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/structure.py` & `fhi-vibes-1.0.5/vibes/helpers/structure.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/supercell/__init__.py` & `fhi-vibes-1.0.5/vibes/helpers/supercell/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from vibes.helpers.geometry import get_cubicness
 from vibes.helpers.lattice import fractional
 from vibes.helpers.numerics import clean_matrix
 from vibes.helpers.utils import Timer
 from vibes.helpers.warnings import warn
 from vibes.structure.misc import get_sysname
 
-from . import supercell as sc
-
 
 def get_lattice_points(
     cell, supercell, tolerance=1e-5, sort=True, fortran=True, verbose=False
 ):
     """
         S = M . L
 
@@ -84,14 +82,16 @@
         print(f"\ninv_lattice:                  \n{inv_lattice}\n")
 
     # maximal distance = diagonal of the cell
     # points generated beyond this won't lie inside the supercell
     dmax = 2.5 * np.linalg.norm(superlattice.sum(axis=1))
 
     if fortran:
+        from . import supercell as sc
+
         all_lattice_points = sc.supercell.find_lattice_points(
             lattice.T, inv_superlattice.T, n_lattice_points, max_iterations, tolerance
         ).T
         lattice_points = all_lattice_points[:n_lattice_points]
         lattice_points_extended = [
             p
             for p in all_lattice_points[n_lattice_points:]
@@ -176,15 +176,15 @@
         sorted lattice point list
     """
 
     return sorted(lattice_points, key=lambda x: la.norm(x + [0, 2 * tol, 4 * tol]))
 
 
 def get_commensurate_q_points(cell, supercell, tolerance=1e-5, **kwargs):
-    """ For a commensurate q_points we have
+    """For a commensurate q_points we have
 
         exp( 2*pi q . L_k ) = 1 for any k and L_k being the supercell lattice vectors
 
         in other workds, q is a linear combination of G_k, where G_k are the inverse
         lattice vectors of the supercell lattice. Only those are counted which fit into
         the inverse lattice of the primitive cell.
         This means we have to call lattice_points.get_lattice_points with the inverse
@@ -243,14 +243,15 @@
     lower_limit: int
         lower limit for the elements in the supercell matrix
     upper_limit:int
         upper limit for the elements in the supercell matrix
     verbose: bool
         If True print more information to the console
     """
+    from . import supercell as sc
 
     smatrix = sc.supercell.find_optimal_cell(
         cell,
         np.eye(3),
         target_size=target_size,
         deviation=deviation,
         lower_limit=lower_limit,
@@ -312,15 +313,15 @@
             + f"{cub_ness:.3f} ({cub_ness**3:.3f})"
         )
         print(f"**-> Systems: {get_sysname(prim_cell)}, target size {target_size}")
     return supercell, smatrix
 
 
 def make_supercell(atoms, supercell_matrix, info={}, tol=1e-5, wrap=True):
-    """ Create the lattice points within supercell and attach atoms to each of them
+    """Create the lattice points within supercell and attach atoms to each of them
 
     Parameters
     ----------
     atoms: ase.atoms.Atoms
         primitive cell as atoms object
     supercell_matrix: np.ndarray
         supercell matrix M with convention A = M . a
@@ -340,15 +341,15 @@
     supercell.cell = clean_matrix(supercell.cell)
     if wrap:
         supercell.set_scaled_positions(supercell.get_scaled_positions(wrap=True))
     return supercell
 
 
 def map_indices(atoms1, atoms2, tol=1e-5):
-    """ return indices of atoms in atoms1 in atoms2.
+    """return indices of atoms in atoms1 in atoms2.
 
     Background Information at
     https://gitlab.com/flokno/vibes/blob/devel/examples/devel/sort_atoms/sort.ipynb
 
     Example
     -------
         atoms1 = [H, O1, O2]
```

### Comparing `fhi-vibes-1.0.4/vibes/helpers/supercell/linalg.f90` & `fhi-vibes-1.0.5/vibes/helpers/supercell/linalg.f90`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/supercell/supercell.f90` & `fhi-vibes-1.0.5/vibes/helpers/supercell/supercell.f90`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/utils.py` & `fhi-vibes-1.0.5/vibes/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/virials.py` & `fhi-vibes-1.0.5/vibes/helpers/virials.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/warnings.py` & `fhi-vibes-1.0.5/vibes/helpers/warnings.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/watchdogs.py` & `fhi-vibes-1.0.5/vibes/helpers/watchdogs.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/helpers/xarray.py` & `fhi-vibes-1.0.5/vibes/helpers/xarray.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/hiphive/__init__.py` & `fhi-vibes-1.0.5/vibes/hiphive/__init__.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/integrate.py` & `fhi-vibes-1.0.5/vibes/integrate.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/io.py` & `fhi-vibes-1.0.5/vibes/io.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/k_grid/converge_kgrid.py` & `fhi-vibes-1.0.5/vibes/k_grid/converge_kgrid.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/k_grid/kpointoptimizer.py` & `fhi-vibes-1.0.5/vibes/k_grid/kpointoptimizer.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/keys.py` & `fhi-vibes-1.0.5/vibes/keys.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/konstanten/atomic_masses.py` & `fhi-vibes-1.0.5/vibes/konstanten/atomic_masses.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/konstanten/einheiten.py` & `fhi-vibes-1.0.5/vibes/konstanten/einheiten.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/materials_fp/material_fingerprint.py` & `fhi-vibes-1.0.5/vibes/materials_fp/material_fingerprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
     ener, enerBounds = get_ener(binning, dos[:, 0], min_e, max_e, nbins)
     dos_rebin = np.zeros(ener.shape)
     for ii, e1, e2 in zip(range(len(ener)), enerBounds[0:-1], enerBounds[1:]):
         dos_rebin[ii] = np.sum(
             dos[np.where((dos[:, 0] >= e1) & (dos[:, 0] < e2))[0], 1]
         )
-    return fp_tup(np.array([ener]), dos_rebin, ["DOS"], nbins)
+    return fp_tup(np.array(ener), dos_rebin, ["DOS"], nbins)
 
 
 def scalar_product(fp1, fp2, col=0, pt="All", normalize=False, tanimoto=False):
     """Calculates the dot product between two finger prints
 
     Parameters
     ----------
```

### Comparing `fhi-vibes-1.0.4/vibes/molecular_dynamics/_defaults.py` & `fhi-vibes-1.0.5/vibes/molecular_dynamics/_defaults.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/molecular_dynamics/context.py` & `fhi-vibes-1.0.5/vibes/molecular_dynamics/context.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/molecular_dynamics/utils.py` & `fhi-vibes-1.0.5/vibes/molecular_dynamics/utils.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/molecular_dynamics/workflow.py` & `fhi-vibes-1.0.5/vibes/molecular_dynamics/workflow.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phono3py/_defaults.py` & `fhi-vibes-1.0.5/vibes/phono3py/_defaults.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phono3py/postprocess.py` & `fhi-vibes-1.0.5/vibes/phono3py/postprocess.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phono3py/wrapper.py` & `fhi-vibes-1.0.5/vibes/phono3py/wrapper.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phonopy/_defaults.py` & `fhi-vibes-1.0.5/vibes/phonopy/_defaults.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phonopy/context.py` & `fhi-vibes-1.0.5/vibes/phonopy/context.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phonopy/postprocess.py` & `fhi-vibes-1.0.5/vibes/phonopy/postprocess.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phonopy/utils.py` & `fhi-vibes-1.0.5/vibes/phonopy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from ase.io import read
 from phonopy.file_IO import parse_FORCE_CONSTANTS, read_force_constants_hdf5
 from phonopy.structure.atoms import PhonopyAtoms
 
 from vibes.helpers import Timer, progressbar, talk, warn
 from vibes.helpers.converters import input2dict
 from vibes.helpers.fileformats import last_from_yaml
-from vibes.helpers.supercell.supercell import supercell as fort
 from vibes.phonopy._defaults import displacement_id_str
 from vibes.structure.convert import to_Atoms
 
 _prefix = "phonopy.utils"
 
 
 def last_calculation_id(trajectory_file):
@@ -83,15 +82,15 @@
     for nn, scell in enumerate(cells):
         if scell is None:
             continue
         scell.info[info_str] = nn
 
 
 def get_supercells_with_displacements(phonon):
-    """ Create a phonopy object and supercells etc.
+    """Create a phonopy object and supercells etc.
 
     Parameters
     ----------
     phonon: phonopy.Phonopy
         The phonopy object with displacement_dataset
 
     Returns
@@ -318,14 +317,16 @@
         sc_r[aa], _ = get_distances([spos[p2s]], spos, cell=supercell.cell, pbc=True)
 
     # find mapping from supercell to origin atom in primitive cell
     primitive.cell = primitive_cell
     map2prim = _map2prim(primitive, new_supercell)
 
     if fortran:
+        from vibes.helpers.supercell.supercell import supercell as fort
+
         talk(".. use fortran", prefix=_prefix)
         fc_out = fort.remap_force_constants(
             positions=new_supercell.positions,
             pairs=sc_r,
             fc_in=force_constants,
             map2prim=map2prim,
             inv_lattice=new_supercell.get_reciprocal_cell(),
```

### Comparing `fhi-vibes-1.0.4/vibes/phonopy/workflow.py` & `fhi-vibes-1.0.5/vibes/phonopy/workflow.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/phonopy/wrapper.py` & `fhi-vibes-1.0.5/vibes/phonopy/wrapper.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/relaxation/_defaults.py` & `fhi-vibes-1.0.5/vibes/relaxation/_defaults.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/relaxation/context.py` & `fhi-vibes-1.0.5/vibes/relaxation/context.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/relaxation/workflow.py` & `fhi-vibes-1.0.5/vibes/relaxation/workflow.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/settings.py` & `fhi-vibes-1.0.5/vibes/settings.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/slurm/generate.py` & `fhi-vibes-1.0.5/vibes/slurm/generate.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/slurm/render.py` & `fhi-vibes-1.0.5/vibes/slurm/render.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/slurm/submit.py` & `fhi-vibes-1.0.5/vibes/slurm/submit.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/son.py` & `fhi-vibes-1.0.5/vibes/son.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/spglib/q_mesh.py` & `fhi-vibes-1.0.5/vibes/spglib/q_mesh.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/spglib/wrapper.py` & `fhi-vibes-1.0.5/vibes/spglib/wrapper.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/structure/convert.py` & `fhi-vibes-1.0.5/vibes/structure/convert.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/structure/io.py` & `fhi-vibes-1.0.5/vibes/structure/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """read, format, and write structures and inform about them"""
 
 import datetime
 
 import numpy as np
 
 from vibes.helpers.brillouinzone import get_special_points
-from vibes.helpers.geometry import get_cubicness, inscribed_sphere_in_box
+from vibes.helpers.geometry import (
+    get_cubicness,
+    inscribed_sphere_in_box,
+    bounding_sphere_of_box,
+)
 from vibes.helpers.numerics import clean_matrix
 from vibes.helpers.utils import talk
 from vibes.konstanten import n_geom_digits, symprec, v_unit
 from vibes.spglib.wrapper import get_symmetry_dataset
 from vibes.structure.misc import get_sysname
 
 
@@ -153,17 +157,19 @@
     print(f"  Species:           {msg}")
     print(f"  Periodicity:       {atoms.pbc}")
     if verbosity > 0 and any(atoms.pbc):
         print(f"  Lattice:  ")
         for vec in atoms.cell:
             print(f"    {vec}")
         cub = get_cubicness(atoms.cell)
-        print(f"  Cubicness:         {cub:.3f} ({cub**3:.3f})")
-        sh = inscribed_sphere_in_box(atoms.cell)
-        print(f"  Largest Cutoff:    {sh:.3f} AA")
+        print(f"  Cubicness:           {cub:.3f} ({cub**3:.3f})")
+        r = inscribed_sphere_in_box(atoms.cell)
+        print(f"  Largest Cutoff:      {r:.3f} AA")
+        r = bounding_sphere_of_box(atoms.cell)
+        print(f"  Bounding box rad.:   {r/2:.3f} AA")
 
     print("")
 
     if symprec is not None:
         sds = get_symmetry_dataset(atoms, symprec=symprec)
 
         print(f"  Spacegroup:          {sds.international} ({sds.number})")
```

### Comparing `fhi-vibes-1.0.4/vibes/structure/misc.py` & `fhi-vibes-1.0.5/vibes/structure/misc.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/tdep/wrapper.py` & `fhi-vibes-1.0.5/vibes/tdep/wrapper.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/templates/config_files/fireworksrc.template` & `fhi-vibes-1.0.5/vibes/templates/config_files/fireworksrc.template`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/templates/settings/aims_full` & `fhi-vibes-1.0.5/vibes/templates/settings/aims_full`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/README.md` & `fhi-vibes-1.0.5/vibes/trajectory/README.md`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/analysis.py` & `fhi-vibes-1.0.5/vibes/trajectory/analysis.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/dataset.py` & `fhi-vibes-1.0.5/vibes/trajectory/dataset.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/heat_flux.py` & `fhi-vibes-1.0.5/vibes/trajectory/heat_flux.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/io.py` & `fhi-vibes-1.0.5/vibes/trajectory/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         "metadata": map_metadata,
         "single_point_calculator": single_point_calculator,
     }
     list = _map_create_atoms(pre_trajectory, **kw)
     trajectory = Trajectory(list, metadata=metadata)
     timer2()
 
-    timer3 = Timer(".. set raw hash")
+    timer3 = Timer(".. set raw hash", verbose=verbose)
     trajectory.hash_raw = hash_file(file)
     timer3()
 
     timer("done")
 
     if fc_file:
         fc = io.parse_force_constants(fc_file, two_dim=False)
```

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/plotting.py` & `fhi-vibes-1.0.5/vibes/trajectory/plotting.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/trajectory.py` & `fhi-vibes-1.0.5/vibes/trajectory/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 dct = dct["atoms"]
             return dict2atoms(dct)
         if self.debug:
             warn("primitive cell not provided in trajectory metadata")
 
     @primitive.setter
     def primitive(self, atoms):
-        """ Set the supercell atoms object """
+        """ Set the primitive atoms object """
         assert isinstance(atoms, Atoms)
         dct = atoms2dict(atoms)
         self.metadata["primitive"] = dct
         talk(".. primitive added to metadata.")
 
     @property
     def supercell(self):
```

### Comparing `fhi-vibes-1.0.4/vibes/trajectory/utils.py` & `fhi-vibes-1.0.5/vibes/trajectory/utils.py`

 * *Files identical despite different names*

### Comparing `fhi-vibes-1.0.4/setup.py` & `fhi-vibes-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,30 +39,30 @@
  'vibes.templates.settings',
  'vibes.trajectory']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ase>=3.20.0,<3.23',
+['ase>=3.20.0,<4.0.0',
  'attrs>=19.1',
  'click>=8.0',
  'click_aliases>=1.0',
  'click_completion>=0.5.2',
  'jconfigparser>=0.1.2,<0.2.0',
  'jinja2>=2.10',
  'matplotlib>=3.1,<4.0',
  'netCDF4>=1.5',
  'numpy>=1.17.5,<2.0.0',
- 'pandas>=1.0',
+ 'pandas>=1.0,<2.0',
  'phonopy>=2.6,<3.0',
  'scipy>=1.1.1,<2.0.0',
  'seaborn>=0.11.0',
  'son>=0.4.1,<0.5.0',
- 'spglib>=1.12,<2.0',
+ 'spglib>=1.12',
  'tables>=3.5,<4.0',
  'xarray>=0.13']
 
 extras_require = \
 {':python_full_version >= "3.6.0" and python_full_version < "3.7.0"': ['importlib_resources',
                                                                        'dataclasses'],
  'fireworks': ['fireworks>=1.9,<2.0',
@@ -76,17 +76,17 @@
  'postgresql': ['psycopg2>=2.8.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['vibes = vibes.cli:cli']}
 
 setup_kwargs = {
     'name': 'fhi-vibes',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'Fritz Haber Institute Vibrational Simulations',
-    'long_description': 'FHI-vibes\n===\n\nWelcome to `FHI-vibes`, a `python` package for calculating, analyzing, and understanding the vibrational properties of solids from first principles. `FHI-vibes` is intended to seamlessly bridge between the harmonic approximation and fully anharmonic molecular dynamics simulations. To this end, `FHI-vibes` builds on several [existing packages](https://vibes-developers.gitlab.io/vibes/Credits/) and interfaces them in a consistent and user-friendly fashion. \n\nIn the documentation and tutorials, knowledge of first-principles electronic-structure theory as well as proficiency with _ab initio_ codes such as [FHI-aims](https://aimsclub.fhi-berlin.mpg.de/) and high-performance computing are assumed. Additional experience with Python, the [Atomic Simulation Environment (ASE)](https://wiki.fysik.dtu.dk/ase/), or [Phonopy](https://atztogo.github.io/phonopy/) is helpful, but not needed.\n\n`FHI-vibes` provides the following features:\n\n- Geometry optimization via [ASE](https://wiki.fysik.dtu.dk/ase/ase/optimize.html#module-ase.optimize),\n- harmonic phonon calculations via [Phonopy](https://atztogo.github.io/phonopy/),\n- molecular dynamics simulations in [NVE](https://wiki.fysik.dtu.dk/ase/ase/md.html#constant-nve-simulations-the-microcanonical-ensemble), [NVT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.langevin), and [NPT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.nptberendsen) ensembles,\n- [harmonic sampling](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.96.115504), and\n- [anharmonicity quantification](https://journals.aps.org/prmaterials/abstract/10.1103/PhysRevMaterials.4.083809).\n\nMost of the functionality is high-throughput ready via [fireworks](https://materialsproject.github.io/fireworks/#).\n\n## Overview\n\n- [Installation](https://vibes-developers.gitlab.io/vibes/Installation)\n- [Tutorial](https://vibes-developers.gitlab.io/vibes/Tutorial/0_intro)\n- [Documentation](https://vibes-developers.gitlab.io/vibes/Documentation/0_intro)\n- [Credits](https://vibes-developers.gitlab.io/vibes/Credits)\n- [References](https://vibes-developers.gitlab.io/vibes/References)\n\n\n## News\n\n- `FHI-vibes` got [published in JOSS](https://joss.theoj.org/papers/10.21105/joss.02671)!\n- [Our anharmonicity measure got published!](https://journals.aps.org/prmaterials/abstract/10.1103/PhysRevMaterials.4.083809)\n- [… the best is yet to come.](https://www.youtube.com/watch?v=B-Jq26BCwDs)\n\n## Changelog\n\n#### v1.0.4\n\n- looser dependencies\n- [various bug fixes](https://gitlab.com/vibes-developers/vibes/-/merge_requests?scope=all&state=merged)\n\n#### v1.0.3\n\n- update dependencies to allow `phonopy` versions up to 2.8\n\n#### v1.0.2\n\n- First official release after passing the [JOSS review](https://github.com/openjournals/joss-reviews/issues/2671).\n- Several additions to the documentation.\n\n#### v1.0.0a10\n\n- Enable conversion of trajectories to `ase.io.Trajectory` files for viewing with ASE [(!37)](https://gitlab.com/vibes-developers/vibes/-/merge_requests/37)\n- Important fix for running NPT dynamics [(!36)](https://gitlab.com/vibes-developers/vibes/-/merge_requests/36)\n- We have a changelog now!\n',
+    'long_description': 'FHI-vibes\n===\n\nWelcome to `FHI-vibes`, a `python` package for calculating, analyzing, and understanding the vibrational properties of solids from first principles. `FHI-vibes` is intended to seamlessly bridge between the harmonic approximation and fully anharmonic molecular dynamics simulations. To this end, `FHI-vibes` builds on several [existing packages](https://vibes-developers.gitlab.io/vibes/Credits/) and interfaces them in a consistent and user-friendly fashion. \n\nIn the documentation and tutorials, knowledge of first-principles electronic-structure theory as well as proficiency with _ab initio_ codes such as [FHI-aims](https://aimsclub.fhi-berlin.mpg.de/) and high-performance computing are assumed. Additional experience with Python, the [Atomic Simulation Environment (ASE)](https://wiki.fysik.dtu.dk/ase/), or [Phonopy](https://atztogo.github.io/phonopy/) is helpful, but not needed.\n\n`FHI-vibes` provides the following features:\n\n- Geometry optimization via [ASE](https://wiki.fysik.dtu.dk/ase/ase/optimize.html#module-ase.optimize),\n- harmonic phonon calculations via [Phonopy](https://atztogo.github.io/phonopy/),\n- molecular dynamics simulations in [NVE](https://wiki.fysik.dtu.dk/ase/ase/md.html#constant-nve-simulations-the-microcanonical-ensemble), [NVT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.langevin), and [NPT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.nptberendsen) ensembles,\n- [harmonic sampling](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.96.115504), and\n- [anharmonicity quantification](https://journals.aps.org/prmaterials/abstract/10.1103/PhysRevMaterials.4.083809).\n\nMost of the functionality is high-throughput ready via [fireworks](https://materialsproject.github.io/fireworks/#).\n\nA reference implementation of the [ab initio Green Kubo method](https://arxiv.org/abs/2209.01139) is [available](https://gitlab.com/vibes-developers/vibes/-/merge_requests/57). However, we ask you to contact the developers before using this functionality as it requires extra instructions.\n\n## Overview\n\n- [Installation](https://vibes-developers.gitlab.io/vibes/Installation)\n- [Tutorial](https://vibes-developers.gitlab.io/vibes/Tutorial/0_intro)\n- [Documentation](https://vibes-developers.gitlab.io/vibes/Documentation/0_intro)\n- [Credits](https://vibes-developers.gitlab.io/vibes/Credits)\n- [References](https://vibes-developers.gitlab.io/vibes/References)\n\n## Changelog\n\n#### v1.0.5\n\n- bugfix\n\n#### v1.0.4\n\n- looser dependencies\n- [various bug fixes](https://gitlab.com/vibes-developers/vibes/-/merge_requests?scope=all&state=merged)\n\n#### v1.0.3\n\n- update dependencies to allow `phonopy` versions up to 2.8\n\n#### v1.0.2\n\n- First official release after passing the [JOSS review](https://github.com/openjournals/joss-reviews/issues/2671).\n- Several additions to the documentation.\n\n#### v1.0.0a10\n\n- Enable conversion of trajectories to `ase.io.Trajectory` files for viewing with ASE [(!37)](https://gitlab.com/vibes-developers/vibes/-/merge_requests/37)\n- Important fix for running NPT dynamics [(!36)](https://gitlab.com/vibes-developers/vibes/-/merge_requests/36)\n- We have a changelog now!\n',
     'author': 'Florian Knoop',
     'author_email': 'knoop@fhi-berlin.mpg.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/vibes-developers/vibes',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fhi-vibes-1.0.4/PKG-INFO` & `fhi-vibes-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhi-vibes
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fritz Haber Institute Vibrational Simulations
 Home-page: https://gitlab.com/vibes-developers/vibes
 License: MIT
 Keywords: physics
 Author: Florian Knoop
 Author-email: knoop@fhi-berlin.mpg.de
 Requires-Python: >=3.6.1,<4.0.0
@@ -14,41 +14,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: fireworks
 Provides-Extra: hiphive
 Provides-Extra: phono3py
 Provides-Extra: postgresql
-Requires-Dist: ase (>=3.20.0,<3.23)
+Requires-Dist: ase (>=3.20.0,<4.0.0)
 Requires-Dist: attrs (>=19.1)
 Requires-Dist: click (>=8.0)
 Requires-Dist: click_aliases (>=1.0)
 Requires-Dist: click_completion (>=0.5.2)
 Requires-Dist: dataclasses; python_full_version >= "3.6.0" and python_full_version < "3.7.0"
 Requires-Dist: fabric (>=2.4,<3.0); extra == "fireworks"
 Requires-Dist: fireworks (>=1.9,<2.0); extra == "fireworks"
 Requires-Dist: hiphive (>=0.5.0,<0.6.0); extra == "hiphive"
 Requires-Dist: importlib_resources; python_full_version >= "3.6.0" and python_full_version < "3.7.0"
 Requires-Dist: jconfigparser (>=0.1.2,<0.2.0)
 Requires-Dist: jinja2 (>=2.10)
 Requires-Dist: matplotlib (>=3.1,<4.0)
 Requires-Dist: netCDF4 (>=1.5)
 Requires-Dist: numpy (>=1.17.5,<2.0.0)
-Requires-Dist: pandas (>=1.0)
+Requires-Dist: pandas (>=1.0,<2.0)
 Requires-Dist: paramiko (>=2.4,<3.0); extra == "fireworks"
 Requires-Dist: phono3py (>=1.21,<2.0); extra == "phono3py"
 Requires-Dist: phonopy (>=2.6,<3.0)
 Requires-Dist: psycopg2 (>=2.8.0,<3.0.0); extra == "postgresql"
 Requires-Dist: pymongo (>=3.8,<4.0); extra == "fireworks"
 Requires-Dist: python-gssapi (>=0.6.4,<0.7.0); extra == "fireworks"
 Requires-Dist: requests (>=2.25,<3.0); extra == "fireworks"
 Requires-Dist: scipy (>=1.1.1,<2.0.0)
 Requires-Dist: seaborn (>=0.11.0)
 Requires-Dist: son (>=0.4.1,<0.5.0)
-Requires-Dist: spglib (>=1.12,<2.0)
+Requires-Dist: spglib (>=1.12)
 Requires-Dist: tables (>=3.5,<4.0)
 Requires-Dist: xarray (>=0.13)
 Project-URL: Repository, https://gitlab.com/vibes-developers/vibes
 Description-Content-Type: text/markdown
 
 FHI-vibes
 ===
@@ -63,30 +63,29 @@
 - harmonic phonon calculations via [Phonopy](https://atztogo.github.io/phonopy/),
 - molecular dynamics simulations in [NVE](https://wiki.fysik.dtu.dk/ase/ase/md.html#constant-nve-simulations-the-microcanonical-ensemble), [NVT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.langevin), and [NPT](https://wiki.fysik.dtu.dk/ase/ase/md.html#module-ase.md.nptberendsen) ensembles,
 - [harmonic sampling](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.96.115504), and
 - [anharmonicity quantification](https://journals.aps.org/prmaterials/abstract/10.1103/PhysRevMaterials.4.083809).
 
 Most of the functionality is high-throughput ready via [fireworks](https://materialsproject.github.io/fireworks/#).
 
+A reference implementation of the [ab initio Green Kubo method](https://arxiv.org/abs/2209.01139) is [available](https://gitlab.com/vibes-developers/vibes/-/merge_requests/57). However, we ask you to contact the developers before using this functionality as it requires extra instructions.
+
 ## Overview
 
 - [Installation](https://vibes-developers.gitlab.io/vibes/Installation)
 - [Tutorial](https://vibes-developers.gitlab.io/vibes/Tutorial/0_intro)
 - [Documentation](https://vibes-developers.gitlab.io/vibes/Documentation/0_intro)
 - [Credits](https://vibes-developers.gitlab.io/vibes/Credits)
 - [References](https://vibes-developers.gitlab.io/vibes/References)
 
+## Changelog
 
-## News
-
-- `FHI-vibes` got [published in JOSS](https://joss.theoj.org/papers/10.21105/joss.02671)!
-- [Our anharmonicity measure got published!](https://journals.aps.org/prmaterials/abstract/10.1103/PhysRevMaterials.4.083809)
-- [… the best is yet to come.](https://www.youtube.com/watch?v=B-Jq26BCwDs)
+#### v1.0.5
 
-## Changelog
+- bugfix
 
 #### v1.0.4
 
 - looser dependencies
 - [various bug fixes](https://gitlab.com/vibes-developers/vibes/-/merge_requests?scope=all&state=merged)
 
 #### v1.0.3
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

