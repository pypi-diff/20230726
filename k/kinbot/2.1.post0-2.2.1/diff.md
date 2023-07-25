# Comparing `tmp/kinbot-2.1.post0.tar.gz` & `tmp/kinbot-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinbot-2.1.post0.tar", last modified: Fri Jan  6 19:46:58 2023, max compression
+gzip compressed data, was "kinbot-2.2.1.tar", last modified: Tue Jul 25 22:03:10 2023, max compression
```

## Comparing `kinbot-2.1.post0.tar` & `kinbot-2.2.1.tar`

### file list

```diff
@@ -1,177 +1,190 @@
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.379540 kinbot-2.1.post0/
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.254643 kinbot-2.1.post0/KinBot.egg-info/
--rw-r--r--   0 cmartia  (129185) 694259999    10804 2023-01-06 19:46:58.000000 kinbot-2.1.post0/KinBot.egg-info/PKG-INFO
--rw-r--r--   0 cmartia  (129185) 694259999     4681 2023-01-06 19:46:58.000000 kinbot-2.1.post0/KinBot.egg-info/SOURCES.txt
--rw-r--r--   0 cmartia  (129185) 694259999        1 2023-01-06 19:46:58.000000 kinbot-2.1.post0/KinBot.egg-info/dependency_links.txt
--rw-r--r--   0 cmartia  (129185) 694259999       64 2023-01-06 19:46:58.000000 kinbot-2.1.post0/KinBot.egg-info/entry_points.txt
--rw-r--r--   0 cmartia  (129185) 694259999       87 2023-01-06 19:46:58.000000 kinbot-2.1.post0/KinBot.egg-info/requires.txt
--rw-r--r--   0 cmartia  (129185) 694259999       51 2023-01-06 19:46:58.000000 kinbot-2.1.post0/KinBot.egg-info/top_level.txt
--rw-r--r--   0 cmartia  (129185) 694259999     1508 2022-02-16 23:12:29.000000 kinbot-2.1.post0/LICENSE
--rw-r--r--   0 cmartia  (129185) 694259999    10804 2023-01-06 19:46:58.379071 kinbot-2.1.post0/PKG-INFO
--rw-r--r--   0 cmartia  (129185) 694259999     8073 2023-01-05 23:13:56.000000 kinbot-2.1.post0/README.md
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.285772 kinbot-2.1.post0/kinbot/
--rw-r--r--   0 cmartia  (129185) 694259999      988 2022-02-16 23:12:29.000000 kinbot-2.1.post0/kinbot/__init__.py
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.289022 kinbot-2.1.post0/kinbot/ase_modules/
--rw-r--r--   0 cmartia  (129185) 694259999        0 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/__init__.py
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.291670 kinbot-2.1.post0/kinbot/ase_modules/calculators/
--rw-r--r--   0 cmartia  (129185) 694259999        0 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/calculators/__init__.py
--rw-r--r--   0 cmartia  (129185) 694259999     4193 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/calculators/gaussian.py
--rw-r--r--   0 cmartia  (129185) 694259999     7274 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/calculators/qchem.py
--rw-r--r--   0 cmartia  (129185) 694259999   101469 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/constraints.py
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.295368 kinbot-2.1.post0/kinbot/ase_modules/io/
--rw-r--r--   0 cmartia  (129185) 694259999        0 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/io/__init__.py
--rw-r--r--   0 cmartia  (129185) 694259999    31889 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/io/formats.py
--rw-r--r--   0 cmartia  (129185) 694259999    50748 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/io/gaussian.py
--rw-r--r--   0 cmartia  (129185) 694259999     9177 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/ase_modules/io/zmatrix.py
--rw-r--r--   0 cmartia  (129185) 694259999     4037 2022-02-16 23:12:29.000000 kinbot-2.1.post0/kinbot/bfgs.py
--rw-r--r--   0 cmartia  (129185) 694259999    10140 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/bond_combinations.py
--rw-r--r--   0 cmartia  (129185) 694259999     7846 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/cheminfo.py
--rw-r--r--   0 cmartia  (129185) 694259999    29330 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/conformers.py
--rw-r--r--   0 cmartia  (129185) 694259999     3283 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/constants.py
--rw-r--r--   0 cmartia  (129185) 694259999     1349 2022-02-16 23:12:29.000000 kinbot-2.1.post0/kinbot/exceptions.py
--rw-r--r--   0 cmartia  (129185) 694259999     4022 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/find_motif.py
--rw-r--r--   0 cmartia  (129185) 694259999     8464 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/frequencies.py
--rw-r--r--   0 cmartia  (129185) 694259999    11495 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/geometry.py
--rw-r--r--   0 cmartia  (129185) 694259999    11003 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/hindered_rotors.py
--rw-r--r--   0 cmartia  (129185) 694259999     7366 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/irc.py
--rw-r--r--   0 cmartia  (129185) 694259999    11673 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/kb.py
--rw-r--r--   0 cmartia  (129185) 694259999      218 2022-02-16 23:12:29.000000 kinbot-2.1.post0/kinbot/license_message.py
--rw-r--r--   0 cmartia  (129185) 694259999    17775 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/mesmer.py
--rw-r--r--   0 cmartia  (129185) 694259999    45085 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/mess.py
--rw-r--r--   0 cmartia  (129185) 694259999    17471 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/modify_geom.py
--rw-r--r--   0 cmartia  (129185) 694259999     8439 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/molpro.py
--rw-r--r--   0 cmartia  (129185) 694259999    30760 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/optimize.py
--rw-r--r--   0 cmartia  (129185) 694259999     3931 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/orca.py
--rw-r--r--   0 cmartia  (129185) 694259999    17053 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/parameters.py
--rw-r--r--   0 cmartia  (129185) 694259999    61981 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/pes.py
--rw-r--r--   0 cmartia  (129185) 694259999    10001 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/postprocess.py
--rw-r--r--   0 cmartia  (129185) 694259999    40688 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/qc.py
--rw-r--r--   0 cmartia  (129185) 694259999     5628 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/reac_General.py
--rw-r--r--   0 cmartia  (129185) 694259999     7986 2023-01-05 17:16:03.000000 kinbot-2.1.post0/kinbot/reac_family.py
--rw-r--r--   0 cmartia  (129185) 694259999    97491 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/reaction_finder.py
--rw-r--r--   0 cmartia  (129185) 694259999     8830 2023-01-05 17:21:25.000000 kinbot-2.1.post0/kinbot/reaction_finder_bimol.py
--rw-r--r--   0 cmartia  (129185) 694259999    42519 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/reaction_generator.py
--rw-r--r--   0 cmartia  (129185) 694259999     7308 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/reader_gauss.py
--rw-r--r--   0 cmartia  (129185) 694259999     7309 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/reader_qchem.py
--rw-r--r--   0 cmartia  (129185) 694259999    35243 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/stationary_pt.py
--rw-r--r--   0 cmartia  (129185) 694259999    11294 2022-03-10 22:26:21.000000 kinbot-2.1.post0/kinbot/symmetry.py
--rw-r--r--   0 cmartia  (129185) 694259999     2566 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/thread_kinbot.py
--rw-r--r--   0 cmartia  (129185) 694259999     2920 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/uncertaintyAnalysis.py
--rw-r--r--   0 cmartia  (129185) 694259999     4544 2023-01-05 23:13:56.000000 kinbot-2.1.post0/kinbot/utils.py
--rw-r--r--   0 cmartia  (129185) 694259999    43867 2022-11-23 00:24:36.000000 kinbot-2.1.post0/kinbot/zmatrix.py
--rw-r--r--   0 cmartia  (129185) 694259999     1586 2023-01-06 19:46:01.000000 kinbot-2.1.post0/pyproject.toml
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.326480 kinbot-2.1.post0/reactions/
--rw-r--r--   0 cmartia  (129185) 694259999      988 2022-02-16 23:12:29.000000 kinbot-2.1.post0/reactions/__init__.py
--rw-r--r--   0 cmartia  (129185) 694259999     1035 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_12_shift_S_F.py
--rw-r--r--   0 cmartia  (129185) 694259999     1027 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_12_shift_S_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     1000 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Cyclic_Ether_Formation.py
--rw-r--r--   0 cmartia  (129185) 694259999      560 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Diels_alder_addition.py
--rw-r--r--   0 cmartia  (129185) 694259999     1059 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_HO2_Elimination_from_PeroxyRadical.py
--rw-r--r--   0 cmartia  (129185) 694259999     1446 2022-11-23 00:24:36.000000 kinbot-2.1.post0/reactions/reac_Intra_Diels_alder_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     1329 2022-11-23 00:24:36.000000 kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Endocyclic_F.py
--rw-r--r--   0 cmartia  (129185) 694259999      835 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Endocyclic_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     1354 2022-11-23 00:24:36.000000 kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Exocyclic_F.py
--rw-r--r--   0 cmartia  (129185) 694259999      960 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Exocyclic_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     3512 2022-11-23 00:24:36.000000 kinbot-2.1.post0/reactions/reac_Intra_R_Add_Endocyclic_F.py
--rw-r--r--   0 cmartia  (129185) 694259999     2245 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Intra_R_Add_ExoTetCyclic_F.py
--rw-r--r--   0 cmartia  (129185) 694259999     1149 2022-11-23 00:24:36.000000 kinbot-2.1.post0/reactions/reac_Intra_R_Add_Exocyclic_F.py
--rw-r--r--   0 cmartia  (129185) 694259999      854 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Intra_disproportionation_F.py
--rw-r--r--   0 cmartia  (129185) 694259999      847 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Intra_disproportionation_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     1912 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Korcek_step2.py
--rw-r--r--   0 cmartia  (129185) 694259999     1112 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Korcek_step2_even.py
--rw-r--r--   0 cmartia  (129185) 694259999     1260 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Korcek_step2_odd.py
--rw-r--r--   0 cmartia  (129185) 694259999      512 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_R_Addition_COm3_R.py
--rw-r--r--   0 cmartia  (129185) 694259999      511 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_R_Addition_CSm_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     4353 2022-11-23 00:24:36.000000 kinbot-2.1.post0/reactions/reac_R_Addition_MultipleBond.py
--rw-r--r--   0 cmartia  (129185) 694259999      892 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_Retro_Ene.py
--rw-r--r--   0 cmartia  (129185) 694259999     2693 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_abstraction.py
--rw-r--r--   0 cmartia  (129185) 694259999      796 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_barrierless_saddle.py
--rw-r--r--   0 cmartia  (129185) 694259999     3212 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_beta_delta.py
--rw-r--r--   0 cmartia  (129185) 694259999      789 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_birad_recombination_F.py
--rw-r--r--   0 cmartia  (129185) 694259999      608 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_birad_recombination_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     5893 2022-02-16 23:12:29.000000 kinbot-2.1.post0/reactions/reac_combinatorial.py
--rw-r--r--   0 cmartia  (129185) 694259999      698 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_cpd_H_migration.py
--rw-r--r--   0 cmartia  (129185) 694259999     1031 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_h2_elim.py
--rw-r--r--   0 cmartia  (129185) 694259999      383 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_homolytic_scission.py
--rw-r--r--   0 cmartia  (129185) 694259999     4381 2022-11-23 00:24:36.000000 kinbot-2.1.post0/reactions/reac_intra_H_migration.py
--rw-r--r--   0 cmartia  (129185) 694259999     1741 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_intra_H_migration_suprafacial.py
--rw-r--r--   0 cmartia  (129185) 694259999     1072 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_intra_OH_migration.py
--rw-r--r--   0 cmartia  (129185) 694259999     2326 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_intra_OH_migration_Exocyclic_F.py
--rw-r--r--   0 cmartia  (129185) 694259999     1590 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_intra_R_migration.py
--rw-r--r--   0 cmartia  (129185) 694259999      963 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_ketoenol.py
--rw-r--r--   0 cmartia  (129185) 694259999      716 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r12_cycloaddition.py
--rw-r--r--   0 cmartia  (129185) 694259999     1157 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r12_insertion_R.py
--rw-r--r--   0 cmartia  (129185) 694259999     1178 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r13_insertion_CO2.py
--rw-r--r--   0 cmartia  (129185) 694259999     1156 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r13_insertion_ROR.py
--rw-r--r--   0 cmartia  (129185) 694259999     1173 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r13_insertion_RSR.py
--rw-r--r--   0 cmartia  (129185) 694259999      580 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r14_birad_scission.py
--rw-r--r--   0 cmartia  (129185) 694259999      784 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r14_cyclic_birad_scission_R.py
--rw-r--r--   0 cmartia  (129185) 694259999      592 2022-03-10 22:26:21.000000 kinbot-2.1.post0/reactions/reac_r22_cycloaddition.py
--rw-r--r--   0 cmartia  (129185) 694259999       38 2023-01-06 19:46:58.379667 kinbot-2.1.post0/setup.cfg
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.337912 kinbot-2.1.post0/tests/
--rw-r--r--   0 cmartia  (129185) 694259999      988 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/__init__.py
--rw-r--r--   0 cmartia  (129185) 694259999     2204 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/bfgs.py
--rw-r--r--   0 cmartia  (129185) 694259999     6336 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/cheminfo.py
--rw-r--r--   0 cmartia  (129185) 694259999     2387 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/dihedrals.py
--rw-r--r--   0 cmartia  (129185) 694259999     6116 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/find_motif.py
--rw-r--r--   0 cmartia  (129185) 694259999    36092 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/frequencies.py
--rw-r--r--   0 cmartia  (129185) 694259999    11199 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/geometry.py
--rw-r--r--   0 cmartia  (129185) 694259999     6108 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/modify_geom.py
--rw-r--r--   0 cmartia  (129185) 694259999     2159 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/multimolecular.py
--rw-r--r--   0 cmartia  (129185) 694259999     2119 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/resonance.py
--rw-r--r--   0 cmartia  (129185) 694259999     2617 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/symmetry.py
--rw-r--r--   0 cmartia  (129185) 694259999     3663 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tests/test_kinbot.py
-drwxr-xr-x   0 cmartia  (129185) 694259999        0 2023-01-06 19:46:58.378384 kinbot-2.1.post0/tpl/
--rw-r--r--   0 cmartia  (129185) 694259999      988 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/__init__.py
--rw-r--r--   0 cmartia  (129185) 694259999      973 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/arrow.png
--rw-r--r--   0 cmartia  (129185) 694259999     1301 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_gauss_hir.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     2521 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_gauss_irc.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1893 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_gauss_opt_well.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1225 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_gauss_ring_conf.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1715 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_gauss_ts_end.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     2174 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_gauss_ts_search.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1983 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/ase_nwchem_freq_well.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     2100 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_nwchem_irc.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1657 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/ase_nwchem_opt_well.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     2474 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/ase_nwchem_ts_end.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1941 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/ase_nwchem_ts_search.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     3175 2023-01-05 23:13:56.000000 kinbot-2.1.post0/tpl/ase_nwchem_ts_search_ase_constraints.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1035 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/ase_qchem_hir.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     2345 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/ase_qchem_irc.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     2181 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/ase_qchem_opt_well.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1901 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/ase_qchem_ts_end.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999     1622 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/ase_qchem_ts_search.tpl.py
--rw-r--r--   0 cmartia  (129185) 694259999       42 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/mess_2tst.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      171 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_atom.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       81 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/mess_barrier.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      148 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_barrier_union.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      612 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_barrierless.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      110 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_bimol.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       76 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/mess_core_rr.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      435 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_dummy.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      360 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_fragment.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      347 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_fragment_OH.tpl
--rw-r--r--   0 cmartia  (129185) 694259999     1165 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_header.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      267 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_hinderedrotor.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      272 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/mess_outerrrho.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      481 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_pst.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       87 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/mess_pstfragment.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      266 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_rrho.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      133 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/mess_termol.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      206 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_tunneling.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       81 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/mess_variational.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      414 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_well.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      141 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/mess_well_union.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      299 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/molpro.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      190 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/pbs.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       44 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/pbs_mesmer.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       40 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/pbs_mess.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       43 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/pbs_mess_uq.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       29 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/pbs_molpro.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       56 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/pbs_python.tpl
--rw-r--r--   0 cmartia  (129185) 694259999     3093 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/pesviewer.inp.tpl
--rw-r--r--   0 cmartia  (129185) 694259999      189 2022-11-23 00:24:36.000000 kinbot-2.1.post0/tpl/slurm.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       19 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/slurm_mesmer.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       22 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/slurm_mess_uq.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       22 2022-08-10 16:55:58.000000 kinbot-2.1.post0/tpl/slurm_molpro.tpl
--rw-r--r--   0 cmartia  (129185) 694259999       33 2022-02-16 23:12:29.000000 kinbot-2.1.post0/tpl/slurm_python.tpl
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.192429 kinbot-2.2.1/
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.097986 kinbot-2.2.1/KinBot.egg-info/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11569 2023-07-25 22:03:10.000000 kinbot-2.2.1/KinBot.egg-info/PKG-INFO
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5803 2023-07-25 22:03:10.000000 kinbot-2.2.1/KinBot.egg-info/SOURCES.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        1 2023-07-25 22:03:10.000000 kinbot-2.2.1/KinBot.egg-info/dependency_links.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       64 2023-07-25 22:03:10.000000 kinbot-2.2.1/KinBot.egg-info/entry_points.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       76 2023-07-25 22:03:10.000000 kinbot-2.2.1/KinBot.egg-info/requires.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       22 2023-07-25 22:03:10.000000 kinbot-2.2.1/KinBot.egg-info/top_level.txt
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1508 2022-02-16 23:12:29.000000 kinbot-2.2.1/LICENSE
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11569 2023-07-25 22:03:10.191845 kinbot-2.2.1/PKG-INFO
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8791 2023-07-13 20:15:45.000000 kinbot-2.2.1/README.md
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.120249 kinbot-2.2.1/kinbot/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1011 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/__init__.py
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.122307 kinbot-2.2.1/kinbot/ase_modules/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/__init__.py
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.123865 kinbot-2.2.1/kinbot/ase_modules/calculators/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/calculators/__init__.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4193 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/calculators/gaussian.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7274 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/calculators/qchem.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)   101469 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/constraints.py
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.126138 kinbot-2.2.1/kinbot/ase_modules/io/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/io/__init__.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    31889 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/io/formats.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    50748 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/io/gaussian.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     9177 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/ase_modules/io/zmatrix.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4037 2022-02-16 23:12:29.000000 kinbot-2.2.1/kinbot/bfgs.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10140 2023-03-06 20:04:33.000000 kinbot-2.2.1/kinbot/bond_combinations.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7879 2023-03-28 21:40:32.000000 kinbot-2.2.1/kinbot/cheminfo.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2178 2023-03-28 19:03:13.000000 kinbot-2.2.1/kinbot/config_log.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    29928 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/conformers.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3295 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/constants.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1349 2022-02-16 23:12:29.000000 kinbot-2.2.1/kinbot/exceptions.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4022 2023-03-06 20:04:33.000000 kinbot-2.2.1/kinbot/find_motif.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8838 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/frequencies.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11495 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/geometry.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11036 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/hindered_rotors.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8209 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/irc.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11604 2023-07-20 23:59:58.000000 kinbot-2.2.1/kinbot/kb.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      218 2022-02-16 23:12:29.000000 kinbot-2.2.1/kinbot/license_message.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    17617 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/mesmer.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    44596 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/mess.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    18001 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/modify_geom.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8477 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/molpro.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    31272 2023-07-24 19:08:19.000000 kinbot-2.2.1/kinbot/optimize.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3885 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/orca.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    18148 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/parameters.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    65967 2023-07-24 23:31:23.000000 kinbot-2.2.1/kinbot/pes.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    10469 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/postprocess.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    45146 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/qc.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5628 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reac_General.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8655 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reac_family.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)   100159 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reaction_finder.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8792 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reaction_finder_bimol.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    45393 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reaction_generator.py
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.152611 kinbot-2.2.1/kinbot/reactions/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      988 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/__init__.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1722 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reactions/reac_12_shift_S_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1568 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reactions/reac_12_shift_S_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1000 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Cyclic_Ether_Formation.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      560 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Diels_alder_addition.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1059 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_HO2_Elimination_from_PeroxyRadical.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1446 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_Diels_alder_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1329 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Endocyclic_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      835 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Endocyclic_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1354 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Exocyclic_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      960 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Exocyclic_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3512 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_R_Add_Endocyclic_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2797 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_R_Add_ExoTetCyclic_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1149 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_R_Add_Exocyclic_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      854 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_disproportionation_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      847 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Intra_disproportionation_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1912 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Korcek_step2.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1112 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Korcek_step2_even.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1260 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Korcek_step2_odd.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      512 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_R_Addition_COm3_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      511 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_R_Addition_CSm_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4353 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_R_Addition_MultipleBond.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      892 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_Retro_Ene.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2693 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_abstraction.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      796 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_barrierless_saddle.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3212 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_beta_delta.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      967 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reactions/reac_bimol_disproportionation_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      789 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_birad_recombination_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      608 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_birad_recombination_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     5893 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_combinatorial.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      698 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_cpd_H_migration.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1031 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_h2_elim.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      383 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_homolytic_scission.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4381 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_intra_H_migration.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1741 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_intra_H_migration_suprafacial.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1072 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_intra_OH_migration.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2326 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_intra_OH_migration_Exocyclic_F.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2124 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reactions/reac_intra_R_migration.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      963 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_ketoenol.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      716 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r12_cycloaddition.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1157 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r12_insertion_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1178 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r13_insertion_CO2.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1156 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r13_insertion_ROR.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1173 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r13_insertion_RSR.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      580 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r14_birad_scission.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      784 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r14_cyclic_birad_scission_R.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      592 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reactions/reac_r22_cycloaddition.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     8304 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/reader_gauss.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     7291 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/reader_qchem.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    37874 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/stationary_pt.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11294 2022-03-10 22:26:21.000000 kinbot-2.2.1/kinbot/symmetry.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2566 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/thread_kinbot.py
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.183219 kinbot-2.2.1/kinbot/tpl/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      988 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/__init__.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1246 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_gauss_hir.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3010 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_gauss_irc.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1838 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_gauss_opt_well.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1218 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_gauss_ring_conf.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1661 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_gauss_ts_end.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2103 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_gauss_ts_search.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1983 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_nwchem_freq_well.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2100 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_nwchem_irc.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1657 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_nwchem_opt_well.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2474 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_nwchem_ts_end.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1941 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_nwchem_ts_search.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3175 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_nwchem_ts_search_ase_constraints.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1035 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_qchem_hir.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2345 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_qchem_irc.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2181 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_qchem_opt_well.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1901 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_qchem_ts_end.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1622 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/ase_qchem_ts_search.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1051 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_sella_hir.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1818 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_sella_irc.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3630 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_sella_opt_well.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4351 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_sella_ring_conf.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2908 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_sella_ts_end.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1348 2023-07-13 20:15:45.000000 kinbot-2.2.1/kinbot/tpl/ase_sella_ts_search.tpl.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       22 2023-03-28 19:03:13.000000 kinbot-2.2.1/kinbot/tpl/local_molpro.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       42 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_2tst.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      171 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_atom.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       81 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_barrier.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      148 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_barrier_union.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      612 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_barrierless.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      110 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_bimol.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      110 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_bimol_union.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       76 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_core_rr.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      435 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_dummy.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      360 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_fragment.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      347 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_fragment_OH.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      215 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_freerotor.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1165 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_header.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      267 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_hinderedrotor.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      272 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_outerrrho.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      481 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_pst.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       87 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_pstfragment.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      266 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_rrho.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      133 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_termol.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      412 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_ts.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      206 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_tunneling.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       81 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_variational.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      414 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_well.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      141 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/mess_well_union.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      299 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/molpro.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      190 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/pbs.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       44 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/pbs_mesmer.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       40 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/pbs_mess.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       43 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/pbs_mess_uq.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       29 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/pbs_molpro.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       56 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/pbs_python.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3093 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/pesviewer.inp.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      209 2023-03-28 21:40:57.000000 kinbot-2.2.1/kinbot/tpl/slurm.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       19 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/slurm_mesmer.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       18 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/slurm_mess.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       22 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/slurm_mess_uq.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       22 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/slurm_molpro.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       40 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/slurm_orca.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       33 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/tpl/slurm_python.tpl
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2920 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/uncertaintyAnalysis.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     4582 2023-07-13 20:15:40.000000 kinbot-2.2.1/kinbot/utils.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    43900 2023-03-07 01:35:51.000000 kinbot-2.2.1/kinbot/zmatrix.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     1605 2023-07-25 21:49:54.000000 kinbot-2.2.1/pyproject.toml
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)       38 2023-07-25 22:03:10.192582 kinbot-2.2.1/setup.cfg
+drwxr-xr-x   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)        0 2023-07-25 22:03:10.190906 kinbot-2.2.1/tests/
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)      988 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/__init__.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2204 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/bfgs.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6336 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/cheminfo.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2387 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/dihedrals.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6116 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/find_motif.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    36092 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/frequencies.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)    11199 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/geometry.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     6108 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/modify_geom.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2159 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/multimolecular.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2119 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/resonance.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     2617 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/symmetry.py
+-rw-r--r--   0 cmartia  (129185) SANDIA-EON\Domain Users (694259999)     3663 2022-02-16 23:12:29.000000 kinbot-2.2.1/tests/test_kinbot.py
```

### Comparing `kinbot-2.1.post0/KinBot.egg-info/PKG-INFO` & `kinbot-2.2.1/KinBot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinbot
-Version: 2.1.post0
+Version: 2.2.1
 Summary: Automated reaction kinetics for gas-phase species
 Author-email: Judit Zádor <jzador@sandia.gov>, Ruben Vande Vijver <ruben.vandevijver@ugent.be>, Carles Martí <cmartia@sandia.gov>, Amanda Dewyer <adewyer@sandia.gov>
 Maintainer-email: Judit Zádor <jzador@sandia.gov>, Carles Martí <cmartia@sandia.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, zadorlab
         All rights reserved.
@@ -39,69 +39,73 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 License-File: LICENSE
 
 [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/zadorlab/KinBot)
 
-# KinBot: Automated reaction pathway search for gas-phase molecules
+# KinBot: Automated Reaction Kinetics of Gas-Phase Organic Species over Multiwell Potential Energy Surfaces
 
 <p>
-    <img src="graphics/kinbot_logo_V2.png" width="220" height="240" />
+    <img src="https://raw.githubusercontent.com/zadorlab/KinBot/master/graphics/kinbot_logo_V2.png" width="220" height="240" />
 </p>
 
 ## Description
 This repository contains the KinBot code version 2.0,
 a tool for automatically searching for reactions on the potential energy surface.
 
-If you are using this tool in scientific publications, please reference this git repo and the following publications:
+If you are using this tool in scientific publications, please reference the following publications:
 
 * Ruben Van de Vijver, Judit Zádor: KinBot: _Automated stationary point search on potential energy surfaces_, Comp. Phys. Comm., **2019**, 248, 106947. https://doi.org/10.1016/j.cpc.2019.106947
-* Judit Zádor, Carles Martí, Ruben Van de Vijver, Sommer L. Johansen, Yoona Yang, Hope A. Michelsen, Habib N. Najm, J. Phys. Chem. A, **2023**, ASAP. https://doi.org/10.1021/acs.jpca.2c06558
+* Judit Zádor, Carles Martí, Ruben Van de Vijver, Sommer L. Johansen, Yoona Yang, Hope A. Michelsen, Habib N. Najm: _Automated reaction kinetics of gas-phase organic species over multiwell potential energy surfaces_, J. Phys. Chem. A, **2023**, 127, 565–588. https://doi.org/10.1021/acs.jpca.2c06558
 
 We appreciate if you send us the DOI of your published paper that used KinBot, so we can feature it here below.
 
 ## How to Install
-Make sure all dependencies are correctly installed. The dependencies are lister here https://github.com/zadorlab/KinBot/wiki/Setting-Up-KinBot-on-Your-System 
 
-Clone the project to the place where you want to run it. Make sure you switch to the latest version, e.g., 2.0.5:
+KinBot can be installed both in three different ways, from the PyPI index (`pip install`), from the conda-forge repo (`conda install`) or by cloning this github repo and then install it locally.
 
-    git branch 2.0.5
+### PyPI
 
-You can find the latest stable version's tag if you click on the Branch button above on this page.
+    pip install kinbot
 
-In your local space go into the KinBot/ directory. Run the following:
+> **Note**
+>  KinBot only works with Python >= 3.8.
 
-    python setup.py build
-    python setup.py install
-    
-If you do not have admin priveleges, you might have to run
+### conda-forge
 
-    python setup.py build
-    python setup.py install --user
-    
-Moreover, if you plan to modify the code, you need to install it as:
+    conda install -c conda-forge kinbot
 
-    python setup.py build
-    python setup.py develop --user
-    
-Please note that you will need the ase version linked to at https://github.com/zadorlab/ase installed
-and linked to in your path during the installation of KinBot. This version of ase has changes within it that
-are local to KinBot, using any other ase versions will likely result in errors when trying to run reaction searches.
+### From Github
+
+If you want to have the very last version of KinBot without waiting for a 
+release or you want to modify KinBot acccording to your needs you can clone the project 
+from github:
+
+    git clone git@github.com:zadorlab/KinBot.git
+
+and then, from within the KinBot directory produced after cloning, type:
+
+    pip install -e .
+ 
+> **Note**
+> If you want to modify KinBot yourself it's better to fork the project 
+> into your own repository and then clone it.
 
 ## How to Run
-To run KinBot (which will only explore one well), make an input file (e.g. input.json) and run:
+To run a single-well exploration of KinBot, make an input file (e.g. input.json) and run:
 
     kinbot input.json
 
 To run a full PES search, make an input file (e.g. input.json) and run:
 
     pes input.json
 
@@ -110,20 +114,23 @@
 ## Documentation
 See [wiki](https://github.com/zadorlab/KinBot/wiki).
 
 ## List of files in this project
 See [list](https://github.com/zadorlab/KinBot/wiki/KinBot-file-structure).
 
 ## Authors
-* Judit Zador (jzador@sandia.gov)
+* Judit Zádor (jzador@sandia.gov)
 * Ruben Van de Vijver (Ruben.VandeVijver@UGent.be)
 * Amanda Dewyer
 * Carles Martí (cmartia@sandia.gov)
 
 ## Papers using KinBot
+* Martí, C., Michelsen, H. A., Najm, H. N., Zádor, J.: _Comprehensive kinetics on the C7H7 potential energy surface under combustion conditions._ J. Phys. Chem. A, **2023**, 127, 1941–1959. https://pubs.acs.org/doi/full/10.1021/acs.jpca.2c08035  
+* Zádor, J, Martí, C., Van de Vijver, R., Johansen, S. L., Yang, Y., Michelsen, H. A., Najm, H. N.: _Automated reaction kinetics of gas-phase organic species over multiwell potential energy surfaces._ J. Phys. Chem. A, **2023**, 127, 565–588. https://doi.org/10.1021/acs.jpca.2c06558
+* Lockwood, K. S., Ahmed, S. F., Huq, N. A., Stutzman, S. C., Foust, T. D., Labbe, N. J.: _Advances in predictive chemistry enable a multi-scale rational design approach for biofuels with advantaged properties_ Sustainable Energy Fuels, **2022**, 6, 5371-5383. https://doi.org/10.1039/D2SE00773H 
 * Takahashi, L., Yoshida, S., Fujima, J., Oikawa, H., Takahashi, K.: _Unveiling the reaction pathways of hydrocarbons via experiments, computations and data science._ Phys. Chem. Chem. Phys., **2022**, 24, 29841-29849. https://pubs.rsc.org/en/content/articlelanding/2022/CP/D2CP04499D
 * Doner, A. C., Zádor, J., Rotavera, B.: _Stereoisomer-dependent unimolecular kinetics of 2,4-dimethyloxetane peroxy radicals._ Faraday Discuss., **2022**, 238, 295-319. https://doi.org/10.1039/D2FD00029F
 * Ramasesha, K., Savee, J. D., Zádor, J., Osborn, D. L.: _A New Pathway for Intersystem Crossing: Unexpected Products in the O(3P) + Cyclopentene Reaction._ J. Phys. Chem. A, **2021**, 125 9785-9801. https://doi.org/10.1021/acs.jpca.1c05817
 * Rogers, C. O, Lockwood, K. S., Nguyen, Q. L. D., Labbe, N. J.: _Diol isomer revealed as a source of methyl ketene from propionic acid unimolecular decomposition._ Int. J. Chem. Kinet., **2021**, 53, 1272–1284. https://doi.org/10.1002/kin.21532
 * Lockwood, K. S., Labbe, N. J.: _Insights on keto-hydroperoxide formation from O2 addition to the beta-tetrahydrofuran radical._ Proceedings of the Combustion Institute, **2021**, 38, 1, 533. https://doi.org/10.1016/j.proci.2020.06.357
 * Sheps, L., Dewyer, A. L., Demireva, M., and Zádor, J.: _Quantitative Detection of Products and Radical Intermediates in Low-Temperature Oxidation of Cyclopentane._ J. Phys. Chem. A **2021**, 125, 20, 4467. https://doi.org/10.1021/acs.jpca.1c02001
 * Zhang, J., Vermeire, F., Van de Vijver, R., Herbinet, O.; Battin-Leclerc, F., Reyniers, M.-F., Van Geem, K. M.: _Detailed experimental and kinetic modeling study of 3-carene pyrolysis._ Int. J. Chem. Kinet., **2020**, 52, 785-795. https://doi.org/10.1002/kin.21400
```

### Comparing `kinbot-2.1.post0/LICENSE` & `kinbot-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/PKG-INFO` & `kinbot-2.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinbot
-Version: 2.1.post0
+Version: 2.2.1
 Summary: Automated reaction kinetics for gas-phase species
 Author-email: Judit Zádor <jzador@sandia.gov>, Ruben Vande Vijver <ruben.vandevijver@ugent.be>, Carles Martí <cmartia@sandia.gov>, Amanda Dewyer <adewyer@sandia.gov>
 Maintainer-email: Judit Zádor <jzador@sandia.gov>, Carles Martí <cmartia@sandia.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, zadorlab
         All rights reserved.
@@ -39,69 +39,73 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 License-File: LICENSE
 
 [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/zadorlab/KinBot)
 
-# KinBot: Automated reaction pathway search for gas-phase molecules
+# KinBot: Automated Reaction Kinetics of Gas-Phase Organic Species over Multiwell Potential Energy Surfaces
 
 <p>
-    <img src="graphics/kinbot_logo_V2.png" width="220" height="240" />
+    <img src="https://raw.githubusercontent.com/zadorlab/KinBot/master/graphics/kinbot_logo_V2.png" width="220" height="240" />
 </p>
 
 ## Description
 This repository contains the KinBot code version 2.0,
 a tool for automatically searching for reactions on the potential energy surface.
 
-If you are using this tool in scientific publications, please reference this git repo and the following publications:
+If you are using this tool in scientific publications, please reference the following publications:
 
 * Ruben Van de Vijver, Judit Zádor: KinBot: _Automated stationary point search on potential energy surfaces_, Comp. Phys. Comm., **2019**, 248, 106947. https://doi.org/10.1016/j.cpc.2019.106947
-* Judit Zádor, Carles Martí, Ruben Van de Vijver, Sommer L. Johansen, Yoona Yang, Hope A. Michelsen, Habib N. Najm, J. Phys. Chem. A, **2023**, ASAP. https://doi.org/10.1021/acs.jpca.2c06558
+* Judit Zádor, Carles Martí, Ruben Van de Vijver, Sommer L. Johansen, Yoona Yang, Hope A. Michelsen, Habib N. Najm: _Automated reaction kinetics of gas-phase organic species over multiwell potential energy surfaces_, J. Phys. Chem. A, **2023**, 127, 565–588. https://doi.org/10.1021/acs.jpca.2c06558
 
 We appreciate if you send us the DOI of your published paper that used KinBot, so we can feature it here below.
 
 ## How to Install
-Make sure all dependencies are correctly installed. The dependencies are lister here https://github.com/zadorlab/KinBot/wiki/Setting-Up-KinBot-on-Your-System 
 
-Clone the project to the place where you want to run it. Make sure you switch to the latest version, e.g., 2.0.5:
+KinBot can be installed both in three different ways, from the PyPI index (`pip install`), from the conda-forge repo (`conda install`) or by cloning this github repo and then install it locally.
 
-    git branch 2.0.5
+### PyPI
 
-You can find the latest stable version's tag if you click on the Branch button above on this page.
+    pip install kinbot
 
-In your local space go into the KinBot/ directory. Run the following:
+> **Note**
+>  KinBot only works with Python >= 3.8.
 
-    python setup.py build
-    python setup.py install
-    
-If you do not have admin priveleges, you might have to run
+### conda-forge
 
-    python setup.py build
-    python setup.py install --user
-    
-Moreover, if you plan to modify the code, you need to install it as:
+    conda install -c conda-forge kinbot
 
-    python setup.py build
-    python setup.py develop --user
-    
-Please note that you will need the ase version linked to at https://github.com/zadorlab/ase installed
-and linked to in your path during the installation of KinBot. This version of ase has changes within it that
-are local to KinBot, using any other ase versions will likely result in errors when trying to run reaction searches.
+### From Github
+
+If you want to have the very last version of KinBot without waiting for a 
+release or you want to modify KinBot acccording to your needs you can clone the project 
+from github:
+
+    git clone git@github.com:zadorlab/KinBot.git
+
+and then, from within the KinBot directory produced after cloning, type:
+
+    pip install -e .
+ 
+> **Note**
+> If you want to modify KinBot yourself it's better to fork the project 
+> into your own repository and then clone it.
 
 ## How to Run
-To run KinBot (which will only explore one well), make an input file (e.g. input.json) and run:
+To run a single-well exploration of KinBot, make an input file (e.g. input.json) and run:
 
     kinbot input.json
 
 To run a full PES search, make an input file (e.g. input.json) and run:
 
     pes input.json
 
@@ -110,20 +114,23 @@
 ## Documentation
 See [wiki](https://github.com/zadorlab/KinBot/wiki).
 
 ## List of files in this project
 See [list](https://github.com/zadorlab/KinBot/wiki/KinBot-file-structure).
 
 ## Authors
-* Judit Zador (jzador@sandia.gov)
+* Judit Zádor (jzador@sandia.gov)
 * Ruben Van de Vijver (Ruben.VandeVijver@UGent.be)
 * Amanda Dewyer
 * Carles Martí (cmartia@sandia.gov)
 
 ## Papers using KinBot
+* Martí, C., Michelsen, H. A., Najm, H. N., Zádor, J.: _Comprehensive kinetics on the C7H7 potential energy surface under combustion conditions._ J. Phys. Chem. A, **2023**, 127, 1941–1959. https://pubs.acs.org/doi/full/10.1021/acs.jpca.2c08035  
+* Zádor, J, Martí, C., Van de Vijver, R., Johansen, S. L., Yang, Y., Michelsen, H. A., Najm, H. N.: _Automated reaction kinetics of gas-phase organic species over multiwell potential energy surfaces._ J. Phys. Chem. A, **2023**, 127, 565–588. https://doi.org/10.1021/acs.jpca.2c06558
+* Lockwood, K. S., Ahmed, S. F., Huq, N. A., Stutzman, S. C., Foust, T. D., Labbe, N. J.: _Advances in predictive chemistry enable a multi-scale rational design approach for biofuels with advantaged properties_ Sustainable Energy Fuels, **2022**, 6, 5371-5383. https://doi.org/10.1039/D2SE00773H 
 * Takahashi, L., Yoshida, S., Fujima, J., Oikawa, H., Takahashi, K.: _Unveiling the reaction pathways of hydrocarbons via experiments, computations and data science._ Phys. Chem. Chem. Phys., **2022**, 24, 29841-29849. https://pubs.rsc.org/en/content/articlelanding/2022/CP/D2CP04499D
 * Doner, A. C., Zádor, J., Rotavera, B.: _Stereoisomer-dependent unimolecular kinetics of 2,4-dimethyloxetane peroxy radicals._ Faraday Discuss., **2022**, 238, 295-319. https://doi.org/10.1039/D2FD00029F
 * Ramasesha, K., Savee, J. D., Zádor, J., Osborn, D. L.: _A New Pathway for Intersystem Crossing: Unexpected Products in the O(3P) + Cyclopentene Reaction._ J. Phys. Chem. A, **2021**, 125 9785-9801. https://doi.org/10.1021/acs.jpca.1c05817
 * Rogers, C. O, Lockwood, K. S., Nguyen, Q. L. D., Labbe, N. J.: _Diol isomer revealed as a source of methyl ketene from propionic acid unimolecular decomposition._ Int. J. Chem. Kinet., **2021**, 53, 1272–1284. https://doi.org/10.1002/kin.21532
 * Lockwood, K. S., Labbe, N. J.: _Insights on keto-hydroperoxide formation from O2 addition to the beta-tetrahydrofuran radical._ Proceedings of the Combustion Institute, **2021**, 38, 1, 533. https://doi.org/10.1016/j.proci.2020.06.357
 * Sheps, L., Dewyer, A. L., Demireva, M., and Zádor, J.: _Quantitative Detection of Products and Radical Intermediates in Low-Temperature Oxidation of Cyclopentane._ J. Phys. Chem. A **2021**, 125, 20, 4467. https://doi.org/10.1021/acs.jpca.1c02001
 * Zhang, J., Vermeire, F., Van de Vijver, R., Herbinet, O.; Battin-Leclerc, F., Reyniers, M.-F., Van Geem, K. M.: _Detailed experimental and kinetic modeling study of 3-carene pyrolysis._ Int. J. Chem. Kinet., **2020**, 52, 785-795. https://doi.org/10.1002/kin.21400
```

### Comparing `kinbot-2.1.post0/README.md` & `kinbot-2.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/zadorlab/KinBot)
 
-# KinBot: Automated reaction pathway search for gas-phase molecules
+# KinBot: Automated Reaction Kinetics of Gas-Phase Organic Species over Multiwell Potential Energy Surfaces
 
 <p>
-    <img src="graphics/kinbot_logo_V2.png" width="220" height="240" />
+    <img src="https://raw.githubusercontent.com/zadorlab/KinBot/master/graphics/kinbot_logo_V2.png" width="220" height="240" />
 </p>
 
 ## Description
 This repository contains the KinBot code version 2.0,
 a tool for automatically searching for reactions on the potential energy surface.
 
-If you are using this tool in scientific publications, please reference this git repo and the following publications:
+If you are using this tool in scientific publications, please reference the following publications:
 
 * Ruben Van de Vijver, Judit Zádor: KinBot: _Automated stationary point search on potential energy surfaces_, Comp. Phys. Comm., **2019**, 248, 106947. https://doi.org/10.1016/j.cpc.2019.106947
-* Judit Zádor, Carles Martí, Ruben Van de Vijver, Sommer L. Johansen, Yoona Yang, Hope A. Michelsen, Habib N. Najm, J. Phys. Chem. A, **2023**, ASAP. https://doi.org/10.1021/acs.jpca.2c06558
+* Judit Zádor, Carles Martí, Ruben Van de Vijver, Sommer L. Johansen, Yoona Yang, Hope A. Michelsen, Habib N. Najm: _Automated reaction kinetics of gas-phase organic species over multiwell potential energy surfaces_, J. Phys. Chem. A, **2023**, 127, 565–588. https://doi.org/10.1021/acs.jpca.2c06558
 
 We appreciate if you send us the DOI of your published paper that used KinBot, so we can feature it here below.
 
 ## How to Install
-Make sure all dependencies are correctly installed. The dependencies are lister here https://github.com/zadorlab/KinBot/wiki/Setting-Up-KinBot-on-Your-System 
 
-Clone the project to the place where you want to run it. Make sure you switch to the latest version, e.g., 2.0.5:
+KinBot can be installed both in three different ways, from the PyPI index (`pip install`), from the conda-forge repo (`conda install`) or by cloning this github repo and then install it locally.
 
-    git branch 2.0.5
+### PyPI
 
-You can find the latest stable version's tag if you click on the Branch button above on this page.
+    pip install kinbot
 
-In your local space go into the KinBot/ directory. Run the following:
+> **Note**
+>  KinBot only works with Python >= 3.8.
 
-    python setup.py build
-    python setup.py install
-    
-If you do not have admin priveleges, you might have to run
+### conda-forge
 
-    python setup.py build
-    python setup.py install --user
-    
-Moreover, if you plan to modify the code, you need to install it as:
+    conda install -c conda-forge kinbot
 
-    python setup.py build
-    python setup.py develop --user
-    
-Please note that you will need the ase version linked to at https://github.com/zadorlab/ase installed
-and linked to in your path during the installation of KinBot. This version of ase has changes within it that
-are local to KinBot, using any other ase versions will likely result in errors when trying to run reaction searches.
+### From Github
+
+If you want to have the very last version of KinBot without waiting for a 
+release or you want to modify KinBot acccording to your needs you can clone the project 
+from github:
+
+    git clone git@github.com:zadorlab/KinBot.git
+
+and then, from within the KinBot directory produced after cloning, type:
+
+    pip install -e .
+ 
+> **Note**
+> If you want to modify KinBot yourself it's better to fork the project 
+> into your own repository and then clone it.
 
 ## How to Run
-To run KinBot (which will only explore one well), make an input file (e.g. input.json) and run:
+To run a single-well exploration of KinBot, make an input file (e.g. input.json) and run:
 
     kinbot input.json
 
 To run a full PES search, make an input file (e.g. input.json) and run:
 
     pes input.json
 
@@ -59,20 +62,23 @@
 ## Documentation
 See [wiki](https://github.com/zadorlab/KinBot/wiki).
 
 ## List of files in this project
 See [list](https://github.com/zadorlab/KinBot/wiki/KinBot-file-structure).
 
 ## Authors
-* Judit Zador (jzador@sandia.gov)
+* Judit Zádor (jzador@sandia.gov)
 * Ruben Van de Vijver (Ruben.VandeVijver@UGent.be)
 * Amanda Dewyer
 * Carles Martí (cmartia@sandia.gov)
 
 ## Papers using KinBot
+* Martí, C., Michelsen, H. A., Najm, H. N., Zádor, J.: _Comprehensive kinetics on the C7H7 potential energy surface under combustion conditions._ J. Phys. Chem. A, **2023**, 127, 1941–1959. https://pubs.acs.org/doi/full/10.1021/acs.jpca.2c08035  
+* Zádor, J, Martí, C., Van de Vijver, R., Johansen, S. L., Yang, Y., Michelsen, H. A., Najm, H. N.: _Automated reaction kinetics of gas-phase organic species over multiwell potential energy surfaces._ J. Phys. Chem. A, **2023**, 127, 565–588. https://doi.org/10.1021/acs.jpca.2c06558
+* Lockwood, K. S., Ahmed, S. F., Huq, N. A., Stutzman, S. C., Foust, T. D., Labbe, N. J.: _Advances in predictive chemistry enable a multi-scale rational design approach for biofuels with advantaged properties_ Sustainable Energy Fuels, **2022**, 6, 5371-5383. https://doi.org/10.1039/D2SE00773H 
 * Takahashi, L., Yoshida, S., Fujima, J., Oikawa, H., Takahashi, K.: _Unveiling the reaction pathways of hydrocarbons via experiments, computations and data science._ Phys. Chem. Chem. Phys., **2022**, 24, 29841-29849. https://pubs.rsc.org/en/content/articlelanding/2022/CP/D2CP04499D
 * Doner, A. C., Zádor, J., Rotavera, B.: _Stereoisomer-dependent unimolecular kinetics of 2,4-dimethyloxetane peroxy radicals._ Faraday Discuss., **2022**, 238, 295-319. https://doi.org/10.1039/D2FD00029F
 * Ramasesha, K., Savee, J. D., Zádor, J., Osborn, D. L.: _A New Pathway for Intersystem Crossing: Unexpected Products in the O(3P) + Cyclopentene Reaction._ J. Phys. Chem. A, **2021**, 125 9785-9801. https://doi.org/10.1021/acs.jpca.1c05817
 * Rogers, C. O, Lockwood, K. S., Nguyen, Q. L. D., Labbe, N. J.: _Diol isomer revealed as a source of methyl ketene from propionic acid unimolecular decomposition._ Int. J. Chem. Kinet., **2021**, 53, 1272–1284. https://doi.org/10.1002/kin.21532
 * Lockwood, K. S., Labbe, N. J.: _Insights on keto-hydroperoxide formation from O2 addition to the beta-tetrahydrofuran radical._ Proceedings of the Combustion Institute, **2021**, 38, 1, 533. https://doi.org/10.1016/j.proci.2020.06.357
 * Sheps, L., Dewyer, A. L., Demireva, M., and Zádor, J.: _Quantitative Detection of Products and Radical Intermediates in Low-Temperature Oxidation of Cyclopentane._ J. Phys. Chem. A **2021**, 125, 20, 4467. https://doi.org/10.1021/acs.jpca.1c02001
 * Zhang, J., Vermeire, F., Van de Vijver, R., Herbinet, O.; Battin-Leclerc, F., Reyniers, M.-F., Van Geem, K. M.: _Detailed experimental and kinetic modeling study of 3-carene pyrolysis._ Int. J. Chem. Kinet., **2020**, 52, 785-795. https://doi.org/10.1002/kin.21400
```

### Comparing `kinbot-2.1.post0/kinbot/__init__.py` & `kinbot-2.2.1/kinbot/reactions/__init__.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/ase_modules/calculators/gaussian.py` & `kinbot-2.2.1/kinbot/ase_modules/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/ase_modules/calculators/qchem.py` & `kinbot-2.2.1/kinbot/ase_modules/calculators/qchem.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/ase_modules/constraints.py` & `kinbot-2.2.1/kinbot/ase_modules/constraints.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/ase_modules/io/formats.py` & `kinbot-2.2.1/kinbot/ase_modules/io/formats.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/ase_modules/io/gaussian.py` & `kinbot-2.2.1/kinbot/ase_modules/io/gaussian.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/ase_modules/io/zmatrix.py` & `kinbot-2.2.1/kinbot/ase_modules/io/zmatrix.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/bfgs.py` & `kinbot-2.2.1/kinbot/bfgs.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/bond_combinations.py` & `kinbot-2.2.1/kinbot/bond_combinations.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/cheminfo.py` & `kinbot-2.2.1/kinbot/cheminfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 import sys
 import os
+import logging
+
 import numpy as np
-import pkg_resources
 from PIL import Image
-import logging
+
+from kinbot import kb_path
 
 # try to import pybel
 try:
     import pybel
     pybel.ob.obErrorLog.SetOutputLevel(0)
 except ImportError:
     try:
         from openbabel import pybel
         pybel.ob.obErrorLog.SetOutputLevel(0)
     except:
         print('Warning: Pybel could not be imported.')
         print('Certain features or the whole code might not run properly.')
         pass
 
+logger = logging.getLogger('KinBot')
+
 num_to_syms = {1: 'H', 6: 'C', 7: 'N', 8: 'O', 16: 'S'}
 syms_to_num = {'H': 1, 'C': 6, 'N': 7, 'O': 8, 'S': 16}
 
 
 def get_molecular_formula(smi):
     """
     Return the molecular formula of the molecule corresponding to the smiles
     """
     try:
         mol = Chem.AddHs(Chem.MolFromSmiles(smi))
     except NameError:
-        logging.error('RDKit is not installed or loaded correctly.')
+        logger.error('RDKit is not installed or loaded correctly.')
         sys.exit()
     return rdMolDescriptors.CalcMolFormula(mol)
 
 
 def create_rxn_depiction(react_smiles, prod_smiles, cdir, name):
     """
     Create a 2D depiction of a chemical reaction,
@@ -44,23 +48,23 @@
     """
     react_png = f'{cdir}/react.png'
     prod_png = f'{cdir}/prod.png'
 
     try:
         obmol = pybel.readstring("smi", react_smiles)
     except NameError:
-        logging.error('Cannot create 2D structures, Pybel is not loaded or installed properly.')
+        logger.error('Cannot create 2D structures, Pybel is not loaded or installed properly.')
         sys.exit()
 
     obmol.draw(show=False, filename=react_png)
 
     obmol = pybel.readstring("smi", prod_smiles)
     obmol.draw(show=False, filename=prod_png)
 
-    arrow = pkg_resources.resource_filename('tpl', 'arrow.png')
+    arrow = f'{kb_path}/tpl/arrow.png'
     images = map(Image.open, [react_png, arrow, prod_png])
     widths, heights = zip(*(i.size for i in images))
 
     total_width = sum(widths)
     total_height = max(heights)
 
     new_im = Image.new('RGB', (total_width, total_height), (255, 255, 255))
@@ -83,40 +87,41 @@
     if obabel:  # use OpenBabel
         try:
             obmol = pybel.readstring('smi', smi)
         except NameError:
             message = '\nPybel is required to use the smiles input format.\n'
             message += 'If pybel is unavailable, use the geometry as input.\n'
             message += 'Else install OpenBabel with python bindings.\nExiting...\n'
+            logger.error(message)
             sys.exit(message)
         obmol.OBMol.AddHydrogens()
         obmol.make3D()
         bond = np.zeros((len(obmol.atoms), len(obmol.atoms)), dtype=int)
         for i in range(len(obmol.atoms)):
             for j in range(len(obmol.atoms)):
-                if not obmol.OBMol.GetBond(i+1, j+1) is None:
+                if obmol.OBMol.GetBond(i+1, j+1):
                     try:
                         order = obmol.OBMol.GetBond(i+1, j+1).GetBO()
                     except:
                         try:
                             order = obmol.OBMol.GetBond(i+1, j+1).GetBondOrder()
                         except:
-                            logging.error('Something went wrong with OpenBabel')
+                            logger.error('Something went wrong with OpenBabel')
                             sys.exit()
                     bond[i][j] = order
         for at in obmol.atoms:
             pos = at.coords
             sym = num_to_syms[at.atomicnum]
             structure += [sym, pos[0], pos[1], pos[2]]
         return obmol, structure, bond
     else:  # use RDKit
         try:
             rdmol = Chem.AddHs(Chem.MolFromSmiles(smi))
         except NameError:
-            logging.error('RDKit is not installed or loaded correctly.')
+            logger.error('RDKit is not installed or loaded correctly.')
             sys.exit()
         AllChem.EmbedMolecule(rdmol, AllChem.ETKDG())
         AllChem.MMFFOptimizeMolecule(rdmol)
         atoms = rdmol.GetAtoms()
         bond = np.zeros((len(atoms), len(atoms)), dtype=int)
         for i in range(len(rdmol.GetAtoms())):
             for j in range(len(rdmol.GetAtoms())):
@@ -134,15 +139,15 @@
 def create_ob_mol(smi):
     """
     Method to create a Molecule Object from ObenBabel
     """
     try:
         obmol = pybel.readstring('smi', smi)
     except NameError:
-        logging.error('Pybel is not installed or loaded correctly.')
+        logger.error('Pybel is not installed or loaded correctly.')
         sys.exit()
     obmol.OBMol.AddHydrogens()
     return obmol
 
 
 def create_rdkit_mol(bond, atom):
     """
@@ -151,21 +156,21 @@
     try:
         from rdkit import Chem
         from rdkit.Chem import AllChem
         from rdkit.Chem import rdMolDescriptors
         from rdkit import RDLogger
         RDLogger.DisableLog('rdApp.*')
     except ImportError:
-        logging.warning('RDKit could not be imported.')
+        logger.warning('RDKit could not be imported.')
         pass
 
     try:
         m = Chem.MolFromSmiles('[' + atom[0] + ']')
     except NameError:
-        logging.error('RDKit is not installed or loaded correctly.')
+        logger.error('RDKit is not installed or loaded correctly.')
         sys.exit()
 
     mw = Chem.RWMol(m)
     for i in range(1, len(atom)):
         dummy = Chem.MolFromSmiles('[' + atom[i] + ']')
         at = dummy.GetAtoms()[0]
         # at = Chem.Atom(syms_to_num[atom[i]])
@@ -200,44 +205,44 @@
 def create_inchi(job, chemid, xyz_file=''):
     if xyz_file == '':
         xyz_file = os.path.expanduser(job) + 'xyz/' + chemid + '.xyz'
     obmol = list(pybel.readfile('xyz', xyz_file))[0]
     try:
         obmol = list(pybel.readfile('xyz', xyz_file))[0]
     except NameError:
-        logging.error('Pybel is not installed or loaded correctly.')
+        logger.error('Pybel is not installed or loaded correctly.')
         sys.exit()
 
     # return obmol.write("inchi", opt={'T': 'nostereo'}).split()[0]
     return obmol.write("inchi").split()[0]
 
 
 def create_inchi_from_smi(smi):
     """
     Method to create the InChI of a structure given its smiles.
     OpenBabel is used for this.
     """
     try:
         obmol = pybel.readstring('smi', smi)
     except NameError:
-        logging.error('Pybel is not installed or loaded correctly.')
+        logger.error('Pybel is not installed or loaded correctly.')
         sys.exit()
 
     return obmol.write("inchi").split()[0]
 
 
 def create_smiles(inchi):
     """
     Method to create the smiles of a structure given its InChI.
     OpenBabel is used for this.
     """
     try:
         obmol = pybel.readstring('inchi', inchi)
     except NameError:
-        logging.error('Pybel is not installed or loaded correctly.')
+        logger.error('Pybel is not installed or loaded correctly.')
         sys.exit()
 
     return obmol.write("smi").split()[0]
 
 
 def create_smi_from_geom(atom, geom):
     inchi = create_inchi_from_geom(atom, geom)
```

### Comparing `kinbot-2.1.post0/kinbot/conformers.py` & `kinbot-2.2.1/kinbot/conformers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
 import random
 import time
 import copy
 import logging
-import numpy as np
 from shutil import copyfile
 
+import numpy as np
 from ase.db import connect
 from ase import Atoms
 from ase.units import invcm, Hartree, kcal, mol
 from ase.thermochemistry import IdealGasThermo
+import rmsd
+
 from kinbot import geometry
 from kinbot import zmatrix
 from kinbot.stationary_pt import StationaryPoint
 from kinbot import constants
-import rmsd
+
+logger = logging.getLogger('KinBot')
+
 
 class Conformers:
     """
     Class that does all the steps for the conformers of one species
     """
     def __init__(self, species, par, qc, semi_emp=0):
         """
@@ -80,14 +84,17 @@
             # Number of random conformers in case no
             # exhaustive search is done
             self.nconfs = par['random_conf_semi_emp']
 
         # db to be used for skipping conf generation
         self.db = connect('kinbot.db')
 
+        self.imagfreq_threshold = par['imagfreq_threshold']
+        self.flat_ring_dih_angle = par['flat_ring_dih_angle']
+
     def generate_ring_conformers(self, cart):
         """
         Generate the conformers of a cyclic structure
         by randomly sampling the dihedrals of the ring
         """
         # iterate the different rings in the species
         ncyc = len(self.species.cycle_chain)
@@ -102,15 +109,15 @@
                 # divided by the number of atoms in the ring
                 cycdih = 0.
                 # list of flat sections of the ring
                 flat_ring_dih = []  
                 for dih in dihs:
                     val = geometry.calc_dihedral(cart[dih[0]], cart[dih[1]],
                                                  cart[dih[2]], cart[dih[3]])[0]
-                    if abs(val) < 5.:
+                    if abs(val) < self.flat_ring_dih_angle:
                         flat_ring_dih.append(True)
                     else:
                         flat_ring_dih.append(False)
                         cycdih += np.abs(val)
                 # only care about flatness for non-flat parts
                 n_dih_nonflat = len(cyc) - np.sum(flat_ring_dih)
                 if n_dih_nonflat > 0:
@@ -186,33 +193,33 @@
         """
         job = self.get_job_name(index, cyc=1)
 
         status, geom = self.qc.get_qc_geom(job, self.species.natom)
         if status == 1:  # still running
             return np.zeros((self.species.natom, 3)), -1
         elif status == -1:  # conformer search failed
-            logging.debug('Conformer search failed for scan point {}'.format(job))
+            logger.debug('Conformer search failed for scan point {}'.format(job))
             return np.zeros((self.species.natom, 3)), 1
         else:
             if self.start_ring_conformer_search(index, geom):
-                logging.debug('Running the next dihedral for conformer {}'.format(job))
+                logger.debug('Running the next dihedral for conformer {}'.format(job))
                 return geom, -1
             else:
                 # check if all the bond lenghts are withing 10% or the original bond lengths
                 temp = StationaryPoint('temp',
                                        self.species.charge,
                                        self.species.mult,
                                        atom=self.species.atom,
                                        geom=geom)
                 temp.bond_mx()
                 if geometry.equal_geom(self.species, temp, 0.10):
-                    logging.debug('Successfully finished conformer {}'.format(job))
+                    logger.debug('Successfully finished conformer {}'.format(job))
                     return geom, 0
                 else:
-                    logging.debug('Conformer too far from original structure {}'.format(job))
+                    logger.debug('Conformer too far from original structure {}'.format(job))
                     return np.zeros((self.species.natom, 3)), 1
 
     def check_ring_conformers(self, wait=0):
         """
         Check if the conformer optimizations finished.
         Test them, and submit frequency calculations.
         Then select the lowest energy one.
@@ -268,48 +275,48 @@
         # what is length of conf_dihed?
         theoretical_confs = np.power(self.grid, len(self.species.conf_dihed)) * cycles
 
         if rotor != -999:
             if len(self.species.conf_dihed) > self.max_dihed or theoretical_confs > self.nconfs:
                 if rotor == 0:
                     if self.info: 
-                        logging.info('\tRandom conformer search is carried out for {}.'.format(name))
+                        logger.info('\tRandom conformer search is carried out for {}.'.format(name))
                         self.info = False
 
                     # skipping generation if done
                     if self.cyc_conf > 1:
                         nrandconf = int(round(self.nconfs / self.cyc_conf) + 2)
                     else:
                         nrandconf = self.nconfs
                     if os.path.exists('{}.log'.format(self.get_job_name(nrandconf - 1))) and os.path.exists('conf/{}_low.log'.format(name)): 
                         rows = self.db.select(name=self.get_job_name(nrandconf - 1))
                         for row in rows:
                             self.conf = nrandconf
-                            logging.debug('\tLast conformer was found in kinbot.db, generation is skipped for {}.'.format(self.get_job_name(nrandconf)))
+                            logger.debug('\tLast conformer was found in kinbot.db, generation is skipped for {}.'.format(self.get_job_name(nrandconf)))
                             return 1
 
                 self.generate_conformers_random_sampling(cart)
                 return 0
 
         # retraction from the recursion
         if rotor == len(self.species.conf_dihed) or rotor == -999:
             self.qc.qc_conf(self.species, cart, self.conf, semi_emp=self.semi_emp)
             if self.conf == 0:
-                logging.debug('Theoretical number of conformers is {} for {}.'.format(theoretical_confs, name))
+                logger.debug('Theoretical number of conformers is {} for {}.'.format(theoretical_confs, name))
             self.conf += 1
             return 0
 
         # skipping generation if done
         if os.path.exists('{}.log'.format(self.get_job_name(theoretical_confs - 1))) and os.path.exists('conf/{}_low.log'.format(name)): 
             rows = self.db.select(name=self.get_job_name(theoretical_confs - 1))
             for row in rows:
                 self.conf = theoretical_confs
                 if print_warning:
-                    logging.debug('Theoretical number of conformers is {} for {}.'.format(theoretical_confs, name))
-                    logging.info('\tLast conformer was found in kinbot.db, generation is skipped for {}.'.format(name))
+                    logger.debug('Theoretical number of conformers is {} for {}.'.format(theoretical_confs, name))
+                    logger.info('\tLast conformer was found in kinbot.db, generation is skipped for {}.'.format(name))
                 return 1
 
         cart = np.asarray(cart)
         zmat_atom, zmat_ref, zmat, zmatorder = zmatrix.make_zmat_from_cart(self.species, rotor, cart, 1)
 
         rotor += 1
 
@@ -321,15 +328,14 @@
                 if zmat_ref[i][2] == 1:
                     zmat[i][2] += 360. / self.grid
             cartmod = zmatrix.make_cart_from_zmat(zmat, zmat_atom, zmat_ref, self.species.natom, self.species.atom, zmatorder)
             self.generate_conformers(rotor, cartmod)
 
         return 0
 
-
     def generate_conformers_random_sampling(self, ini_cart):
         """
         Generate a random sampling of each dihedral for a number nconfs of conformers
         """
         if self.cyc_conf > 1:
             nrandconf = int(round(self.nconfs/self.cyc_conf) + 2)
         else:
@@ -403,15 +409,18 @@
             # check if conformational search is finished
             name = self.get_name()
             for i, si in enumerate(status):
                 if si == -1:
                     status[i] = self.test_conformer(i)[1]
             # problem: if the first sample has 2 imaginary frequencies, what to do then?
             if all([si >= 0 for si in status]):
-                lowest_totenergy = 0.
+                # These refer to the conformer with lowest E + ZPE, 
+                # not the individual lowest.
+                lowest_energy = np.inf
+                lowest_zpe = np.inf
                 lowest_e_geom = self.species.geom
                 final_geoms = []  # list of all final conformer geometries
                 totenergies = []
                 frequencies = []
 
                 for ci in range(self.conf):
                     if status[ci] == 0:  # this is a valid confomer
@@ -425,56 +434,58 @@
                         err, freq = self.qc.get_qc_freq(job, self.species.natom)
                         final_geoms.append(geom)
                         totenergies.append(energy + zpe)
                         if freq != []:
                             frequencies.append(freq)
                         else:
                             frequencies.append(None)
-                        if lowest_totenergy == 0.:  # likely / hopefully the first sample was valid
+                        if lowest_energy is np.inf:  # likely / hopefully the first sample was valid
                             if ci != 0:
-                                logging.debug('For {} conformer 0 failed.'.format(name)) 
+                                logger.debug('For {} conformer 0 failed.'.format(name)) 
                             err, freq = self.qc.get_qc_freq(job, self.species.natom)
                             if self.species.natom > 1:
                                 # job fails if conformer freq array is empty
                                 if len(freq) > 0:
                                     if self.species.wellorts:
                                         if freq[0] >= 0.:
                                             err = -1
                                         if self.species.natom > 2 and freq[1] <= 0.:
                                             err = -1
                                     else:
                                         if freq[0] <= 0.:
                                             err = -1
                                 else:
-                                    logging.warning("Conformer {} failed due to empty freq array".format(ci))
+                                    logger.warning("Conformer {} failed due to empty freq array".format(ci))
                                     err = -1
                             if err == 0:
-                                lowest_totenergy = energy + zpe
-                        if energy + zpe < lowest_totenergy:
+                                lowest_energy = energy
+                                lowest_zpe = zpe
+                        if energy + zpe <= lowest_energy + lowest_zpe:
                             err, freq = self.qc.get_qc_freq(job, self.species.natom)
                             ratio = 0.8
                             # job fails if conformers freq array is empty
                             if len(freq) > 0:
                                 if self.species.wellorts:
                                     if freq[0] / self.species.freq[0] < ratio:
                                         err = -1 
                                     if freq[0] / self.species.freq[0] > 1. / ratio:
                                         err = -1 
                                     if self.species.natom > 2 and freq[1] <= 0.:
                                         err = -1
                                 else:
-                                    if freq[0] <= -50.:  # note that now we allow negative frequencies here as well
+                                    if freq[0] <= -1. * self.imagfreq_threshold:  # note that now we allow negative frequencies here as well
                                         err = -1
-                            else:
-                                logging.warning("Conformer {} failed due to empty freq array".format(ci))
+                            elif self.species.natom > 1:
+                                logger.warning("Conformer {} failed due to empty freq array".format(ci))
                                 err = -1
                             if err == 0:
                                 lowest_job = job
                                 lowest_conf = str(ci).zfill(self.zf)
-                                lowest_totenergy = energy + zpe
+                                lowest_energy = energy
+                                lowest_zpe = zpe
                                 lowest_e_geom = geom
                         if err == -1:
                             status[ci] = 1  # make it invalid
                     else:
                         totenergies.append(0.)
                         final_geoms.append(np.zeros((self.species.natom, 3)))
                         if self.species.natom == 1:
@@ -496,16 +507,16 @@
                     self.db.write(mol, name='conf/{}_low'.format(name), 
                              data={'energy': row_last.data.get('energy'),
                              'frequencies': row_last.data.get('frequencies'),
                              'zpe': row_last.data.get('zpe'),
                              'status': row_last.data.get('status')})
                 except UnboundLocalError:
                     pass
-                
-                return 1, lowest_conf, lowest_e_geom, lowest_totenergy,\
+
+                return 1, lowest_conf, lowest_e_geom, lowest_energy,\
                        final_geoms, totenergies, frequencies, status
 
             else:
                 if wait:
                     time.sleep(1)
                 else:
                     return 0, lowest_conf, np.zeros((self.species.natom, 3)), self.species.energy,\
@@ -519,15 +530,15 @@
         name = self.get_name()
 
         job = 'conf/{}_low'.format(name)
         err, energy = self.qc.get_qc_energy(job)
         err, zpe = self.qc.get_qc_zpe(job)
         err, geom = self.qc.get_qc_geom(job, self.species.natom)
                 
-        return geom, energy + zpe 
+        return geom, energy, zpe 
 
     def find_unique(self, conformers, energies, frequencies, valid, temp=None, boltz=None):
         """
         Given a set of conformers, finds the set of unique ones.
         Algorithm:
         If valid:
             If energy is close to test energy:
@@ -548,25 +559,29 @@
         frequencies_unq = []
         indices_unq = []
 
         if temp is not None:
             # calculate the Gibbs free energy for all conformers
             # at T = temp, P = 101325 Pa
             gibbs = []
+            geo_type = 'nonlinear'
             for vi, val in enumerate(valid):
-                if frequencies[vi][0] > 0:
-                    vib_energies = [ff * invcm for ff in frequencies[vi]]  # convert to eV
+                if frequencies == [None]:
+                    vib_energies = [0]
+                    geo_type = 'monatomic'
                 else:
-                    vib_energies = [ff * invcm for ff in frequencies[vi][1:]]  # convert to eV
+                    vib_energies = [ff * invcm for ff in frequencies[vi] if ff > 0]  # convert to eV
+                    if np.shape(frequencies)[1] == 3 * len(self.species.atom) - 5:
+                        geo_type = 'linear'
                 potentialenergy = energies[vi] * Hartree  # convert to eV
                 atoms = Atoms(symbols=self.species.atom, positions=conformers[vi])
                 thermo = IdealGasThermo(vib_energies=vib_energies,
                                         potentialenergy=potentialenergy,
                                         atoms=atoms,
-                                        geometry='nonlinear',
+                                        geometry=geo_type,
                                         symmetrynumber=1, spin=(self.species.mult-1)/2)
                 gibbs.append(thermo.get_gibbs_energy(temperature=temp, pressure=101325., verbose=False))
 
         for vi, val in enumerate(valid):
             unique = True
             if val == 0:
                 for ei, en in enumerate(energies_unq):
```

### Comparing `kinbot-2.1.post0/kinbot/constants.py` & `kinbot-2.2.1/kinbot/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,16 +110,17 @@
 for e in epsilon:
     epsilon[e] = epsilon[e] * units.kB / units.invcm
 
 # submission keywords
 qsubmit = {'pbs': 'qsub'}
 qsubmit['slurm'] = 'sbatch'
 # extensions
-qext = {'pbs': '.pbs'}
-qext['slurm'] = '.sbatch'
+qext = {'pbs': '.pbs',
+        'slurm': '.sbatch',
+        }
 
 
 def main():
     """
     This module contains constants and run-specific settings.
     """
```

### Comparing `kinbot-2.1.post0/kinbot/exceptions.py` & `kinbot-2.2.1/kinbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/find_motif.py` & `kinbot-2.2.1/kinbot/find_motif.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/frequencies.py` & `kinbot-2.2.1/kinbot/frequencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from ase.data import atomic_numbers, covalent_radii
 
 from kinbot import constants
 from kinbot import geometry
 
 
 def get_frequencies(species, hess, geom, checkdist=0, massweighted=False):
     """"Calculates three sets of frequencies:
@@ -28,15 +29,16 @@
     masses = np.array(masses)
 
     # Translate molecule's center of mass to (0, 0, 0)
     geom = geom - geometry.get_center_of_mass(geom, atom)
 
     # Mass-weight the hessian
     if not massweighted:
-        hess /= np.sqrt(np.outer(masses, masses))
+        # Cannot use /= on immutable arrays read from db. (Sella)
+        hess = hess / np.sqrt(np.outer(masses, masses))
 
     # STEP 1: calculate the initial frequencies
     all_eigvals, all_eigvecs = np.linalg.eig(hess)
 
     all_modes = all_eigvecs.T
     all_modes /= np.sqrt(masses[np.newaxis, :])
     for mode in all_modes:
@@ -228,15 +230,19 @@
         if atj not in visited and atj not in forbidden:
             if species.bond[atj, ati] > 0:
                 if checkdist == 0:
                     division.append(atj)
                     visited.append(atj)
                     get_neighbors(atj, visited, forbidden, division, species, natom, checkdist)
                 else:
-                    cutoff = constants.st_bond[''.join(sorted(species.atom[atj] + species.atom[ati]))]
+                    try:
+                        cutoff = constants.st_bond[''.join(sorted(species.atom[atj] + species.atom[ati]))]
+                    except KeyError:
+                        cutoff = 1.2 * (covalent_radii[atomic_numbers[species.atom[ati]]] 
+                                        + covalent_radii[atomic_numbers[species.atom[atj]]])
                     if species.dist[atj, ati] < cutoff:
                         division.append(atj)
                         visited.append(atj)
                         get_neighbors(atj, visited, forbidden, division, species, natom, checkdist)
 
 
 def skip_rotor(name, rot):
```

### Comparing `kinbot-2.1.post0/kinbot/geometry.py` & `kinbot-2.2.1/kinbot/geometry.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/hindered_rotors.py` & `kinbot-2.2.1/kinbot/hindered_rotors.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import matplotlib.pyplot as plt
 from kinbot import constants
 from kinbot import geometry
 from kinbot import zmatrix
 from kinbot.frequencies import skip_rotor
 from kinbot.stationary_pt import StationaryPoint
 
+logger = logging.getLogger('KinBot')
+
 
 class HIR:
     """
     Class that does all the steps for the HIR calculations of one species
     """
     def __init__(self, species, qc, par):
         """
@@ -52,15 +54,15 @@
             self.hir_status.append([-1 for i in range(self.nrotation)])
             self.hir_energies.append([-1 for i in range(self.nrotation)])
             self.hir_geoms.append([[] for i in range(self.nrotation)])
 
         for rotor in range(len(self.species.dihed)):
             if skip_rotor(self.species.name, self.species.dihed[rotor]) == 1:
                 self.hir_status[rotor] = [2 for i in range(self.nrotation)]
-                logging.info('\tFor {} rotor {} was skipped in HIR.'.format(self.species.name, rotor))
+                logger.info('\tFor {} rotor {} was skipped in HIR.'.format(self.species.name, rotor))
                 continue
 
             cart = np.asarray(cart)
             zmat_atom, zmat_ref, zmat, zmatorder = zmatrix.make_zmat_from_cart(self.species, rotor, cart, 0)
 
             # first element has same geometry
             # ( TODO: this shouldn't be recalculated)
@@ -127,30 +129,30 @@
                             success = -1
                 if success == 1:
                     err, energy = self.qc.get_qc_energy(job)
                     self.hir_status[rotor][ai] = 0
                     self.hir_energies[rotor][ai] = energy
                     self.hir_geoms[rotor][ai] = geom
                 elif success == -1:
-                    logging.warning("Hindered rotor optimization not successful for {}".format(job))
+                    logger.warning("Hindered rotor optimization not successful for {}".format(job))
                     self.hir_status[rotor][ai] = 1
                     self.hir_energies[rotor][ai] = -1
                     self.hir_geoms[rotor][ai] = geom
 
         return 0
 
     def check_hir(self, wait=0):
         """
         Check for hir calculations and optionally wait for them to finish
         """
         while 1:
             # check if all the calculations are finished
             self.test_hir()
             if len(self.species.dihed) == 0:
-                logging.debug(f'No hindered rotors for {self.species.name}.')
+                logger.debug(f'No hindered rotors for {self.species.name}.')
             for rotor in range(len(self.species.dihed)):
                 status = self.hir_status[rotor]
                 energies = self.hir_energies[rotor]
                 # energies taken if status = 0, successful geom check or normal gauss termination
                 ens = [(energies[i] - energies[0]) * constants.AUtoKCAL for i in range(len(status)) if status[i] == 0]
 
             # if job finishes status set to 0 or 1, if all done then do the following calculation
@@ -159,23 +161,23 @@
                     if self.hir_status[rotor][0] == 2:  # skipped rotor
                         continue
                     if self.species.wellorts:
                         job = self.species.name + '_hir_' + str(rotor)
                     else:
                         job = str(self.species.chemid) + '_hir_' + str(rotor)
                     if len(ens) < self.nrotation - 2:
-                        logging.warning("More than 2 HIR calculations failed for " + job)
+                        logger.warning("More than 2 HIR calculations failed for " + job)
 
                     angles = [i * 2 * np.pi / float(self.nrotation) for i in range(self.nrotation)]
                     # write profile to file
                     self.write_profile(rotor, job)
                     # Check to see if HIR failed, job will continue if failed, but warning will be generated
                     a = self.fourier_fit(job, angles, rotor)
                     if(a == 0):
-                        logging.warning("FAILED HIR - empty energy array sent to fourier_fit for " + job)
+                        logger.warning("FAILED HIR - empty energy array sent to fourier_fit for " + job)
                     else:
                         self.hir_fourier.append(self.fourier_fit(job, angles, rotor))
                 return 1
             else:
                 if wait:
                     time.sleep(1)
                 else:
```

### Comparing `kinbot-2.1.post0/kinbot/irc.py` & `kinbot-2.2.1/kinbot/irc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import numpy as np
 import os
 import logging
 from shutil import copyfile
-import pkg_resources
 
+from kinbot import kb_path
 from kinbot.stationary_pt import StationaryPoint
 
+logger = logging.getLogger('KinBot')
+
 
 class IRC:
     """
     Class to run the IRC's for one specific reaction
     """
     def __init__(self, rxn, par):
         # instance of the reac_family object
@@ -43,15 +45,15 @@
                                                 self.rxn.species.natom,
                                                 allow_error=1)
             if err == -1:
                 return 0
             if self.problem_in_geom(geom):
                 # this happens seldom that all the atoms are
                 # very close to one another (problem in Gaussian)
-                logging.warning('Problem with product geometry for {}'.format(instance_name))
+                logger.warning('Problem with product geometry for {}'.format(instance_name))
                 return 0
 
             temp = StationaryPoint(irc_name,
                                    self.rxn.species.charge,
                                    self.rxn.species.mult,
                                    atom=self.rxn.species.atom,
                                    geom=geom)
@@ -74,27 +76,27 @@
                 if temp.chemid == self.rxn.species.chemid and all(temp.chiral[at] == self.rxn.species.chiral[at] for at in range(self.rxn.species.natom)):
                     ini_well_hits += 1
                 else:
                     prod_hit = i  # this leaves the possibility of a chirality changing reaction
 
         if ini_well_hits == 0:
             if self.par['bimol']:
-                logging.info('\tNeither IRC leads to the initial reactants for {}'.format(instance_name))
+                logger.info('\tNeither IRC leads to the initial reactants for {}'.format(instance_name))
             else:
-                logging.info('\tNeither IRC leads to the initial well for {}'.format(instance_name))
+                logger.info('\tNeither IRC leads to the initial well for {}'.format(instance_name))
             return 0
         elif ini_well_hits == 2:
             if self.par['bimol']:
-                logging.info('\tBoth IRCs lead to the initial reactants, identical reaction found: {}'.format(instance_name))
+                logger.info('\tBoth IRCs lead to the initial reactants, identical reaction found: {}'.format(instance_name))
             else:
-                logging.info('\tBoth IRCs lead to the initial well, identical reaction found: {}'.format(instance_name))
+                logger.info('\tBoth IRCs lead to the initial well, identical reaction found: {}'.format(instance_name))
             return 0
         else:
             # ircs OK: well and product found
-            logging.info('\tIRCs successful for {}'.format(instance_name))
+            logger.info('\tIRCs successful for {}'.format(instance_name))
             return st_pts[prod_hit]
 
     def problem_in_geom(self, geom):
         # check if interatomic distances are closer than 0.3 Angstrom
         for i in range(len(geom)):
             for j in range(i + 1, len(geom)):
                 dist = np.linalg.norm(geom[i] - geom[j])
@@ -115,54 +117,74 @@
         """
         Carry out the IRC calculation.
         """
         instance_name = self.rxn.instance_name
         err, geom = self.rxn.qc.get_qc_geom(instance_name,
                                             self.rxn.species.natom)
         directions = ['Forward', 'Reverse']
-        for i, direction in enumerate(directions):
+        for direction in directions:
             irc_name = '{}_IRC_{}'.format(instance_name, direction[0])
 
             # This boolean is false if the checkpoint file is available
             # and true if no checkpoint file is found.
-            # In the latter case, the geometry needs to be supplies to
+            # In the latter case, the geometry needs to be supplied to
             # the gaussian calculation and the keywords
             # geom(AllCheck,NoKeepConstants) guess=Read need to be removed
             start_from_geometry = 0
             if self.rxn.qc.qc == 'gauss':
+                code = 'gaussian'  # Sella
+                Code = 'Gaussian'  # Sella
                 # copy the chk file
                 if os.path.exists(instance_name + '.chk'):
                     copyfile(instance_name + '.chk', irc_name + '.chk')
                 else:
                     start_from_geometry = 1
 
-            if self.rxn.qc.qc == 'nwchem' and direction == 'Reverse':
-                direction = 'Backward'
+            elif self.rxn.qc.qc == 'nwchem':
+                code = 'nwchem'  # Sella
+                Code = 'NWChem'  # Sella
+                if direction == 'Reverse':
+                    direction = 'Backward'
+            elif self.rxn.qc.qc == 'qchem':
+                code = 'qchem'  # Sella
+                Code = 'QChem'  # Sella
+            else:
+                raise ValueError(f'Unexpected code name: {self.rxn.qc.qc}.'
+                                 ' ¯\_(ツ)_/¯')
 
-            odft = self.rxn.species.mult > 1
             kwargs = self.rxn.qc.get_qc_arguments(irc_name,
                                                   self.rxn.species.mult,
                                                   self.rxn.species.charge,
                                                   irc=direction.lower(),
                                                   start_from_geom=start_from_geometry)
             prod_kwargs = self.rxn.qc.get_qc_arguments(irc_name + '_prod', self.rxn.species.mult, self.rxn.species.charge)
             if self.rxn.qc.qc == 'gauss':
                 #prod_kwargs['opt'] = 'CalcFC, Tight'
                 prod_kwargs['opt'] = 'CalcFC'
+            if self.par['use_sella']:
+                kwargs.pop('irc', None)
+                kwargs.pop('geom', None)
+                kwargs.pop('guess', None)
+                prod_kwargs.pop('opt', None)
+                prod_kwargs.pop('freq', None)
 
-            template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_irc.tpl.py'.format(qc=self.rxn.qc.qc))
+                template_file = f'{kb_path}/tpl/ase_sella_irc.tpl.py'
+            else:
+                template_file = f'{kb_path}/tpl/ase_{self.rxn.qc.qc}_irc.tpl.py'
             template = open(template_file, 'r').read()
             template = template.format(label=irc_name,
                                        kwargs=kwargs,
                                        prod_kwargs=prod_kwargs,
                                        atom=list(self.rxn.species.atom),
                                        geom=list([list(gi) for gi in geom]),
                                        ppn=self.rxn.qc.ppn,
                                        qc_command=self.par['qc_command'],
-                                       working_dir=os.getcwd())
+                                       working_dir=os.getcwd(),
+                                       code=code,
+                                       Code=Code)
 
             with open('{}.py'.format(irc_name), 'w') as f:
                 f.write(template)
 
             self.rxn.qc.submit_qc(irc_name, singlejob=0)
 
         return 0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kinbot-2.1.post0/kinbot/kb.py` & `kinbot-2.2.1/kinbot/kb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import sys
-import logging
 import datetime
 import copy
 
 from kinbot import license_message
 from kinbot import postprocess
 from kinbot.parameters import Parameters
 from kinbot.mess import MESS
 from kinbot.optimize import Optimize
 from kinbot.reaction_finder import ReactionFinder
 from kinbot.reaction_finder_bimol import ReactionFinderBimol
 from kinbot.reaction_generator import ReactionGenerator
 from kinbot.stationary_pt import StationaryPoint
 from kinbot.qc import QuantumChemistry
 from kinbot.utils import make_dirs, clean_files
+from kinbot.config_log import config_log
 
 
 def main():
     if sys.version_info.major < 3:
         print(f'KinBot only runs with python 3.8 or higher. You have python {sys.version_info.major}.{sys.version_info.minor}. Bye!')
         sys.exit(-1)
     elif sys.version_info.minor < 8:
@@ -34,89 +34,90 @@
 
     # initialize the parameters for this run
     masterpar = Parameters(input_file)
     par = masterpar.par
     input_file = masterpar.input_file
     # set up the logging environment
     if par['verbose']:
-        logging.basicConfig(filename='kinbot.log', level=logging.DEBUG)
+        logger = config_log('KinBot', 'debug')
     else:
-        logging.basicConfig(filename='kinbot.log', level=logging.INFO)
+        logger = config_log('KinBot')
 
     # write the license message and the parameters to the log file
-    logging.info(license_message.message)
-    logging.info('Input parameters')
-    for param in par:
-        logging.info('{} {}'.format(param, par[param]))
+    logger.info(license_message.message)
+    logger.info('Input parameters')
+    par_str = "\n\t".join([str(p) + ": " + str(par[p])for p in par])
+
+    logger.info(par_str)
     # time stamp of the KinBot start
-    logging.info('Starting KinBot at {}'.format(datetime.datetime.now()))
+    logger.info('Starting KinBot')
 
     make_dirs(par)
 
     if par['bimol'] == 0:
         # initialize the reactant
         well0 = StationaryPoint('well0',
                                 par['charge'],
                                 par['mult'],
                                 smiles=par['smiles'],
                                 structure=par['structure'])
         well0.short_name = 'w1'
         # write the initial reactant geometry to a file for visualization
-        with open('geometry.xyz', 'w') as geom_out:
+        with open('initial_geometry.xyz', 'w') as geom_out:
             geom_out.write('{}\n\n'.format(well0.natom))
             for i, at in enumerate(well0.atom):
                 x, y, z = well0.geom[i]
                 geom_out.write('{} {:.6f} {:.6f} {:.6f}\n'.format(at, x, y, z))
             geom_out.write('\n\n')
 
         # characterize the initial reactant
         well0.characterize()
         well0.name = str(well0.chemid)
         start_name = well0.name
         if well0.name in par['skip_chemids']:
-            logging.info('This chemid is skipped, nothing to do here')
-            logging.info('Finished KinBot at {}'.format(datetime.datetime.now()))
+            logger.info('This chemid is skipped, nothing to do here')
+            logger.info('Finished KinBot at {}'.format(datetime.datetime.now()))
             print("Done!")
-            return 
+            return
 
         # initialize the qc instance
         qc = QuantumChemistry(par)
 
         clean_files()
 
         # start the initial optimization of the reactant
-        logging.info('Starting optimization of initial well...')
+        logger.info('Starting optimization of initial well...')
         qc.qc_opt(well0, well0.geom)
         err, well0.geom = qc.get_qc_geom(str(well0.chemid) + '_well',
                                          well0.natom, wait=1)
-        logging.debug(f'Initial well opt error {err}.')
+        logger.debug(f'Initial well opt error {err}.')
         err, well0.freq = qc.get_qc_freq(str(well0.chemid) + '_well',
                                          well0.natom, wait=1)
-        logging.debug(f'Initial well freq error {err}, frequencies are {well0.freq}.')
+        logger.debug(f'Initial well freq error {err}, frequencies are {well0.freq}.')
         if err < 0:
-            logging.error('Error with initial structure optimization.')
+            logger.error('Error with initial structure optimization.')
             return
         if well0.freq[0] <= 0:
-            logging.warning(f'First frequency is {well0.freq[0]} for initial structure.')
+            logger.warning(f'First frequency is {well0.freq[0]} for initial structure.')
             well0.freq[0] *= -1.
         if well0.freq[1] <= 0:
-            logging.error(f'Second frequency is {well0.freq[1]} for initial structure.')
+            logger.error(f'Second frequency is {well0.freq[1]} for initial structure.')
             return
 
         # characterize again and look for differences
         well0 = StationaryPoint('well0',
                                 par['charge'],
                                 par['mult'],
                                 atom=copy.deepcopy(well0.atom),
                                 geom=copy.deepcopy(well0.geom))
         well0.short_name = 'w1'
         well0.characterize()
         well0.name = str(well0.chemid)
         if well0.name != start_name:
-            logging.error('The first well optimized to a structure different from the input.')
+            logger.error('The first well optimized to a structure different from the input.')
             return
 
         # do an MP2 optimization of the reactant,
         # to compare some scan barrier heigths to
         if par['families'] == ['all'] or \
                 'birad_recombination_R' in par['families'] or \
                 'r12_cycloaddition' in par['families'] or \
@@ -124,46 +125,46 @@
                 'R_Addition_MultipleBond' in par['families'] or \
                 (par['skip_families'] != ['none'] and
                 ('birad_recombination_R' not in par['skip_families'] or
                 'r12_cycloaddition' not in par['skip_families'] or
                 'r14_birad_scission' not in par['skip_families'] or
                 'R_Addition_MultipleBond' not in par['skip_families'])) or \
                 par['reaction_search'] == 0:
-            logging.debug('Starting MP2 optimization of initial well...')
+            logger.debug('Starting MP2 optimization of initial well...')
             qc.qc_opt(well0, well0.geom, mp2=1)
             err, geom = qc.get_qc_geom(str(well0.chemid) + '_well_mp2', well0.natom, 1)
 
         # comparison for barrierless scan
         if par['barrierless_saddle']:
-            logging.debug('Optimization of intial well for barrierless at {}/{}'.
+            logger.debug('Optimization of intial well for barrierless at {}/{}'.
                     format(par['barrierless_saddle_method'], par['barrierless_saddle_basis']))
             qc.qc_opt(well0, well0.geom, bls=1)
             err, geom = qc.get_qc_geom(str(well0.chemid) + '_well_bls', well0.natom, 1)
 
         # characterize again and look for differences
         well0.characterize()
         well0.name = str(well0.chemid)
 
         err, well0.energy = qc.get_qc_energy(str(well0.chemid) + '_well', 1)
         err, well0.zpe = qc.get_qc_zpe(str(well0.chemid) + '_well', 1)
         # to save the starting energy to make thresholds consistent
-        well0.start_energy = well0.energy 
-        well0.start_zpe = well0.zpe 
+        well0.start_energy = well0.energy
+        well0.start_zpe = well0.zpe
 
         well_opt = Optimize(well0, par, qc, wait=1)
         well_opt.do_optimization()
         if well_opt.shigh == -999:
-            logging.error('Error with high level optimization of initial structure.')
+            logger.error('Error with high level optimization of initial structure.')
             return
 
         # if par['pes']:
         #    filecopying.copy_to_database_folder(well0.chemid, well0.chemid, qc)
 
         if par['reaction_search'] == 1:
-            logging.info('\tStarting reaction search...')
+            logger.info('Starting reaction search...')
             rf = ReactionFinder(well0, par, qc)
             rf.find_reactions()
             rg = ReactionGenerator(well0, par, qc, input_file)
             rg.generate()
 
     # BIMOLECULAR REACTANTS
     elif par['bimol'] == 1:
@@ -191,37 +192,37 @@
         well0.characterize()
         well0.short_name = 'w1'
         well0.chemid = '_'.join(sorted([fragments['frag_a'].name, fragments['frag_b'].name]))
         well0.name = str(well0.chemid)
  
         qc = QuantumChemistry(par)
 
-        logging.info('\tStarting optimization of fragments...')
+        logger.info('\tStarting optimization of fragments...')
         for frag in fragments.values():
             qc.qc_opt(frag, frag.geom)
             err, frag.geom = qc.get_qc_geom(str(frag.chemid) + '_well',
                                             frag.natom, wait=1)
             if err < 0:
-                logging.error(f'Error with initial structure optimization of {frag.name}.')
+                logger.error(f'Error with initial structure optimization of {frag.name}.')
                 return
             err, frag.freq = qc.get_qc_freq(str(frag.chemid) + '_well',
                                             frag.natom, wait=1)
             if frag.freq[0] <= 0. and frag.freq[0] >= -20.:
-                logging.warning(f'Found imaginary frequency {frag.freq[0]} for {frag.name}. It is flipped.')
+                logger.warning(f'Found imaginary frequency {frag.freq[0]} for {frag.name}. It is flipped.')
                 frag.freq[0] *= -1.
             elif frag.freq[0] < -20.:
-                logging.error(f'Found imaginary frequency {frag.freq[0]} for {frag.name}.')
+                logger.error(f'Found imaginary frequency {frag.freq[0]} for {frag.name}.')
                 return
             if frag.freq[1] <= 0:
-                logging.error(f'Found two imaginary frequencies {frag.freq[1]} for {frag.name}.')
+                logger.error(f'Found two imaginary frequencies {frag.freq[1]} for {frag.name}.')
                 return
             # characterize again and look for differences
             frag.characterize()
             if frag.name != str(frag.chemid):
-                logging.error(f'Reactant {frag} optimized to a structure different from the input.')
+                logger.error(f'Reactant {frag} optimized to a structure different from the input.')
                 return
 
         well0.energy = 0.
         well0.zpe = 0.
         well0.fragA = fragments['frag_a']  # update
         well0.fragB = fragments['frag_b']  # update
         well0.structure = [well0.fragA.structure, well0.fragB.structure]  # update, used in reactions
@@ -230,47 +231,50 @@
             err, frag.zpe = qc.get_qc_zpe(str(frag.chemid) + '_well', 1)
             well0.energy += frag.energy
             well0.zpe += frag.zpe
 
             frag_opt = Optimize(frag, par, qc, wait=1)
             frag_opt.do_optimization()
             if frag_opt.shigh == -999:
-                logging.error(f'Error with high level optimization for {frag.name}.')
+                logger.error(f'Error with high level optimization for {frag.name}.')
                 return
 
         well0.fragA = fragments['frag_a']  # update
         well0.fragB = fragments['frag_b']  # update
         well0.energy = 0.
         well0.zpe = 0.
         for frag in fragments.values():
             well0.energy += frag.energy
             well0.zpe += frag.zpe
         # if par['pes']:
         #    filecopying.copy_to_database_folder(well0.chemid, well0.chemid, qc)
 
         if par['reaction_search'] == 1:
-            logging.info('\tStarting bimolecular reaction search...')
+            logger.info('\tStarting bimolecular reaction search...')
             rf = ReactionFinderBimol(well0, par, qc)
             rf.find_reactions()
             rg = ReactionGenerator(well0, par, qc, input_file)
             rg.generate()
 
     if par['me'] > 0:  # it will be 2 for kinbots when the mess file is needed but not run
         mess = MESS(par, well0)
         mess.write_input(qc)
 
         if par['me'] == 1:
-            logging.info('\tStarting Master Equation calculations')
+            logger.info('Starting Master Equation calculations')
             if par['me_code'] == 'mess':
                 mess.run()
 
     postprocess.create_summary_file(well0, qc, par)
     postprocess.createPESViewerInput(well0, qc, par)
     postprocess.creatMLInput(well0, qc, par)
 
-    logging.info('Finished KinBot at {}'.format(datetime.datetime.now()))
-    print("Done!")
+    logger.info('KinBot finished.')
+    try:
+        print("Done!")
+    except OSError:
+        pass
     return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `kinbot-2.1.post0/kinbot/mesmer.py` & `kinbot-2.2.1/kinbot/mesmer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-import sys
 import os
-import numpy as np
-import re
 import subprocess
 import time
-import copy
 import xml.etree.cElementTree as ET
 import xml.dom.minidom as minidom
 
-import pkg_resources
-
+from kinbot import kb_path
 from kinbot import constants
-from kinbot import frequencies
-from kinbot import cheminfo
 
 
 class MESMER:
     """
     Class that reads and write all MESMER files and runs MESMER
     """
     def __init__(self, par, species):
@@ -323,20 +316,20 @@
         write a pbs/slurm file for the me/all.xml input file
         submit the pbs/slurm file to the queue
         wait for the mess run to finish
         """
 
         # open the the header and the specific templates
         if self.par['queue_template'] == '':
-            q_file = pkg_resources.resource_filename('tpl', self.par['queuing'] + '.tpl')
+            q_file = f'{kb_path}/tpl/{self.par["queuing"]}.tpl'
         else:
             q_file = self.par['queue_template']
         with open(q_file) as f:
             tpl_head = f.read()
-        q_file = pkg_resources.resource_filename('tpl', self.par['queuing'] + '_mesmer.tpl')
+        q_file = f'{kb_path}/tpl/{self.par["queuing"]}_mesmer.tpl'
         with open(q_file) as f:
             tpl = f.read()
         submitscript = 'run_mesmer' + constants.qext[self.par['queuing']] 
         with open(submitscript, 'a') as qu:
             if self.par['queue_template'] == '':
                 if self.par['queuing'] == 'pbs':
                     qu.write((tpl_head + tpl).format(name='mesmer', ppn=self.par['ppn'], queue_name=self.par['queue_name'], dir='me'))
```

### Comparing `kinbot-2.1.post0/kinbot/mess.py` & `kinbot-2.2.1/kinbot/mess.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import stat
 import numpy as np
 import subprocess
 import time
-import pkg_resources
 from collections import Counter
 
+from kinbot import kb_path
 from kinbot import constants
 from kinbot import frequencies
 from kinbot.uncertaintyAnalysis import UQ
 
 
 class MESS:
     """
@@ -24,69 +24,62 @@
         self.well_names = {}
         self.bimolec_names = {}
         self.fragment_names = {}
         self.ts_names = {}
         self.termolec_names = {}
         self. barrierless_names = {}
         # read all templates to create mess input
-        with open(pkg_resources.resource_filename('tpl', 'mess_header.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_header.tpl') as f:
             self.headertpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_dummy.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_dummy.tpl') as f:
             self.dummytpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_termol.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_termol.tpl') as f:
             self.termoltpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_fragment.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_fragment.tpl') as f:
             self.fragmenttpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_fragment_OH.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_fragment_OH.tpl') as f:
             self.fragmenttplOH = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_pstfragment.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_pstfragment.tpl') as f:
             self.pstfragmenttpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_hinderedrotor.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_hinderedrotor.tpl') as f:
             self.hinderedrotortpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_freerotor.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_freerotor.tpl') as f:
             self.freerotortpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_atom.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_atom.tpl') as f:
             self.atomtpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_tunneling.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_tunneling.tpl') as f:
             self.tunneltpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_well.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_well.tpl') as f:
             self.welltpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_well_union.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_well_union.tpl') as f:
             self.welluniontpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_bimol.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_bimol.tpl') as f:
             self.bimoltpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_barrierless.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_barrierless.tpl') as f:
             self.blbimoltpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_barrier.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_barrier.tpl') as f:
             self.barriertpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_barrier_union.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_barrier_union.tpl') as f:
             self.barrieruniontpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_rrho.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_rrho.tpl') as f:
             self.rrhotpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_core_rr.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_core_rr.tpl') as f:
             self.corerrtpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_pst.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_pst.tpl') as f:
             self.psttpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_variational.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_variational.tpl') as f:
             self.variationaltpl = f.read()
-        with open(pkg_resources.resource_filename('tpl', 'mess_2tst.tpl')) as f:
+        with open(f'{kb_path}/tpl/mess_2tst.tpl') as f:
             self.twotstpl = f.read()
 
 
-    def write_header(self):
+    def write_header(self, lot):
         """
         Create the header block for MESS
         """
-        # Read the header template
-        if self.par['single_point_key'] == 'MYDZA':
-            lot = 'CCSD(T)-F12/cc-pVDZ-f12'
-        elif self.par['single_point_key'] == 'MYTZA':
-            lot = 'CCSD(T)-F12/cc-pVTZ-f12'
-        else:
-            lot = 'CCSD(T)-F12'
         header = self.headertpl.format(LevelOfTheory=lot,
                                        TemperatureList=' '.join([str(ti) for ti in self.par['TemperatureList']]),
                                        PressureList=' '.join([str(pi) for pi in self.par['PressureList']]),
                                        EnergyStepOverTemperature=self.par['EnergyStepOverTemperature'],
                                        ExcessEnergyOverTemperature=self.par['ExcessEnergyOverTemperature'],
                                        ModelEnergyLimit=self.par['ModelEnergyLimit'],
                                        CalculationMethod=self.par['CalculationMethod'],
@@ -141,33 +134,37 @@
         write the input for all the wells, bimolecular products and barriers
         both in a separate file, as well as in one large ME file
         """
         uq = UQ(self.par)
 
         # create short names for all the species, bimolecular products and barriers
         self.create_short_names()
-        header = self.write_header()
+        header = self.write_header(f'{self.par["high_level_method"]}/'
+                                   f'{self.par["high_level_basis"]}')
 
         # filter ts's with the same reactants and products:
         ts_unique = {}  # key: ts name, value: [prod_name, energy]
         ts_all = {}
         for index, reaction in enumerate(self.species.reac_obj):
             if self.species.reac_ts_done[index] == -1:
                 rxnProds = []
                 for x in reaction.products:
                     rxnProds.append(x.chemid)
                 rxnProds.sort()
                 prod_name = '_'.join([str(pi) for pi in rxnProds])
                 new = 1
                 remove = []
-                ts_all[reaction.instance_name] = [prod_name, reaction.ts.energy  + reaction.ts.zpe]
+                ts_all[reaction.instance_name] = [prod_name, reaction.ts.energy
+                                                  + reaction.ts.zpe]
                 for ts in ts_unique:
                     if ts_unique[ts][0] == prod_name:
-                        # check for the barrier with the lowest energy
-                        if ts_unique[ts][1] > reaction.ts.energy + reaction.ts.zpe:
+                        # check for the barrier with the lowest energy  # check if hom_sci is first
+                        if (ts_unique[ts][1] > reaction.ts.energy + reaction.ts.zpe
+                                or 'hom_sci' in ts) \
+                                and 'hom_sci' not in reaction.instance_name:
                             # remove the current barrier
                             remove.append(ts)
                         else:
                             new = 0
                 for ts in remove:
                     ts_unique.pop(ts, None)
                 if new:
@@ -285,16 +282,14 @@
             dum = self.dummytpl.format(barrier='tsd', reactant=self.well_names[self.species.chemid], dummy='d1')
 
             mess_iter = "{0:04d}".format(uq_iter)
 
             with open('me/mess_%s.inp' % mess_iter, 'w') as f_out:
                 f_out.write(header + divider + wells + bimols + tss + termols + barrierless + divider + 'End ! end kinetics\n')
 
-        #uq.format_uqtk_data() 
-
         return 0
 
 
     def write_termol(self, species_list, reaction, uq_iter, bless=0):
         # Create the dummy MESS block for ter-molecular products.
         termol = ''
         terPr_name = '_'.join(sorted([str(species.chemid) for species in species_list]))
@@ -661,14 +656,16 @@
 
         pids = []  # list of job pids
 
         batch_list = ''
         uq_iter = 0
         pid_stats = []
         for uq_iter in range(self.par['uq_n']):
+            if self.par["queuing"] == 'local':
+                return 0
             submitscript = f'me/run_mess_{str(uq_iter).zfill(4)}{constants.qext[self.par["queuing"]]}'
             self.write_submitscript(submitscript, uq_iter)
             batch_list += f'sbatch {submitscript}\n'
             if not self.par['run_me']:
                 continue
             while len(pids) > self.par['uq_max_runs']:
                 time.sleep(5)
@@ -699,21 +696,21 @@
 
     def write_submitscript(self, submitscript, uq_iter):
         """
         write a pbs or slurm file for the me/all.inp mess input file
         """
 
         if self.par['queue_template'] == '':
-            q_file = pkg_resources.resource_filename('tpl', self.par['queuing'] + '.tpl')
+            q_file = f'{kb_path}/tpl/{self.par["queuing"]}.tpl'
         else:
             q_file = self.par['queue_template']
         with open(q_file) as f:
             tpl_head = f.read()
 
-        q_file = pkg_resources.resource_filename('tpl', self.par['queuing'] + '_mess_uq.tpl')
+        q_file = f'{kb_path}/tpl/{self.par["queuing"]}_mess_uq.tpl'
         with open(q_file) as f:
             tpl = f.read()
 
         with open(submitscript, 'w') as f:
             mess_iter = "{0:04d}".format(uq_iter)
             if self.par['queue_template'] == '':
                 if self.par['queuing'] == 'pbs':
```

### Comparing `kinbot-2.1.post0/kinbot/modify_geom.py` & `kinbot-2.2.1/kinbot/modify_geom.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 import logging
 import time
 import numpy as np
 
 from ase import Atoms
 from ase.io import write
 from ase.calculators.singlepoint import SinglePointCalculator
+from ase.data import atomic_numbers, covalent_radii
 
 from kinbot import bfgs
 from kinbot import constants
 from kinbot import find_motif
 from kinbot import geometry
 from kinbot import zmatrix
 
+logger = logging.getLogger('KinBot')
+
 
 class cost_function():
     def __init__(self, coords):
         self.coords = coords
 
     def eval(self, x):
         """
@@ -103,18 +106,18 @@
     To change a dihedral angle: [atom1, atom2, atom3, atom4,
                                  dihedarl_angle_in_degrees]
 
     Bond is the bond matrix of the molecule
     """
 
     start_time = time.time()
-    logging.debug('Starting coordinate modification for {}'.format(name))
-    logging.debug('Changes:')
+    logger.debug('Starting coordinate modification for {}'.format(name))
+    logger.debug('Changes:')
     for c in changes:
-        logging.debug('\t{}'.format('\t'.join([str(ci) for ci in c])))
+        logger.debug('\t{}'.format('\t'.join([str(ci) for ci in c])))
 
     step = 1
     atoms_list = []
 
     count = 0
     fname = '{}_{}.xyz'.format(name, count)
     while os.path.exists(fname):
@@ -176,20 +179,20 @@
                 new_geom[atj] = perform_rotation(new_geom[atj], new_geom[ci[1]], rot_ax, new_angle - orig_angle)
                 step = append_geom(species.natom, step, 1., species.atom, new_geom, np.zeros((species.natom * 3)), atoms_list, f_out=f_out)
 
     coords = get_coords(species, bond, new_geom, changes, 0)
     # optimize the geometry to meet the coords list
     x0 = np.reshape(new_geom, 3 * species.natom)
     cost_fct = cost_function(coords)
-    logging.debug('Starting BFGS')
+    logger.debug('Starting BFGS')
     gs = ''  # initial geomtry string
     for i, at in enumerate(species.atom):
         x, y, z = new_geom[i]
         gs += '{}, {:.8f}, {:.8f}, {:.8f}, \n'.format(at, x, y, z)
-    logging.debug("For the following initial geometry:\n" + gs)
+    logger.debug("For the following initial geometry:\n" + gs)
 
     opt = bfgs.BFGS()
     x_opt, x_i, g_i = opt.optimize(cost_fct, x0)
 
     new_geom = np.reshape(x_opt, (species.natom, 3))
     for i, xi in enumerate(x_i):
         geomi = np.reshape(xi, (species.natom, 3))
@@ -199,15 +202,15 @@
     if write_files:
         write(fname.replace('.xyz', '.traj'), atoms_list)
         f_out.close()
 
     success = control_changes(species, name, geom, new_geom, changes, bond)
 
     end_time = time.time()
-    logging.debug('Finished coordinate changes after {:.2f} seconds'.format(end_time - start_time))
+    logger.debug('Finished coordinate changes after {:.2f} seconds'.format(end_time - start_time))
     return success, new_geom
 
 
 def control_changes(species, name, geom, new_geom, changes, bond):
     """
     This method controls three things:
     1. the changes are all correct
@@ -225,61 +228,66 @@
         cs += '[{}]\n'.format(', '.join([str(cij) for cij in ci]))
 
     # check if the changes are good
     for ci in changes:
         if len(ci) == 3:
             bond_length = np.linalg.norm(new_geom[ci[0]] - new_geom[ci[1]])
             if np.abs(bond_length - ci[2]) > 0.05:  # use a 0.05 Angstrom cutoff
-                logging.debug("The modified bond length is not correct")
-                logging.debug("Expected {}, got {}".format(ci[2], bond_length))
-                logging.debug("Species name: " + name)
-                logging.debug("For the following initial geometry:\n" + gs)
-                logging.debug("And the following change list:\n" + cs)
+                logger.debug("The modified bond length is not correct")
+                logger.debug("Expected {}, got {}".format(ci[2], bond_length))
+                logger.debug("Species name: " + name)
+                logger.debug("For the following initial geometry:\n" + gs)
+                logger.debug("And the following change list:\n" + cs)
                 success = 0
         if len(ci) == 4:
             angle = geometry.calc_angle(new_geom[ci[0]], new_geom[ci[1]], new_geom[ci[2]])
             change_angle = np.radians(ci[3])
             if np.abs(angle - change_angle) > 0.05:  # use a 0.05 radians cutoff
-                logging.debug("The modified angle is not correct")
-                logging.debug("Expected {}, got {}".format(change_angle, angle))
-                logging.debug("Species name: " + name)
-                logging.debug("For the following initial geometry:\n" + gs)
-                logging.debug("And the following change list:\n" + cs)
+                logger.debug("The modified angle is not correct")
+                logger.debug("Expected {}, got {}".format(change_angle, angle))
+                logger.debug("Species name: " + name)
+                logger.debug("For the following initial geometry:\n" + gs)
+                logger.debug("And the following change list:\n" + cs)
                 success = 0
 
     # check if the bond lengths are good:
     for i in range(species.natom - 1):
         for j in range(i + 1, species.natom):
             if bond[i][j] > 0:
                 is_change = 0
                 for ci in changes:
                     if i in ci and j in ci:
                         is_change = 1
                 if not is_change:
                     new_bond = np.linalg.norm(new_geom[i] - new_geom[j])
                     orig_bond = np.linalg.norm(geom[i] - geom[j])
                     if np.abs(new_bond - orig_bond) > 0.1:  # use a 0.1 Angstrom cutoff
-                        logging.debug("The bond length {} {} is not correct after modifications".format(i, j))
-                        logging.debug("Expected {}, got {}".format(orig_bond, new_bond))
-                        logging.debug("Species name: " + name)
-                        logging.debug("For the following initial geometry:\n" + gs)
-                        logging.debug("And the following change list:\n" + cs)
+                        logger.debug("The bond length {} {} is not correct after modifications".format(i, j))
+                        logger.debug("Expected {}, got {}".format(orig_bond, new_bond))
+                        logger.debug("Species name: " + name)
+                        logger.debug("For the following initial geometry:\n" + gs)
+                        logger.debug("And the following change list:\n" + cs)
                         success = 0
 
     # check if non-bonded atoms are too close:
     for i in range(species.natom - 1):
         for j in range(i + 1, species.natom):
             if bond[i][j] == 0:
                 dist = np.linalg.norm(new_geom[i] - new_geom[j])
-                minb = constants.st_bond[''.join(sorted([species.atom[i], species.atom[j]]))]
+                try:
+                    minb = constants.st_bond[''.join(sorted([species.atom[i], species.atom[j]]))]
+                except KeyError:
+                    minb = 1.2 * (covalent_radii[atomic_numbers[species.atom[i]]] 
+                                  + covalent_radii[atomic_numbers[species.atom[j]]])
+
                 if dist < minb:
-                    logging.debug("The atoms {} {} are too close after modifications".format(i, j))
-                    logging.debug("Species name: " + name)
-                    logging.debug("For the following initial geometry:\n" + gs)
-                    logging.debug("And the following change list:\n" + cs)
+                    logger.debug("The atoms {} {} are too close after modifications".format(i, j))
+                    logger.debug("Species name: " + name)
+                    logger.debug("For the following initial geometry:\n" + gs)
+                    logger.debug("And the following change list:\n" + cs)
                     success = 0
 
     return success
 
 
 def write_zmat(zmat_atom, zmat_ref, zmat, geom, atom):
     i = 0
@@ -328,15 +336,19 @@
                 elif len(change) == 5:
                     # take the current interatomic distance
                     d = np.linalg.norm(geom[i] - geom[j]) ** 2
                     coords.append([i, j, d, 10])
             else:
                 if mode == 0:
                     d = np.linalg.norm(geom[i] - geom[j]) ** 2
-                    d_min = (constants.st_bond[''.join(sorted([atom[i], atom[j]]))] * 1.2) ** 2
+                    try:
+                        d_min = (constants.st_bond[''.join(sorted([atom[i], atom[j]]))] * 1.2) ** 2
+                    except KeyError:
+                        d_min = (1.44 * (covalent_radii[atomic_numbers[atom[i]]] 
+                                         + covalent_radii[atomic_numbers[atom[j]]])) ** 2
                     if np.sqrt(d) < 4.:  # use a cutoff of 4 angstroms
                         if bond[i][j] > 0:
                             coords.append([i, j, d, 1. / d])  # use a larger weight for bonds
                         else:
                             # check if i and j have the same neighbor
                             same_neighbor = 0
                             for k in range(natom):
```

### Comparing `kinbot-2.1.post0/kinbot/molpro.py` & `kinbot-2.2.1/kinbot/molpro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
-import pkg_resources
 import logging
 import numpy as np
 
+from kinbot import kb_path
 from kinbot import constants
 
+logger = logging.getLogger('KinBot')
+
+
 
 class Molpro:
     """
     Class to write and read molpro file and to run molpro
     """
     def __init__(self, species, par):
         self.species = species
@@ -20,20 +23,21 @@
         which is either the one in the system, or provided
         by the user.
         : bls is whether it is a bls rection
         : name is an alternative name for the file
         : shift_vec is for bls to define the direction of shift in prod scan
         : natom1 is the number of atoms in the second fragment
         """
+
         if bls == 1 and shift_vec is None:
             tpl_file = self.par['barrierless_saddle_single_point_template']
         elif bls == 1 and shift_vec is not None:
             tpl_file = self.par['barrierless_saddle_prod_single_point_template']
         elif self.par['single_point_template'] == '':
-            tpl_file = pkg_resources.resource_filename('tpl', 'molpro.tpl')
+            tpl_file = f'{kb_path}/tpl/molpro.tpl'
         else:
             tpl_file = self.par['single_point_template']
 
         with open(tpl_file) as f:
             tpl = f.read()
 
         fname = self.get_name(name)
@@ -59,15 +63,15 @@
                                       spin=spin,
                                       charge=self.species.charge
                                       ))
 
         else:
             closed = (nelectron - self.par['barrierless_saddle_nelectron']) / 2
             if closed.is_integer() is not True:
-                logging.warning("The number of closed orbitals is not an integer,\n\
+                logger.warning("The number of closed orbitals is not an integer,\n\
                              the CASPT2-like calculation will crash, but\n\
                              KinBot carries on for now. Revise your input,\n\
                              barrierless_saddle_nelectron is incorrect.")
             else:
                 closed = int(closed)
 
             occ = closed + self.par['barrierless_saddle_norbital']
@@ -125,14 +129,16 @@
         key is the keyword for the energy we want to read
         returns 1, energy if successful
         returns 0, -1 if the energy or the file was not there
         A non-object-oriented version is used in pes.py
         """
         fname = self.get_name(name)
         status = os.path.exists('molpro/' + fname + '.out')
+        if fname == '10000000000000000001':  # proton
+            return 1, 0.0
         if status:
             with open('molpro/' + fname + '.out') as f:
                 lines = f.readlines()
             for index, line in enumerate(reversed(lines)):
                 if ('SETTING ' + key) in line:
                     return 1, float(line.split()[3])
         return 0, -1
@@ -140,21 +146,21 @@
     def create_molpro_submit(self, name=''):
         """
         write a pbs or slurm file for the molpro input file
         """
         fname = self.get_name(name)
 
         # open the template head and template
-        if self.par['queue_template'] == '':
-            molpro_head = pkg_resources.resource_filename('tpl', self.par['queuing'] + '.tpl')
+        if self.par['q_temp_l3'] == '':
+            molpro_head = f'{kb_path}/tpl/{self.par["queuing"]}.tpl'
         else:
-            molpro_head = self.par['queue_template'] 
+            molpro_head = self.par['q_temp_l3'] 
         with open(molpro_head) as f:
             tpl_head = f.read()
-        molpro_tpl = pkg_resources.resource_filename('tpl', self.par['queuing'] + '_molpro.tpl')
+        molpro_tpl = f'{kb_path}/tpl/{self.par["queuing"]}_molpro.tpl'
         with open(molpro_tpl) as f:
             tpl = f.read()
         # substitution
         with open(f'molpro/{fname}.{self.par["queuing"]}', 'w') as f:
             if self.par['queuing'] == 'pbs':
                 f.write((tpl_head + tpl).format(
                         name=fname,
```

### Comparing `kinbot-2.1.post0/kinbot/optimize.py` & `kinbot-2.2.1/kinbot/optimize.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from kinbot.hindered_rotors import HIR
 from kinbot.molpro import Molpro
 from kinbot.orca import Orca
 from kinbot import reader_gauss, reader_qchem
 from kinbot.stationary_pt import StationaryPoint
 from kinbot import constants
 
+logger = logging.getLogger('KinBot')
+
+
 class Optimize:
     """
     This class does the following:
 
     1. Conformational search of the species
     2. High level optimization and freq calc of the species
     3. Hindered rotor scans
@@ -27,15 +30,16 @@
     """
 
     def __init__(self, species, par, qc, wait=0):
         self.species = species
         try:
             delattr(self.species, 'cycle_chain')
         except AttributeError:
-            logging.debug("{} has no cycle_chain attribute to delete".format(self.species.chemid))
+            logger.debug(f"{self.species.chemid} has no cycle_chain attribute "
+                         f"to delete")
         if self.species.wellorts:
             self.species.characterize(bond_mx=self.species.bond)
             self.name = str(self.species.name)
         else:
             self.species.characterize()
             self.name = str(self.species.chemid)
         self.par = par
@@ -60,15 +64,16 @@
         self.skip_conf_check = 0  # initialize
 
     def do_optimization(self):
         while 1:
             # do the conformational search
             if self.par['conformer_search'] == 1:
                 if self.scycconf == -1 and self.sconf == -1:
-                    logging.info('\tStarting conformational search of {}'.format(self.name))
+                    logger.info('\tStarting conformational search of '
+                                f'{self.name}')
                     self.species.confs = Conformers(self.species, self.par, self.qc)
 
                 # first do the cyclic part of the molecule
                 if self.scycconf == -1:
                     # start the ring conf search
                     if len(self.species.cycle_chain) > 0:
                         # there are rings in the molecule, do a search
@@ -84,30 +89,33 @@
                     # ring conf search is running, check if finished
                     status, self.species.confs.cyc_conf_geoms = self.species.confs.check_ring_conformers()
                     if status:
                         # ring conf search is finished
                         self.scycconf = 1
                 # first do an semi empirical optimization if requested by the user
                 if self.par['semi_emp_conformer_search'] == 1:
-                    logging.info('\tSemi-empirical conformer search is starting for {}'.format(self.name))
+                    logger.info('\tSemi-empirical conformer search is starting '
+                                f'for {self.name}')
                     if self.ssemi_empconf == -1:
                         # semi empirical part has not started yet
                         self.species.semi_emp_confs = Conformers(self.species, self.par, self.qc, semi_emp=1)
                         for geom in self.species.confs.cyc_conf_geoms:
                             # take all the geometries from the cyclic part
                             # generate the conformers for the current geometry
                             self.species.semi_emp_confs.generate_conformers(0, geom)
                         # set conf status to running
                         self.ssemi_empconf = 0
                         if self.ssemi_empconf == 0:
                             # semi empirical conformational search is running
                             # check if the conformational search is done
                             status, lowest_conf, geom, self.semi_emp_low_energy, self.semi_emp_conformers, self.semi_emp_energies = self.species.semi_emp_confs.check_conformers(wait=self.wait)
                             if status == 1:
-                                logging.info("\tSemi- empirical lowest energy conformer for species {} is number {}".format(self.name, lowest_conf))
+                                logger.info("\tSemi- empirical lowest energy "
+                                            f"conformer for species {self.name}"
+                                            f" is number {lowest_conf}")
                                 # set conf status to finished
                                 self.ssemi_empconf = 1
                 else:
                     self.ssemi_empconf = 1
                 if self.ssemi_empconf == 1 and self.scycconf == 1:
                     # do open chain part if cyclic (if there were any) and semi empirical (if requested) parts are done
                     if self.sconf == -1:
@@ -115,54 +123,59 @@
                         # if semi empirical conformer were searched for, start from those, 
                         # else start from cyclic conformers
                         if self.par['semi_emp_conformer_search'] == 1:
                             self.species.confs.nconfs = 1
                             for i, geom in enumerate(self.semi_emp_conformers):
                                 if (self.semi_emp_energies[i] - self.semi_emp_low_energy) * constants.AUtoKCAL < self.par['semi_emp_confomer_threshold']:
                                     self.species.confs.generate_conformers(-999, geom)
-                            logging.info("\tThere are {} structures below the {} kcal/mol threshold for species {} in the semiempirical search.". \
+                            logger.info("\tThere are {} structures below the {} kcal/mol threshold for species {} in the semiempirical search.". \
                                          format(i, self.par['semi_emp_confomer_threshold'], self.name))
                         else:
                             print_warning = True
                             for geom in self.species.confs.cyc_conf_geoms:
                                 # take all the geometries from the cyclic part
                                 # generate the conformers for the current geometry
                                 self.skip_conf_check = self.species.confs.generate_conformers(0, geom, print_warning=print_warning)
                                 print_warning = False
                         # set conf status to running
                         self.sconf = 0
                     if self.sconf == 0:
                         # conformational search is running
                         # check if the conformational search is done
-                        if self.skip_conf_check == 0 or self.par['multi_conf_tst'] or self.par['print_conf'] or self.par['calc_aie']:
+                        if self.skip_conf_check == 0 \
+                                or self.par['multi_conf_tst'] \
+                                or self.par['print_conf'] \
+                                or self.par['calc_aie']:
                             status, lowest_conf, geom, low_energy, conformers, energies, frequency_vals, valid =\
                                     self.species.confs.check_conformers(wait=self.wait)
                             if status == 1:
                                 self.species.conformer_geom, self.species.conformer_energy, \
                                         self.species.conformer_zeroenergy, \
                                         self.species.conformer_freq, self.species.conformer_index = \
                                         self.species.confs.find_unique(conformers, 
                                         energies, 
                                         frequency_vals, 
                                         valid,
                                         self.par['multi_conf_tst_temp'],
                                         self.par['multi_conf_tst_boltz'])
-                                logging.info(f'\tLowest energy conformer for species {self.name} is number {lowest_conf}')
+                                logger.info(f'\tLowest energy conformer for species {self.name} is number {lowest_conf}')
                                 if self.par['multi_conf_tst'] or self.par['print_conf'] or self.par['calc_aie']:
-                                    logging.info(f'\tAt {self.par["multi_conf_tst_temp"]} K with {100*self.par["multi_conf_tst_boltz"]}% cutoff')
-                                    logging.info(f'\t\t the unique conformers for species {self.name} are {self.species.conformer_index}')
+                                    logger.info(f'\tAt {self.par["multi_conf_tst_temp"]} K '
+                                                f'with {100*self.par["multi_conf_tst_boltz"]}% '
+                                                f'cutoff the unique conformers for species {self.name} '
+                                                f'are {self.species.conformer_index}')
                                 # save lowest energy conformer as species geometry
                                 self.species.geom = geom
                                 # save lowest energy conformer energy
                                 self.species.energy = low_energy
                                 # set conf status to finished
                                 self.sconf = 1
                         elif self.skip_conf_check == 1:
-                            self.species.geom, self.species.energy = self.species.confs.lowest_conf_info()
-                            logging.info('\tEnergy and geometry updated based on conf/{}_low file.'.format(self.name))
+                            self.species.geom, self.species.energy, self.species.zpe = self.species.confs.lowest_conf_info()
+                            logger.info('\tEnergy and geometry updated based on conf/{}_low file.'.format(self.name))
                             self.sconf = 1
 
             else:
                 # no conf search necessary, set status to finished
                 self.sconf = 1
             if self.sconf == 1:  # conf search is finished
                 # if the conformers were already done in a previous run
@@ -196,24 +209,24 @@
                                                        )
                                 if self.par['calc_aie']:
                                      for ci, conindx in enumerate(self.species.conformer_index):
                                         self.qc.qc_aie(self.species, 
                                                        self.species.conformer_geom[ci], 
                                                        ext=f'{str(conindx).zfill(4)}',
                                                        )
-                                     logging.info('\tStarting AIE optimization(s) of {}'.format(name))
-                            logging.info('\tStarting high level optimization(s) of {}'.format(name))
+                                     logger.info('\tStarting AIE optimization(s) of {}'.format(name))
+                            logger.info('\tStarting high level optimization(s) of {}'.format(name))
                             self.shigh = 0  # set the high status to running
                         if self.shigh == 0:
                             # high level calculation is running
                             # check if finished
                             status = self.qc.check_qc(self.log_name(1))
                             if status == 'error':
                                 # found an error
-                                logging.warning('High level optimization failed for {}'.format(self.name))
+                                logger.warning('High level optimization failed for {}'.format(self.name))
                                 self.shigh = -999
                             elif status == 'normal':
                                 self.compare_structures()  # this switches shigh to 0.5 or 1
                         if self.shigh == 0.5:  # the top one was tested already and was ok
                             stati = [0] * len(self.species.conformer_index)
                             for ci, conindx in enumerate(self.species.conformer_index):
                                 status = self.qc.check_qc(self.log_name(1, conf=conindx))
@@ -229,23 +242,23 @@
                         # no high-level calculations necessary, set status to finished
                         self.shigh = 1
                     if self.shigh == 1:
                         # do the HIR calculation
                         if self.par['rotor_scan'] == 1 and self.par['multi_conf_tst'] != 1:
                             if self.shir == -1:
                                 # hir not stated yet
-                                logging.info('\tStarting hindered rotor calculations of {}'.format(self.name))
+                                logger.info('\tStarting hindered rotor calculations of {}'.format(self.name))
                                 self.species.hir = HIR(self.species, self.qc, self.par)
                                 self.species.hir.generate_hir_geoms(copy.deepcopy(self.species.geom), self.par['rigid_hir'])
                                 self.shir = 0
                             if self.shir == 0:
                                 # hir is running
                                 # check if it is done:
                                 status = self.species.hir.check_hir(wait=self.wait)
-                                if status:
+                                if status:  # Finished correctly
                                     if len(self.species.hir.hir_energies) > 0:
                                         # check if along the hir potential a structure was found with a lower energy
                                         min_en = self.species.hir.hir_energies[0][0]
                                         min_rotor = -1
                                         min_ai = -1
                                         for rotor in range(len(self.species.dihed)):
                                             for ai in range(self.species.hir.nrotation):
@@ -254,44 +267,44 @@
                                                     min_en = self.species.hir.hir_energies[rotor][ai]
                                                     min_rotor = rotor
                                                     min_ai = ai
                                         if min_rotor > -1:
                                             self.restart += 1
                                             if self.restart < self.par['rotation_restart']:
                                                 # lower energy structure found
-                                                logging.warning(f'Lower energy conformer during HIR for {self.name} for rotor {min_rotor}. Restart #{self.restart}')
-                                                logging.debug('Rotor: ' + str(min_rotor))
-                                                logging.debug('Scan point: ' + str(min_ai))
+                                                logger.warning(f'Lower energy conformer during HIR for {self.name} for rotor {min_rotor}. Restart #{self.restart}')
+                                                logger.debug('Rotor: ' + str(min_rotor))
+                                                logger.debug('Scan point: ' + str(min_ai))
                                                 job = self.log_name(1, hir=1, r=min_rotor, s=min_ai)
 
                                                 err, self.species.geom = self.qc.get_qc_geom(job, self.species.natom)
                                                 # delete the high_level log file and the hir log files
                                                 if os.path.exists(self.log_name(1) + '.log'):
-                                                    logging.debug(f'Removing file {self.log_name(1)}.log')
+                                                    logger.debug(f'Removing file {self.log_name(1)}.log')
                                                     os.remove(self.log_name(1) + '.log')
                                                 for rotor in range(len(self.species.dihed)):
                                                     for ai in range(self.species.hir.nrotation):
                                                         if os.path.exists(self.log_name(1, hir=1, r=rotor, s=ai) + '.log'):
-                                                            logging.debug('Removing file ' + self.log_name(1, hir=1, r=rotor, s=ai) + '.log')
+                                                            logger.debug('Removing file ' + self.log_name(1, hir=1, r=rotor, s=ai) + '.log')
                                                             os.remove(self.log_name(1, hir=1, r=rotor, s=ai)  + '.log')
                                                 # set the status of high and hir back to not started
                                                 self.shigh = -1
                                                 self.shir = -1
                                             else:
-                                                logging.warning('Lower energy conformer, but reached max restart for {}'.format(self.name))
+                                                logger.warning('Lower energy conformer, but reached max restart for {}'.format(self.name))
                                                 self.shir = 1
                                         else:
                                             self.shir = 1
                                     else:
                                         self.shir = 1
                         else:
                             # no hir calculations necessary, set status to finished
                             self.shir = 1
                             if self.par['multi_conf_tst'] == 1:
-                                logging.debug('No rotor scans performed because multi conformer TST is requested.')
+                                logger.debug('No rotor scans performed because multi conformer TST is requested.')
                     if not self.wait or self.shir == 1 or self.shigh == -999:
                         # break the loop if no waiting is required or
                         # if the hir calcs are done or
                         # if the high level calc failed
                         break
                     else:
                         time.sleep(1)
@@ -322,20 +335,21 @@
                         molp = Molpro(self.species, self.par)
                         if 'barrierless_saddle' in self.name:
                             key = self.par['barrierless_saddle_single_point_key']
                             molp.create_molpro_input(bls=1)
                         else:
                             key = self.par['single_point_key']
                             molp.create_molpro_input()
-                        molp.create_molpro_submit()
+                        if self.par['queuing'] != 'local':
+                            molp.create_molpro_submit()
                         status, molpro_energy = molp.get_molpro_energy(key)
                         if status:
                             self.species.energy = molpro_energy
 
-                    if self.par['single_point_qc'] == 'orca':
+                    elif self.par['single_point_qc'] == 'orca':
                         orca = Orca(self.species, self.par)
                         key = self.par['single_point_key']
                         orca.create_orca_input()
                         orca.create_orca_submit()
                         status, orca_energy = orca.get_orca_energy(key)
                         if status:
                             self.species.energy = orca_energy
@@ -474,32 +488,32 @@
                 #q_coord = q_coord[q_review]
                 #q_atoms = q_atoms[q_review]
                 result_rmsd = rotation_method(p_coord, q_coord)
                 #if result_rmsd > 0.15:
                 #    same_geom = 0
             else:
                 result_rmsd = 'not done'
-            logging.info(f'\t{self.name} high level rmsd: {result_rmsd}, '\
+            logger.info(f'\t{self.name} high level rmsd: {result_rmsd}, '\
                          f'same(0.15): {geometry.equal_geom(self.species, dummy, 0.15)}, '\
                          f'corr: {geometry.matrix_corr(imagmode, imagmode_high)}, '\
                          f'same: {same_geom}')
         else:
             same_geom = geometry.equal_geom(self.species, dummy, 0.1)
 
         # checking if L2 frequencies are okay
         err, fr = self.qc.get_qc_freq(self.log_name(1, conf), self.species.natom)
         if self.species.natom == 1:
             freq_ok = 1
         elif len(fr) == 1 and fr[0] == 0:
             freq_ok = 0
-        elif self.species.wellorts == 0 and fr[0] > -50.:
+        elif self.species.wellorts == 0 and fr[0] > -1. * self.par['imagfreq_threshold']:
             freq_ok = 1
             if fr[0] < 0.:
                 fr[0] *= -1.
-                logging.warning(f'Negative frequency {fr[0]} detected in {self.name}. Flipped.')
+                logger.warning(f'Negative frequency {fr[0]} detected in {self.name}. Flipped.')
         elif self.species.wellorts == 1 and fr[0] < 0. and fr[1] > 0.:
             freq_ok = 1
         else:
             freq_ok = 0
 
         if conf == -1:
             # update properties for base structure
@@ -511,25 +525,25 @@
                 if self.par['multi_conf_tst'] == 0:
                     self.shigh = 1
                 else:
                     self.shigh = 0.5
             else:
                 # geometry diverged to other structure
                 if not same_geom:
-                    logging.warning('High level optimization converged to different structure for {}, related channels are deleted.'.format(self.name))
+                    logger.warning('High level optimization converged to different structure for {}, related channels are deleted.'.format(self.name))
                 if not freq_ok:
-                    logging.warning('Wrong number of imaginary frequencies for {}, related channels are deleted.'.format(self.name))
+                    logger.warning('Wrong number of imaginary frequencies for {}, related channels are deleted.'.format(self.name))
                 self.shigh = -999
         else:
             # update property of conformers
             inx = self.species.conformer_index.index(conf) 
             if same_geom and freq_ok:
                 err, self.species.conformer_geom[inx] = self.qc.get_qc_geom(self.log_name(1, conf=conf), self.species.natom)
                 err, self.species.conformer_energy[inx] = self.qc.get_qc_energy(self.log_name(1, conf=conf))
                 err, self.species.conformer_freq[inx] = self.qc.get_qc_freq(self.log_name(1, conf=conf), self.species.natom)   # TODO use fr variable
                 err, zpe = self.qc.get_qc_zpe(self.log_name(1, conf=conf))
                 self.species.conformer_zeroenergy[inx] = self.species.conformer_energy[inx] + zpe
             else:
                 self.species.conformer_index[inx] = -999
-                logging.warning(f'High level optimization failed for {self.log_name(1, conf=conf)}')
+                logger.warning(f'High level optimization failed for {self.log_name(1, conf=conf)}')
 
         return
```

### Comparing `kinbot-2.1.post0/kinbot/orca.py` & `kinbot-2.2.1/kinbot/orca.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-import pkg_resources
 
+from kinbot import kb_path
 from kinbot import constants
 
 
 class Orca:
     """
     Class to write and read orca file and to run orca
     """
@@ -67,20 +67,20 @@
         """
         write a submission file for the orca input file
         """
         fname = self.get_name(name)
 
         # open the template head and template
         if self.par['queue_template'] == '':
-            orca_head = pkg_resources.resource_filename('tpl', self.par['queuing'] + '.tpl')
+            orca_head = f'{kb_path}/tpl/{self.par["queuing"]}.tpl'
         else:
             orca_head = self.par['queue_template'] 
         with open(orca_head) as f:
             tpl_head = f.read()
-        orca_tpl = pkg_resources.resource_filename('tpl', self.par['queuing'] + '_orca.tpl')
+        orca_tpl = f'{kb_path}/tpl/{self.par["queuing"]}_orca.tpl'
         with open(orca_tpl) as f:
             tpl = f.read()
         # substitution
         with open(f"orca/{fname}.{self.par['queuing']}", 'w') as f:
             if self.par['queuing'] == 'pbs':
                 f.write((tpl_head + tpl).format(
                         name=fname,
```

### Comparing `kinbot-2.1.post0/kinbot/parameters.py` & `kinbot-2.2.1/kinbot/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 initializer.
 """
 import sys
 import json
 import logging
 from ase import units
 
+logger = logging.getLogger('KinBot')
+
 
 class Parameters:
     """
     This class initiates all parameters to their defaults and reads in the
     user-defined variables, which overwrite the defaults
     """
     def __init__(self, inpfile=None):
@@ -52,25 +54,27 @@
             'families': ['all'],
             # Which reaction families to include in the search bimolecular reactions
             'bimol_families': ['all'],
             # Which reaction families to skip in the search
             'skip_families': ['none'],
             # Which chemids to skip kinbot runs for during PES calculations
             'skip_chemids': ['none'],
+            # Which chemids to keep kinbot runs for during PES calculations
+            'keep_chemids': ['none'],
             # Skip specific reactions, usually makes sense once the search is done
             'skip_reactions': ['none'],
             # perform variational calculations for the homolytic scissions
             'variational': 0,
             # break specific bonds in the homolytic search
             # this is a dictionary written as:
             # {chemid1: [[atom1, atom2], [atom3, atom4], ...], [chemid2: [..]]}
             'barrierless_saddle': {},
-            # starting distance for barrierless_saddle searches, A
+            # starting distance for barrierless_saddle searches in Å
             'barrierless_saddle_start': 2.0,
-            # step size in A
+            # step size in Å
             'barrierless_saddle_step': 0.2,
             # for the hom_sci family, using the same format as in barrierless_saddle
             'homolytic_bonds': {},
             # if requested with specific_reaction = 1
             # then only these bonds are broken and formed
             # atom index for break/form bonds starts at 0
             'specific_reaction': 0,
@@ -110,14 +114,16 @@
             # Number of HIR restarts in case a lower energy point gets found
             'rotation_restart': 3,
             # Maximum number of diherals for which exhaustive
             # comformation searches are done
             'max_dihed': 5,
             # Number of random conformers in case no exhaustive search is done
             'random_conf': 500,
+            # Dihedral angle to consider a section of a ring flat
+            'flat_ring_dih_angle': 5.,
             # Maximum number of diherals for which exhaustive
             # comformation searches are done at semi empirical level
             'max_dihed_semi_emp': 5,
             # Number of random conformers in case no exhaustive search is done
             # at semi empirical level
             'random_conf_semi_emp': 500,
             # threshold of conformers at semi empirical level to take to the L1 level
@@ -220,20 +226,32 @@
             'barrierless_saddle_single_point_key': '',
             # Command string to be used for single point energy calculation
             'single_point_command': '',
             # Hindered rotor max optimization steps
             'hir_maxcycle': None,
             # Non-rigid or rigid hir
             'rigid_hir': 0,
+            # use_sella
+            'use_sella': False,
+            # Threshold to accept negative frequencies for floppy structures, this is a positive number
+            'imagfreq_threshold': 50.,
 
             # COMPUTATIONAL ENVIRONEMNT
             # Which queuing system to use
             'queuing': 'pbs',  # or slurm
             # Template for queue:
             'queue_template': '',
+            # Queue template for AM1 jobs
+            'q_temp_am1': None,
+            # Queue template for high jobs
+            'q_temp_hi': None, 
+            # Queue template for MP2 jobs
+            'q_temp_mp2': None,
+            # Queue template for MP2 jobs
+            'q_temp_l3': None,
             # Name of the queue
             'queue_name': 'medium',
             # E.g. the type of node or anything that comes with -C in SLURM
             'slurm_feature': '',
             # Number of cores to run the L0-L2 qc jobs on
             'ppn': 1,
             # Number of cores to run the L3 qc jobs on
@@ -333,39 +351,46 @@
         if self.par['high_level'] == 1 and self.par['conformer_search'] == 0:
             err = 'Conformer search has to be done before L2.'
 
         if self.par['uq'] == 0:
             self.par['uq_n'] = 1
 
         if self.par['bimol'] == 1 and self.par['method'] == 'b3lyp':
-            logging.warning('B3LYP is not recommended as L1 for bimolecular reactions.')
-            logging.warning('Choose for instance M06-2X or wB97XD.')
+            logger.warning('B3LYP is not recommended as L1 for bimolecular reactions.')
+            logger.warning('Choose for instance M06-2X or wB97XD.')
             print('B3LYP is not recommended as L1 for bimolecular reactions.')
             print('Choose for instance M06-2X.')
 
         if self.par['bimol'] and len(self.par['structure']) != 2:
             err = 'For bimolecular reactions two fragments need to be defined.'
 
         if self.par['multi_conf_tst'] and not self.par['conformer_search']:
             err = 'For multi conformer tst calculation conformer search needs to be activated.'
 
+        if self.par['imagfreq_threshold'] < 0:
+            err = 'The threshold for imaginary freqency has to be a positive number, interpreted as an imaginary value.'
+
         if not self.par['multi_conf_tst']:
             self.par['multi_conf_tst_temp'] = None
             self.par['multi_conf_tst_boltz'] = 0.05 
 
         if self.par['multi_conf_tst']:
             self.par['rotor_scan'] = 0
 
+        for par in ['q_temp_am1', 'q_temp_hi', 'q_temp_mp2', 'q_temp_l3']:
+            if self.par[par] is None:
+                self.par[par] = self.par['queue_template']
+
         self.par['well_uq'] = float(self.par['well_uq'])
         self.par['barrier_uq'] = float(self.par['barrier_uq'])
         self.par['freq_uq'] = float(self.par['freq_uq'])
         self.par['imagfreq_uq'] = float(self.par['imagfreq_uq'])
 
         if err is not None:
-            logging.error(err)
+            logger.error(err)
             sys.exit(-1)
 
         return
 
     def read_user_input(self):
         """
         Read the user input file and overwrite the default values
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kinbot-2.1.post0/kinbot/pes.py` & `kinbot-2.2.1/kinbot/pes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 This is the main class to run KinBot to explore
 a full PES instead of only the reactions of one well
 """
 import sys
 import os
 import stat
 import shutil
-import logging
 import datetime
 import time
 import subprocess
 import json
-import pkg_resources
 import networkx as nx
 import numpy as np
 from copy import deepcopy
 
 from ase.db import connect
 
+from kinbot import kb_path
 from kinbot import constants
 from kinbot import license_message
 from kinbot.parameters import Parameters
 from kinbot.stationary_pt import StationaryPoint
 from kinbot.mess import MESS
 from kinbot.uncertaintyAnalysis import UQ
+from kinbot.config_log import config_log
 
 
 def main():
     if sys.version_info.major < 3:
         print(f'KinBot only runs with python 3.8 or higher. You have python {sys.version_info.major}.{sys.version_info.minor}. Bye!')
         sys.exit(-1)
     elif sys.version_info.minor < 8:
@@ -64,19 +64,23 @@
     # print the license message to the console
     print(license_message.message)
 
     # initialize the parameters
     par = Parameters(input_file).par
 
     # set up the logging environment
-    logging.basicConfig(filename='pes.log', level=logging.INFO)
+    global logger
+    if par['verbose']:
+        logger = config_log('KinBot', mode='pes', level='debug')
+    else:
+        logger = config_log('KinBot', mode='pes')
 
-    logging.info(license_message.message)
+    logger.info(license_message.message)
     msg = 'Starting the PES search at {}'.format(datetime.datetime.now())
-    logging.info(msg)
+    logger.info(msg)
 
     well0 = StationaryPoint('well0',
                             par['charge'],
                             par['mult'],
                             smiles=par['smiles'],
                             structure=par['structure'])
     well0.characterize()
@@ -102,72 +106,83 @@
     # list of all jobs
     jobs = []
     # dict of the pid's for all jobs
     pids = {}
     a = 0
     b = 0
     c = 0
+
+    if 'none' not in par['keep_chemids']:
+        with open('chemids', 'w') as f:
+            for keep in par['keep_chemids']:
+                f.write(keep + '\n')
+                write_input_keep(input_file, keep, os.getcwd())
+
+    if 'none' in par['skip_chemids']:
+        logger.info('No KinBot runs to be skipped.')
+    if 'none' in par['keep_chemids']:
+        logger.info('All valid explored KinBot runs are kept.')
+
     while 1:
         j = len(jobs)
         if j != a:
-            logging.info('{0} {1} {2}'.format("len(jobs): ", j, "\n"))
+            logger.info('{0} {1} {2}'.format("len(jobs): ", j, "\n"))
         a = j
         with open('chemids', 'r') as f:
             jobs = f.read().split('\n')
             jobs = [ji for ji in jobs if ji != '']
 
         if len(jobs) > j:
-            logging.info('\tPicked up new jobs: ' + ' '.join(jobs[j:]))
+            logger.info('Picked up new jobs: ' + ' '.join(jobs[j:]))
 
         k = len(running)
         l = len(finished)
         if b != k:
-            logging.info('{0} {1} {2}'.format("len(running): ", len(running), "\n"))
+            logger.info('{0} {1} {2}'.format("len(running): ", len(running), "\n"))
         b = k
         if c != l:
-            logging.info('{0} {1} {2}'.format("len(finished): ", len(finished), "\n"))
+            logger.info('{0} {1} {2}'.format("len(finished): ", len(finished), "\n"))
         c = l
         if len(finished) == len(jobs):
             time.sleep(2)
             if len(finished) == len(jobs):
                 break
 
         while (len(running) < par['simultaneous_kinbot'] and
                len(running) + len(finished) < len(jobs)):
             # start a new job
             job = jobs[len(running) + len(finished)]
             kb = 1
-            logging.info('Job: {}'.format(job))
-            if 'none' in par['skip_chemids']:
-                logging.info('No KinBot runs to be skipped')
-            else:
-                if job in par['skip_chemids']:
-                    kb = 0
-            logging.info('kb: {}'.format(kb))
+            logger.info('Job: {}'.format(job))
+            if job in par['skip_chemids'] and 'none' not in par['skip_chemids']:
+                kb = 0
+            if job not in par['keep_chemids'] and 'none' not in par['keep_chemids']:
+                kb = 0
+            logger.info(f'kb: {kb} for {job}')
             if kb == 1:
                 pid = 0
                 if not no_kinbot:
                     pid = submit_job(job, par)  # kinbot is submitted here
                 else:
                     get_wells(job)
                 pids[job] = pid
                 t = datetime.datetime.now()
-                logging.info('\tStarted job {} at {}'.format(job, t))
+                logger.info('Started job {} at {}'.format(job, t))
                 running.append(job)
             elif kb == 0:
-                logging.info('Skipping Kinbot for {}'.format(job))
+                logger.info('Skipping Kinbot for {}'.format(job))
                 finished.append(job)
             else:
-                logging.info('kb value not 0 or 1')
+                logger.info('kb value not 0 or 1')
 
         # check if a thread is done
         for job in running:
             if not check_status(job, pids[job]):
                 t = datetime.datetime.now()
-                logging.info('\tFinished job {} at {}'.format(job, t))
+                logger.info('Finished job {} at {}'.format(job, t))
                 finished.append(job)
                 if not no_kinbot:
                     # write a temporary pes file
                     # remove old xval and im_extent files
                     try:
                         os.remove('{}_xval.txt'.format(par['title']))
                     except OSError:
@@ -196,37 +211,44 @@
                 summary_lines.append('\t{}'.format(job))
             waiting = jobs[len(running) + len(finished):]
             summary_lines.append('')
             summary_lines.append('Waiting:')
             for job in waiting:
                 summary_lines.append('\t{}'.format(job))
             with open('pes_summary.txt', 'w') as f:
-                f.write('\n'.join(summary_lines))
+                f.write('\n'.join(summary_lines) + '\n')
             time.sleep(1)
 
     # delete skipped jobs from the jobs before sending to postprocess
     for skip in par['skip_chemids']:
         try:
             jobs.pop(jobs.index(skip))
         except ValueError:
             pass
 
+    # only keep the jobs we wanted
+    if 'none'not in par['keep_chemids']:
+        jobs = par['keep_chemids']
+
     postprocess(par, jobs, task, names, well0.mass)
     # make molpro inputs for all keys above
     # place submission script in the directory for offline submission
     # read in the molpro energies for the keys in the above three dicts
     # for key in newdict.keys():
     #      print(key)
     # if all energies are there
     # do something like postprocess, but with new energies
     # postprocess_L3(saddle_zpe, well_zpe, prod_zpe, saddle_energy, well_energy, prod_energy, conn)
 
     # Notify user the search is done
-    logging.info('PES search done!')
-    print('PES search done!')
+    logger.info('PES search done!')
+    try:
+        print('PES search done!')
+    except OSError:
+        pass
 
 
 def get_wells(job):
     """
     Read the summary file and add the wells to the chemid list
     """
     try:
@@ -251,15 +273,14 @@
                 new_wells.append(prod[0])
     if len(new_wells) > 0:
         with open('chemids', 'a') as f:
             f.write('\n'.join(new_wells) + '\n')
     
 
 def postprocess(par, jobs, task, names, mass):
-
     """
     postprocess a pes search
     par: parameters of the search
     jobs: all of the jobs that were run
     temp: this is a temporary output file writing
     """
 
@@ -401,24 +422,30 @@
                     reactions.append([reactant, ts, prod, barrier])
         # copy the xyz files
         copy_from_kinbot(ji, 'xyz')
         # copy the L3 calculations here, whatever was in those directories, inp, out, pbs, etc.
         try:
             copy_from_kinbot(ji, par['single_point_qc'])
         except:
-            logging.warning(f'L3 calculations were not copied from {ji}')
+            logger.warning(f'L3 calculations were not copied from {ji}')
     # create a connectivity matrix for all wells and products
     conn, bars = get_connectivity(wells, products, reactions)
     # create a batch submission for all L3 jobs
     if par['queuing'] == 'pbs':
         cmd = 'qsub'
         ext = 'pbs'
     elif par['queuing'] == 'slurm':
         cmd = 'sbatch'
         ext = 'slurm'
+    elif par['queuing'] == 'local':
+        cmd = ''
+        ext = ''
+        pass
+    else:
+        raise ValueError(f'Unexpected value for queueing: {par["queuing"]}')
 
     batch_submit = ''
 
     well_energies = {}
     well_l3energies = {}
     for well in wells:
         energy = get_energy(parent[well], well, 0, par['high_level'])  # from the db
@@ -480,42 +507,44 @@
                     l3done = 0
                     batch_submit += f'{cmd} {reac[1]}.{ext}\n'
                 elif not par['L3_calc']:
                     pass
                 else:
                     ts_l3energies[reac[1]] = ((l3energy + zpe) - (base_l3energy + base_zpe)) * constants.AUtoKCAL
 
-    logging.info('l3done status {}'.format(l3done))
+    logger.info('l3done status {}'.format(l3done))
     # clean duplicates
-    batch_submit = set(batch_submit.split())
+    batch_submit = list(set(batch_submit.split('\n')))
+    batch_submit.reverse()
     batch_submit = '\n'.join(batch_submit)
     batch = f'{par["single_point_qc"]}/batch_L3_{par["queuing"]}.sub'
-    with open(batch, 'w') as f:
-        f.write(batch_submit)
-    os.chmod(batch, stat.S_IRWXU)  # read, write, execute by owner
+    if par['queuing'] != 'local':
+        with open(batch, 'w') as f:
+            f.write(batch_submit)
+        os.chmod(batch, stat.S_IRWXU)  # read, write, execute by owner
 
     if l3done == 1 and par['L3_calc']:
-        logging.info('Energies are updated to L3 in ME and PESViewer.')
+        logger.info('Energies are updated to L3 in ME and PESViewer.')
         well_energies = well_l3energies
         prod_energies = prod_l3energies
         for reac in reactions:  # swap out the barrier
             if 'barrierless' not in reac[1]:
                 reac[3] = ts_l3energies[reac[1]]
             if 'barrierless_saddle' in reac[1]:
                 reac[3] = ts_l3energies[reac[1]]
 
-        logging.info('L3 energies in kcal/mol, incl. ZPE')
+        logger.info('L3 energies in kcal/mol, incl. ZPE')
         for well in wells:
-            logging.info('{}   {:.2f}'.format(well, well_l3energies[well]))
+            logger.info('{}   {:.2f}'.format(well, well_l3energies[well]))
         for prod in products:
-            logging.info('{}   {:.2f}'.format(prod, prod_l3energies[prod]))
+            logger.info('{}   {:.2f}'.format(prod, prod_l3energies[prod]))
         for ts in ts_l3energies:
-            logging.info('{}   {:.2f}'.format(ts, ts_l3energies[ts]))
+            logger.info('{}   {:.2f}'.format(ts, ts_l3energies[ts]))
     else:
-        logging.info(f'Energies used are at the L2 ({par["high_level_method"]}/'
+        logger.info(f'Energies used are at the L2 ({par["high_level_method"]}/'
                      f'{par["high_level_basis"]}) level of theory.')
 
     # if L3 was done and requested, everything below is done with that
     # filter according to tasks
     wells, products, reactions, highlight = filter(par,
                                                    wells,
                                                    products,
@@ -559,21 +588,22 @@
                           barrierless,
                           well_energies,
                           prod_energies,
                           parent,
                           mass,
                           l3done)
 
-    check_l2_l3()
-
     if par['single_point_qc'].lower() == 'molpro':
+        if l3done:
+            check_l3_l2(par['single_point_key'], parent, reactions)
         t1_analysis(par['single_point_key'])
 
 
-def filter(par, wells, products, reactions, conn, bars, well_energies, task, names):
+def filter(par, wells, products, reactions, conn, bars, well_energies, task,
+           names):
     """
     Filter the wells, products and reactions according to the task
     and the names
     """
     # list of reactions to highlight
     highlight = []
     # 1. all: This is the default showing all pathways
@@ -586,15 +616,14 @@
     # 5. temperature
     # 6. threshold_reapply: apply the barrier threshold
     # cutoff at the highest level that was done
 
     # filter the reactions according to the task
     if task == 'all':
         filtered_reactions = reactions
-        pass
     elif task == 'lowestpath':
         all_rxns = get_all_pathways(wells, products, reactions, names, conn)
         # this is the maximum energy along the minimun energy pathway
         min_energy = None
         min_rxn = None
         for rxn_list in all_rxns:
             barriers = [ri[3] for ri in rxn_list]
@@ -605,16 +634,16 @@
                 if max(barriers) < min_energy:
                     min_energy = max(barriers)
                     min_rxn = rxn_list
         filtered_reactions = min_rxn
     elif task == 'allpaths':
         all_rxns = get_all_pathways(wells, products, reactions, names, conn)
         filtered_reactions = []
-        for list in all_rxns:
-            for rxn in list:
+        for rxnlist in all_rxns:
+            for rxn in rxnlist:
                 new = 1
                 for r in filtered_reactions:
                     if r[1] == rxn[1]:
                         new = 0
                 if new:
                     filtered_reactions.append(rxn)
         # this is the maximum energy along the minimun energy pathway
@@ -635,45 +664,45 @@
         if len(names) == 1:
             filtered_reactions = []
             for rxn in reactions:
                 prod_name = '_'.join(sorted(rxn[2]))
                 if names[0] == rxn[0] or names[0] == prod_name:
                     filtered_reactions.append(rxn)
         else:
-            logging.error('Only one name should be given for a well filter')
-            logging.error('Received: ' + ' '.join(names))
+            logger.error('Only one name should be given for a well filter')
+            logger.error('Received: ' + ' '.join(names))
             sys.exit(-1)
     elif task == 'temperature':
         if len(names) == 1:
             try:
                 # read the temperature
                 temperature = float(names[0])
             except ValueError:
-                logging.error('A float is needed for a temperature filter')
-                logging.error('Received: ' + ' '.join(names))
+                logger.error('A float is needed for a temperature filter')
+                logger.error('Received: ' + ' '.join(names))
                 sys.exit(-1)
             filtered_reactions = []
             # iterate the wells
             wells, filtered_reactions = filter_boltzmann(wells[0],
                                                          [wells[0]],
                                                          reactions,
                                                          filtered_reactions,
                                                          well_energies,
                                                          temperature)
         else:
-            logging.error('Only one argument should be given for a temperature filter')
-            logging.error('Received: ' + ' '.join(names))
+            logger.error('Only one argument should be given for a temperature filter')
+            logger.error('Received: ' + ' '.join(names))
             sys.exit(-1)
     elif task == 'l2threshold':
         filtered_reactions = []
         for rxn in reactions:
             if rxn[3] < par['barrier_threshold']:
                 filtered_reactions.append(rxn)
     else:
-        logging.error('Could not recognize task ' + task)
+        logger.error('Could not recognize task ' + task)
         sys.exit(-1)
 
     # filter the wells
     filtered_wells = []
     for well in wells:
         for rxn in filtered_reactions:
             prod_name = '_'.join(sorted(rxn[2]))
@@ -792,26 +821,26 @@
         paths = nx.all_simple_paths(G, start, end, cutoff=max_length)
         rxns = []
         for path in paths:
             if is_pathway(wells, products, path, names):
                 rxns.append(get_pathway(wells, products, reactions, path, names))
         return rxns
     else:
-        logging.error('Cannot find a lowest path if the number of species is not 2')
-        logging.error('Found species: ' + ' '.join(names))
+        logger.error('Cannot find a lowest path if the number of species is not 2')
+        logger.error('Found species: ' + ' '.join(names))
 
 
 def get_index(wells, products, name):
     try:
         i = wells.index(name)
     except ValueError:
         try:
             i = products.index(name) + len(wells)
         except ValueError:
-            logging.error('Could not find reactant ' + name)
+            logger.error('Could not find reactant ' + name)
             sys.exit(-1)
     return i
 
 
 def get_name(wells, products, i):
     if i < len(wells):
         name = wells[i]
@@ -874,14 +903,15 @@
     for f in files:
         if f.endswith('.out'):
             if not os.path.exists(f'{dirname}/{f}'):
                 shutil.copy(f'{well}/{dirname}/{f}', f'{dirname}/{f}')
         else:
             shutil.copy(f'{well}/{dirname}/{f}', f'{dirname}/{f}')
 
+
 def get_rxn(prods, rxns):
     for rxn in rxns:
         if prods == '_'.join(sorted(rxn[2])):
             return rxn
 
 
 def create_short_names(wells, products, reactions, barrierless):
@@ -936,27 +966,26 @@
         n = n + 1
 
     return well_short, pr_short, fr_short, ts_short, nobar_short
 
 
 def create_mess_input(par, wells, products, reactions, barrierless,
                       well_energies, prod_energies, parent, mass, l3done):
-    """
-    When calculating a full pes, the files from the separate wells
+    """When calculating a full pes, the files from the separate wells
     are read and concatenated into one file
     Two things per file need to be updated
     1. the names of all the wells, bimolecular products and ts's
     2. all the zpe corrected energies
     If it is a multi_conf_tst calculation, then the ZeroEnergies and
     ImaginaryFrequency values need to be also changed for each species in the Union.
     The lowest energy species has L3 energies (if calculated), while the 
     others are corrected with their DeltaL2 energies.
     """
 
-    logging.info(f"uq value: {par['uq']}")
+    logger.info(f"uq value: {par['uq']}")
     short_names = create_short_names(wells, products, reactions, barrierless)
     well_short, pr_short, fr_short, ts_short, nobar_short = short_names
 
     # list of the strings to write to mess input file
     s = []
 
     # Create the header block for MESS
@@ -969,24 +998,19 @@
                             smiles=par['smiles'],
                             structure=par['structure'])
 
     mess = MESS(par, dummy)
     uq = UQ(par)
 
     if l3done:
-        if par['single_point_key'] == 'MYDZA':
-            lot = 'CCSD(T)-F12/cc-pVDZ-f12'
-        elif par['single_point_key'] == 'MYTZA':
-            lot = 'CCSD(T)-F12/cc-pVTZ-f12'
-        else:
-            lot = 'CCSD(T)-F12'
+        lot = 'L3'
     else:
         lot = f'{par["high_level_method"]}/{par["high_level_basis"]}'
 
-    header_file = pkg_resources.resource_filename('tpl', 'mess_header.tpl')
+    header_file = f'{kb_path}/tpl/mess_header.tpl'
     with open(header_file) as f:
         tpl = f.read()
 
     for uq_iter in range(par['uq_n']):
         mess_iter = "{0:04d}".format(uq_iter)
 
         e_well = par['epsilon'] * uq.calc_factor('epsilon', uq_iter)
@@ -1099,15 +1123,15 @@
             os.mkdir('me')
 
         with open(f'me/mess_{mess_iter}.inp', 'w') as f:
             f.write(header)
             f.write('\n'.join(s))
 
         if par['multi_conf_tst']:
-            logging.info('\tUpdating ZPE and tunneling parameters for multi_conf_tst...')
+            logger.debug('\tUpdating ZPE and tunneling parameters for multi_conf_tst...')
             with open(f'me/mess_{mess_iter}_corr.inp', 'w') as fcorr:
                 with open(f'me/mess_{mess_iter}.inp', 'r') as f:
                     lines = f.read().split('\n')
                     for line in lines:
                         words = line.split()
                         if 'ZeroEnergy' in line:
                             if len(words) == 4:
@@ -1220,34 +1244,27 @@
                                                     prod_name,
                                                     high))
     barrierless_lines = []
     index = 0
     prev_prod = []
     for rxn in barrierless:
         prod_name = '_'.join(sorted(rxn[2]))
-        new = 1
-        for item in prev_prod:
-            if prod_name == item:
-                new = 0
-                break
-        if new:
-            barrierless_lines.append('{name} {react} {prod}'.format(name='nobar_' + str(index),
+        barrierless_lines.append('{name} {react} {prod}'.format(name='nobar_' + str(index),
                                                                     react=rxn[0],
                                                                     prod=prod_name))
-            prev_prod.append(prod_name)
-            index = index + 1
+        index = index + 1
 
     well_lines = '\n'.join(well_lines)
     bimol_lines = '\n'.join(bimol_lines)
     ts_lines = '\n'.join(ts_lines)
     barrierless_lines = '\n'.join(barrierless_lines)
 
     # write everything to a file
     fname = 'pesviewer.inp'
-    template_file_path = pkg_resources.resource_filename('tpl', fname + '.tpl')
+    template_file_path = f'{kb_path}/tpl/{fname}.tpl'
     with open(template_file_path) as template_file:
         template = template_file.read()
     template = template.format(id=par['title'],
                                wells=well_lines,
                                bimolecs=bimol_lines,
                                ts=ts_lines,
                                barrierless=barrierless_lines)
@@ -1260,20 +1277,15 @@
     Create an interactive plot with pyvis
     """
     if len(wells) < 2:
         return -2
     try:
         from pyvis import network as net
     except ImportError:
-        logging.warning('pyvis cannot be imported, no interactive plot is made.')
-        return -1
-    try:
-        from IPython.core.display import display, HTML
-    except ImportError:
-        logging.warning('IPython cannot be imported, no interactive plot is made.')
+        logger.warning('pyvis cannot be imported, no interactive plot is made.')
         return -1
 
     # For now we are assuming the all of the 2D depictions
     # are in place, which were created with PESViewer
     # Later we can add those in independently, but
     # this is not needed, just requires a quick run of
     # PESViewer
@@ -1321,19 +1333,19 @@
         if hasattr(row, 'data'):
             energy = row.data.get('energy')
     try:
         # ase energies are always in ev, convert to hartree
         energy *= constants.EVtoHARTREE
     except UnboundLocalError or TypeError:
         # this happens when the job is not found in the database
-        logging.error('Could not find {} in directory {} database.'.format(job, directory))
-        logging.error('Exiting...')
+        logger.error('Could not find {} in directory {} database.'.format(job, directory))
+        logger.error('Exiting...')
         sys.exit(-1)
     except TypeError:
-        logging.warning('Could not find {} in directory {}'.format(job, directory))
+        logger.warning('Could not find {} in directory {}'.format(job, directory))
         energy = 0.
     return energy
 
 
 def get_l3energy(job, par, bls=0):
     """
     Get the L3, single-point energies.
@@ -1341,55 +1353,57 @@
     """
 
     if bls:
         key = par['barrierless_saddle_single_point_key']
     else:
         key = par['single_point_key']
 
+    if job == '10000000000000000001':  # proton
+        return 1, 0.0
     if par['single_point_qc'] == 'molpro':
         if os.path.exists(f'molpro/{job}.out'):
             with open(f'molpro/{job}.out', 'r') as f:
                 lines = f.readlines()
                 for line in reversed(lines):
                     if ('SETTING ' + key) in line:
                         e = float(line.split()[3])
-                        logging.info('L3 electronic energy for {} is {} Hartree.'.format(job, e))
+                        logger.info('L3 electronic energy for {} is {} Hartree.'.format(job, e))
                         return 1, e  # energy was found
     elif par['single_point_qc'] == 'orca':
         if os.path.exists(f'orca/{job}_property.txt'):
             with open(f'orca/{job}_property.txt', 'r') as f:
                 lines = f.readlines()
                 for line in reversed(lines):
                     if (key) in line:
                         e = float(line.split()[-1])
-                        logging.info('L3 electronic energy for {} is {} Hartree.'.format(job, e))
+                        logger.info('L3 electronic energy for {} is {} Hartree.'.format(job, e))
                         return 1, e  # energy was found
     elif par['single_point_qc'] == 'gauss':
         if os.path.exists('gauss/' + job + '.log'):
             gaussname = 'gauss/' + job + '.log'
         elif os.path.exists('gauss/' + job + '_high.log'):
             gaussname = 'gauss/' + job + '_high.log'
         elif os.path.exists('gauss/' + job + '_well_high.log'):
             gaussname = 'gauss/' + job + '_well_high.log'
         else:
-            logging.info('L3 for {} is missing.'.format(job))
+            logger.info('L3 for {} is missing.'.format(job))
             return 0, -1  # job not yet started to run
 
         with open(gaussname) as f:
             lines = f.readlines()
             for line in reversed(lines):
                 if (key) in line:
                     words = line.split()
                     wi = words.index(key) + 2
                     e = float(words[wi].replace('D', 'E'))
-                    logging.info('L3 electronic energy for {} is {} Hartree.'.format(job, e))
+                    logger.info('L3 electronic energy for {} is {} Hartree.'.format(job, e))
                     return 1, e  # energy was found
  
     # if no file or no energy found
-    logging.info('L3 for {} is missing.'.format(job))
+    logger.info('L3 for {} is missing.'.format(job))
     return 0, -1  # job not yet started to run or not finished
 
 
 def get_zpe(jobdir, job, ts, high_level, mp2=0, bls=0):
     db = connect(jobdir + '/kinbot.db')
     if ts:
         j = job
@@ -1403,32 +1417,32 @@
         j += '_high'
     rows = db.select(name=j)
     zpe = None 
     for row in rows:
         if hasattr(row, 'data'):
             zpe = row.data.get('zpe')
     if zpe == None: 
-        logging.warning('Could not find zpe for {} in directory {}'.format(job, jobdir))
+        logger.warning('Could not find zpe for {} in directory {}'.format(job, jobdir))
         zpe = 1.  # a large value
     return zpe
 
 
 def check_status(job, pid):
-    command = ['ps', '-u', 'root', '-N', '-o', 'pid,s,user,%cpu,%mem,etime,args']
+    command = ['ps', 'u',]
     process = subprocess.Popen(command,
                                shell=False,
                                stdout=subprocess.PIPE,
                                stdin=subprocess.PIPE,
                                stderr=subprocess.PIPE)
     out, err = process.communicate()
     out = out.decode()
     lines = out.split('\n')
     for line in lines:
         if len(line) > 0:
-            if str(pid) == line.split()[0]:
+            if str(pid) == line.split()[1]:
                 return 1
     return 0
 
 
 def submit_job(chemid, par):
     """
     Submit a kinbot run using subprocess and return the pid
@@ -1442,18 +1456,22 @@
     except OSError:
         pass
     try:
         os.system(f'rm -f {chemid}/kinbot_monitor.out')
     except OSError:
         pass
 
-    if par['queue_template'] != '':
-        shutil.copyfile('{}'.format(par['queue_template']), '{}/{}'.format(chemid, par['queue_template']))
+    for tmpl in ['queue_template', 'q_temp_am1', 'q_temp_mp2', 'q_temp_hi', 
+                 'q_temp_l3']:
+        if par[tmpl] != '':
+            shutil.copyfile('{}'.format(par[tmpl]), 
+                            '{}/{}'.format(chemid, par[tmpl]))
     if par['single_point_template'] != '':
-        shutil.copyfile('{}'.format(par['single_point_template']), '{}/{}'.format(chemid, par['single_point_template']))
+        shutil.copyfile('{}'.format(par['single_point_template']), 
+                        '{}/{}'.format(chemid, par['single_point_template']))
     if par['barrierless_saddle_single_point_template'] != '':
         shutil.copyfile('{}'.format(par['barrierless_saddle_single_point_template']), '{}/{}'
                         .format(chemid, par['barrierless_saddle_single_point_template']))
         shutil.copyfile('{}'.format(par['barrierless_saddle_prod_single_point_template']), '{}/{}'
                         .format(chemid, par['barrierless_saddle_prod_single_point_template']))
     outfile = open(f'{chemid}/kinbot.out', 'w')
     errfile = open(f'{chemid}/kinbot.err', 'w')
@@ -1494,62 +1512,138 @@
     # don't do ME for these kinbots but write the files
     if me:
         par2['me'] = 2
 
     file_name = directory + str(species.chemid) + '.json'
     with open(file_name, 'w') as outfile:
         json.dump(par2, outfile, indent=4, sort_keys=True)
+    return
+
 
+def write_input_keep(input_file, keepchemid, root):
+    directory = root + '/' + str(keepchemid) + '/'
+    if not os.path.exists(directory):
+        print(f'Cannot keep a well that is not already explored. Please correct the keep_chemids parameter. Bye!')
+        sys.exit(-1)
 
-def check_l2_l3():
-    """Perform a check on the difference between L2 and L3 energy differences.
+    par_keep = Parameters(f'{directory}{keepchemid}.json').par
+    # make a new parameters instance and overwrite some keys
+    input_file = '{}'.format(input_file)
+    par_new = Parameters(input_file).par
+    # overwrite the title
+    par_new['title'] = par_keep['title']
+    par_new['structure'] = par_keep['structure']
+    par_new['barrier_threshold'] = par_keep['barrier_threshold']
+    par_new['pes'] = 1
+    par_new['me'] = 2
+
+    file_name = directory + str(keepchemid) + '.json'
+    with open(file_name, 'w') as outfile:
+        json.dump(par_new, outfile, indent=4, sort_keys=True)
+    return
+
+
+def check_l3_l2(l3_key: str, parent_specs: dict, reactions: list) -> None:
+    """Perform a check on the difference between L3 and L2 energy differences.
+
+    @param l3_key: Pattern to search for in L3 calculations.
+    @param parent_specs: Dictionary of species' chemids with its parent species.
+    @param reactions: List of all reaction names in the PES.
     """
     # Get L3 energies
     l3_energies = {}
-    logging.info(f'L2-L3 Energy difference Analysis (Ha):')
+    logger.info(f'L3-L2 Energy difference Analysis. Energy units: kcal/mol.')
     if not os.path.isdir('molpro'):
-        logging.warning("Unable to perform L2-L3 check. The molpro directory "
-                        "is missing")
+        logger.warning("Unable to perform L3-L2 check. The molpro directory "
+                        "is missing.")
+        return
+    if len([f for f in os.listdir('molpro/') if f.endswith('.out')]) == 0:
+        logger.warning("Unable to perform L3-L2 check. The molpro directory "
+                        "is empty.")
         return
-    for file in [f for f in os.listdir('molpro/') if
-                 f[::-1].startswith('tuo.')]:
-        st_pt_name = file.split('.')[0]
-        with open(f'molpro/{file}') as out_fh:
-            for line in out_fh:
-                if 'MYDZA' not in line:
-                    continue
-                l3_energies[st_pt_name] = float(line.split()[3])
+
+    # Get L3 energies
+    for st_pt in list(parent_specs.keys()) + [r[1] for r in reactions]:
+        if "_" in st_pt and all([frag.isdigit() for frag in st_pt.split('_')]):
+            # Bimolecular species
+            l3_energies[st_pt] = 0
+            for frag in st_pt.split('_'):
+                if not os.path.isfile(f'molpro/{frag}.out'):
+                    if st_pt in l3_energies:
+                        del l3_energies[st_pt]
+                    break
+                with open(f'molpro/{frag}.out') as out_fh:
+                    for line in out_fh:
+                        if l3_key not in line:
+                            continue
+                        l3_energies[st_pt] += float(line.split()[3])
+                        break
+        elif os.path.isfile(f'molpro/{st_pt}.out'):
+            # Wells and TSs
+            with open(f'molpro/{st_pt}.out') as out_fh:
+                for line in out_fh:
+                    if l3_key not in line:
+                        continue
+                    l3_energies[st_pt] = float(line.split()[3])
+                    break
 
     # Get L2 Energies and its difference respect L3.
     e_diffs = {}
-    for st_pt_name in l3_energies:
-        try:
-            if st_pt_name.isdigit():
-                db = connect(f'{st_pt_name}/kinbot.db')
-                rows = db.select(name=f'{st_pt_name}_well_high')
-            else:
-                db = connect(f'{st_pt_name.split("_")[0]}/kinbot.db')
-                rows = db.select(name=f'{st_pt_name}_high')
+    for st_pt in l3_energies:
+        if any([c.isalpha() for c in st_pt]):  # TSs (have letters in the name)
+            db_path = f'{st_pt.split("_")[0]}/kinbot.db'
+        else:  # Wells and Bimolecular products
+            db_path = f'{parent_specs[st_pt]}/kinbot.db'
+        if not os.path.isfile(db_path):
+            logger.warning(f"Unable to find L2 energy for {st_pt}.")
+            continue
+        db = connect(db_path)
+        if st_pt.isdigit():
+            # Wells
+            rows = db.select(name=f'{st_pt}_well_high')
+        elif all([fr.isdigit() for fr in st_pt.split('_')]):
+            # Bimolecular species.
+            l2_energy = 0
+            for frag in st_pt.split('_'):
+                rows = db.select(name=f'{frag}_well_high')
+                try:
+                    final_row = next(rows)
+                except StopIteration:
+                    logger.warning(f"Unable to find L2 energy for {frag}.")
+                    l2_energy = np.nan
+                    break
+                for row in rows:
+                    final_row = row
+                l2_energy += final_row.data["energy"] * constants.EVtoHARTREE
+        else:
+            rows = db.select(name=f'{st_pt}_high')
+
+        if "_" not in st_pt or any([c.isalpha() for c in st_pt]):
+            # Wells and TSs
+            try:
+                final_row = next(rows)
+            except StopIteration:
+                logger.warning(f"Unable to find L2 energy for {st_pt}.")
+                continue
             for row in rows:
                 final_row = row
-            e_diff = final_row.data["energy"] * constants.EVtoHARTREE \
-                     - l3_energies[st_pt_name]
-            e_diffs[st_pt_name] = e_diff
-        except:  # TODO try to catch the exact exception.
-            logging.warning(f"Unable to read db for {st_pt_name}")
-            continue
-    e_diff_avg = np.average(list(e_diffs.values()))
-    e_diff_std = np.std(list(e_diffs.values()))
-    logging.info(f'Avg difference: {e_diff_avg}. Max: '
-                 f'{max(e_diffs.values())}, Min: {min(e_diffs.values())}, '
-                 f'STDEV: {e_diff_std}.')
-    for st_pt_name, e_diff in e_diffs.items():
-        if e_diff > 5 * constants.KCALtoHARTREE:
-            logging.info(f"Outlying L2-L3 difference found for {st_pt_name}. "
-                         f"Energy difference: {e_diff}.")
+            l2_energy = final_row.data["energy"] * constants.EVtoHARTREE
+        e_diff = l3_energies[st_pt] - l2_energy
+        e_diffs[st_pt] = e_diff / constants.KCALtoHARTREE
+
+    e_diff_avg = np.round(np.average(list(e_diffs.values())), 1)
+    e_diff_std = np.round(np.std(list(e_diffs.values())), 1)
+    logger.info(f'Avg difference: {e_diff_avg} kcal/mol, '
+                 f'Max: {np.round(max(e_diffs.values()), 1)} kcal/mol, '
+                 f'Min: {np.round(min(e_diffs.values()), 1)} kcal/mol, '
+                 f'STDEV: {e_diff_std} kcal/mol.')
+    for st_pt, e_diff in e_diffs.items():
+        if not e_diff_avg * 0.9 < e_diff < e_diff_avg * 1.1:
+            logger.info(f"Outlying L2-L3 difference found for {st_pt}. "
+                         f"Energy difference: {np.round(e_diff, 1)} kcal/mol.")
 
 
 def t1_analysis(lot='TZ'):
     import os
     try:
         import matplotlib.pyplot as plt
         do_plot = True
@@ -1557,49 +1651,54 @@
         do_plot = False
 
     if 'TZ' in lot.upper():
         lot = 'TZ'
     elif 'DZ' in lot.upper():
         lot = 'DZ'
     else:
-        logging.warning('Unable to perform a summary of T1 diagnostics: '
+        logger.warning('Unable to perform a summary of T1 diagnostics: '
                         'Unrecognized single_point_key.')
         return
     T1s = []
     for f in os.listdir('molpro/'):
         if not f.endswith('.out'):
             continue
         with open(f'molpro/{f}') as fh:
             do_read1 = False
             do_read2 = False
             for line in fh:
                 if lot in line:
                     do_read1 = True
                     do_read2 = False
-                if "Starting UCCSD calculation" in line:
+                if "Starting UCCSD calculation" in line or "Starting RCCSD calculation" in line:
                     do_read2 = True
                 elif do_read1 and do_read2 and 'T1 diagnostic:' in line:
                     T1s.append(float(line.split()[9]))
                     break
-    counts, bins = np.histogram(T1s)
+    if T1s:
+        counts, bins = np.histogram(T1s)
+    else:
+        logger.warning('Unable to perform a summary of T1 diagnostics: '
+                        'No T1 Diagnostics results found.')
+        return
 
     if do_plot:
         fig1, ax1 = plt.subplots()  # Histogram
         ax1.bar(bins[1:], counts, width=bins[1]*0.7)
         ax1.set_xlabel('T1 Diagnostic')
         ax1.set_ylabel('Counts')
         fig1.savefig('T1_histo.png')
 
         fig2, ax2 = plt.subplots()  # Cumulative counts.
         ax2.plot(sorted(T1s), range(len(T1s)))
         ax2.set_xlabel('T1 Diagnostic')
         ax2.set_ylabel('Cumulative counts')
-        fig2.savefig('T1_cum_count.png')
+        fig2.savefig('T1_cumul_count.png')
     else:
-        logging.warning('Matplotlib not found. Unable to plot T1 diagnostics '
+        logger.warning('Matplotlib not found. Unable to plot T1 diagnostics '
                         'summary.')
 
-    logging.info(f"T1 histogram:\nBins: {bins}\nCounts: {counts}.")
+    logger.info(f"T1 histogram:\nBins: {bins}\nCounts: {counts}.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `kinbot-2.1.post0/kinbot/postprocess.py` & `kinbot-2.2.1/kinbot/postprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 It includes
 1. Writing a summary file with all successful and failed
 reactions, including their barrier heights and which products are formed
 
 2. Writing an input file for the PES viewer.
 """
 import os
-import pkg_resources
 import numpy as np
 
+from kinbot import kb_path
 from kinbot import license_message
 from kinbot import constants
 
 
 def creatMLInput(species, qc, par):
     """
     Create the files for the input of the Machine Learning tool
@@ -89,14 +89,18 @@
     for index in range(len(species.reac_inst)):
         if species.reac_ts_done[index] == -1:
             ts = species.reac_obj[index].ts
             if species.reac_type[index] == 'R_Addition_MultipleBond' and not par['high_level']:
                 mp2_energy = qc.get_qc_energy(str(species.chemid) + '_well_mp2')[1]
                 mp2_zpe = qc.get_qc_zpe(str(species.chemid) + '_well_mp2')[1]
                 energy = (ts.energy + ts.zpe - mp2_energy - mp2_zpe) * constants.AUtoKCAL
+            elif species.reac_type[index] == 'hom_sci':
+                energy = (sum([pr.energy + pr.zpe 
+                              for pr in species.reac_obj[index].products])
+                          - species.energy - species.zpe) * constants.AUtoKCAL
             else:
                 energy = (ts.energy + ts.zpe - species.energy - species.zpe) * constants.AUtoKCAL
             prod_name = ''
             name = []
             for prod in species.reac_obj[index].products:
                 name.append(str(prod.chemid))
             prod_name = ' '.join(sorted(name))
@@ -134,101 +138,122 @@
     # use this well as point zero for the energy
     wells.append('{} 0.0'.format(species.chemid))
     well_energy = species.energy + species.zpe
 
     # iterate the reactions and search for single products
     # i.e. other wells on the pes
     for index in range(len(species.reac_inst)):
-        if species.reac_ts_done[index] == -1:
-            if len(species.reac_obj[index].prod_opt) == 1:
-                st_pt = species.reac_obj[index].prod_opt[0].species
-                name = str(st_pt.chemid)
-                if name not in well_names:
-                    make_xyz(species.atom, st_pt.geom, str(st_pt.chemid), dir_xyz)
-                    energy = (st_pt.energy + st_pt.zpe - well_energy) * constants.AUtoKCAL
-                    wells.append('{name} {energy:.2f}'.format(name=st_pt.chemid, energy=energy))
-                    well_names.append(name)
+        if species.reac_ts_done[index] != -1 \
+                or len(species.reac_obj[index].prod_opt) != 1:
+            continue
+        st_pt = species.reac_obj[index].prod_opt[0].species
+        name = str(st_pt.chemid)
+        if name in well_names:
+            continue
+        make_xyz(species.atom, st_pt.geom, str(st_pt.chemid), dir_xyz)
+        energy = (st_pt.energy + st_pt.zpe - well_energy) * constants.AUtoKCAL
+        wells.append(f'{st_pt.chemid} {energy:.2f}')
+        well_names.append(name)
 
     # list of the lines for the pesviewer input file
     bimolecs = []
     # list of the names of the bimolecular products
     bimolec_names = []
     # add the bimolecular products from the regular reactions
     for index in range(len(species.reac_inst)):
-        if species.reac_ts_done[index] == -1:
-            if len(species.reac_obj[index].prod_opt) > 1:
-                energy = 0. - well_energy
-                names = []
-                for prod_opt in species.reac_obj[index].prod_opt:
-                    st_pt = prod_opt.species
-                    energy += st_pt.energy + st_pt.zpe
-                    names.append(str(st_pt.chemid))
-                name = '_'.join(sorted(names))
-
-                for i, prod_opt in enumerate(species.reac_obj[index].prod_opt):
-                    st_pt = prod_opt.species
-                    with open("pesviewer_data.txt", 'a') as pesdata:
-                        pesdata.write("Species: {}\n\tEnergy: {}\n\tZPE: {}\n".format(st_pt.chemid, st_pt.energy, st_pt.zpe))
-                    # make twice the same file but with a different name
-                    # TODO: is there no better way?
-                    # this is for the pes viewer
-                    make_xyz(st_pt.atom, st_pt.geom, name + str(i + 1), dir_xyz)
-                    # this is for the rmg postprocessing
-                    make_xyz(st_pt.atom, st_pt.geom, str(st_pt.chemid), dir_xyz)
-                energy = energy * constants.AUtoKCAL
-                if name not in bimolec_names:
-                    bimolecs.append('{name} {energy:.2f}'.format(name=name, energy=energy))
-                    bimolec_names.append(name)
+        if species.reac_ts_done[index] != -1 \
+                or len(species.reac_obj[index].prod_opt) <= 1:
+            continue
+        energy = 0. - well_energy
+        names = []
+        for prod_opt in species.reac_obj[index].prod_opt:
+            st_pt = prod_opt.species
+            energy += st_pt.energy + st_pt.zpe
+            names.append(str(st_pt.chemid))
+        name = '_'.join(sorted(names))
+
+        for i, prod_opt in enumerate(species.reac_obj[index].prod_opt):
+            st_pt = prod_opt.species
+            with open('pesviewer_data.txt', 'a') as pesdata:
+                pesdata.write(f'Species: {st_pt.chemid}\n'
+                              f'\tEnergy: {st_pt.energy}\n'
+                              f'\tZPE: {st_pt.zpe}\n')
+            # make twice the same file but with a different name
+            # TODO: is there no better way?
+            # this is for the pes viewer
+            make_xyz(st_pt.atom, st_pt.geom, name + str(i + 1), dir_xyz)
+            # this is for the rmg postprocessing
+            make_xyz(st_pt.atom, st_pt.geom, str(st_pt.chemid), dir_xyz)
+        energy = energy * constants.AUtoKCAL
+        if name not in bimolec_names:
+            bimolecs.append(f'{name} {energy:.2f}')
+            bimolec_names.append(name)
 
     # list of the lines of the ts's
     tss = []
     # dict keeping track of the ts's
     # key: ts name
     # value: [energy,prod_names]
     ts_list = {}
     for index in range(len(species.reac_inst)):
-        if species.reac_ts_done[index] == -1:
-            ts = species.reac_obj[index].ts
-            if species.reac_type[index] == 'R_Addition_MultipleBond' and not par['high_level']:
-                we_energy = qc.get_qc_energy(str(species.chemid) + '_well_mp2')[1]
-                we_zpe = qc.get_qc_zpe(str(species.chemid) + '_well_mp2')[1]
-                energy = (ts.energy + ts.zpe - we_energy - we_zpe) * constants.AUtoKCAL
-            else:
-                energy = (ts.energy + ts.zpe - well_energy) * constants.AUtoKCAL
-            name = []
-            for st_pt in species.reac_obj[index].products:
-                name.append(str(st_pt.chemid))
-            prod_name = '_'.join(sorted(name))
-            add = 1
-            for t in ts_list:
-                if ts_list[t][1] == prod_name and np.abs(ts_list[t][0] - energy) < 1.0:
-                    add = 0
-            if add:
-                ts_list[species.reac_name[index]] = [energy, prod_name]
-                tss.append('{ts} {energy:.2f} {react} {prod}'.format(ts=species.reac_name[index],
-                                                                     energy=energy,
-                                                                     react=species.chemid,
-                                                                     prod=prod_name))
+        if species.reac_ts_done[index] != -1:
+            continue
+        ts = species.reac_obj[index].ts
+        if species.reac_type[index] == 'R_Addition_MultipleBond' \
+                and not par['high_level']:
+            we_energy = qc.get_qc_energy(str(species.chemid) + '_well_mp2')[1]
+            we_zpe = qc.get_qc_zpe(str(species.chemid) + '_well_mp2')[1]
+            energy = (ts.energy + ts.zpe - we_energy - we_zpe) * constants.AUtoKCAL
+        elif species.reac_type[index] == 'hom_sci':
+            continue
+        else:
+            energy = (ts.energy + ts.zpe - well_energy) * constants.AUtoKCAL
+        name = []
+        for st_pt in species.reac_obj[index].products:
+            name.append(str(st_pt.chemid))
+        prod_name = '_'.join(sorted(name))
+        add = 1
+        for t in ts_list:
+            if ts_list[t][1] == prod_name and np.abs(ts_list[t][0] - energy) < 1.0:
+                add = 0
+        if add:
+            ts_list[species.reac_name[index]] = [energy, prod_name]
+            tss.append(f'{species.reac_name[index]} {energy:.2f} '
+                       f'{species.chemid} {prod_name}')
+    
+    # Barrierless reactions
+    bless = []
+    for index in range(len(species.reac_inst)):
+        if species.reac_ts_done[index] != -1 or species.reac_type[index] != 'hom_sci':
+            continue
+        name = []
+        for st_pt in species.reac_obj[index].products:
+            name.append(str(st_pt.chemid))
+        prod_name = '_'.join(sorted(name))
+        if prod_name not in [v[1] for v in ts_list.values()]:
+            bless.append(f'{species.reac_name[index]} {species.chemid} {prod_name}')
 
     # make strings from the different lists
     wells = '\n'.join(wells)
     bimolecs = '\n'.join(bimolecs)
     tss = '\n'.join(tss)
-    barrierless = ''
+    barrierless = '\n'.join(bless)
 
     # write everything to a file
     fname = 'pesviewer.inp'
-    template_file_path = pkg_resources.resource_filename('tpl', fname + '.tpl')
+    template_file_path = f'{kb_path}/tpl/{fname}.tpl'
     with open(template_file_path) as template_file:
         template = template_file.read()
-    template = template.format(id=species.chemid, wells=wells, bimolecs=bimolecs, ts=tss, barrierless=barrierless)
+    template = template.format(id=species.chemid, wells=wells, ts=tss, 
+                               bimolecs=bimolecs, barrierless=barrierless)
     with open(fname, 'w') as f:
         f.write(template)
 
 
 def make_xyz(atoms, geom, name, directory):
     s = []
     s.append('%i\n' % len(geom))
     for index in range(len(geom)):
-        s.append('%s %.6f %.6f %.6f' % (atoms[index], geom[index][0], geom[index][1], geom[index][2]))
+        s.append('%s %.6f %.6f %.6f' % (atoms[index], geom[index][0], 
+                                        geom[index][1], geom[index][2]))
     with open(directory + '/' + name + '.xyz', 'w') as f:
         f.write('\n'.join(s))
```

### Comparing `kinbot-2.1.post0/kinbot/qc.py` & `kinbot-2.2.1/kinbot/qc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
 import sys
 import subprocess
 import logging
-import numpy as np
 import re
 import time
 from datetime import datetime
 import copy
-import pkg_resources
-from shutil import copyfile
 
+import numpy as np
 from ase.db import connect
+
+from kinbot import kb_path
 from kinbot import constants
 from kinbot import geometry
 
+logger = logging.getLogger('KinBot')
+
 
 class QuantumChemistry:
     """
     This class provides the link between KinBot and the qc code
     It choses the write options, submits the jobs and checks
     the jobs for success or failure
     """
@@ -107,15 +109,15 @@
                         'barrierless_saddle' in job or \
                         (mult == 1 and 'R_Addition_MultipleBond' in job):
                         kwargs['guess'] = 'Read,Mix'
                     if self.par['bimol']:
                         kwargs['method'] = self.method
                         kwargs['basis'] = self.basis
                         kwargs['opt'] = 'QST3,AddRedundant'
-                        del kwargs['guess']
+                        kwargs.pop('guess', None)
                 else:
                     kwargs['method'] = self.method
                     kwargs['basis'] = self.basis
                     if self.par['calcall_ts'] == 1:
                         kwargs['opt'] = 'NoFreeze,TS,CalcAll,NoEigentest,MaxCycle=999'
                         # not sending the frequency calculation for CalcAll
                     else:
@@ -138,15 +140,15 @@
                         (mult == 1 and 'R_Addition_MultipleBond' in job):
                         kwargs['guess'] = 'Read,Mix'  # Always is illegal here
                     else:
                         kwargs['guess'] = 'Read'
                     kwargs['irc'] = 'RCFC,{},MaxPoints={},StepSize={}'.format(irc, self.irc_maxpoints, self.irc_stepsize)
                 else:
                     kwargs['irc'] = 'RCFC,CalcFC,{},MaxPoints={},StepSize={}'.format(irc, self.irc_maxpoints, self.irc_stepsize)
-                del kwargs['freq']
+                kwargs.pop('freq', None)
             if high_level:
                 kwargs['method'] = self.high_level_method
                 kwargs['basis'] = self.high_level_basis
                 if len(self.opt) > 0:
                     kwargs['opt'] = 'NoFreeze,TS,CalcFC,NoEigentest,' \
                                     'MaxCycle=999,{}'.format(self.opt)  # to overwrite possible CalcAll
                 else:
@@ -155,19 +157,19 @@
                 kwargs['freq'] = 'freq'
                 if len(self.integral) > 0:
                     kwargs['integral'] = self.integral
                 if 'barrierless_saddle' in job:  # completely overwrite normal settings
                     kwargs['method'] = self.bls_high_level_method
                     kwargs['basis'] = self.bls_high_level_basis
                     kwargs['opt'] = 'NoFreeze,TS,CalcAll,NoEigentest,MaxCycle=999'  # to overwrite possible CalcAll
-                    del kwargs['freq']
+                    kwargs.pop('freq', None)
             if hir:
                 kwargs['opt'] = 'ModRedun,CalcFC'
                 if (not ts) or (ts and (not self.par['calcall_ts'])):
-                    del kwargs['freq']
+                    kwargs.pop('freq', None)
                 if ts:
                     if self.par['hir_maxcycle'] is None:
                         kwargs['opt'] = 'ModRedun,CalcFC,TS,NoEigentest'
                     else:
                         kwargs['opt'] = 'ModRedun,CalcFC,TS,NoEigentest,MaxCycle={}'.format(self.par['hir_maxcycle'])
                 if rigid == 1:
                     try:
@@ -299,37 +301,59 @@
         """
         from kinbot.geometry import calc_dihedral
         if species.wellorts:
             job = 'hir/' + species.name + '_hir_' + str(rot_index) + '_' + str(ang_index).zfill(2)
         else:
             job = 'hir/' + str(species.chemid) + '_hir_' + str(rot_index) + '_' + str(ang_index).zfill(2)
 
-        kwargs = self.get_qc_arguments(job, species.mult, species.charge, ts=species.wellorts, step=1, max_step=1,
+        kwargs = self.get_qc_arguments(job, species.mult, species.charge, 
+                                       ts=species.wellorts, step=1, max_step=1,
                                        high_level=1, hir=1, rigid=rigid)
         #kwargs['fix'] = fix  # for old hacked ASE version
 
-        if self.qc == 'gauss':
-            kwargs['addsec'] = f"{' '.join(str(f) for f in fix[0])} F"
-            del kwargs['chk']
+        if self.qc == 'gauss': 
+            code = 'gaussian'
+            Code = 'Gaussian'
+            if not self.par['use_sella']:
+                kwargs['addsec'] = f"{' '.join(str(f) for f in fix[0])} F"
+                kwargs.pop('chk', None)
         elif self.qc == 'qchem':
-            dihedral = calc_dihedral(geom[fix[0][0]-1], geom[fix[0][1]-1], geom[fix[0][2]-1], geom[fix[0][3]-1])[0]
-            kwargs['addsec'] = f"$opt\nCONSTRAINT\ntors {' '.join(str(f) for f in fix[0])} {dihedral}\n" \
-                               f"ENDCONSTRAINT\n$end"
-
+            code = 'qchem'
+            Code = 'QChem'
+            if not self.par['use_sella']:
+                dihedral = calc_dihedral(geom[fix[0][0]-1], geom[fix[0][1]-1], 
+                                         geom[fix[0][2]-1], geom[fix[0][3]-1])[0]
+                kwargs['addsec'] = "$opt\nCONSTRAINT\ntors " \
+                                   f"{' '.join(str(f) for f in fix[0])} " \
+                                   f"{dihedral}\nENDCONSTRAINT\n$end"
+        elif self.qc == 'nwchem':
+            code = 'nwchem'
+            Code = 'NWChem'
+        else:
+            raise ValueError(f'Unexpected vale for qc parameter: {self.qc}')
 #        atom, geom, dummy = self.add_dummy(species.atom, geom, species.bond)
-
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_hir.tpl.py'.format(qc=self.qc))
+        if self.par['use_sella']:
+            kwargs.pop('chk', None)
+            kwargs.pop('opt', None)
+            kwargs.pop('freq', None)
+            template_file = f'{kb_path}/tpl/ase_sella_hir.tpl.py'
+        else:
+            template_file = f'{kb_path}/tpl/ase_{self.qc}_hir.tpl.py'
         template = open(template_file, 'r').read()
         template = template.format(label=job,
                                    kwargs=kwargs,
                                    atom=list(species.atom),
                                    geom=list([list(gi) for gi in geom]),
                                    ppn=self.ppn,
                                    qc_command=self.qc_command,
-                                   working_dir=os.getcwd())
+                                   working_dir=os.getcwd(),
+                                   fix=fix[0],
+                                   code=code,
+                                   Code=Code,
+                                   order=species.wellorts)
 
         with open(f'{job}.py', 'w') as f:
             f.write(template)
 
         self.submit_qc(job)
 
         return 0
@@ -343,36 +367,59 @@
         qc: 'gauss' or 'nwchem' or 'qchem'
         scan: list of dihedrals to be scanned and their values
         wellorts: 0 for wells and 1 for saddle points
         conf_nr: number of the conformer in the conformer search
         scan_nr: number of the scan for this conformer
         """
         if species.wellorts:
-            job = 'conf/' + species.name + '_r' + str(conf_nr).zfill(self.zf) + '_' + str(scan_nr).zfill(self.zf)
+            job = 'conf/' + species.name + '_r' + str(conf_nr).zfill(self.zf) \
+                  + '_' + str(scan_nr).zfill(self.zf)
         else:
-            job = 'conf/' + str(species.chemid) + '_r' + str(conf_nr).zfill(self.zf) + '_' + str(scan_nr).zfill(self.zf)
-
-        kwargs = self.get_qc_arguments(job, species.mult, species.charge, ts=species.wellorts, step=1, max_step=1, hir=1)
+            job = 'conf/' + str(species.chemid) + '_r' \
+                  + str(conf_nr).zfill(self.zf) + '_' \
+                  + str(scan_nr).zfill(self.zf)
+
+        kwargs = self.get_qc_arguments(job, species.mult, species.charge, 
+                                       ts=species.wellorts, step=1, max_step=1, 
+                                       hir=1)
 
-        del kwargs['opt']
-        del kwargs['chk']
+        kwargs.pop('opt', None)
+        kwargs.pop('chk', None)
         kwargs['method'] = 'am1'
         kwargs['basis'] = ''
 
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_ring_conf.tpl.py'.format(qc=self.qc))
+        if self.qc == 'gauss':
+            code = 'gaussian'
+            Code = 'Gaussian'
+        elif self.qc == 'qchem':
+            code = 'qchem'
+            Code = 'QChem'
+        elif self.qc == 'nwchem':
+            code = 'nwchem'
+            Code = 'NWChem'
+        else:
+            raise ValueError(f'Unexpected vale for qc parameter: {self.qc}')
+
+        if self.par['use_sella']:
+            template_file = f'{kb_path}/tpl/ase_sella_ring_conf.tpl.py'
+        else:
+            template_file = f'{kb_path}/tpl/ase_{self.qc}_ring_conf.tpl.py'
         template = open(template_file, 'r').read()
         template = template.format(label=job,
                                    kwargs=kwargs,
                                    atom=list(species.atom),
                                    geom=list([list(gi) for gi in geom]),
                                    fix=fix,
                                    change=change,
                                    ppn=self.ppn,
                                    qc_command=self.qc_command,
-                                   working_dir=os.getcwd())
+                                   working_dir=os.getcwd(),
+                                   order=species.wellorts,
+                                   code=code,
+                                   Code=Code)
 
         with open(f'{job}.py', 'w') as f:
             f.write(template)
 
         self.submit_qc(job)
         return 0
 
@@ -385,43 +432,63 @@
         """
         add = ''
         if semi_emp:
             add = 'semi_emp_'
         if species.wellorts:
             job = 'conf/' + species.name + '_' + add + str(index).zfill(self.zf)
         else:
-            job = 'conf/' + str(species.chemid) + '_' + add + str(index).zfill(self.zf)
+            job = 'conf/' + str(species.chemid) + '_' + add \
+                  + str(index).zfill(self.zf)
 
         if species.wellorts:
             kwargs = self.get_qc_arguments(job, species.mult, species.charge, 
                                            ts=1, step=1, max_step=1)
         else:
             kwargs = self.get_qc_arguments(job, species.mult, species.charge)
-            if self.qc == 'gauss':
+            if self.qc == 'gauss' and not self.par['use_sella']:
                 if self.par['opt'].casefold() == 'Tight'.casefold(): 
                     kwargs['opt'] = 'CalcFC, Tight'
                 else:
                     kwargs['opt'] = 'CalcFC'
+
         if self.qc == 'gauss':
-            del kwargs['chk']
+            code = 'gaussian'
+            Code = 'Gaussian'
+            kwargs.pop('chk', None)
+        elif self.qc == 'qchem':
+            code = 'qchem'
+            Code = 'QChem'
+        elif self.qc == 'nwchem':
+            code = 'nwchem'
+            Code = 'NWChem'
+        else:
+            raise ValueError(f'Unexpected vale for qc parameter: {self.qc}')
+        
         if semi_emp:
             kwargs['method'] = self.par['semi_emp_method']
             kwargs['basis'] = ''
         if species.natom < 3:
-            del kwargs['Symm'] 
-        
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_opt_well.tpl.py'.format(qc=self.qc))
+            kwargs.pop('Symm', None)
+        if self.par['use_sella']:
+            kwargs.pop('opt', None)
+            kwargs.pop('freq', None)
+            template_file = f'{kb_path}/tpl/ase_sella_opt_well.tpl.py'
+        else:        
+            template_file = f'{kb_path}/tpl/ase_{self.qc}_opt_well.tpl.py'
         template = open(template_file, 'r').read()
         template = template.format(label=job,
                                    kwargs=kwargs,
                                    atom=list(species.atom),
                                    geom=list([list(gi) for gi in geom]),
-                                   ppn=self.ppn,
+                                   ppn=self.ppn,  # QChem and NWChem
                                    qc_command=self.qc_command,
-                                   working_dir=os.getcwd())
+                                   working_dir=os.getcwd(),
+                                   code=code,    # Sella
+                                   Code=Code,    # Sella
+                                   order=species.wellorts)    
         
         with open(f'{job}.py', 'w') as f:
             f.write(template)
 
         self.submit_qc(job)
 
         return 0
@@ -436,15 +503,15 @@
         job0 = f'aie/{str(species.chemid)}_AIE0_{ext}'  # neutral
         job1 = f'aie/{str(species.chemid)}_AIE1_{ext}'  # cation
         kwargs0 = self.get_qc_arguments(job0, species.mult, species.charge, aie=1)
         if species.mult == 1: m1 = 2
         elif species.mult == 2: m1 = 1
         elif species.mult == 3: m1 = 2
         kwargs1 = self.get_qc_arguments(job1, m1, species.charge + 1, aie=1)
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_opt_well.tpl.py'.format(qc=self.qc))
+        template_file = f'{kb_path}/tpl/ase_{self.qc}_opt_well.tpl.py'
         template = open(template_file, 'r').read()
         t0 = template.format(label=job0,
                              kwargs=kwargs0,
                              atom=list(species.atom),
                              geom=list([list(gi) for gi in geom]),
                              ppn=self.ppn,
                              qc_command=self.qc_command,
@@ -462,15 +529,16 @@
         with open(f'{job1}.py', 'w') as f:
             f.write(t1)
         self.submit_qc(job0)
         self.submit_qc(job1)
 
         return 0
 
-    def qc_opt(self, species, geom, high_level=0, mp2=0, bls=0, ext=None, fdir=None):
+    def qc_opt(self, species, geom, high_level=0, mp2=0, bls=0, ext=None, 
+               fdir=None):
         """
         Creates a geometry optimization input and runs it.
         """
         if ext is None:
             job = str(species.chemid) + '_well'
             if high_level:
                 job = str(species.chemid) + '_well_high'
@@ -483,49 +551,68 @@
 
         if fdir is not None:
             job = f'{fdir}/{job}'
 
         # TODO: Code exceptions into their own function/py script that opt can call.
         # TODO: Fix symmetry numbers for calcs as well if needed
         # O2
-        if species.chemid == "320320000000000000001":
+        if species.chemid == '320320000000000000001':
             mult = 3
         # CH2
-        elif species.chemid == "140260020000000000001":
+        elif species.chemid == '140260020000000000001':
             mult = 3
         else:
             mult = species.mult
 
         kwargs = self.get_qc_arguments(job, mult, species.charge,
                                        high_level=high_level)
 
         if self.qc == 'gauss':
+            code = 'gaussian'
+            Code = 'Gaussian'
             if self.par['opt'].casefold() == 'Tight'.casefold(): 
                 kwargs['opt'] = 'CalcFC, Tight'
             else:
                 kwargs['opt'] = 'CalcFC'
+        elif self.qc == 'qchem':
+            code = 'qchem'
+            Code = 'QChem'
+        elif self.qc == 'nwchem':
+            code = 'nwchem'
+            Code = 'NWChem'   
+        else:
+            raise ValueError(f'Unexpected vale for qc parameter: {self.qc}')
+        
         if mp2:
             kwargs['method'] = self.scan_method
             kwargs['basis'] = self.scan_basis
-        if high_level and self.qc == 'gauss':
-            if self.opt:
-                kwargs['opt'] = 'CalcFC, {}'.format(self.opt)
+        if high_level and self.qc == 'gauss'and self.opt \
+                and not self.par['use_sella']:
+            kwargs['opt'] = 'CalcFC, {}'.format(self.opt)
         if species.natom < 3:
-            del kwargs['Symm'] 
+            kwargs.pop('Symm', None)
         # the integral is set in the get_qc_arguments parts, bad design
+        if self.par['use_sella']:
+            kwargs.pop('opt', None)
+            kwargs.pop('freq', None)
+            template_file = f'{kb_path}/tpl/ase_sella_opt_well.tpl.py'
+        else:
+            template_file = f'{kb_path}/tpl/ase_{self.qc}_opt_well.tpl.py'
 
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_opt_well.tpl.py'.format(qc=self.qc))
         template = open(template_file, 'r').read()
         template = template.format(label=job,
                                    kwargs=kwargs,
                                    atom=list(species.atom),
                                    geom=list([list(gi) for gi in geom]),
-                                   ppn=self.ppn,
+                                   ppn=self.ppn,  # QChem and NWChem
                                    qc_command=self.qc_command,
-                                   working_dir=os.getcwd())
+                                   working_dir=os.getcwd(),
+                                   code=code,    # Sella
+                                   Code=Code,    # Sella
+                                   order=0)      # Sella
 
         with open(f'{job}.py', 'w') as f:
             f.write(template)
 
         self.submit_qc(job)
         return 0
 
@@ -539,34 +626,55 @@
                 job += '_high'
         else:
             job += ext
 
         if fdir is not None:
             job = f'{fdir}/{job}'
 
-        kwargs = self.get_qc_arguments(job, species.mult, species.charge, ts=1, step=1, max_step=1, high_level=1)
-
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_ts_end.tpl.py'.format(qc=self.qc))
+        kwargs = self.get_qc_arguments(job, species.mult, species.charge, ts=1, 
+                                       step=1, max_step=1, high_level=1)
+        
+        if self.qc == 'gauss':
+            code = 'gaussian'
+            Code = 'Gaussian'
+        elif self.qc == 'qchem':
+            code = 'qchem'
+            Code = 'QChem'
+        elif self.qc == 'nwchem':
+            code = 'nwchem'
+            Code = 'NWChem'
+        else:
+            raise ValueError(f"Unrecognized qc option: {self.qc}")
+        
+        if self.par['use_sella']:
+            kwargs.pop('addsec', None)
+            kwargs.pop('opt', None)
+            kwargs.pop('freq', None)
+            template_file = f'{kb_path}/tpl/ase_sella_ts_end.tpl.py'
+        else:
+            template_file = f'{kb_path}/tpl/ase_{self.qc}_ts_end.tpl.py'
         template = open(template_file, 'r').read()
         template = template.format(label=job,
                                    kwargs=kwargs,
                                    atom=list(species.atom),
                                    geom=list([list(gi) for gi in geom]),
                                    ppn=self.ppn,
                                    qc_command=self.qc_command,
-                                   working_dir=os.getcwd())
+                                   working_dir=os.getcwd(),
+                                   code=code,
+                                   Code=Code)
 
         with open(f'{job}.py', 'w') as f:
             f.write(template)
 
         self.submit_qc(job)
 
         return 0
 
-    def submit_qc(self, job, singlejob=1):
+    def submit_qc(self, job, singlejob=1, jobtype=None):
         """Submit a job to the queue, unless the job:
             * has finished with Normal termination
             * has finished with Error termination
             * is currently running
         However, if the optional parameter singlejob is set to zero, then
         the job is run only if it has finished earlier with normal termination.
         This is for continuations, when the continuing jobs overwrite each other.
@@ -583,43 +691,49 @@
             if check == 'running':
                 return 0
 
         if self.queue_job_limit > 0:
             self.limit_jobs()
 
         try:
-            if self.par['queue_template'] == '':
-                template_head_file = pkg_resources.resource_filename('tpl', self.queuing + '.tpl')
+            if jobtype == 'am1':
+                template_head_file = self.par['q_temp_am1']
+            elif job.endswith('mp2') and self.par['q_temp_mp2']:
+                template_head_file = self.par['q_temp_mp2']
+            elif job.endswith('high') and self.par['q_temp_hi']:
+                template_head_file = self.par['q_temp_hi']
+            elif self.par['queue_template'] == '':
+                template_head_file = f'{kb_path}/tpl/{self.queuing}.tpl'
             else:
                 template_head_file = self.par['queue_template']
         except OSError:
-            logging.error('KinBot does not recognize queuing system {}.'.format(self.queuing))
-            logging.error('Or no file is found at {}.'.format(self.par['queue_template']))
-            logging.error('Exiting')
+            logger.error('KinBot does not recognize queuing system {}.'.format(self.queuing))
+            logger.error('Or no file is found at {}.'.format(self.par['queue_template']))
+            logger.error('Exiting')
             sys.exit()
 
         if self.queuing == 'local':
-            logging.error(f'Output file for job {job} is missing. Unable to '
-                          'carry out calculations when queuing is \'local\'.')
+            logger.error(f'Job {job} is missing in the database or the output '
+                         'file is not present. Unable to run calculations when '
+                         'queuing is \'local\'.')
             sys.exit()
 
-        template_file = pkg_resources.resource_filename('tpl', self.queuing + '_python.tpl')
+        template_file = f'{kb_path}/tpl/{self.queuing}_python.tpl'
         python_file = f'{job}.py'
-        name = job.split('/')[-1]
         python_template = open(template_head_file, 'r').read() + open(template_file, 'r').read()
 
         if self.queuing == 'pbs':
             python_template = python_template.format(name=job, ppn=self.ppn, queue_name=self.queue_name,
-                                                        errdir='perm', python_file=python_file, arguments='')
+                                                     errdir='perm', python_file=python_file, arguments='')
         elif self.queuing == 'slurm':
             python_template = python_template.format(name=job, ppn=self.ppn, queue_name=self.queue_name, errdir='perm',
-                                                        slurm_feature=self.slurm_feature, python_file=python_file, arguments='')
+                                                     slurm_feature=self.slurm_feature, python_file=python_file, arguments='')
         else:
-            logging.error('KinBot does not recognize queuing system {}.'.format(self.queuing))
-            logging.error('Exiting')
+            logger.error('KinBot does not recognize queuing system {}.'.format(self.queuing))
+            logger.error('Exiting')
             sys.exit()
 
         qu_file = '{}{}'.format(job, constants.qext[self.queuing])
         with open(qu_file, 'w') as f_out_qu:
             f_out_qu.write(python_template)
 
         command = [constants.qsubmit[self.queuing], job + constants.qext[self.queuing]]
@@ -632,20 +746,20 @@
                 pid = out.split('\n')[0].split('.')[0]
             elif self.queuing == 'slurm':
                 pid = out.split('\n')[0].split()[3]
         except:
             msg = 'Something went wrong when submitting a job'
             msg += 'This is the standard output:\n' + out
             msg += '\nThis is the standard error:\n' + err
-            logging.error(msg)
+            logger.error(msg)
             sys.exit()
         self.job_ids[job] = pid
 
         now = datetime.now()
-        logging.debug(f'SUBMITTED {job} on {now.ctime()}')
+        logger.debug(f'SUBMITTED {job} on {now.ctime()}')
         return 1  # important to keep it 1, this is the natural counter of jobs submitted
 
     def get_qc_geom(self, job, natom, wait=0, allow_error=0, previous=0):
         """
         Get the geometry from the ase database file.
         Returns it, with the following conditions about the status of the job.
         If wait = 0, return an (1, empty array) when the job is still running (instead of the geometry).
@@ -803,15 +917,15 @@
         rows = self.db.select(name=job)
         # take the last entry
         for row in rows:
             if hasattr(row, 'data'):
                 zpe = row.data.get('zpe')
             else:
                 zpe = 0.0
-                logging.warning("{} has no zpe in database. ZPE SET TO 0.0".format(job))
+                logger.warning("{} has no zpe in database. ZPE SET TO 0.0".format(job))
 
         if zpe is None:
             zpe = 0.00
 
         return 0, zpe
 
     def read_qc_hess(self, job, natom):
@@ -819,15 +933,19 @@
         Read the hessian of a gaussian chk file
         """
 
         check = self.check_qc(job)
         if check != 'normal':
             return []
 
-        if self.qc == 'gauss':
+        if self.par['use_sella']:
+            db = connect('kinbot.db')
+            row = next(db.select(name=job))
+            hess = row.data['hess']
+        elif self.qc == 'gauss':
             hess = np.zeros((3 * natom, 3 * natom))
             fchk = str(job) + '.fchk'
             if not os.path.exists(fchk):
                 # create the fchk file using formchk
                 os.system('formchk ' + job + '.chk > /dev/null')
 
             with open(fchk) as f:
@@ -844,14 +962,17 @@
                     n = 0
                     for i in range(3 * natom):
                         for j in range(i + 1):
                             hess[i][j] = hess_flat[n]
                             hess[j][i] = hess_flat[n]
                             n += 1
                     break
+            else:
+                raise FileNotFoundError(f'Hessian matrix not found on {fchk}.')
+            
         elif self.qc == 'qchem':
             hess = []
             row = 0
             do_read = False
             if natom == 1:
                 return np.zeros([3, 3])
             with open(job + '_freq.out') as f:
@@ -899,20 +1020,20 @@
         Possible returns:
         running - the job is either running or is in the queue
         status - this can be normal or error, read from the database.
                  Only happens if log file had a done stamp and it was in the db.
         0 - job is not in the db or log file is not there with a done stamp or both.
             ==> this one resets the step number to 0
         """
-        #logging.debug('Checking job {}'.format(job))
+        # logger.debug('Checking job {}'.format(job))
         devnull = open(os.devnull, 'w')
         if self.queuing == 'pbs':
             command = 'qstat -f | grep ' + '"Job Id: ' + self.job_ids.get(job, '-1') + '"' + ' > /dev/null'
             if int(subprocess.call(command, shell=True, stdout=devnull, stderr=devnull)) == 0:
-                #logging.debug('Job is running')
+                # logger.debug('Job is running')
                 return 'running'
         elif self.queuing == 'slurm':
             # command = 'scontrol show job ' + self.job_ids.get(job,'-1') + ' | grep "JobId=' + self.job_ids.get(job,'-1') + '"' + ' > /dev/null'
             command = 'squeue'
             process = subprocess.Popen(command,
                                        shell=True,
                                        stdout=subprocess.PIPE,
@@ -922,72 +1043,71 @@
             out = out.decode()
             for line in out.split('\n'):
                 if len(line) > 0:
                     while line.startswith(' '):
                         line = line[1:]
                     pid = line.split()[0]
                     if pid == self.job_ids.get(job, '-1'):
-                        logging.debug('Job is running')
+                        logger.debug('Job is running')
                         return 'running'
         elif self.queuing == 'local':
             pass
-
         else:
-            logging.error('KinBot does not recognize queuing system {}.'.format(self.queuing))
-            logging.error('Exiting')
+            logger.error('KinBot does not recognize queuing system {}.'.format(self.queuing))
+            logger.error('Exiting')
             sys.exit()
         # if int(subprocess.call(command, shell=True, stdout=devnull, stderr=devnull)) == 0:
         #     return 'running'
 
         if self.is_in_database(job):
             for i in range(1):
-
                 if self.qc == 'gauss':
                     log_file = job + '.log'
                 elif self.qc == 'nwchem':
                     log_file = job + '.out'
                 elif self.qc == 'qchem':
                     log_file = job + '.out'
                 else:
                     raise ValueError('Unknown code')
                 log_file_exists = os.path.exists(log_file)
                 if log_file_exists:
                     with open(log_file, 'r') as f:
                         try:
                             last_line = f.readlines()[-1]
                             if 'done' not in last_line:
-                                logging.debug(f'Log file {log_file} is present, but has no "done" stamp.')
+                                logger.debug(f'Log file {log_file} is present, '
+                                             'but has no "done" stamp.')
                                 return 0
                         except IndexError:
-                            logging.debug(f'Log file {log_file} is present, but it is empty.')
+                            logger.debug(f'Log file {log_file} is present, but it is empty.')
                             pass
-                    logging.debug('Log file is present after {} iterations'.format(i))
+                    logger.debug('Log file is present after {} iterations'.format(i))
                     # by deleting a log file, you allow restarting a job
                     # open the database
                     rows = self.db.select(name=job)
                     data = None
                     # take the last entry
                     for row in rows:
                         if hasattr(row, 'data'):
                             data = row.data
                     if data is None:
-                        logging.debug('Data is not in database...')
+                        logger.debug('Data is not in database...')
                         return 0
                     else:
-                        logging.debug('Returning status {}'.format(data['status']))
+                        logger.debug('Returning status {}'.format(data['status']))
                         return data['status']
                 else:
-                    logging.debug('Checking againg for log file')
+                    logger.debug('Checking againg for log file')
                     log_file_exists = os.path.exists(log_file)
                     time.sleep(1)
 
-            logging.debug('log file {} does not exist'.format(log_file))
+            logger.debug('log file {} does not exist'.format(log_file))
             return 0
         else:
-            logging.debug('job {} is not in database'.format(job))
+            logger.debug('job {} is not in database'.format(job))
             return 0
 
     def limit_jobs(self):
         """
         Check how many jobs are in the queue from the user, and if larger than the limit,
         then wait for resources to free up.
         """
```

### Comparing `kinbot-2.1.post0/kinbot/reac_General.py` & `kinbot-2.2.1/kinbot/reac_General.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/reac_family.py` & `kinbot-2.2.1/kinbot/reac_family.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 import os
 import numpy as np
-import pkg_resources
+
+from kinbot import kb_path
 from kinbot import modify_geom
 from kinbot import geometry
-from reactions.reac_abstraction import abstraction_align
+from kinbot.reactions.reac_abstraction import abstraction_align
 
 
 def carry_out_reaction(rxn, step, command, bimol=0):
     """
     Verify what has been done and what needs to be done
-    skip: boolean which tells to skip the first 12 steps in case of an instance shorter than 4
-    scan: boolean which tells if this is part of an energy scan along a bond length coordinate
+    skip: boolean which tells to skip the first 12 steps in case of an instance 
+        shorter than 4
+    scan: boolean which tells if this is part of an energy scan along a bond 
+        length coordinate
     """
     if step > 0:
         status = rxn.qc.check_qc(rxn.instance_name)
         if status != 'normal' and status != 'error':
             return step
   
-    kwargs = rxn.qc.get_qc_arguments(rxn.instance_name, rxn.species.mult, rxn.species.charge, ts=1,
-                                     step=step, max_step=rxn.max_step, scan=rxn.scan)
+    kwargs = rxn.qc.get_qc_arguments(rxn.instance_name, rxn.species.mult, 
+                                     rxn.species.charge, ts=1, step=step, 
+                                     max_step=rxn.max_step, scan=rxn.scan)
     if step == 0:
         if rxn.qc.is_in_database(rxn.instance_name):
             if rxn.qc.check_qc(rxn.instance_name) == 'normal':  # log file is present and is in the db
                 err, freq = rxn.qc.get_qc_freq(rxn.instance_name, rxn.species.natom)
                 if err == 0 and len(freq) > 0.:  # only final calculations have frequencies
                     err, geom = rxn.qc.get_qc_geom(rxn.instance_name, rxn.species.natom)
                     step = rxn.max_step + 1  # this shortcuts the search, jumps to the end
                     return step
             if rxn.qc.check_qc(rxn.instance_name) == 'error':  # log file is present and is in the db
                 err, geom = rxn.qc.get_qc_geom(rxn.instance_name, rxn.species.natom, allow_error=1)
                 if np.sum(geom) == 0:
                     return -1  # we don't want this to be repeated
 
-
         if rxn.skip and len(rxn.instance) < 4:
             step = 12
         geom = rxn.species.geom
         if bimol:
             if rxn.family_name == 'abstraction':
                 # gives the reactant and product geometry guesses
                 geom, _, _ = abstraction_align(rxn.species.geom, rxn.instance, rxn.species.atom, rxn.species.fragA.natom)
 
     elif step == rxn.max_step and rxn.scan:
-        err, geom = rxn.qc.get_qc_geom(rxn.instance_name, rxn.species.natom, allow_error=1, previous=1)
+        err, geom = rxn.qc.get_qc_geom(rxn.instance_name, rxn.species.natom, 
+                                       allow_error=1, previous=1)
     else:
         err, geom = rxn.qc.get_qc_geom(rxn.instance_name, rxn.species.natom, allow_error=1)
         if bimol:
             if rxn.family_name == 'abstraction':
                 # gives the reactant and product geometry guesses
                 _, geom_prod, geom_ts = abstraction_align(geom, rxn.instance, rxn.species.atom, rxn.species.fragA.natom)
 
-
     step, fix, change, release = rxn.get_constraints(step, geom)
 
     if step > rxn.max_step:
         return step
 
     # apply the geometry changes here and fix the coordinates that changed
     change_starting_zero = []
     for c in change:
         c_new = [ci - 1 for ci in c[:-1]]
         c_new.append(c[-1])
         change_starting_zero.append(c_new)
     if len(change_starting_zero) > 0:
-        success, geom = modify_geom.modify_coordinates(rxn.species, rxn.instance_name, geom, change_starting_zero,
+        success, geom = modify_geom.modify_coordinates(rxn.species, 
+                                                       rxn.instance_name, geom, 
+                                                       change_starting_zero,
                                                        rxn.species.bond)
         for c in change:
             fix.append(c[:-1])
         change = []
 
-    #atom, geom, dummy = rxn.qc.add_dummy(rxn.species.atom, geom, rxn.species.bond)
+    # atom, geom, dummy = rxn.qc.add_dummy(rxn.species.atom, geom,
+    #                                      rxn.species.bond)
 
     if rxn.qc.qc == 'gauss':
+        code = 'gaussian'
+        Code = 'Gaussian'
         kwargs['addsec'] = ''
         if not bimol or step == 0:
             # here addsec contains the constraints
             for fixi in fix:
                 kwargs['addsec'] += f"{' '.join(str(f) for f in fixi)} F\n"
             for chi in change:
                 kwargs['addsec'] += f"{' '.join(str(ch) for ch in chi)} F\n"
@@ -90,14 +98,16 @@
             kwargs['addsec'] += f'\n{rxn.instance[0] + 1} {rxn.instance[2] + 1}\n\n'
             kwargs['addsec'] += f'ts geometry guess\n\n{rxn.species.charge} {rxn.species.mult}\n'
             for ii, at in enumerate(rxn.species.atom):
                 kwargs['addsec'] += f'{at} {geom_ts[ii][0]} {geom_ts[ii][1]} {geom_ts[ii][2]}\n'
             kwargs['addsec'] += f'\n{rxn.instance[0] + 1} {rxn.instance[2] + 1}\n\n'
 
     elif rxn.qc.qc == 'qchem':
+        code = 'qchem'
+        Code = 'QChem'
         if (not bimol or step == 0) and step < rxn.max_step:
             kwargs['addsec'] = '$opt\nCONSTRAINT\n'
             for fixi in fix:
                 if len(fixi) == 2:
                     fix_type = 'stre'
                     val = np.linalg.norm(geom[fixi[0] - 1] - geom[fixi[1] - 1])
                 elif len(fixi) == 3:
@@ -112,50 +122,60 @@
                 dist = np.linalg.norm(geom[chi[0] - 1] - geom[chi[1] - 1])
                 kwargs['addsec'] += f"{' '.join(str(ch) for ch in chi)} {dist}\n"
             for reli in release:
                 dist = np.linalg.norm(geom[reli][0] - geom[reli][1])
                 kwargs['addsec'] += f"{' '.join(str(rel) for rel in reli)} {dist}\n"
             kwargs['addsec'] += 'ENDCONSTRAINT\n$end\n'
         elif bimol and step == 1:
-            raise NotImplementedError('Bimolecular reactions are not yet implemented'
-                                      ' in QChem')
+            raise NotImplementedError('Bimolecular reactions are not yet '
+                                      'implemented in QChem')
     # if not bimol:
     #     ntrial = 3
     # else:
     #     ntrial = 1
 
     if step < rxn.max_step:
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_ts_search.tpl.py'.format(qc=rxn.qc.qc))
+        if rxn.par['use_sella']:
+            kwargs.pop('addsec', None)
+            kwargs.pop('opt', None)
+            template_file = f'{kb_path}/tpl/ase_sella_ts_search.tpl.py'
+        else:
+            template_file = f'{kb_path}/tpl/ase_{rxn.qc.qc}_ts_search.tpl.py'
         template = open(template_file,'r').read()
         template = template.format(label=rxn.instance_name, 
                                    kwargs=kwargs, 
-                                   #atom=list(atom),
                                    atom=list(rxn.species.atom),
                                    geom=list([list(gi) for gi in geom]),
-                                   #dummy=dummy,
                                    bimol=bimol,
                                    ppn=rxn.qc.ppn,
                                    qc_command=command,
                                    working_dir=os.getcwd(),
                                    scan=rxn.scan,
-                                   )
-                                   #ntrial=ntrial,
+                                   code=code,
+                                   Code=Code,
+                                   fix=fix)
     else:
-        template_file = pkg_resources.resource_filename('tpl', 'ase_{qc}_ts_end.tpl.py'.format(qc=rxn.qc.qc))
+        if rxn.par['use_sella']:
+            kwargs.pop('addsec', None)
+            kwargs.pop('opt', None)
+            template_file = f'{kb_path}/tpl/ase_sella_ts_end.tpl.py'
+        else:
+            template_file = f'{kb_path}/tpl/ase_{rxn.qc.qc}_ts_end.tpl.py'
         template = open(template_file, 'r').read()
     
         template = template.format(label=rxn.instance_name, 
-                                   kwargs=kwargs, 
-                                   #atom=list(atom),
+                                   kwargs=kwargs,
                                    atom=list(rxn.species.atom),
                                    geom=list([list(gi) for gi in geom]),
-                                   #dummy=dummy,
                                    ppn=rxn.qc.ppn,
                                    qc_command=command,
-                                   working_dir=os.getcwd())
+                                   working_dir=os.getcwd(),
+                                   code=code,
+                                   Code=Code)
                                    
     with open('{}.py'.format(rxn.instance_name),'w') as f_out:
         f_out.write(template)
 
-    step += rxn.qc.submit_qc(rxn.instance_name, singlejob=0)
+    step += rxn.qc.submit_qc(rxn.instance_name, singlejob=0, 
+                             jobtype=kwargs['method'])
 
     return step
```

### Comparing `kinbot-2.1.post0/kinbot/reaction_finder.py` & `kinbot-2.2.1/kinbot/reaction_finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import numpy as np
 import sys
 import copy
 import logging
 
 from kinbot import bond_combinations
 from kinbot import find_motif
-from reactions.reac_Cyclic_Ether_Formation import CyclicEtherFormation
-from reactions.reac_Diels_alder_addition import DielsAlder
-from reactions.reac_Intra_Diels_alder_R import IntraDielsAlder
-from reactions.reac_12_shift_S_F import S12ShiftF
-from reactions.reac_12_shift_S_R import S12ShiftR
-from reactions.reac_cpd_H_migration import CpdHMigration
-from reactions.reac_intra_H_migration import IntraHMigration
-from reactions.reac_intra_H_migration_suprafacial import IntraHMigrationSuprafacial
-from reactions.reac_intra_OH_migration import IntraOHMigration
-from reactions.reac_intra_OH_migration_Exocyclic_F import IntraOHMigrationExocyclicF
-from reactions.reac_Intra_R_Add_Endocyclic_F import IntraRAddEndocyclicF
-from reactions.reac_Intra_R_Add_Exocyclic_F import IntraRAddExocyclicF
-from reactions.reac_Intra_R_Add_ExoTetCyclic_F import IntraRAddExoTetCyclicF
-from reactions.reac_intra_R_migration import IntraRMigration
-from reactions.reac_Retro_Ene import RetroEne
-from reactions.reac_r22_cycloaddition import R22Cycloaddition
-from reactions.reac_r12_insertion_R import R12Insertion
-from reactions.reac_r13_insertion_RSR import R13InsertionRSR
-from reactions.reac_r13_insertion_ROR import R13InsertionROR
-from reactions.reac_r13_insertion_CO2 import R13InsertionCO2
-from reactions.reac_r12_cycloaddition import R12Cycloaddition
-from reactions.reac_R_Addition_MultipleBond import RAdditionMultipleBond
-from reactions.reac_R_Addition_CSm_R import RAdditionCS
-from reactions.reac_R_Addition_COm3_R import RAdditionCO
-from reactions.reac_Korcek_step2_odd import KorcekStep2Odd
-from reactions.reac_Korcek_step2_even import KorcekStep2Even
-from reactions.reac_Korcek_step2 import KorcekStep2
-from reactions.reac_ketoenol import KetoEnol
-from reactions.reac_Intra_RH_Add_Exocyclic_R import IntraRHAddExoR
-from reactions.reac_Intra_RH_Add_Exocyclic_F import IntraRHAddExoF
-from reactions.reac_Intra_RH_Add_Endocyclic_R import IntraRHAddEndoR
-from reactions.reac_Intra_RH_Add_Endocyclic_F import IntraRHAddEndoF
-from reactions.reac_HO2_Elimination_from_PeroxyRadical import HO2Elimination
-from reactions.reac_beta_delta import BetaDelta
-from reactions.reac_birad_recombination_F import BiradRecombinationF
-from reactions.reac_birad_recombination_R import BiradRecombinationR
-from reactions.reac_Intra_disproportionation_R import IntraDisproportionationR
-from reactions.reac_Intra_disproportionation_F import IntraDisproportionationF
-from reactions.reac_r14_birad_scission import R14BiradScission
-from reactions.reac_r14_cyclic_birad_scission_R import R14CyclicBiradScission
-from reactions.reac_barrierless_saddle import BarrierlessSaddle
-from reactions.reac_h2_elim import H2Elim
-from reactions.reac_homolytic_scission import HS 
+from kinbot.reactions.reac_Cyclic_Ether_Formation import CyclicEtherFormation
+from kinbot.reactions.reac_Diels_alder_addition import DielsAlder
+from kinbot.reactions.reac_Intra_Diels_alder_R import IntraDielsAlder
+from kinbot.reactions.reac_12_shift_S_F import S12ShiftF
+from kinbot.reactions.reac_12_shift_S_R import S12ShiftR
+from kinbot.reactions.reac_cpd_H_migration import CpdHMigration
+from kinbot.reactions.reac_intra_H_migration import IntraHMigration
+from kinbot.reactions.reac_intra_H_migration_suprafacial import IntraHMigrationSuprafacial
+from kinbot.reactions.reac_intra_OH_migration import IntraOHMigration
+from kinbot.reactions.reac_intra_OH_migration_Exocyclic_F import IntraOHMigrationExocyclicF
+from kinbot.reactions.reac_Intra_R_Add_Endocyclic_F import IntraRAddEndocyclicF
+from kinbot.reactions.reac_Intra_R_Add_Exocyclic_F import IntraRAddExocyclicF
+from kinbot.reactions.reac_Intra_R_Add_ExoTetCyclic_F import IntraRAddExoTetCyclicF
+from kinbot.reactions.reac_intra_R_migration import IntraRMigration
+from kinbot.reactions.reac_Retro_Ene import RetroEne
+from kinbot.reactions.reac_r22_cycloaddition import R22Cycloaddition
+from kinbot.reactions.reac_r12_insertion_R import R12Insertion
+from kinbot.reactions.reac_r13_insertion_RSR import R13InsertionRSR
+from kinbot.reactions.reac_r13_insertion_ROR import R13InsertionROR
+from kinbot.reactions.reac_r13_insertion_CO2 import R13InsertionCO2
+from kinbot.reactions.reac_r12_cycloaddition import R12Cycloaddition
+from kinbot.reactions.reac_R_Addition_MultipleBond import RAdditionMultipleBond
+from kinbot.reactions.reac_R_Addition_CSm_R import RAdditionCS
+from kinbot.reactions.reac_R_Addition_COm3_R import RAdditionCO
+from kinbot.reactions.reac_Korcek_step2_odd import KorcekStep2Odd
+from kinbot.reactions.reac_Korcek_step2_even import KorcekStep2Even
+from kinbot.reactions.reac_Korcek_step2 import KorcekStep2
+from kinbot.reactions.reac_ketoenol import KetoEnol
+from kinbot.reactions.reac_Intra_RH_Add_Exocyclic_R import IntraRHAddExoR
+from kinbot.reactions.reac_Intra_RH_Add_Exocyclic_F import IntraRHAddExoF
+from kinbot.reactions.reac_Intra_RH_Add_Endocyclic_R import IntraRHAddEndoR
+from kinbot.reactions.reac_Intra_RH_Add_Endocyclic_F import IntraRHAddEndoF
+from kinbot.reactions.reac_HO2_Elimination_from_PeroxyRadical import HO2Elimination
+from kinbot.reactions.reac_beta_delta import BetaDelta
+from kinbot.reactions.reac_birad_recombination_F import BiradRecombinationF
+from kinbot.reactions.reac_birad_recombination_R import BiradRecombinationR
+from kinbot.reactions.reac_Intra_disproportionation_R import IntraDisproportionationR
+from kinbot.reactions.reac_Intra_disproportionation_F import IntraDisproportionationF
+from kinbot.reactions.reac_r14_birad_scission import R14BiradScission
+from kinbot.reactions.reac_r14_cyclic_birad_scission_R import R14CyclicBiradScission
+from kinbot.reactions.reac_barrierless_saddle import BarrierlessSaddle
+from kinbot.reactions.reac_h2_elim import H2Elim
+from kinbot.reactions.reac_bimol_disproportionation_R import BimolDisproportionationR
+from kinbot.reactions.reac_homolytic_scission import HS
+from kinbot.reactions.reac_combinatorial import Combinatorial
 
-from reactions.reac_combinatorial import Combinatorial
+logger = logging.getLogger('KinBot')
 
 
 class ReactionFinder:
     """
     Class to find all the potential reactions starting from a well.
     """
     
@@ -124,14 +126,17 @@
                           '12_shift_S_R': self.search_12_shift_S_R, 
                           'R_Addition_CSm_R': self.search_R_Addition_CSm_R, 
                           'r13_insertion_RSR': self.search_r13_insertion_RSR, 
                           'beta_delta': self.search_beta_delta, 
                           'h2_elim': self.search_h2_elim,
                           'hom_sci': self.search_hom_sci,
                           'barrierless_saddle': self.search_barrierless_saddle,
+                          'Intra_disproportionation_F': self.search_Intra_disproportionation_F, 
+                          'Intra_disproportionation_R': self.search_Intra_disproportionation_R, 
+                          'bimol_disproportionation_R': self.search_bimol_disproportionation_R, 
                           }
 
         if 'combinatorial' in self.families:
             reaction_names['combinatorial'] = self.search_combinatorial        
  
         atom = self.species.atom
         natom = self.species.natom
@@ -160,22 +165,22 @@
                             reaction_names[rn](natom, atom, bond, rad)
 
         for name in self.reactions:
             self.reaction_matrix(self.reactions[name], name) 
         
         for index in range(len(self.species.reac_name)-1):
             if self.species.reac_name[index] in self.species.reac_name[index + 1:]:
-                logging.error('Found reaction name "{}" more than once'
+                logger.error('Found reaction name "{}" more than once'
                                .format(self.species.reac_name[index]))
-                logging.error('Exiting')
+                logger.error('Exiting')
                 sys.exit()
 
-        logging.info('\tFound the following reactions:')
+        logger.info('\tFound the following reactions:')
         for rxn in self.species.reac_name:
-            logging.info('\t\t{}'.format(rxn))
+            logger.info('\t\t{}'.format(rxn))
         
         return 0  
    
 
     def search_combinatorial(self, natom, atom, bond, rad):
         """ 
         This is a method to create all possible combinations of maximum 3 bond breakings 
@@ -1927,14 +1932,55 @@
 #            if self.one_reaction_fam and new:
 #                if self.reac_bonds != {frozenset({inst[-1], inst[-2]})} or self.prod_bonds != {frozenset({inst[0], inst[-1]})}:
 #                    new = 0
         
         return 0
 
 
+    def search_bimol_disproportionation_R(self, natom, atom, bond, rad):
+        """ 
+        This is an RMG class.
+          X                  X
+          |                  |
+        R=R  *R*-R-H <== H-R-R-R=R
+          |   |              | | 
+          Y   Z              Y Z
+        """
+
+        if np.sum(rad) != 0: return
+        
+        name = 'bimol_disproportionation_R'
+        
+        if not name in self.reactions:
+            self.reactions[name] = []
+
+        rxns = [] #reactions found with the current resonance isomer
+        
+        for ringsize in range(5, 6):
+            motif = ['X' for i in range(ringsize)]
+            motif[-1] = 'H'
+            
+            instances = find_motif.start_motif(motif, natom, bond, atom, -1, self.species.atom_eqv)
+            
+            bondpattern = ['X' for i in range(ringsize - 1)]
+            bondpattern[0] = 2
+            
+            for instance in instances:
+                if find_motif.bondfilter(instance, bond, bondpattern) == 0:
+                    rxns += [instance] 
+
+        self.new_reaction(rxns, name, a=0, b=-1)
+#            # filter for specific reaction after this
+#            if self.one_reaction_fam and new:
+#                if self.reac_bonds != {frozenset({inst[-1], inst[-2]})} or self.prod_bonds != {frozenset({inst[0], inst[-1]})}:
+#                    new = 0
+        
+        return 0
+
+
     def search_beta_delta(self, natom, atom, bond, rad):
         """
         This is not an RMG class.
 
         A*-B-C-D-E ==> A=B + C=D + E* 
 
         It is the parallel breaking of not just the beta but also of the gamma bond, resulting in two unsaturated bonds and a radical.
@@ -1983,20 +2029,14 @@
 
         motif = ['H','X','X','H']
         instances = find_motif.start_motif(motif, natom, bond, atom, -1, self.species.atom_eqv)
         for instance in instances: 
             rxns += [instance]
 
         self.new_reaction(rxns, name, a=0, b=-1, cross=True)
-#            # filter for the same reactions
-#            for instance in self.reactions[name]:
-#                if inst[0] == instance[0] and inst[-1] == instance[-1]:
-#                    new = 0
-#                if inst[0] == instance[-1] and inst[-1] == instance[0]:
-#                    new = 0
 #            # filter for specific reaction after this
 #            if self.one_reaction_fam and new:
 #                if self.reac_bonds != {frozenset({inst[0], inst[1]}), frozenset({inst[2], inst[3]})} or self.prod_bonds != {frozenset({inst[0], inst[3]})}:
 #                    new = 0
 
         return 0
 
@@ -2026,21 +2066,15 @@
         else: 
             try:
                 rxns = self.par['homolytic_bonds'][str(self.species.chemid)]
             except KeyError:
                 pass
                 
 
-        self.new_reaction(rxns, name, a=0, b=1, cross=True)
-#        for inst in rxns:
-#            new = 1
-#            # filter for the same reactions
-#            for instance in self.reactions[name]:
-#                if inst[0] == instance[1] and inst[1] == instance[0]:
-#                    new = 0
+        self.new_reaction(rxns, name, a=0, b=1, cross=True, aid=True)
 #            # filter for specific reaction after this
 #            if self.one_reaction_fam and new:
 #                if self.reac_bonds != {frozenset({inst[0], inst[1]}), frozenset({inst[2], inst[3]})} or self.prod_bonds != {frozenset({inst[0], inst[3]})}:
 #                    new = 0
 
         return 0
 
@@ -2273,14 +2307,18 @@
                 name = str(self.species.chemid) + '_' + reac_id + '_' + str(reac_list[i][0] + 1) + '_' + str(reac_list[i][3] + 1)
                 self.species.reac_name.append(name)
                 self.species.reac_obj.append(H2Elim(self.species, self.qc, self.par, reac_list[i], name))
             elif reac_id == 'hom_sci':
                 name = str(self.species.chemid) + '_' + reac_id + '_' + str(reac_list[i][0] + 1) + '_' + str(reac_list[i][1] + 1)
                 self.species.reac_name.append(name)
                 self.species.reac_obj.append(HS(self.species, self.qc, self.par, reac_list[i], name))
+            elif reac_id == 'bimol_disproportionation_R':
+                name = str(self.species.chemid) + '_' + reac_id + '_' + str(reac_list[i][0] + 1) + '_' + str(reac_list[i][-1] + 1)
+                self.species.reac_name.append(name)
+                self.species.reac_obj.append(BimolDisproportionationR(self.species, self.qc, self.par, reac_list[i], name))
             elif reac_id == 'barrierless_saddle':
                 name = str(self.species.chemid) + '_' + reac_id + '_' + str(reac_list[i][0] + 1) + '_' + str(reac_list[i][1] + 1)
                 self.species.reac_name.append(name)
                 self.species.reac_obj.append(BarrierlessSaddle(self.species, self.qc, self.par, reac_list[i], name))
             elif reac_id == 'combinatorial':
                 name = str(self.species.chemid) + '_' + reac_id + '_' + str(i)
                 self.species.reac_name.append(name)
@@ -2308,29 +2346,41 @@
         except AttributeError:
             self.species.calc_maxbond()
         for inst, instance in enumerate(instances):
             if all(self.species.maxbond[instance[ii]][instance[ii + 1]] > 1 for ii in range(len(instance) - 2)):
                 if np.linalg.norm(self.species.geom[instance[pivot1]] - self.species.geom[instance[pivot2]]) > cutoff:
                     mask[inst] = False
                     numbers = [ii + 1 for ii in instance]
-                    logging.info(f'{name} reaction {numbers} over rigid backbone with cutoff {cutoff} A is removed.')
+                    logger.info(f'{name} reaction {numbers} over rigid backbone with cutoff {cutoff} A is removed.')
         return list(np.array(instances, dtype=object)[mask])
 
 
-    def new_reaction(self, rxns, name, a=None, b=None, c=None, d=None, e=None, length=None, full=False, cross=False):
+    def new_reaction(self, rxns, name, a=None, b=None, c=None, d=None, e=None, 
+                     length=None, full=False, cross=False, aid=False):
         """
         Returns 1 if new, and 0 if not new
         Checks a variable number of identical elements
         Also can check full equivalency (full=True), same lenght (length=True), and 
         equivalency between elements that are interchangeable (cross=True)
+        if aid is True, then it will throw away reactions where there is already one
+           with the same atom IDs involved - at least important for hom_sci
         """
 
         for inst in rxns:
             new = True
             for instance in self.reactions[name]:
+                if aid == True:
+                    if (self.species.atomid[inst[a]] == self.species.atomid[instance[a]] and
+                            self.species.atomid[inst[b]] == self.species.atomid[instance[b]]):
+                        new = False
+                        break
+                    if (self.species.atomid[inst[b]] == self.species.atomid[instance[a]] and
+                            self.species.atomid[inst[a]] == self.species.atomid[instance[b]]):
+                        new = False
+                        break
                 if cross == True:
                     if (inst[a] == instance[a] and inst[b] == instance[b]):
                         new = False
                         break 
                     if (inst[a] == instance[b] and inst[b] == instance[a]):
                         new = False
                         break
```

### Comparing `kinbot-2.1.post0/kinbot/reaction_finder_bimol.py` & `kinbot-2.2.1/kinbot/reaction_finder_bimol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 import sys
-import copy
 import logging
 
-from kinbot import bond_combinations
-from kinbot import find_motif
-from reactions.reac_abstraction import Abstraction
+from kinbot.reactions.reac_abstraction import Abstraction
+
+logger = logging.getLogger('KinBot')
 
 
 class ReactionFinderBimol:
     """
     Class to find all reactions for bimolecular starting species.
     """
     
@@ -71,22 +70,22 @@
                             reaction_names[rn](natomB, atomB, bondB, radB, uniqB, natomA, atomA, bondA, radA, uniqA, natomA)  # swapping roles for all families
 
         for name in self.reactions:
             self.reaction_matrix(self.reactions[name], name) 
         
         for index in range(len(self.species.reac_name)-1):
             if self.species.reac_name[index] in self.species.reac_name[index + 1:]:
-                logging.error('Found reaction name "{}" more than once'
+                logger.error('Found reaction name "{}" more than once'
                                .format(self.species.reac_name[index]))
-                logging.error('Exiting')
+                logger.error('Exiting')
                 sys.exit()
 
-        logging.info('\tFound the following bimolecular reactions:')
+        logger.info('\tFound the following bimolecular reactions:')
         for rxn in self.species.reac_name:
-            logging.info('\t\t{}'.format(rxn))
+            logger.info('\t\t{}'.format(rxn))
         
         return 0  
    
 
     def search_abstraction(self, natomA, atomA, bondA, radA, uniqA, natomB, atomB, bondB, radB, uniqB, shift):
         """ 
         This is a general atom abstraction family.
```

### Comparing `kinbot-2.1.post0/kinbot/reaction_generator.py` & `kinbot-2.2.1/kinbot/reaction_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os, sys
-import numpy as np
 import shutil
 import time
 import logging
 import copy
+import itertools
+
+import numpy as np
 
 from kinbot import constants
 #from kinbot import filecopying
 from kinbot import pes
 from kinbot import postprocess
 from kinbot import reac_family
 from kinbot import cheminfo
@@ -15,14 +17,16 @@
 from kinbot.optimize import Optimize
 from kinbot.stationary_pt import StationaryPoint
 from kinbot.molpro import Molpro
 from ase.db import connect
 from ase import Atoms
 
 
+logger = logging.getLogger('KinBot')
+
 class ReactionGenerator:
     """
     This class generates the reactions using the qc codes
     It builds an initial guess for the ts, runs that ts towards a saddle point
     and does IRC calculations
     """
 
@@ -65,20 +69,24 @@
         products_waiting_status = [[] for i in self.species.reac_inst]
         count = len(self.species.reac_inst)
         frag_unique = []
 
         while alldone:
             for index, instance in enumerate(self.species.reac_inst):
                 obj = self.species.reac_obj[index]
+                if obj.instance_name in self.par['skip_reactions'] \
+                        and self.species.reac_ts_done[index] != -999:
+                    logger.info(f'\tRemoving reaction {obj.instance_name}.')
+                    self.species.reac_ts_done[index] = -999
                 # START REACTION SEARCH
                 if self.species.reac_ts_done[index] == 0 and self.species.reac_step[index] == 0:
                     # verify after restart if search has failed in previous kinbot run
                     status = self.qc.check_qc(obj.instance_name)
                     if status == 'error':
-                        logging.info('\tRxn search failed for {}'
+                        logger.info('\tRxn search failed for {}'
                                      .format(obj.instance_name))
                         self.species.reac_ts_done[index] = -999
                 if self.species.reac_type[index] == 'hom_sci' and self.species.reac_ts_done[index] == 0:  # no matter what, set to 2
                     # somewhat messy manipulation to force the new bond matrix for hom_sci
                     obj.products = StationaryPoint(f'{instance}_prod', self.species.charge, self.species.mult,
                                                    atom=self.species.atom, geom=self.species.geom, wellorts=0)
                     obj.products.characterize()
@@ -94,116 +102,118 @@
                 if self.species.reac_ts_done[index] == 0:  # ts search is ongoing
                     if obj.scan == 0:  # don't do a scan of a bond
                         if self.species.reac_step[index] == obj.max_step + 1:
                             status, freq = self.qc.get_qc_freq(obj.instance_name, self.species.natom)
                             if status == 0 and freq[0] < 0. and freq[1] > 0.:
                                 self.species.reac_ts_done[index] = 1
                             elif status == 0 and freq[0] > 0.:
-                                logging.info('\tRxn search failed for {}, no imaginary freq.'
+                                logger.info('\tRxn search failed for {}, no imaginary freq.'
                                              .format(obj.instance_name))
                                 self.species.reac_ts_done[index] = -999
                             elif status == 0 and freq[1] < 0.:
-                                logging.info('\tRxn search failed for {}, more than one imaginary freq.'
+                                logger.info('\tRxn search failed for {}, more than one imaginary freq.'
                                              .format(obj.instance_name))
                                 self.species.reac_ts_done[index] = -999
                             elif status == -1: 
-                                logging.info('\tRxn search failed for {}'
+                                logger.info('\tRxn search failed for {}'
                                              .format(obj.instance_name))
                                 self.species.reac_ts_done[index] = -999
                         else:
                             self.species.reac_step[index] = reac_family.carry_out_reaction(
                                                             obj, self.species.reac_step[index], self.par['qc_command'],
                                                             bimol=self.par['bimol'])
                             if self.species.reac_step[index] == -1:
                                 self.species.reac_ts_done[index] = -999
-                                logging.info('\tRxn search failed for {} because of 0 0 0 geometry.'
+                                logger.info('\tRxn search failed for {} because of 0 0 0 geometry.'
                                              .format(obj.instance_name))
 
                     else:  # do a bond scan
                         if self.species.reac_step[index] == self.par['scan_step'] + 1:
                             status, freq = self.qc.get_qc_freq(obj.instance_name, self.species.natom)
                             if status == 0 and freq[0] < 0. and freq[1] > 0.:
                                 self.species.reac_ts_done[index] = 1
                             elif status == 0 and freq[0] > 0.:
-                                logging.info('\tRxn search failed for {}, no imaginary freq.'.format(obj.instance_name))
+                                logger.info('\tRxn search failed for {}, no imaginary freq.'.format(obj.instance_name))
                                 self.species.reac_ts_done[index] = -999
                             elif status == 0 and freq[1] < 0.:
-                                logging.info('\tRxn search failed for {}, more than one imaginary freq.'.format(obj.instance_name))
+                                logger.info('\tRxn search failed for {}, more than one imaginary freq.'.format(obj.instance_name))
                                 self.species.reac_ts_done[index] = -999
                             elif status == -1:
-                                logging.info('\tRxn search using scan failed for {} in TS optimization stage.'.format(obj.instance_name))
+                                logger.info('\tRxn search using scan failed for {} in TS optimization stage.'.format(obj.instance_name))
                                 self.species.reac_ts_done[index] = -999
                         else:
                             if self.species.reac_step[index] == 0:
                                 self.species.reac_step[index] = reac_family.carry_out_reaction(
                                                                 obj, self.species.reac_step[index], self.par['qc_command'],
                                                                 bimol=self.par['bimol'])
                                 if self.species.reac_step[index] == -1:
                                     self.species.reac_ts_done[index] = -999
-                                    logging.info('\tRxn search failed for {} because of 0 0 0 geometry.'
+                                    logger.info('\tRxn search failed for {} because of 0 0 0 geometry.'
                                                  .format(obj.instance_name))
                             elif self.species.reac_step[index] < self.par['scan_step']:
                                 status = self.qc.check_qc(obj.instance_name)
                                 if status == 'error':
-                                    logging.info('\tRxn search using scan failed for {} in step {}'
+                                    logger.info('\tRxn search using scan failed for {} in step {}'
                                                  .format(obj.instance_name, self.species.reac_step[index]))
                                     self.species.reac_ts_done[index] = -999
                                 else:
                                     err, energy = self.qc.get_qc_energy(obj.instance_name)
                                     if err == 0:
                                         self.species.reac_scan_energy[index].append(energy)
-                                        logging.debug(f'Scan energy for {obj.instance_name} in step {self.species.reac_step[index]}:')
-                                        logging.debug(f'{self.species.reac_scan_energy[index][-1]} Hartree.')
+                                        logger.debug(f'Scan energy for {obj.instance_name} in step {self.species.reac_step[index]}:')
+                                        logger.debug(f'{self.species.reac_scan_energy[index][-1]} Hartree.')
                                         # need at least 3 points for a maximum
                                         if len(self.species.reac_scan_energy[index]) >= 3:
                                             ediff = np.diff(self.species.reac_scan_energy[index])
                                             if ediff[-1] < 0 and ediff[-2] > 0:  # max
-                                                logging.info(f'\tMaximum found for {obj.instance_name}.')
+                                                logger.info(f'\tMaximum found for {obj.instance_name}.')
                                                 e_in_kcal = [constants.AUtoKCAL * (self.species.reac_scan_energy[index][ii] - 
                                                                self.species.reac_scan_energy[index][0]) 
                                                                for ii in range(len(self.species.reac_scan_energy[index]))]
                                                 e_in_kcal = np.round(e_in_kcal, 2)
-                                                logging.info(f'\tEnergies: {e_in_kcal}')
-                                                logging.debug(f'Derivatives: {ediff}')
+                                                logger.info(f'\tEnergies: {e_in_kcal}')
+                                                logger.debug(f'Derivatives: {ediff}')
                                                 self.species.reac_step[index] = self.par['scan_step']  # ending the scan
                                             if len(ediff) >= 3:
                                                 if any([edf == 0 for edf in ediff[-2:]]):
-                                                    logging.warning(f'Calculation failed in the bond scan of {obj.instance_name}.')
+                                                    logger.warning(f'Calculation failed in the bond scan of {obj.instance_name}.')
                                                     self.species.reac_ts_done[index] = -999
                                                     continue
                                                 if 10. * (ediff[-3] / ediff[-2]) < (ediff[-2] / ediff[-1]):  # sudden change in slope
-                                                    logging.info(f'\tSudden change in slope for for {obj.instance_name}.')
-                                                    logging.info(f'\tRelative energies (kcal/mol): {self.species.reac_scan_energy[index]}')
-                                                    logging.debug(f'Derivatives: {ediff}')
+                                                    logger.info(f'\tSudden change in slope for for {obj.instance_name}.')
+                                                    logger.info(f'\tRelative energies (kcal/mol): {self.species.reac_scan_energy[index]}')
+                                                    logger.debug(f'Derivatives: {ediff}')
                                                     self.species.reac_step[index] = self.par['scan_step']  # ending the scan
                                      
                                         # scan continues, and if reached scan_step, then goes for full optimization
                                         self.species.reac_step[index] = reac_family.carry_out_reaction(
                                                                         obj, self.species.reac_step[index], self.par['qc_command'],
                                                                         bimol=self.par['bimol'])
                                         if self.species.reac_step[index] == -1:
                                             self.species.reac_ts_done[index] = -999
-                                            logging.info('\tRxn search failed for {} because of 0 0 0 geometry.'
+                                            logger.info('\tRxn search failed for {} because of 0 0 0 geometry.'
                                                          .format(obj.instance_name))
                             else:  # the last step was reached, and no max or inflection was found
-                                logging.info('\tRxn search using scan failed for {}, no saddle guess found.'
+                                if self.qc.check_qc(obj.instance_name) == 'running':
+                                    continue
+                                logger.info('\tRxn search using scan failed for {}, no saddle guess found.'
                                              .format(obj.instance_name))
                                 db = connect('{}/kinbot.db'.format(os.getcwd()))
                                 # error line, H atom is just placeholder
                                 db.write(Atoms('H'), name=obj.instance_name, data = {'status': 'error'})
                                 # this is copied here so that a non-AM1 file is in place
                                 shutil.copy(f'{os.getcwd()}/{self.species.chemid}_well.log', f'{os.getcwd()}/{obj.instance_name}.log')
                                 self.species.reac_ts_done[index] = -999
 
                 elif self.species.reac_ts_done[index] == 1:
                     status = self.qc.check_qc(obj.instance_name)
                     if status == 'running':
                         continue
                     elif status == 'error':
-                        logging.info('\tRxn search failed (gaussian error) for {}'
+                        logger.info('\tRxn search failed (gaussian error) for {}'
                                      .format(obj.instance_name))
                         self.species.reac_ts_done[index] = -999
                     else:
                         # check the barrier height:
                         ts_energy = self.qc.get_qc_energy(obj.instance_name)[1]
                         ts_zpe = self.qc.get_qc_zpe(obj.instance_name)[1]
                         if self.species.reac_type[index] == 'R_Addition_MultipleBond':
@@ -216,147 +226,171 @@
                             ending = 'well'
                             thresh = self.par['barrier_threshold']
                         sp_energy = self.qc.get_qc_energy('{}_{}'.format(str(self.species.chemid), ending))[1]
                         sp_zpe = self.qc.get_qc_zpe('{}_{}'.format(str(self.species.chemid), ending))[1]
                         try:
                             barrier = (ts_energy + ts_zpe - sp_energy - sp_zpe) * constants.AUtoKCAL
                         except TypeError:
-                            logging.error(f'Faulty calculations, check or delete files for {obj.instance_name}.')
+                            logger.error(f'Faulty calculations, check or delete files for {obj.instance_name}.')
                             sys.exit(-1)
                         if barrier > thresh:
-                            logging.info('\tRxn barrier too high ({0:.2f} kcal/mol) for {1}'
+                            logger.info('\tRxn barrier too high ({0:.2f} kcal/mol) for {1}'
                                          .format(barrier, obj.instance_name))
                             self.species.reac_ts_done[index] = -999
                         else:
                             obj.irc = IRC(obj, self.par)  # TODO: this doesn't seem like a good design
                             irc_status = obj.irc.check_irc()
                             if 0 in irc_status:
-                                logging.info('\tRxn barrier is {0:.2f} kcal/mol for {1}'
+                                logger.info('\tRxn barrier is {0:.2f} kcal/mol for {1}'
                                              .format(barrier, obj.instance_name))
                                 # No IRC started yet, start the IRC now
-                                logging.info('\tStarting IRC calculations for {}'
+                                logger.info('\tStarting IRC calculations for {}'
                                              .format(obj.instance_name))
                                 obj.irc.do_irc_calculations()
                             elif irc_status[0] == 'running' or irc_status[1] == 'running':
                                 continue
                             else:
                                 # IRC's have successfully finished, have an error, in any case
                                 # read the geometries and try to make products out of them
                                 # verify which of the ircs leads back to the reactant, if any
                                 prod = obj.irc.irc2stationary_pt()
                                 if prod == 0:
-                                    logging.info('\tNo product found for {}'.format(obj.instance_name))
+                                    logger.info('\tNo product found for {}'.format(obj.instance_name))
                                     self.species.reac_ts_done[index] = -999
                                 else:
                                     obj.products = prod
                                     obj.product_bonds = prod.bond
                                     self.species.reac_ts_done[index] = 2
 
                 elif self.species.reac_ts_done[index] == 2:
-                    if len(products_waiting_status[index]) == 0:
+                    if len(products_waiting_status[index]) == 0:  # not started optimization yet
                         # identify bimolecular products and wells
-                        fragments, maps = obj.products.start_multi_molecular()
-                        obj.products = []
+                        fragments, maps = obj.products.start_multi_molecular(vary_charge=True)
 
-                        a = []
+                        a = []  # cleaned up list of products
                         for frag in fragments:
                             a.append(frag)
                             if len(frag_unique) == 0:
                                 frag_unique.append(frag)
                             elif len(frag_unique) > 0:
                                 new = 1
-                                for fragb in frag_unique:
+                                for fragb in frag_unique:  # check if there is already this fragment somewhere earlier
                                     if frag.chemid == fragb.chemid:
                                         e, geom2 = self.qc.get_qc_geom(str(fragb.chemid) + '_well', fragb.natom)
                                         if e == 0:
                                             a.pop()
                                             frag = fragb
                                             a.append(frag)
                                             new = 0
                                             break
                                 if new:
                                     frag_unique.append(frag)
+
                         obj.products_final = []
+
+                        frag_opt_done = 0
                         for frag in a:
                             self.qc.qc_opt(frag, frag.geom)
                             e, geom2 = self.qc.get_qc_geom(str(frag.chemid) + '_well', frag.natom)
-                            obj.products_final.append(frag)
+                            if e != 1:  # e == 1 means it's running
+                                frag_opt_done += 1
 
-                        # check products make sure they are the same
-                        for i, st_pt_i in enumerate(obj.products_final):
-                            for j, st_pt_j in enumerate(obj.products_final):
-                                if st_pt_i.chemid == st_pt_j.chemid and i < j:
-                                    obj.products_final[j] = obj.products_final[i]
-
-                    # print products generated by IRC
-                    products = []
-                    for i, st_pt in enumerate(obj.products_final):
-                        products.append(st_pt.chemid)
-
-                    products.extend([' ', ' ', ' '])
-                    logging.info('\tReaction {} leads to products {} {} {}'
-                                 .format(obj.instance_name, products[0], products[1], products[2]))
-
-                    hom_sci_energy = 0
-                    for i, st_pt in enumerate(obj.products_final):
-                        chemid = st_pt.chemid
-                        e, st_pt.geom = self.qc.get_qc_geom(str(st_pt.chemid) + '_well', st_pt.natom)
-                        if e < 0:
-                            logging.info('\tProduct optimization failed for {}, product {}'
-                                         .format(obj.instance_name, st_pt.chemid))
-                            self.species.reac_ts_done[index] = -999
-                            err = -1
-                        elif e != 0:
-                            err = -1
-                        else:
-                            _, st_pt.energy = self.qc.get_qc_energy(str(st_pt.chemid) + '_well')
-                            _, st_pt.zpe = self.qc.get_qc_zpe(str(st_pt.chemid) + '_well')
-                            if self.species.reac_type[index] == 'hom_sci':  
-                                hom_sci_energy += st_pt.energy + st_pt.zpe
-                            st_pt.characterize()  
-                            if chemid != st_pt.chemid:
-                                obj.products_final.pop(i)
-                                newfrags, newmaps = st_pt.start_multi_molecular()  # newfrags is list of stpt obj
-                                products_waiting_status[index] = [0 for frag in newfrags]
-                                frag_chemid = []
-                                for ii, newfr in enumerate(newfrags):
-                                    newfr.characterize()
-                                    for prod in frag_unique:
-                                        if newfr.chemid == prod.chemid:
-                                            newfrags.pop(ii)
-                                            newfr = prod
+                        if frag_opt_done == len(a):  # both fragments are done
+                            for frag in a:
+                                obj.products_final.append(frag)
+
+                            # if the two fragments are identical, make them the same object
+                            for i, st_pt_i in enumerate(obj.products_final):
+                                for j, st_pt_j in enumerate(obj.products_final):
+                                    if st_pt_i.chemid == st_pt_j.chemid and i < j:
+                                        obj.products_final[j] = obj.products_final[i]
+
+                            # print products generated by IRC
+                            products = []
+                            for i, st_pt in enumerate(obj.products_final):
+                                products.append(st_pt.chemid)
+
+                            products.extend([' ', ' ', ' '])
+                            logger.info('\tReaction {} leads to products {} {} {}'
+                                         .format(obj.instance_name, products[0], products[1], products[2]))
+
+                            hom_sci_energy = 0
+                            for i, st_pt in enumerate(obj.products_final):
+                                chemid = st_pt.chemid
+                                e, st_pt.geom = self.qc.get_qc_geom(str(st_pt.chemid) + '_well', st_pt.natom)
+                                if e < 0:
+                                    logger.info('\tProduct optimization failed for {}, product {}'
+                                                 .format(obj.instance_name, st_pt.chemid))
+                                    self.species.reac_ts_done[index] = -999
+                                    err = -1
+                                elif e != 0:
+                                    err = -1
+                                else:
+                                    _, st_pt.energy = self.qc.get_qc_energy(str(st_pt.chemid) + '_well')
+                                    _, st_pt.zpe = self.qc.get_qc_zpe(str(st_pt.chemid) + '_well')
+                                    if self.species.reac_type[index] == 'hom_sci': # TODO energy is the sum of all possible fragments  
+                                        hom_sci_energy += st_pt.energy + st_pt.zpe
+                                    st_pt.characterize()  
+                                    if chemid != st_pt.chemid:
+                                        obj.products_final.pop(i)
+                                        newfrags, newmaps = st_pt.start_multi_molecular()  # newfrags is list of stpt obj
+                                        products_waiting_status[index] = [0 for frag in newfrags]
+                                        frag_chemid = []
+                                        for ii, newfr in enumerate(newfrags):
+                                            newfr.characterize()
+                                            for prod in frag_unique:
+                                                if newfr.chemid == prod.chemid:
+                                                    newfrags.pop(ii)
+                                                    newfr = prod
+                                                    jj = ii - 1
+                                                    newfrags.insert(jj, newfr)
                                             jj = ii - 1
-                                            newfrags.insert(jj, newfr)
-                                    jj = ii - 1
-                                    obj.products_final.insert(jj, newfr)
-                                    self.qc.qc_opt(newfr, newfr.geom, 0)
-                                    frag_chemid.append(newfr.chemid)
-                                if len(frag_chemid) == 1:
-                                    frag_chemid.append(" ")
-                                for ii, frag in enumerate(newfrags):
-                                    products_waiting_status[index][ii] = 1
-                                logging.info('\ta) Product optimized to other structure for {}'
-                                             ', product {} to {} {}'
-                                             .format(obj.instance_name, chemid, frag_chemid[0], frag_chemid[1]))
-
-                    obj.products = []
-                    for prod in obj.products_final:
-                        obj.products.append(prod)
-                    obj.products_final = []
-
-                    if all([pi == 1 for pi in products_waiting_status[index]]):
-                        if self.species.reac_type[index] == 'hom_sci': 
-                            hom_sci_energy = (hom_sci_energy - self.species.start_energy - self.species.start_zpe) * constants.AUtoKCAL
-                            if hom_sci_energy < self.par['barrier_threshold'] + self.par['hom_sci_threshold_add']:
-                                self.species.reac_ts_done[index] = 3
-                            else:
-                                logging.info(f'\thom_sci energy is too high at {hom_sci_energy} kcal/mol for {obj.instance_name}')
-                                self.species.reac_ts_done[index] = -999
-                        else:
-                            self.species.reac_ts_done[index] = 3
+                                            obj.products_final.insert(jj, newfr)
+                                            self.qc.qc_opt(newfr, newfr.geom, 0)
+                                            frag_chemid.append(newfr.chemid)
+                                        if len(frag_chemid) == 1:
+                                            frag_chemid.append(" ")
+                                        for ii, frag in enumerate(newfrags):
+                                            products_waiting_status[index][ii] = 1
+                                        logger.info('\ta) Product optimized to other structure for {}'
+                                                     ', product {} to {} {}'
+                                                     .format(obj.instance_name, chemid, frag_chemid[0], frag_chemid[1]))
+
+                            obj.products = []
+                            for prod in obj.products_final:
+                                obj.products.append(prod)
+                            obj.products_final = []
+
+                            if all([pi == 1 for pi in products_waiting_status[index]]):
+                                if self.species.charge != 0:  # select the lower energy combination
+                                    # brute for all combinations
+                                    combs = np.array([np.array(i) for i in itertools.product([0, 1], repeat = len(obj.products))])
+                                    val = 1000.
+                                    ens = np.array([i.energy for i in obj.products])
+                                    zpes = np.array([i.zpe for i in obj.products])
+                                    masses = np.array([i.mass for i in obj.products])
+                                    charges = np.array([i.charge for i in obj.products])
+                                    combo = combs[0]
+                                    for comb in combs:
+                                        if sum(comb * masses) == self.species.mass:
+                                            if sum(comb * charges) == self.species.charge:
+                                                if sum(comb * (ens + zpes)) < val:
+                                                    val = sum(comb * (ens + zpes))
+                                                    combo = comb
+                                    combo = combo.astype(bool)
+                                    obj.products = list(np.array(obj.products)[combo])
+                                if self.species.reac_type[index] == 'hom_sci': # TODO energy is the sum of all possible fragments
+                                    hom_sci_energy = (hom_sci_energy - self.species.start_energy - self.species.start_zpe) * constants.AUtoKCAL
+                                    if hom_sci_energy < self.par['barrier_threshold'] + self.par['hom_sci_threshold_add']:
+                                        self.species.reac_ts_done[index] = 3
+                                    else:
+                                        logger.info(f'\thom_sci energy is too high at {round(hom_sci_energy, 2)} kcal/mol for {obj.instance_name}')
+                                        self.species.reac_ts_done[index] = -999
+                                else:
+                                    self.species.reac_ts_done[index] = 3
 
                 elif self.species.reac_ts_done[index] == 3:
                     # wait for the optimization to finish
                     # if two st_pt are the same in the products, we make them exactly identical otherwise
                     # the different ordering of the atoms causes the chemid of the second to be seemingly wrong
                     for i, st_pt_i in enumerate(obj.products):
                         for j, st_pt_j in enumerate(obj.products):
@@ -364,30 +398,30 @@
                                 obj.products[j] = obj.products[i]
 
                     err = 0
                     for st_pt in obj.products:
                         chemid = st_pt.chemid
                         e, st_pt.geom = self.qc.get_qc_geom(str(st_pt.chemid) + '_well', st_pt.natom)
                         if e < 0:
-                            logging.warning('Product optimization failed for {}, product {}...'
+                            logger.warning('Product optimization failed for {}, product {}...'
                                          .format(obj.instance_name, st_pt.chemid))
                             self.species.reac_ts_done[index] = -999
                             err = -1
                         elif e != 0:
                             err = -1
                         else:
                             _, st_pt.energy = self.qc.get_qc_energy(str(st_pt.chemid) + '_well')
                             _, st_pt.zpe = self.qc.get_qc_zpe(str(st_pt.chemid) + '_well')
                             st_pt.characterize()  
                             if chemid == self.species.chemid:
-                                logging.info(f'Product in {obj.instance_name} is identical to the reactant. Reaction deleted.')
+                                logger.info(f'Product in {obj.instance_name} is identical to the reactant. Reaction deleted.')
                                 self.species.reac_ts_done[index] = -999 
                             elif chemid != st_pt.chemid:
                                 # product was optimized to another structure, give warning but don't remove reaction
-                                logging.info('\tb) Product optimized to other structure for {}'
+                                logger.info('\tb) Product optimized to other structure for {}'
                                              ', product {} to {}'
                                              .format(obj.instance_name, chemid, st_pt.chemid))
                                 shutil.copy(f'{os.getcwd()}/{chemid}_well.log', f'{os.getcwd()}/{st_pt.chemid}_well.log')
                                 e, st_pt.geom = self.qc.get_qc_geom(str(st_pt.chemid) + '_well', st_pt.natom)
                                 if e < 0:
                                     err = -1
                     if err == 0:
@@ -424,28 +458,28 @@
                     temp_prod_opt = []  # holding the optimization objects temporarily
                     for st_pt in obj.products:
                         # do the products optimizations
                         # check for products of other reactions that are the same as this product
                         # in the case such products are found, use the same Optimize object for both
                         for i, inst_i in enumerate(self.species.reac_inst):
                             new = 1
-                            if not i == index:
+                            if i != index:
                                 obj_i = self.species.reac_obj[i]
                                 if self.species.reac_ts_done[i] > 3:
                                     for j, st_pt_i in enumerate(obj_i.products):
                                         if st_pt_i.chemid == st_pt.chemid:
                                             if len(obj_i.prod_opt) > j:
                                                 prod_opt = obj_i.prod_opt[j]
                                                 new = 0
                                                 break
                         if new:
                             prod_opt = Optimize(st_pt, self.par, self.qc)
                             prod_opt.do_optimization()
                             if prod_opt.shigh == -999: 
-                                logging.info('\tRxn search failed for {}, prod_opt shigh fail for {}.'
+                                logger.info('\tRxn search failed for {}, prod_opt shigh fail for {}.'
                                              .format(obj.instance_name, prod_opt.species.chemid))
                                 self.species.reac_ts_done[index] = -999
                                 #break  # breaks so that other species is not looked at
                         temp_prod_opt.append(prod_opt)
                     if self.species.reac_ts_done[index] != -999:
                         for tpo in temp_prod_opt:
                             obj.prod_opt.append(tpo)
@@ -468,24 +502,24 @@
                     fails = 0
                     # check if ts is done
                     if self.species.reac_type[index] != 'hom_sci':
                         if not obj.ts_opt.shir == 1:  # last stage in optimize
                             opts_done = 0
                             obj.ts_opt.do_optimization()
                         if obj.ts_opt.shigh == -999:
-                            logging.warning("Reaction {} ts_opt_shigh failure".format(obj.instance_name))
+                            logger.warning("Reaction {} ts_opt_shigh failure".format(obj.instance_name))
                             fails = 1
                     for pr_opt in obj.prod_opt:
                         if not pr_opt.shir == 1:
                             opts_done = 0
                             pr_opt.do_optimization()
                         if pr_opt.shigh == -999:
-                            logging.warning("Reaction {} pr_opt_shigh failure".format(obj.instance_name))
+                            logger.warning("Reaction {} pr_opt_shigh failure".format(obj.instance_name))
                             fails = 1
-                        break
+                        continue
                     if fails:
                         self.species.reac_ts_done[index] = -999
                     elif opts_done:
                         self.species.reac_ts_done[index] = 6
 
                 elif self.species.reac_ts_done[index] == 6:
                     # Finilize the calculations
@@ -493,15 +527,15 @@
                     st_pt = obj.prod_opt[0].species
                     if self.par['pes']:
                         # verify if product is monomolecular, and if it is new
                         if len(obj.products) == 1:
                             st_pt = obj.prod_opt[0].species
                             chemid = st_pt.chemid
                             rel_en = (st_pt.energy - self.species.energy) * constants.AUtoKCAL  # energy contains ZPE! check!!
-                            logging.info(f'\tProduct {obj.instance_name} energy is {np.round(rel_en, 2)} kcal/mol.')
+                            logger.info(f'\tProduct {obj.instance_name} energy is {np.round(rel_en, 2)} kcal/mol.')
                             new_barrier_threshold = self.par['barrier_threshold'] - rel_en 
                             dirwell = os.path.dirname(os.getcwd())
                             jobs = open(dirwell + '/chemids', 'r').read().split('\n')
                             jobs = [ji for ji in jobs]
                             if not str(chemid) in jobs:
                                 # this well is new, add it to the jobs
                                 while 1:
@@ -521,24 +555,24 @@
                         #for frag in frags:
                         #    filecopying.copy_to_database_folder(self.species.chemid, frag.chemid, self.qc)
 
                     # check for wrong number of negative frequencies
                     neg_freq = 0
                     for st_pt in obj.products:
                         if len(st_pt.reduced_freqs):
-                            if st_pt.reduced_freqs[0] <= 0. and st_pt.reduced_freqs[0] >= -50.:
-                                logging.warning(f'Found negative frequency {st_pt.reduced_freqs[0]} cm-1 for a product of {obj.instance_name}. Flipped.')
+                            if -1 * self.par['imagfreq_threshold'] <= st_pt.reduced_freqs[0] <= 0.:
+                                logger.warning(f'Found negative frequency {st_pt.reduced_freqs[0]} cm-1 for a product of {obj.instance_name}. Flipped.')
                                 st_pt.reduced_freqs[0] *= -1.
-                            elif st_pt.reduced_freqs[0] <-50.:
-                                logging.warning(f'Found negative frequency {st_pt.reduced_freqs[0]} cm-1 for a product of {obj.instance_name}.')
+                            elif st_pt.reduced_freqs[0] < -1 * self.par['imagfreq_threshold']:
+                                logger.warning(f'Found negative frequency {st_pt.reduced_freqs[0]} cm-1 for a product of {obj.instance_name}.')
                                 self.species.reac_ts_done[index] = -999
                                 neg_freq = 1
                     if any([fi < 0. for fi in obj.ts.reduced_freqs[1:]]):
-                        print(obj.ts.reduced_freqs)
-                        logging.warning('\tFound more than one negative frequency for ' + obj.instance_name)
+                        logger.warning('Found more than one negative frequency for ' + obj.instance_name)
+                        logger.warning(obj.ts.reduced_freqs)
                         self.species.reac_ts_done[index] = -999
                         neg_freq = 1
 
                     if not neg_freq:
                         # the reaction search is finished
                         self.species.reac_ts_done[index] = -1  # this is the success code
 
@@ -554,15 +588,16 @@
                     if self.par['delete_intermediate_files'] == 1:
                         if not self.species.reac_obj[index].instance_name in deleted:
                             self.delete_files(self.species.reac_obj[index].instance_name)
                             deleted.append(self.species.reac_obj[index].instance_name)
 
             alldone = 1
             for index, instance in enumerate(self.species.reac_inst):
-                if any(self.species.reac_ts_done[i] >= 0 for i in range(len(self.species.reac_inst))):
+                if any(self.species.reac_ts_done[index] >= 0
+                       for i in range(len(self.species.reac_inst))):
                     alldone = 1
                     break
                 else:
                     alldone = 0
 
             # write a small summary while running
             with open('kinbot_monitor.out', 'w') as f_out:
@@ -659,15 +694,15 @@
                 if self.species.reac_ts_done[index] == -1:
                     inchis = obj.get_final_inchis()
                     s.append('FOUND_INCHIS\t' + '\t'.join(inchis))
                 s.append('\n')
             with open('combinatorial.txt', 'w') as f:
                 f.write('\n'.join(s) + '\n')
 
-        logging.info("Reaction generation done!")
+        logger.info("Reaction generation done!")
 
     def delete_files(self, name):
         # job names
         names = []
 
         names.append(name)
         names.append(name + '_high')
```

### Comparing `kinbot-2.1.post0/kinbot/reader_gauss.py` & `kinbot-2.2.1/kinbot/reader_gauss.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,28 +21,52 @@
     for line in reversed(lines):
         if 'SFC Done' in line:
             energy = float(line.split()[4]) / constants.EVtoHARTREE
 
     return energy
 
 
-def read_geom(outfile, mol):
+def read_geom(outfile, mol, max2frag=False, charge=None, mult=None):
     """
     Read the final geometry from a Gaussian file.
+    max2frag: if set to true, the last geometry is taken where
+              the structure has max 2 fragments
+              This is to avoid "exploding" IRC_prod trajectories.
     """
 
     with open(outfile) as f:
         lines = f.readlines()
 
-    geom = np.zeros((len(mol), 3))
-    for index, line in enumerate(reversed(lines)):
-        if 'Input orientation:' in line:
-            for n in range(len(mol)):
-                geom[n][0:3] = np.array(lines[-index+4+n].split()[3:6]).astype(float)
+    start = 0  # start reading here
+    while 1:
+        geom = np.zeros((len(mol), 3))
+        if start == 0:
+            data = lines
+        else:
+            data = lines[:-start+1]
+        for index, line in enumerate(reversed(data)):
+            if 'Input orientation:' in line:
+                for n in range(len(mol)):
+                    geom[n][0:3] = np.array(data[-index+4+n].split()[3:6]).astype(float)
+                start += index  # mark end for next loop if there is
+                break
+
+        if not max2frag:
             break
+        else:
+            from kinbot.stationary_pt import StationaryPoint
+            temp = StationaryPoint('dummy',
+                                   charge,
+                                   mult,
+                                   atom=[i for i in mol.symbols],
+                                   geom=geom)
+            temp.characterize()
+            fragments, maps = temp.start_multi_molecular()
+            if len(fragments) <= 2:
+                break
 
     return geom
 
 
 def read_zpe(outfile):
     """
     Read the zpe
@@ -254,11 +278,12 @@
     outf_end = tail(outfile, 10)
     # Use cartesian coordinates when internal ones fail.
     if 'Error in internal coordinate system' in outf_end \
             and 'cartesian' not in kwargs['opt']:
         kwargs['opt'] += ', cartesian'
     elif 'Error termination request processed by link 9999.' in outf_end:
         kwargs['opt'] = kwargs['opt'].replace('CalcFC', 'CalcAll')
+        kwargs.pop('freq', None)
         if 'cartesian' not in kwargs['opt']:
             kwargs['opt'] += ',Cartesian'
 
     return kwargs
```

### Comparing `kinbot-2.1.post0/kinbot/reader_qchem.py` & `kinbot-2.2.1/kinbot/reader_qchem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Functions to read QChem output files.
 """
-# import logging
-# import os
-# import re
-# import copy
 import logging
 
 import numpy as np
 from ase import Atoms
 
+logger = logging.getLogger('KinBot')
+
 
 def read_geom(outfile, mol=Atoms(), irc=False):
     """Read the final geometry from a QChem output file.
     """
     do_read, done = (False, False)
     with open(outfile) as f:
         for line in f:
@@ -45,15 +43,15 @@
     with open(outfile) as f:
         for line in f:
             if 'Zero point vibrational energy:' in line:
                 zpe = line.split()[4]
     try:
         return float(zpe) * constants.KCALtoHARTREE
     except ValueError:
-        logging.warning(f'Non-numeric ZPE: {zpe}')
+        logger.warning(f'Non-numeric ZPE: {zpe}')
         return np.NAN
 
 
 def read_freq(outfile, atoms):
     """
     Read the frequencies
     """
```

### Comparing `kinbot-2.1.post0/kinbot/stationary_pt.py` & `kinbot-2.2.1/kinbot/stationary_pt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-import sys
-import numpy as np
+import logging
 import copy
 import math
 import itertools
 
+import numpy as np
+from ase.data import covalent_radii, atomic_numbers
+
 from kinbot import cheminfo
 from kinbot import constants
 from kinbot import find_motif
 from kinbot import geometry
 
+logger = logging.getLogger('KinBot')
+
 
 class StationaryPoint:
     """
     This object contains the properties of wells.
     """
 
-    def __init__(self, name, charge, mult, smiles='', structure=None, natom=0, atom=None, geom=None, wellorts=0, fragA=None, fragB=None):
+    def __init__(self, name, charge, mult, smiles='', structure=None, natom=0, 
+                 atom=None, geom=None, wellorts=0, fragA=None, fragB=None):
         self.name = name
         self.mult = mult
         self.charge = charge
         self.short_name = ''  # name for the MESS calculations needs to be shorter
         if geom is None:
             self.geom = []
         else:
@@ -86,14 +91,48 @@
         self.kinbot_freqs = []
         self.reduced_freqs = []
 
         if len(self.geom) == 0:
             self.get_geom()
         if self.natom == 0:
             self.natom = len(atom)
+    
+    @classmethod
+    def from_ase_atoms(cls, atoms, **kwargs):
+        """Builds a stationary point object from an ase.Atoms object.
+
+        Args:
+            atoms (ase.Atoms): The Atoms class from the ase library.
+
+        Returns:
+            StationaryPoint: A Stationary point object with the properties of 
+                the ase.Atoms properties
+        """
+        if 'name' not in kwargs:
+            name = 'StationaryPoint'
+
+        if 'charge' not in kwargs:
+            if atoms.calc is None or 'charge' not in atoms.calc.parameters:
+                charge = sum(atoms.get_initial_charges())
+            else:
+                charge = atoms.calc.parameters['charge']
+
+        if 'mult' not in kwargs:
+            if atoms.calc is None or 'mult' not in atoms.calc.parameters:
+                mult = 1
+            else:
+                mult = atoms.calc.parameters['mult']
+
+        if 'geom' not in kwargs:
+            geom = atoms.positions
+
+        if 'symbols' not in kwargs:
+            symbols = list(atoms.symbols)
+
+        return cls(name, charge, mult, geom=geom, atom=symbols)
 
     def get_geom(self):
         """
         Method reads the structure and converts it to a geometry
         or converts the smiles to a geometry using open babel
         """
         if len(self.structure) == 0:
@@ -157,22 +196,37 @@
 
     def bond_mx(self):
         """ 
         Create bond matrix 
         Also create smiles if possible
         """
         self.distance_mx()
+        for i in range(self.natom):
+            for j in range(self.natom):
+                if i == j:
+                    continue
+                elif self.dist[i][j] < 0.5:
+                    err_msg = 'Incorrect geometry: Found an interatomic ' \
+                              'distance smaller than 0.5 Å.'
+                    logger.error(err_msg)
+                    raise ValueError(err_msg)
+
         self.bond = np.zeros((self.natom, self.natom), dtype=int)
 
         for i in range(self.natom):
             for j in range(self.natom):
                 if i == j: continue
                 atom_pair = [self.atom[i], self.atom[j]]
                 atom_pair = sorted(atom_pair)
-                if self.dist[i][j] < constants.st_bond[''.join(atom_pair)]:
+                try:
+                    bond_thresh = constants.st_bond[''.join(atom_pair)]
+                except KeyError:
+                    bond_thresh = 1.2 * (covalent_radii[atomic_numbers[atom_pair[0]]] 
+                                         + covalent_radii[atomic_numbers[atom_pair[1]]]) 
+                if self.dist[i][j] < bond_thresh:
                     self.bond[i][j] = 1
 
         max_bond = [constants.st_bond[self.atom[i]] for i in range(self.natom)]
         n_bond = np.sum(self.bond, axis=0)
 
         save_n_bond = n_bond
         self.rad = max_bond - n_bond
@@ -335,15 +389,15 @@
 
         mult = 0
         for element in atomlist:
             mult += constants.st_bond[element]
 
         return 1 + mult % 2
 
-    def start_multi_molecular(self):
+    def start_multi_molecular(self, vary_charge=False):
         """
         Iterative method to find all the separate products from a bond matrix
         """
         bond = copy.deepcopy(self.bond)
 
         status = [0 for i in range(self.natom)]  # 1: part of a molecule, 0: not part of a molecule
         atoms = [i for i in range(self.natom)]
@@ -358,52 +412,71 @@
                 at = [atoms[i] for i in range(len(status)) if status[i] == 0]
                 natomi = len(at)
                 fragi = [0 for i in range(self.natom)]
                 if natomi == 1:
                     #this is a molecule containing only one atom
                     fragi[at[0]] = 1
                     atomi = [at[0]]
-                    bool = 0
+                    boole = 0
                 else:
                     natomi = len(at)
-                    bool, sta = self.extract_next_mol(natomi,bondi)
+                    boole, sta = self.extract_next_mol(natomi,bondi)
                     atomi = [at[i] for i in range(natomi) if sta[i] == 1]
                     for i in range(len(sta)):
                         if sta[i] == 1:
                             status[at[i]] = 1
                             fragi[at[i]] = 1
 
-                if not bool and len(mols) == 0:
+                if not boole and len(mols) == 0:
                     #the bond matrix corresponds to one molecule only
                     try:
                         delattr(self, 'cycle_chain')
                     except AttributeError:
                         pass
                     self.characterize()  
                     self.name = str(self.chemid)
                     mols.append(self)
                     break
                 geomi = np.asarray(self.geom)[np.where(np.asarray(fragi) == 1)]
                 natomi = np.sum(fragi)
                 atomi = atomlist[np.where(np.asarray(fragi) == 1)]
-                multi = self.calc_multiplicity(atomi)
-                chargei = self.charge # todo
-                moli = StationaryPoint('prod_%i'%(len(mols)+1), chargei, multi, atom=atomi, natom=natomi, geom=geomi)
-                moli.characterize()  
-                moli.calc_chemid()
-                moli.name = str(moli.chemid)
-
-                mols.append(moli)
-
-                numbering = np.asarray(range(self.natom))
-                # the original atom numbers in the correct order in the fragments, it's a map
-                mapi = numbering[np.where(np.asarray(fragi) == 1)]  
-                maps.append(mapi)
 
-                if bool:
+                if vary_charge and self.charge != 0:
+                    multiply = 2
+                else:
+                    multiply = 1
+                
+                for ch in range(multiply):
+                    # ch == 0 is neutral, ch == 1  is ion case
+                    multi = self.calc_multiplicity(atomi)
+                    # on the second pass, adjust the multiplicity
+                    if ch == 1 and multi == 1:
+                        multi = 2
+                    elif ch == 1 and multi == 2:
+                        multi = 1
+                    if ch == 1 and multi == 3:
+                        multi = 2
+
+                    if ch == 0:   
+                        chargei = 0
+                    elif ch == 1:
+                        chargei = self.charge 
+                    moli = StationaryPoint('prod_%i'%(len(mols)+1), chargei, multi, atom=atomi, natom=natomi, geom=geomi)
+                    moli.characterize()  
+                    moli.calc_chemid()
+                    moli.name = str(moli.chemid)
+
+                    mols.append(moli)
+
+                    numbering = np.asarray(range(self.natom))
+                    # the original atom numbers in the correct order in the fragments, it's a map
+                    mapi = numbering[np.where(np.asarray(fragi) == 1)]  
+                    maps.append(mapi)
+
+                if boole:
                     continue 
                 else:
                     #reached the end, return the molecules
                     break
 
         return mols, maps
 
@@ -528,15 +601,14 @@
                                                                                                                         
     def start_id(self, i):
         """ 
         Initialize recursive loop for id.
         i is the index for the atom to start at.
         """
         
-        
         visit = [0 for k in range(self.natom)]
         depth = 0
         atomid = int(0)
         
         self.atomid[i], visit = self.calc_atomid(visit, depth, i, atomid)
         # a, visit = self.calc_atomid(visit, depth, i, atomid, natom, atom)
 
@@ -756,15 +828,14 @@
                             for neigh in double_neigh:
                                 if sum(self.bond[neigh]) > 2:  # atom has at least one other neighbor
                                     return 1
                     return 0
 
         return 0
     
-
     def calc_chiral(self):
         """
         Calculate self.chiral. 0 if non-chiral, +1 or -1 if chiral. Each atom gets a label like this.
         """
         self.chiral = np.zeros(self.natom)
         # take min of resonance structure bonds
         # as those portions are planar and do not contribute to chirality
@@ -799,15 +870,14 @@
                                     atids.append(self.atomid[j])
                                     positions = np.append(positions, [self.geom[j]], axis=0)
                             if len(set(atids)) == 4:
                                 center = instance[int(dlen / 2)]
                                 self.chiral[center] = self.calc_chiral_hand(self.geom[center], positions, atids)
         return self.chiral
 
-
     def calc_chiral_hand(self, center, ligands, atomids):
         """
         Calculate the handedness of a chiral center. 
         """
 
         largelig = np.argmax(atomids)
        
@@ -844,15 +914,14 @@
         if np.array_equal(xorder, idorder):
             hand = +1 * mirror
         else:
             hand = -1 * mirror
         
         return hand
 
-
     def find_linear(self):
         self.linear = []
         for ati in range(self.natom):
             for atj in range(self.natom):
                 if self.bonds[0][ati][atj] > 0:
                     for atk in range(self.natom):
                         if self.bonds[0][atj][atk] > 0 and atk != ati:
@@ -863,15 +932,14 @@
                                 else:
                                     lin = [atk, atj, ati] 
                                 if lin not in self.linear:
                                     self.linear.append(lin)
 
         return
 
-
     def calc_maxbond(self):
         """
         Needed to find rigid segments
         Takes the maximum of all bond matrices
         """
 
         self.maxbond = self.bonds[0]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kinbot-2.1.post0/kinbot/symmetry.py` & `kinbot-2.2.1/kinbot/symmetry.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/thread_kinbot.py` & `kinbot-2.2.1/kinbot/thread_kinbot.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/uncertaintyAnalysis.py` & `kinbot-2.2.1/kinbot/uncertaintyAnalysis.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/kinbot/utils.py` & `kinbot-2.2.1/kinbot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 def clean_files():
     """Removes files from jobs that ended up erroneously.
     """
     import logging
     import numpy as np
     from kinbot.ase_modules.io.formats import read
+    logger = logging.getLogger('KinBot')
     # delete leftover AM1 calculations
     files = os.listdir()
     com = []
     for ff in files:
         if 'com' in ff:
             com.append(ff)
 
@@ -106,15 +107,15 @@
         with open(cc, 'r') as f:
             if 'am1' in f.read():
                 delfile = True
         if delfile:
             ll = cc.split('.')[0] + '.log'
             try:
                 os.remove(ll)
-                logging.info(f'Stuck AM1 job {ll} is deleted.')
+                logger.info(f'Stuck AM1 job {ll} is deleted.')
             except FileNotFoundError:
                 pass
 
     # delete empty files
     try:
         conf_files = os.listdir('conf')
         conf_files = [f'conf/{ff}' for ff in conf_files]
@@ -132,18 +133,18 @@
             log.append(ff)
 
     for ll in log:
         if not os.path.isfile(ll):
             continue
         if os.path.getsize(ll) < 10:
             os.remove(ll)
-            logging.info(f'Empty file {ll} is deleted.')
+            logger.info(f'Empty file {ll} is deleted.')
         else:
             try:
                 atoms = read(ll)
             except StopIteration:
                 continue
             else:
                 if len(atoms.positions) > 1 and np.all(atoms.positions == 0):
                     os.remove(ll)
-                    logging.info(f'All coordinates of file {ll} are 0, hence '
+                    logger.info(f'All coordinates of file {ll} are 0, hence '
                                  f'it is deleted.')
```

### Comparing `kinbot-2.1.post0/kinbot/zmatrix.py` & `kinbot-2.2.1/kinbot/zmatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import logging
 import numpy as np
 import copy
 
 from kinbot import geometry
 
+logger = logging.getLogger('KinBot')
+
 
 def make_zmat_from_cart(species, rotor, cart, mode):
     """
     Rearrange geometry defined in Cartesian into a Z-matrix,
     with references suitable for a 1-D hindered rotor scan.
     If mode = 0: all rotatable bonds
     If mode = 1: only those bonds, which generate conformers
@@ -232,19 +234,19 @@
             for at in rotor:
                 if at not in zmatorder:
                     to_add.append(at)
                 else:
                     added.append(at)
 
             if len(to_add) == 0:
-                logging.error("error, all atoms of a rotor have been added, without adding this dihedral explicitly")
+                logger.error("error, all atoms of a rotor have been added, without adding this dihedral explicitly")
             elif len(to_add) == 1:
                 at = to_add[0]
                 if rotor.index(at) == 1 or rotor.index(at) == 2:
-                    logging.error("error, all atoms except a middle atom have been added, strange...")
+                    logger.error("error, all atoms except a middle atom have been added, strange...")
                 elif rotor.index(at) == 0:
                     add(j, [at, rotor[1], rotor[2], rotor[3]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
                 elif rotor.index(at) == 3:
                     add(j, [at, rotor[2], rotor[1], rotor[0]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
             elif len(to_add) == 2:
@@ -311,15 +313,15 @@
                     neighbor_list = get_neighbors(rotor[0], bond, natom, rotors, zmatorder)
                     # add rotor[1]
                     add(j, [rotor[1], rotor[0], neighbor_list[0], neighbor_list[1]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     # add rotor[3]
                     add(j, [rotor[3], rotor[2], rotor[1], rotor[0]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
                 else:
-                    logging.error("error, two atoms that need to be added are not the outer atoms of a rotor, strange...")
+                    logger.error("error, two atoms that need to be added are not the outer atoms of a rotor, strange...")
             elif len(to_add) == 3:
                 if added[0] == rotor[0]:
                     neighbor_list = get_neighbors(rotor[0], bond, natom, rotors, zmatorder)
                     add(j, [rotor[1], rotor[0], neighbor_list[0], neighbor_list[1]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
                     add(j, [rotor[2], rotor[1], rotor[0], neighbor_list[0]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
@@ -362,15 +364,15 @@
                     add(j, [rotor[2], rotor[3], neighbor_list[0], neighbor_list[1]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
                     add(j, [rotor[1], rotor[2], rotor[3], neighbor_list[0]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
                     add(j, [rotor[0], rotor[1], rotor[2], rotor[3]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                     j += 1
                 else:
-                    logging.error('error')
+                    logger.error('error')
             else:
                 if len(chain) == 2:  # this is the minimum chain length
                     neighbor_list = get_neighbors(chain[1], bond, natom, rotors, zmatorder)
                     if chain[0] == rotor[0]:
                         add(j, [rotor[0], chain[1], neighbor_list[0], neighbor_list[1]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                         j += 1
                         add(j, [rotor[1], rotor[0], chain[1], neighbor_list[0]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
@@ -500,15 +502,15 @@
                         add(j, [rotor[2], rotor[3], ref_list[0], ref_list[1]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                         j += 1
                         add(j, [rotor[1], rotor[2], rotor[3], ref_list[0]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                         j += 1
                         add(j, [rotor[0], rotor[1], rotor[2], rotor[3]], zmat, zmat_atom, zmatorder, zmat_ref, atom, cart)
                         j += 1
                 else:
-                    logging.error('error, chain length too small')
+                    logger.error('error, chain length too small')
             rot_index += 1
     else:
         # no rotors here, add the first four atoms of the molecule
         zmat_atom = ['X' for i in range(natom)]
         zmat_ref = np.zeros((natom, 3), dtype=int) - 1
         zmat = np.zeros((natom, 3)) - 1
         zmatorder = [-1 for i in range(natom)]
```

### Comparing `kinbot-2.1.post0/pyproject.toml` & `kinbot-2.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-exclude = ["build", "dist", "KinBot.egg-info"]
+exclude = ["build", "dist", "KinBot.egg-info", "graphics"]
+
+[tool.setuptools.package-data]
+"kinbot.tpl" = ["*.tpl"]
 
 [project]
 name = "kinbot"
-version = "2.1.post0"
+version = "2.2.1"
 description = "Automated reaction kinetics for gas-phase species"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 # keywords = []
 authors = [
     {name="Judit Zádor", email="jzador@sandia.gov"},
@@ -27,22 +30,22 @@
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Chemistry"
 ]
 dependencies = [
         "numpy>=1.17.0",
         "ase>=3.19",
         "networkx",
-        "rmsd",
-        "typing-extensions"  # TODO Not a direct dependency. Remove it once rmsd list it as theirs.
+        "rmsd>=1.5.1",
 ]
 
 [project.optional-dependencies]
 plot = [
     "matplotlib",
     "pyvis",
     "rdkit"
@@ -50,8 +53,8 @@
 
 [project.urls]
 homepage = "https://github.com/zadorlab/KinBot"
 documentation = "https://github.com/zadorlab/KinBot/wiki"
 
 [project.scripts]
 kinbot = "kinbot.kb:main"
-pes = "kinbot.pes:main"
+pes = "kinbot.pes:main"
```

### Comparing `kinbot-2.1.post0/reactions/__init__.py` & `kinbot-2.2.1/kinbot/tpl/__init__.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_12_shift_S_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_r13_insertion_CO2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from kinbot import constants
-from kinbot import geometry
 from kinbot.reac_General import GeneralReac
+from kinbot import geometry
 
-class S12ShiftF(GeneralReac):
-    max_step = 12
+class R13InsertionCO2(GeneralReac):
+    max_step = 22
     scan = 0
     skip = 0
-    family_name = 's12shiftf'
-        
+    dihstep = 12
+    family_name = 'r13insertionco2'
 
+    
     def get_constraints(self,step, geom):
         fix = []
         change = []
         release = []
-        if step < self.max_step:
-            self.fix_bonds(fix)
-           
-        if step < self.max_step:
-            final_dist1 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[1]] + self.species.atom[self.instance[2]]))]
-            self.set_bond(1, 2, -999, change, step=step, stmax=self.max_step, findist=final_dist1, geom=geom)
+        self.fix_bonds(fix)
+
+        if step < self.dihstep:
+            self.set_dihedrals(change, step)
+
+        elif step < self.max_step:
+            self.release_dihedrals(release)
+                
+            fval = [2.0, 1.3, 2.0, 2.0]
+            if self.species.atom[self.instance[-1]] == 'H':
+                fval[2] = 1.35
+                fval[3] = 1.35
             
-            final_dist2 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[0]] + self.species.atom[self.instance[2]]))]
-            self.set_bond(0, 2, -999, change, step=step, stmax=self.max_step, findist=final_dist2, geom=geom)
+            self.set_bond(0, 1, -999, change, step=step-11, stmax=10, findist=fval[0], geom=geom)
+            self.set_bond(1, 2, -999, change, step=step-11, stmax=10, findist=fval[1], geom=geom)
+            self.set_bond(2, 3, -999, change, step=step-11, stmax=10, findist=fval[2], geom=geom)
+            self.set_bond(3, 0, -999, change, step=step-11, stmax=10, findist=fval[3], geom=geom)
 
-        self.clean_constraints(change, fix)        
+        self.clean_constraints(change, fix)
         
         return step, fix, change, release
```

### Comparing `kinbot-2.1.post0/reactions/reac_12_shift_S_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_12_shift_S_F.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,38 @@
+from ase.data import atomic_numbers, covalent_radii
+
 from kinbot import constants
-from kinbot import geometry
 from kinbot.reac_General import GeneralReac
 
-class S12ShiftR(GeneralReac):
+class S12ShiftF(GeneralReac):
     max_step = 12
     scan = 0
     skip = 0
-    family_name = 's12shiftr'
-    
+    family_name = 's12shiftf'
+        
 
     def get_constraints(self,step, geom):
         fix = []
         change = []
         release = []
         if step < self.max_step:
             self.fix_bonds(fix)
            
         if step < self.max_step:
-            final_dist1 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[1]]+self.species.atom[self.instance[2]]))]
+            try:
+                final_dist1 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[1]] 
+                                                               + self.species.atom[self.instance[2]]))]
+            except KeyError:
+                final_dist1 = 1.2 * (covalent_radii[atomic_numbers[self.species.atom[self.instance[1]]]] 
+                                     + covalent_radii[atomic_numbers[self.species.atom[self.instance[2]]]])                
             self.set_bond(1, 2, -999, change, step=step, stmax=self.max_step, findist=final_dist1, geom=geom)
-            
-            final_dist2 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[0]]+self.species.atom[self.instance[2]]))]
+            try:       
+                final_dist2 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[0]] 
+                                                           + self.species.atom[self.instance[2]]))]
+            except KeyError:
+                final_dist2 = 1.2 * (covalent_radii[atomic_numbers[self.species.atom[self.instance[0]]]] 
+                                     + covalent_radii[atomic_numbers[self.species.atom[self.instance[2]]]])
             self.set_bond(0, 2, -999, change, step=step, stmax=self.max_step, findist=final_dist2, geom=geom)
 
         self.clean_constraints(change, fix)        
         
         return step, fix, change, release
```

### Comparing `kinbot-2.1.post0/reactions/reac_Cyclic_Ether_Formation.py` & `kinbot-2.2.1/kinbot/reactions/reac_Cyclic_Ether_Formation.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Diels_alder_addition.py` & `kinbot-2.2.1/kinbot/reactions/reac_Diels_alder_addition.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_HO2_Elimination_from_PeroxyRadical.py` & `kinbot-2.2.1/kinbot/reactions/reac_HO2_Elimination_from_PeroxyRadical.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_Diels_alder_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_Diels_alder_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Endocyclic_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Endocyclic_F.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Endocyclic_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Endocyclic_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Exocyclic_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Exocyclic_F.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_RH_Add_Exocyclic_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_RH_Add_Exocyclic_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_R_Add_Endocyclic_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_R_Add_Endocyclic_F.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_R_Add_ExoTetCyclic_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_R_Add_ExoTetCyclic_F.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from ase.data import atomic_numbers, covalent_radii
+
 from kinbot import geometry
 from kinbot.reac_General import GeneralReac
 from kinbot import constants
 
 
 class IntraRAddExoTetCyclicF(GeneralReac):
     max_step = 22
@@ -31,22 +33,30 @@
             else:
                 new_dih = dih + frac * (180. - dih) 
                 ldih.append(new_dih)
             change.append(ldih)
 
         elif step < self.max_step:
             self.release_dihedrals(release)
-            fdist1 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[0]] + self.species.atom[self.instance[-2]]))] * 1.0
+            try:
+                fdist1 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[0]] + self.species.atom[self.instance[-2]]))]
+            except KeyError:
+                fdist1 = 1.2 * (covalent_radii[atomic_numbers[self.species.atom[self.instance[0]]]] 
+                                + covalent_radii[atomic_numbers[self.species.atom[self.instance[-2]]]])
             if ''.join(sorted(self.species.atom[self.instance[0]] + self.species.atom[self.instance[-2]])) == 'CO':
                 if ''.join(sorted(self.species.atom[self.instance[-1]] + self.species.atom[self.instance[-2]])) == 'OO':
                     fdist1 = 1.96
                 else:
                     fdist1 = 1.68
             self.set_bond(0, -2, -999, change, step=step-11, stmax=10, findist=fdist1, geom=geom)
+            try:
+                fdist2 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[-1]] + self.species.atom[self.instance[-2]]))]
+            except KeyError:
+                fdist2 = 1.2 * (covalent_radii[atomic_numbers[self.species.atom[self.instance[-1]]]] 
+                                + covalent_radii[atomic_numbers[self.species.atom[self.instance[-2]]]])
             
-            fdist2 = constants.st_bond[''.join(sorted(self.species.atom[self.instance[-1]] + self.species.atom[self.instance[-2]]))] * 1.0
             if ''.join(sorted(self.species.atom[self.instance[-1]] + self.species.atom[self.instance[-2]])) == 'CO':
                 fdist2 = 1.68
             self.set_bond(-1, -2, -999, change, step=step-11, stmax=10, findist=fdist2, geom=geom)
         self.clean_constraints(change, fix)
         
         return step, fix, change, release
```

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_R_Add_Exocyclic_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_R_Add_Exocyclic_F.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_disproportionation_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_disproportionation_F.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Intra_disproportionation_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_Intra_disproportionation_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Korcek_step2.py` & `kinbot-2.2.1/kinbot/reactions/reac_Korcek_step2.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Korcek_step2_even.py` & `kinbot-2.2.1/kinbot/reactions/reac_Korcek_step2_even.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Korcek_step2_odd.py` & `kinbot-2.2.1/kinbot/reactions/reac_Korcek_step2_odd.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_R_Addition_COm3_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_R_Addition_COm3_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_R_Addition_MultipleBond.py` & `kinbot-2.2.1/kinbot/reactions/reac_R_Addition_MultipleBond.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_Retro_Ene.py` & `kinbot-2.2.1/kinbot/reactions/reac_Retro_Ene.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_abstraction.py` & `kinbot-2.2.1/kinbot/reactions/reac_abstraction.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_barrierless_saddle.py` & `kinbot-2.2.1/kinbot/reactions/reac_barrierless_saddle.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_beta_delta.py` & `kinbot-2.2.1/kinbot/reactions/reac_beta_delta.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_birad_recombination_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_birad_recombination_F.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_birad_recombination_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_birad_recombination_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_combinatorial.py` & `kinbot-2.2.1/kinbot/reactions/reac_combinatorial.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_cpd_H_migration.py` & `kinbot-2.2.1/kinbot/reactions/reac_cpd_H_migration.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_h2_elim.py` & `kinbot-2.2.1/kinbot/reactions/reac_h2_elim.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_intra_H_migration.py` & `kinbot-2.2.1/kinbot/reactions/reac_intra_H_migration.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_intra_H_migration_suprafacial.py` & `kinbot-2.2.1/kinbot/reactions/reac_intra_H_migration_suprafacial.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_intra_OH_migration.py` & `kinbot-2.2.1/kinbot/reactions/reac_intra_OH_migration.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_intra_OH_migration_Exocyclic_F.py` & `kinbot-2.2.1/kinbot/reactions/reac_intra_OH_migration_Exocyclic_F.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_intra_R_migration.py` & `kinbot-2.2.1/kinbot/reactions/reac_intra_R_migration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from ase.data import atomic_numbers, covalent_radii
+
 from kinbot.reac_General import GeneralReac
 from kinbot import constants
 
 
 class IntraRMigration(GeneralReac):
     max_step = 14
     scan = 0
@@ -31,17 +33,27 @@
                 fval = 1.35
                 if self.species.atom[self.instance[-2]] == 'O': fval = 1.2
                 self.set_bond(-2, -1, fval, change)
                 #  step = 13  TODO this was a typo I think
         elif step == 13:
             self.release_angles(release)
             self.release_dihedrals(release)
-                
-            fval = constants.st_bond[''.join(sorted(self.species.atom[self.instance[0]]+self.species.atom[self.instance[-1]]))]*1.0
+            
+            try:
+                fval = constants.st_bond[''.join(sorted(self.species.atom[self.instance[0]]+self.species.atom[self.instance[-1]]))]
+            except KeyError:
+                fval = 1.2 * (covalent_radii[atomic_numbers[self.species.atom[self.instance[0]]]] 
+                              + covalent_radii[atomic_numbers[self.species.atom[self.instance[-1]]]])
+
             self.set_bond(0, -1, fval, change)
             
-            fval = constants.st_bond[''.join(sorted(self.species.atom[self.instance[-2]]+self.species.atom[self.instance[-1]]))]*1.0
+            try:
+                fval = constants.st_bond[''.join(sorted(self.species.atom[self.instance[-2]]+self.species.atom[self.instance[-1]]))]
+            except KeyError:
+                fval = (covalent_radii[atomic_numbers[self.species.atom[self.instance[-2]]]] 
+                        + covalent_radii[atomic_numbers[self.species.atom[self.instance[-1]]]])
+
             self.set_bond(-2, -1, fval, change)
         
         self.clean_constraints(change, fix)
         
         return step, fix, change, release
```

### Comparing `kinbot-2.1.post0/reactions/reac_ketoenol.py` & `kinbot-2.2.1/kinbot/reactions/reac_ketoenol.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_r12_cycloaddition.py` & `kinbot-2.2.1/kinbot/reactions/reac_r12_cycloaddition.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_r12_insertion_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_r12_insertion_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_r13_insertion_CO2.py` & `kinbot-2.2.1/kinbot/reactions/reac_r13_insertion_ROR.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from kinbot.reac_General import GeneralReac
 from kinbot import geometry
 
-class R13InsertionCO2(GeneralReac):
+class R13InsertionROR(GeneralReac):
     max_step = 22
     scan = 0
     skip = 0
     dihstep = 12
-    family_name = 'r13insertionco2'
+    family_name = 'r13insertionror'
+
 
-    
     def get_constraints(self,step, geom):
         fix = []
         change = []
         release = []
         self.fix_bonds(fix)
 
         if step < self.dihstep:
             self.set_dihedrals(change, step)
 
         elif step < self.max_step:
             self.release_dihedrals(release)
-                
-            fval = [2.0, 1.3, 2.0, 2.0]
-            if self.species.atom[self.instance[-1]] == 'H':
-                fval[2] = 1.35
-                fval[3] = 1.35
             
+            fval = [2.0, 1.45, 2.0, 2.0]
+            if self.species.atom[self.instance[0]] == 'H':
+                fval[0] = 1.3
+                fval[3] = 1.3
+
             self.set_bond(0, 1, -999, change, step=step-11, stmax=10, findist=fval[0], geom=geom)
             self.set_bond(1, 2, -999, change, step=step-11, stmax=10, findist=fval[1], geom=geom)
             self.set_bond(2, 3, -999, change, step=step-11, stmax=10, findist=fval[2], geom=geom)
             self.set_bond(3, 0, -999, change, step=step-11, stmax=10, findist=fval[3], geom=geom)
 
         self.clean_constraints(change, fix)
```

### Comparing `kinbot-2.1.post0/reactions/reac_r13_insertion_ROR.py` & `kinbot-2.2.1/kinbot/reactions/reac_r13_insertion_RSR.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from kinbot.reac_General import GeneralReac
 from kinbot import geometry
 
-class R13InsertionROR(GeneralReac):
+class R13InsertionRSR(GeneralReac):
     max_step = 22
     scan = 0
     skip = 0
     dihstep = 12
-    family_name = 'r13insertionror'
+    family_name = 'r13insertionrsr'
+    
 
-
-    def get_constraints(self,step, geom):
+    def get_constraints(self, step, geom):
         fix = []
         change = []
         release = []
         self.fix_bonds(fix)
 
         if step < self.dihstep:
             self.set_dihedrals(change, step)
@@ -21,15 +21,15 @@
         elif step < self.max_step:
             self.release_dihedrals(release)
             
             fval = [2.0, 1.45, 2.0, 2.0]
             if self.species.atom[self.instance[0]] == 'H':
                 fval[0] = 1.3
                 fval[3] = 1.3
-
+            
             self.set_bond(0, 1, -999, change, step=step-11, stmax=10, findist=fval[0], geom=geom)
             self.set_bond(1, 2, -999, change, step=step-11, stmax=10, findist=fval[1], geom=geom)
             self.set_bond(2, 3, -999, change, step=step-11, stmax=10, findist=fval[2], geom=geom)
             self.set_bond(3, 0, -999, change, step=step-11, stmax=10, findist=fval[3], geom=geom)
 
         self.clean_constraints(change, fix)
```

### Comparing `kinbot-2.1.post0/reactions/reac_r13_insertion_RSR.py` & `kinbot-2.2.1/kinbot/reactions/reac_bimol_disproportionation_R.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-from kinbot.reac_General import GeneralReac
 from kinbot import geometry
+from kinbot.reac_General import GeneralReac
+
 
-class R13InsertionRSR(GeneralReac):
+class BimolDisproportionationR(GeneralReac):
     max_step = 22
     scan = 0
     skip = 0
     dihstep = 12
-    family_name = 'r13insertionrsr'
+    family_name = 'bimoldisproportionationr'
     
 
-    def get_constraints(self, step, geom):
+    def get_constraints(self,step, geom):
         fix = []
         change = []
         release = []
         self.fix_bonds(fix)
 
         if step < self.dihstep:
             self.set_dihedrals(change, step)
 
         elif step < self.max_step:
             self.release_dihedrals(release)
-            
-            fval = [2.0, 1.45, 2.0, 2.0]
-            if self.species.atom[self.instance[0]] == 'H':
-                fval[0] = 1.3
-                fval[3] = 1.3
-            
-            self.set_bond(0, 1, -999, change, step=step-11, stmax=10, findist=fval[0], geom=geom)
-            self.set_bond(1, 2, -999, change, step=step-11, stmax=10, findist=fval[1], geom=geom)
-            self.set_bond(2, 3, -999, change, step=step-11, stmax=10, findist=fval[2], geom=geom)
-            self.set_bond(3, 0, -999, change, step=step-11, stmax=10, findist=fval[3], geom=geom)
+                
+            fval = 1.35
+            self.set_bond(0, -1, -999, change, step=step-11, stmax=10, findist=fval, geom=geom)
+            self.set_bond(-2, -1, -999, change, step=step-11, stmax=10, findist=fval, geom=geom)
+            fval = 2.3
+            self.set_bond(-4, -3, -999, change, step=step-11, stmax=10, findist=fval, geom=geom)
 
         self.clean_constraints(change, fix)
         
         return step, fix, change, release
```

### Comparing `kinbot-2.1.post0/reactions/reac_r14_birad_scission.py` & `kinbot-2.2.1/kinbot/reactions/reac_r14_birad_scission.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_r14_cyclic_birad_scission_R.py` & `kinbot-2.2.1/kinbot/reactions/reac_r14_cyclic_birad_scission_R.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/reactions/reac_r22_cycloaddition.py` & `kinbot-2.2.1/kinbot/reactions/reac_r22_cycloaddition.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/__init__.py` & `kinbot-2.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/bfgs.py` & `kinbot-2.2.1/tests/bfgs.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/cheminfo.py` & `kinbot-2.2.1/tests/cheminfo.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/dihedrals.py` & `kinbot-2.2.1/tests/dihedrals.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/find_motif.py` & `kinbot-2.2.1/tests/find_motif.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/frequencies.py` & `kinbot-2.2.1/tests/frequencies.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/geometry.py` & `kinbot-2.2.1/tests/geometry.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/modify_geom.py` & `kinbot-2.2.1/tests/modify_geom.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/multimolecular.py` & `kinbot-2.2.1/tests/multimolecular.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/resonance.py` & `kinbot-2.2.1/tests/resonance.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/symmetry.py` & `kinbot-2.2.1/tests/symmetry.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tests/test_kinbot.py` & `kinbot-2.2.1/tests/test_kinbot.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/__init__.py` & `kinbot-2.2.1/kinbot/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 ## rights to this software.                      ##
 ##                                               ##
 ## Authors:                                      ##
 ##   Judit Zador                                 ##
 ##   Ruben Van de Vijver                         ##
 ##                                               ##
 ###################################################
+
+kb_path = __path__[0]
```

### Comparing `kinbot-2.1.post0/tpl/ase_gauss_hir.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_gauss_hir.tpl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ase import Atoms
-# from ase.calculators.gaussian import Gaussian
 from ase.db import connect
 
-from kinbot.ase_modules.calculators.gaussian import Gaussian  # New
+from kinbot.ase_modules.calculators.gaussian import Gaussian
 from kinbot import reader_gauss
 from kinbot.utils import iowait
 
 db = connect('{working_dir}/kinbot.db')
 label = '{label}'
 logfile = '{label}.log'
```

### Comparing `kinbot-2.1.post0/tpl/ase_gauss_irc.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_gauss_irc.tpl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ase import Atoms
-# from ase.calculators.gaussian import Gaussian
 from ase.db import connect
 
-from kinbot.ase_modules.calculators.gaussian import Gaussian  # New
+from kinbot.ase_modules.calculators.gaussian import Gaussian
 from kinbot import reader_gauss
 from kinbot.utils import iowait
 
 db = connect('{working_dir}/kinbot.db')
 label = '{label}'
 logfile = '{label}.log'
 
@@ -53,19 +52,27 @@
     prod_kwargs = {prod_kwargs}
     calc_prod = Gaussian(**prod_kwargs)
     mol_prod = Atoms(symbols={atom}, positions=mol.positions)
     mol_prod.calc = calc_prod
     try:
         e = mol_prod.get_potential_energy() # use the Gaussian optimizer
         iowait(logfile, 'gauss')
-        mol_prod.positions = reader_gauss.read_geom(logfile, mol_prod)
+        mol_prod.positions = reader_gauss.read_geom(logfile, 
+                                                    mol_prod, 
+                                                    max2frag=True, 
+                                                    charge=kwargs['charge'],
+                                                    mult=kwargs['mult'])
         db.write(mol_prod, name=label, data={{'energy': e, 'status': 'normal'}})
     except RuntimeError: 
         iowait(logfile, 'gauss')
-        mol_prod.positions = reader_gauss.read_geom(logfile, mol_prod)
+        mol_prod.positions = reader_gauss.read_geom(logfile, 
+                                                    mol_prod, 
+                                                    max2frag=True, 
+                                                    charge=kwargs['charge'],
+                                                    mult=kwargs['mult'])
         if mol_prod.positions is not None:
             db.write(mol_prod, name=label, data={{'status': 'normal'}}) 
         else:
             db.write(mol_prod, name=label, data={{'status': 'error'}})
 
     with open(logfile, 'a') as f:
         f.write('done\n')
```

### Comparing `kinbot-2.1.post0/tpl/ase_gauss_opt_well.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_gauss_opt_well.tpl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from ase import Atoms
-# from ase.calculators.gaussian import Gaussian
 from ase.db import connect
 
-from kinbot.ase_modules.calculators.gaussian import Gaussian  # New
+from kinbot.ase_modules.calculators.gaussian import Gaussian
 from kinbot import reader_gauss
 from kinbot.utils import iowait
 
 db = connect('{working_dir}/kinbot.db')
 label = '{label}'
 logfile = '{label}.log'
```

### Comparing `kinbot-2.1.post0/tpl/ase_gauss_ring_conf.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_gauss_ring_conf.tpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ase import Atoms
 from ase.optimize import LBFGS
 from ase.db import connect
 
 from kinbot.ase_modules.calculators.gaussian import Gaussian
-from kinbot.ase_modules.constraints import FixInternals  # New
+from kinbot.ase_modules.constraints import FixInternals
 from kinbot import reader_gauss
 from kinbot.utils import iowait
 
 db = connect('{working_dir}/kinbot.db')
 label = '{label}'
 logfile = '{label}.log'
```

### Comparing `kinbot-2.1.post0/tpl/ase_gauss_ts_end.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_gauss_ts_end.tpl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from ase import Atoms
-#from ase.calculators.gaussian import Gaussian
 from ase.db import connect
 
-from kinbot.ase_modules.calculators.gaussian import Gaussian  # New
+from kinbot.ase_modules.calculators.gaussian import Gaussian
 from kinbot import reader_gauss
 from kinbot.utils import iowait
 
 db = connect('{working_dir}/kinbot.db')
 label = '{label}'
 logfile = '{label}.log'
```

### Comparing `kinbot-2.1.post0/tpl/ase_gauss_ts_search.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_gauss_ts_search.tpl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ase import Atoms
-# from ase.calculators.gaussian import Gaussian
 from ase.db import connect
 
-from kinbot.ase_modules.calculators.gaussian import Gaussian  # New
+from kinbot.ase_modules.calculators.gaussian import Gaussian
 from kinbot import reader_gauss
 from kinbot.utils import iowait
 
 db = connect('{working_dir}/kinbot.db')
 label = '{label}'
 logfile = '{label}.log'
 
@@ -16,15 +15,15 @@
 
 kwargs = {kwargs}
 Gaussian.command = '{qc_command} < PREFIX.com > PREFIX.log'
 calc = Gaussian(**kwargs)
 mol.calc = calc
 
 try:
-    e = mol.get_potential_energy()  # use the Gaussian optimizer (task optimize)
+    e = mol.get_potential_energy()  # use the Gaussian optimizer
 except RuntimeError: 
     e = 0.
  
 iowait(logfile, 'gauss')
 mol.positions = reader_gauss.read_geom(logfile, mol)
 if all([ci == 0 for mp in mol.positions for ci in mp]):
     mol.positions = {geom}  # reset to the original geometry
```

### Comparing `kinbot-2.1.post0/tpl/ase_nwchem_freq_well.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_nwchem_freq_well.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_nwchem_irc.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_nwchem_irc.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_nwchem_opt_well.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_nwchem_opt_well.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_nwchem_ts_end.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_nwchem_ts_end.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_nwchem_ts_search.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_nwchem_ts_search.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_nwchem_ts_search_ase_constraints.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_nwchem_ts_search_ase_constraints.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_qchem_hir.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_qchem_hir.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_qchem_irc.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_qchem_irc.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_qchem_opt_well.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_qchem_opt_well.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_qchem_ts_end.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_qchem_ts_end.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/ase_qchem_ts_search.tpl.py` & `kinbot-2.2.1/kinbot/tpl/ase_qchem_ts_search.tpl.py`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/mess_barrierless.tpl` & `kinbot-2.2.1/kinbot/tpl/mess_barrierless.tpl`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/mess_header.tpl` & `kinbot-2.2.1/kinbot/tpl/mess_header.tpl`

 * *Files identical despite different names*

### Comparing `kinbot-2.1.post0/tpl/pesviewer.inp.tpl` & `kinbot-2.2.1/kinbot/tpl/pesviewer.inp.tpl`

 * *Files identical despite different names*

