# Comparing `tmp/thapbi_pict-1.0.0.tar.gz` & `tmp/thapbi_pict-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thapbi_pict-1.0.0.tar", last modified: Fri May 19 12:47:13 2023, max compression
+gzip compressed data, was "thapbi_pict-1.0.1.tar", last modified: Wed Jul 26 11:33:00 2023, max compression
```

## Comparing `thapbi_pict-1.0.0.tar` & `thapbi_pict-1.0.1.tar`

### file list

```diff
@@ -1,545 +1,549 @@
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:05.000000 thapbi_pict-1.0.0/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      818 2022-02-15 12:09:29.000000 thapbi_pict-1.0.0/.flake8
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      883 2022-02-15 12:09:29.000000 thapbi_pict-1.0.0/.zenodo.json
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    13628 2023-05-19 12:41:38.000000 thapbi_pict-1.0.0/CHANGELOG.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5120 2023-04-28 12:36:14.000000 thapbi_pict-1.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2469 2023-05-19 09:46:34.000000 thapbi_pict-1.0.0/INSTALL.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1094 2022-02-15 12:09:29.000000 thapbi_pict-1.0.0/LICENSE.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4581 2023-04-06 15:07:11.000000 thapbi_pict-1.0.0/MANIFEST.in
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8249 2023-05-19 12:47:05.000000 thapbi_pict-1.0.0/PKG-INFO
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6964 2023-05-19 09:46:34.000000 thapbi_pict-1.0.0/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:56.000000 thapbi_pict-1.0.0/database/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    24077 2023-04-06 15:07:11.000000 thapbi_pict-1.0.0/database/2022-09-16_ITS1_Oomycota_obs.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1737519 2023-04-06 15:07:11.000000 thapbi_pict-1.0.0/database/2022-09-16_ITS1_Oomycota_w32.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   463737 2023-05-19 12:44:02.000000 thapbi_pict-1.0.0/database/ITS1_DB.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1035985 2023-05-19 12:44:02.000000 thapbi_pict-1.0.0/database/ITS1_DB.sql
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3890 2022-06-13 12:04:40.000000 thapbi_pict-1.0.0/database/Nothophytophthora_ITS1_curated.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    65170 2023-04-06 15:07:11.000000 thapbi_pict-1.0.0/database/Phytophthora_ITS1_curated.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3520 2023-05-19 09:46:34.000000 thapbi_pict-1.0.0/database/README.rst
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4647 2023-04-06 15:07:11.000000 thapbi_pict-1.0.0/database/build_ITS1_DB.sh
--rw-r--r--   0 pcock    (896600025) pcock    (896600025)     1052 2020-01-27 13:54:30.000000 thapbi_pict-1.0.0/database/controls.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/database/single_isolates/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/2019-BL-1B_S117_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      832 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/2019-Pp2_S176_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      265 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      283 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/88069-P-infestans-56-A04_S4_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      294 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/P-foliorum-DNA-from-FR-81-D08_S44_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/P-foliorum_S165_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/Pd2c_S105_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/RG161_S139_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      291 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-390-1-or-2-P-lateralis-G07_S79_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      466 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      542 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1218_S174_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1750 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1220_S151_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1222_S187_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1226_S186_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP1227_S103_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      246 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP179-P-citrophthora-58-C05_S29_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1304 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP179_S177_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      583 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      289 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      274 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      278 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      531 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP390_S129_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      579 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1156 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      867 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP538-P-pseudotsugae-54-B04_S16_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      792 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      577 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP660_S153_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2645 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP722-P-kernoviae-84-dil-1-100-C09_S33_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP722_S141_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      582 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2045 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/SRCP1221_S175_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-1-A01_S1_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-1-E02_S50_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-2-B01_S13_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-2-F02_S62_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-2-F09_S69_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-3-C01_S25_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      565 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-3-G02_S74_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T-30-4-3-G09_S81_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      848 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/WL54_S128_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.0/database/single_isolates/WL77_S152_L001.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      539 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/endangered_species/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    52287 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/PRJEB18620.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      503 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_1.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_10.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_11.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_12.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_13.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_14.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_15.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_2.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_3.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_4.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_5.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_6.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_7.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      154 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_8.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      139 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/EM_9.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      200 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S1.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      257 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S10.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      207 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S2.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      203 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S4.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S5.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S6.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      256 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S7.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/expected/S9.template.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9016 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/metadata.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/endangered_species/raw_download/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    29160 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/raw_download/MD5SUM.txt
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/endangered_species/references/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      571 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/references/16S.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3551 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/references/ITS2.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3956 2023-04-06 15:07:13.000000 thapbi_pict-1.0.0/examples/endangered_species/references/Mini-16S.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2392 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/references/Mini-COI.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3356 2022-02-15 12:09:32.000000 thapbi_pict-1.0.0/examples/endangered_species/references/Mini-cyt-b.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5225 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/endangered_species/references/Mini-rbcL.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/endangered_species/references/cyt-b.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      157 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/endangered_species/references/rbcL.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/endangered_species/references/trnL-P6-loop.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2994 2023-04-06 15:07:13.000000 thapbi_pict-1.0.0/examples/endangered_species/references/trnL-UAA.fasta
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3880 2023-04-06 15:07:13.000000 thapbi_pict-1.0.0/examples/endangered_species/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2669 2023-04-06 15:07:13.000000 thapbi_pict-1.0.0/examples/endangered_species/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/fecal_sequel/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    17024 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/PRJNA574765.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      722 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2783 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/curated_bats.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1561 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/metadata.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      135 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/mock_community.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3600 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/observed_3_bats.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/fecal_sequel/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6840 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2229 2023-04-06 15:07:13.000000 thapbi_pict-1.0.0/examples/fecal_sequel/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1502 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fecal_sequel/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/fungal_mock/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7670 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/ITS1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11427 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/ITS2.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21115 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/PRJNA377530.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      368 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2873 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/metadata_AL1.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2433 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/metadata_AL2.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      439 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/mock_community.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/negative_control.known.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:55.000000 thapbi_pict-1.0.0/examples/fungal_mock/raw_data/
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/fungal_mock/raw_data/AL2/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3360 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/raw_data/AL2/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4025 2023-04-06 15:07:13.000000 thapbi_pict-1.0.0/examples/fungal_mock/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1602 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/fungal_mock/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:57.000000 thapbi_pict-1.0.0/examples/great_lakes/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70417 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/MOL16S.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5836 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/PRJNA379165.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      424 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    53173 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/SPH16S.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/great_lakes/expected/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/expected/mock_community.MOL16S.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      152 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/expected/mock_community.SPH16S.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/expected/negative_control.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1298 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/metadata.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/great_lakes/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2016 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3310 2023-04-06 15:07:13.000000 thapbi_pict-1.0.0/examples/great_lakes/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1974 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/great_lakes/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/recycled_water/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   201938 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/recycled_water/PRJNA417859.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/recycled_water/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   260627 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    48276 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2220 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/recycled_water/make_meta.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    19485 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/recycled_water/metadata.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/recycled_water/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    43008 2022-02-15 12:09:33.000000 thapbi_pict-1.0.0/examples/recycled_water/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1894 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/examples/recycled_water/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/recycled_water/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/soil_nematodes/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4498 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/soil_nematodes/PRJEB27581.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      500 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/soil_nematodes/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      594 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/soil_nematodes/metadata.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      499 2022-07-05 14:15:37.000000 thapbi_pict-1.0.0/examples/soil_nematodes/mock_community.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-07-05 14:15:37.000000 thapbi_pict-1.0.0/examples/soil_nematodes/negative_control.known.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/soil_nematodes/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1792 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/soil_nematodes/raw_data/MD5SUM.txt
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2883 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/examples/soil_nematodes/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2392 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/examples/soil_nematodes/setup.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/woody_hosts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/woody_hosts/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/examples/woody_hosts/expected/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/woody_hosts/expected/DNA10MIX_bycopynumber.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/woody_hosts/expected/DNA10MIX_diluted25x.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/woody_hosts/expected/DNA10MIX_undiluted.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      472 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/woody_hosts/expected/DNA15MIX.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3131 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/woody_hosts/metadata.tsv
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2007 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/examples/woody_hosts/run.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      348 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/examples/woody_hosts/setup.sh
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2023-05-19 09:46:34.000000 thapbi_pict-1.0.0/requirements-ext.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      347 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/requirements.txt
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:58.000000 thapbi_pict-1.0.0/scripts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      204 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/scripts/README.rst
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2394 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/scripts/blast_to_fasta.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3305 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/scripts/gg_to_sintax.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1003 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/scripts/make_nr.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      559 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/scripts/make_nr_ctrl_a.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1102 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/scripts/md5.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5549 2022-07-15 14:45:53.000000 thapbi_pict-1.0.0/scripts/missed_refs.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    16418 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/scripts/pooling.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    11772 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/scripts/rst_doc_test.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3629 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/scripts/sample_filter.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1107 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/scripts/swarm2usearch.py
--rwxr-xr-x   0 pcock    (896600025) pcock    (896600025)     1045 2022-10-25 13:52:24.000000 thapbi_pict-1.0.0/scripts/swarm_to_usearch.py
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3222 2023-04-06 15:07:14.000000 thapbi_pict-1.0.0/scripts/unknowns.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       38 2023-05-19 12:47:05.000000 thapbi_pict-1.0.0/setup.cfg
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4140 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/setup.py
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:59.000000 thapbi_pict-1.0.0/tests/
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:59.000000 thapbi_pict-1.0.0/tests/assess/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      325 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/ex1.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      400 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/ex1.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex1.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      258 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex1a.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex1a.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      380 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/ex2.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      369 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex2.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      151 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex2.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      321 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/ex3.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      234 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex3.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       71 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex3.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      383 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/ex4.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex4.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/ex4.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      319 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/fp.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/fp.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       74 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/fp.known.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      173 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/meta.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      638 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/samples.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      378 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/samples.confusion.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/samples.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2278 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/seven.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      195 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/assess/unclassified.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      214 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/unclassified.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       79 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/assess/unclassified.known.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:00.000000 thapbi_pict-1.0.0/tests/classifier/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      826 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2307 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2319 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2331 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2343 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1902 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2263 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2295 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1118 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4305 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4329 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4353 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4377 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3691 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4237 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4281 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      703 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      830 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/corner_cases_query.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary_query.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary_query.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary_query.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary_query.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      232 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary_query.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      382 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary_query.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classifier/genus_boundary_query.onebp.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/classify/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1548 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1614 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      124 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.meta.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1533 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1732 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.reads.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.samples.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.substr.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1244 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      210 2022-03-09 12:53:03.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-etc.meta.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5335 2022-03-09 12:53:03.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-etc.reads.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      962 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/classify/P-infestans-etc.samples.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4187 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/hmm_trim.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4199 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/hmm_trim.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3822 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/classify/hmm_trim.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3992 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/hmm_trim.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4172 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/hmm_trim.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3925 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/classify/hmm_trim.tally.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/conflicts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2137 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/conflicts/default.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      248 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/conflicts/dup_seqs.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/curated-import/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1135 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/curated-import/dup_seqs.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/edit-graph/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      619 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/edit-graph/DNAMIX_S95_L001.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3811 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/edit-graph/DNAMIX_S95_L001.xgmml
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/marker_clash/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2725 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2747 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2702 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.NotITS1.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2616 2022-02-15 12:09:34.000000 thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/marker_clash/Phytophthora_cinnamomi.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      600 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/marker_clash/conflicts.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      662 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/multi_marker/README.rst
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:46:55.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/16S/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/16S/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/ITS2/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/ITS2/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-16S/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      446 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-16S/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-COI/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      223 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-COI/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-cyt-b/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      569 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-rbcL/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      395 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-rbcL/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/rbcL/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/rbcL/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/trnL-P6-loop/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      302 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/trnL-P6-loop/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/trnL-UAA/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/multi_marker/intermediate/trnL-UAA/EM_1_sample.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/raw_data/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    35070 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    47717 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/multi_marker/summary/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1172 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/multi_marker/summary/pooled.reads.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      173 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/multi_marker/summary/pooled.samples.onebp.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:01.000000 thapbi_pict-1.0.0/tests/ncbi-import/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    62168 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/ncbi-import/20th_Century_ITS1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    76127 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1058 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/ncbi-import/hybrid.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5646 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/ncbi-import/multiple_hmm.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:02.000000 thapbi_pict-1.0.0/tests/nematodes/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1207 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/nematodes/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4660 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/nematodes/sample_R1.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6783 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/nematodes/sample_R2.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      483 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/nematodes/sample_flip_a10.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/nematodes/sample_noflip_a10.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:02.000000 thapbi_pict-1.0.0/tests/pipeline/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2567 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/pipeline/thapbi-pict.reads.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      926 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/pipeline/thapbi-pict.samples.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2113 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/pipeline/thapbi-pict.tally.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:02.000000 thapbi_pict-1.0.0/tests/pooling/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1722 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/pooling/example.pooled.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4999 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/pooling/example.samples.onebp.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:02.000000 thapbi_pict-1.0.0/tests/prepare-reads/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/prepare-reads/6e847180a4da6eed316e1fb98b21218f.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2613 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1911 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/prepare-reads/DNAMIX_S95_L001.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2021-04-07 19:03:04.000000 thapbi_pict-1.0.0/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      429 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/prepare-reads/SRR6303948_sample_default.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3434 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/prepare-reads/SRR6303948_sample_primers.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:02.000000 thapbi_pict-1.0.0/tests/read-correction/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2409 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/read-correction/AA.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/read-correction/AA.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      113 2023-04-06 15:07:15.000000 thapbi_pict-1.0.0/tests/read-correction/AA.usearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/AA.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/ACGT.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1043 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/ACGT.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      698 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/ACGT.usearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1158 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/ACGT.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      775 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Brassica.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Brassica.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Brassica.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4588 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Phytophthora_cinnamomi.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2664 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8036 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Rhabditis.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Rhabditis.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/Rhabditis.vsearch.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2476 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/chimeras.before.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2772 2023-02-08 13:36:24.000000 thapbi_pict-1.0.0/tests/read-correction/chimeras.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2253 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/chimeras.unoise.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2772 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/read-correction/chimeras.vsearch.fasta
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:03.000000 thapbi_pict-1.0.0/tests/reads/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq.md5
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   580693 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz.md5
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   679862 2020-09-11 17:49:04.000000 thapbi_pict-1.0.0/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/SRR6303948_sample_1.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/SRR6303948_sample_1.fastq.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/SRR6303948_sample_2.fastq
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/SRR6303948_sample_2.fastq.md5
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      812 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/ena_submit.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      878 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/ena_submit_custom.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      147 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/reads/metadata.tsv
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1908 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/run_tests.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:03.000000 thapbi_pict-1.0.0/tests/sample-tally/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1971 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/sample-tally/DNAMIX_S95_L001.tally.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:03.000000 thapbi_pict-1.0.0/tests/summary/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      550 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/summary/assess-meta.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.0/tests/summary/assess.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      434 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary/classify-meta-req.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      457 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary/classify-meta-req.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary/classify-meta-req.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary/classify-meta-req.swarm.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary/classify-meta-req.swarmid.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      838 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/summary/classify-meta.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      465 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/summary/classify-meta.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/summary/classify-meta.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary/classify-meta.swarm.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary/classify-meta.swarmid.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      738 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/summary/classify.blast.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      365 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/summary/classify.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      749 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/summary/classify.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      188 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary/classify.swarm.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary/classify.swarmid.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:04.000000 thapbi_pict-1.0.0/tests/summary_meta/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1456 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary_meta/A1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/A1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      823 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary_meta/A2.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      630 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/A2.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      674 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary_meta/B1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      666 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/B1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      677 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary_meta/B1r.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      667 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/B1r.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary_meta/C1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/C1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary_meta/X1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/X1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      385 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/summary_meta/Y1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      386 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/Y1.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      138 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/metadata.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2953 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/summary-q.reads.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2022-04-14 14:33:41.000000 thapbi_pict-1.0.0/tests/summary_meta/summary-q.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1021 2022-05-18 10:46:39.000000 thapbi_pict-1.0.0/tests/summary_meta/summary-qu.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1306 2022-05-18 10:46:39.000000 thapbi_pict-1.0.0/tests/summary_meta/summary-u.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3324 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/summary_meta/summary.reads.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1228 2022-04-14 14:33:42.000000 thapbi_pict-1.0.0/tests/summary_meta/summary.samples.1s3g.tsv
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:04.000000 thapbi_pict-1.0.0/tests/synthetic_controls/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11679 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2838 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10447 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9803 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/synthetic_controls/single-plate.ITS1.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10950 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-A.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11366 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-B.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12065 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-C.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12310 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-D.fasta
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3475 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/test_assess.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1240 2023-04-06 15:07:16.000000 thapbi_pict-1.0.0/tests/test_build_db.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4980 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_classify.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1106 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/test_conflicts.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6941 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_curated-import.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3681 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_denoise.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1636 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_dump.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2267 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_edit-graph.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/test_ena-submit.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      991 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_fasta-nr.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3155 2022-07-08 11:55:38.000000 thapbi_pict-1.0.0/tests/test_load-tax.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3297 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/test_marker_clash.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4096 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_multi_marker.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     9683 2022-07-08 11:55:38.000000 thapbi_pict-1.0.0/tests/test_ncbi-import.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4302 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_pipeline.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      872 2022-04-15 14:20:11.000000 thapbi_pict-1.0.0/tests/test_pooling.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4966 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_prepare-reads.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2263 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_sample-tally.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4890 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_summary.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6127 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_synthetic_controls.sh
--rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5659 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/test_woody_hosts.sh
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:04.000000 thapbi_pict-1.0.0/tests/woody_hosts/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1800 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/woody_hosts/DNA_MIXES.assess.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      681 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/woody_hosts/README.rst
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    26225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.0/tests/woody_hosts/all.fasta
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    59744 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/woody_hosts/all.identity.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    60810 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/woody_hosts/all.onebp.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    58076 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/woody_hosts/all.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    36279 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/tests/woody_hosts/denoise.tally.tsv
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10457 2022-02-15 12:09:37.000000 thapbi_pict-1.0.0/tests/woody_hosts/intermediate.tar.bz2
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:05.000000 thapbi_pict-1.0.0/thapbi_pict/
--rw-r--r--   0 pcock    (896600025) pcock    (896600025)  1445888 2023-05-19 12:43:57.000000 thapbi_pict-1.0.0/thapbi_pict/ITS1_DB.sqlite
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1031 2023-05-19 12:41:38.000000 thapbi_pict-1.0.0/thapbi_pict/__init__.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70600 2023-05-19 09:46:34.000000 thapbi_pict-1.0.0/thapbi_pict/__main__.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    24519 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/thapbi_pict/assess.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    30403 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/thapbi_pict/classify.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4186 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/thapbi_pict/conflicts.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    28994 2023-04-06 15:07:17.000000 thapbi_pict-1.0.0/thapbi_pict/db_import.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4854 2022-12-15 14:48:39.000000 thapbi_pict-1.0.0/thapbi_pict/db_orm.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    20741 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/denoise.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7725 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/dump.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    23538 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/edit_graph.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5997 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/ena_submit.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3031 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/fasta_nr.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    32329 2023-05-19 09:46:34.000000 thapbi_pict-1.0.0/thapbi_pict/prepare.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    20282 2023-04-28 12:36:14.000000 thapbi_pict-1.0.0/thapbi_pict/sample_tally.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    33294 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/summary.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    15147 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/taxdump.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    37237 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/utils.py
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5981 2023-04-06 15:07:18.000000 thapbi_pict-1.0.0/thapbi_pict/versions.py
-drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-05-19 12:47:05.000000 thapbi_pict-1.0.0/thapbi_pict.egg-info/
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8249 2023-05-19 12:46:54.000000 thapbi_pict-1.0.0/thapbi_pict.egg-info/PKG-INFO
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    20907 2023-05-19 12:46:55.000000 thapbi_pict-1.0.0/thapbi_pict.egg-info/SOURCES.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        1 2023-05-19 12:46:54.000000 thapbi_pict-1.0.0/thapbi_pict.egg-info/dependency_links.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       58 2023-05-19 12:46:54.000000 thapbi_pict-1.0.0/thapbi_pict.egg-info/entry_points.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      110 2023-05-19 12:46:54.000000 thapbi_pict-1.0.0/thapbi_pict.egg-info/requires.txt
--rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       12 2023-05-19 12:46:54.000000 thapbi_pict-1.0.0/thapbi_pict.egg-info/top_level.txt
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:33:00.947652 thapbi_pict-1.0.1/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      818 2022-02-15 12:09:29.000000 thapbi_pict-1.0.1/.flake8
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      883 2022-02-15 12:09:29.000000 thapbi_pict-1.0.1/.zenodo.json
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    13714 2023-07-26 11:31:51.000000 thapbi_pict-1.0.1/CHANGELOG.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5120 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2469 2023-05-19 09:46:34.000000 thapbi_pict-1.0.1/INSTALL.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1094 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/LICENSE.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4581 2023-04-06 15:07:11.000000 thapbi_pict-1.0.1/MANIFEST.in
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8184 2023-07-26 11:33:00.000000 thapbi_pict-1.0.1/PKG-INFO
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7001 2023-07-26 11:31:51.000000 thapbi_pict-1.0.1/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:42.000000 thapbi_pict-1.0.1/database/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    24077 2023-04-06 15:07:11.000000 thapbi_pict-1.0.1/database/2022-09-16_ITS1_Oomycota_obs.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1737519 2023-04-06 15:07:11.000000 thapbi_pict-1.0.1/database/2022-09-16_ITS1_Oomycota_w32.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   463737 2023-07-26 11:19:10.000000 thapbi_pict-1.0.1/database/ITS1_DB.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)  1035985 2023-07-26 11:19:11.000000 thapbi_pict-1.0.1/database/ITS1_DB.sql
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3890 2022-06-13 12:04:40.000000 thapbi_pict-1.0.1/database/Nothophytophthora_ITS1_curated.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    65170 2023-04-06 15:07:11.000000 thapbi_pict-1.0.1/database/Phytophthora_ITS1_curated.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3520 2023-05-19 09:46:34.000000 thapbi_pict-1.0.1/database/README.rst
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4647 2023-04-06 15:07:11.000000 thapbi_pict-1.0.1/database/build_ITS1_DB.sh
+-rw-r--r--   0 pcock    (896600025) pcock    (896600025)     1052 2020-01-27 13:54:30.000000 thapbi_pict-1.0.1/database/controls.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:44.000000 thapbi_pict-1.0.1/database/single_isolates/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/2019-BL-1B_S117_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      832 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/2019-Pp2_S176_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      265 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      283 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/88069-P-infestans-56-A04_S4_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      294 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/P-foliorum-DNA-from-FR-81-D08_S44_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/P-foliorum_S165_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/Pd2c_S105_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/RG161_S139_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      273 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      291 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-390-1-or-2-P-lateralis-G07_S79_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      466 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      271 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      542 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1218_S174_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1750 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1220_S151_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1222_S187_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1226_S186_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP1227_S103_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      246 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP179-P-citrophthora-58-C05_S29_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1304 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP179_S177_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      269 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      583 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      289 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      276 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      274 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      278 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      531 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP390_S129_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      579 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1156 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      867 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP538-P-pseudotsugae-54-B04_S16_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      279 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      792 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      577 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP660_S153_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2645 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        0 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP722-P-kernoviae-84-dil-1-100-C09_S33_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      264 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP722_S141_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      275 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      582 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      588 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2045 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/SRCP1221_S175_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-1-A01_S1_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-1-E02_S50_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-2-B01_S13_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-2-F02_S62_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-2-F09_S69_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-3-C01_S25_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      565 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-3-G02_S74_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      847 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T-30-4-3-G09_S81_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      848 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      877 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/WL54_S128_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      268 2022-02-15 12:09:30.000000 thapbi_pict-1.0.1/database/single_isolates/WL77_S152_L001.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:44.000000 thapbi_pict-1.0.1/examples/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      539 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:44.000000 thapbi_pict-1.0.1/examples/endangered_species/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    52287 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/PRJEB18620.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      503 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:46.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_1.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_10.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      270 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_11.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_12.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      146 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_13.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_14.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      167 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_15.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_2.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_3.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      108 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_4.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_5.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_6.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      159 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_7.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      154 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_8.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      139 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/EM_9.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      200 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S1.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      257 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S10.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      207 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S2.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      203 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S4.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S5.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S6.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      256 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S7.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      250 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/expected/S9.template.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9016 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/metadata.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:46.000000 thapbi_pict-1.0.1/examples/endangered_species/raw_download/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    29160 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/raw_download/MD5SUM.txt
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:46.000000 thapbi_pict-1.0.1/examples/endangered_species/references/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      571 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/references/16S.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3551 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/references/ITS2.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3956 2023-04-06 15:07:13.000000 thapbi_pict-1.0.1/examples/endangered_species/references/Mini-16S.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2392 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/references/Mini-COI.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3356 2022-02-15 12:09:32.000000 thapbi_pict-1.0.1/examples/endangered_species/references/Mini-cyt-b.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5225 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/endangered_species/references/Mini-rbcL.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/endangered_species/references/cyt-b.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      157 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/endangered_species/references/rbcL.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/endangered_species/references/trnL-P6-loop.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2994 2023-04-06 15:07:13.000000 thapbi_pict-1.0.1/examples/endangered_species/references/trnL-UAA.fasta
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3880 2023-04-06 15:07:13.000000 thapbi_pict-1.0.1/examples/endangered_species/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2669 2023-04-06 15:07:13.000000 thapbi_pict-1.0.1/examples/endangered_species/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:47.000000 thapbi_pict-1.0.1/examples/fecal_sequel/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    17024 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/PRJNA574765.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      722 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2783 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/curated_bats.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1561 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/metadata.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      135 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/mock_community.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3600 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/observed_3_bats.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:47.000000 thapbi_pict-1.0.1/examples/fecal_sequel/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6840 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2229 2023-04-06 15:07:13.000000 thapbi_pict-1.0.1/examples/fecal_sequel/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1502 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fecal_sequel/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:47.000000 thapbi_pict-1.0.1/examples/fungal_mock/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7670 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/ITS1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11427 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/ITS2.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21115 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/PRJNA377530.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      368 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2873 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/metadata_AL1.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2433 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/metadata_AL2.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      439 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/mock_community.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/negative_control.known.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:41.000000 thapbi_pict-1.0.1/examples/fungal_mock/raw_data/
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:47.000000 thapbi_pict-1.0.1/examples/fungal_mock/raw_data/AL2/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3360 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/raw_data/AL2/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4025 2023-04-06 15:07:13.000000 thapbi_pict-1.0.1/examples/fungal_mock/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1602 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/fungal_mock/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:48.000000 thapbi_pict-1.0.1/examples/great_lakes/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70417 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/MOL16S.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5836 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/PRJNA379165.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      424 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    53173 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/SPH16S.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:48.000000 thapbi_pict-1.0.1/examples/great_lakes/expected/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      282 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/expected/mock_community.MOL16S.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      152 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/expected/mock_community.SPH16S.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/expected/negative_control.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1298 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/metadata.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:48.000000 thapbi_pict-1.0.1/examples/great_lakes/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2016 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3310 2023-04-06 15:07:13.000000 thapbi_pict-1.0.1/examples/great_lakes/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1974 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/great_lakes/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:48.000000 thapbi_pict-1.0.1/examples/recycled_water/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   201938 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/recycled_water/PRJNA417859.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/recycled_water/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   260627 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    48276 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2220 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/recycled_water/make_meta.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    19485 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/recycled_water/metadata.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:48.000000 thapbi_pict-1.0.1/examples/recycled_water/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    43008 2022-02-15 12:09:33.000000 thapbi_pict-1.0.1/examples/recycled_water/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1894 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/examples/recycled_water/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1168 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/recycled_water/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:49.000000 thapbi_pict-1.0.1/examples/soil_nematodes/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4498 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/soil_nematodes/PRJEB27581.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      500 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/soil_nematodes/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      594 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/soil_nematodes/metadata.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      499 2022-07-05 14:15:37.000000 thapbi_pict-1.0.1/examples/soil_nematodes/mock_community.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       59 2022-07-05 14:15:37.000000 thapbi_pict-1.0.1/examples/soil_nematodes/negative_control.known.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:49.000000 thapbi_pict-1.0.1/examples/soil_nematodes/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1792 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/soil_nematodes/raw_data/MD5SUM.txt
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2883 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/examples/soil_nematodes/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2392 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/examples/soil_nematodes/setup.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:49.000000 thapbi_pict-1.0.1/examples/woody_hosts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      444 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/woody_hosts/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:49.000000 thapbi_pict-1.0.1/examples/woody_hosts/expected/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/woody_hosts/expected/DNA10MIX_bycopynumber.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/woody_hosts/expected/DNA10MIX_diluted25x.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/woody_hosts/expected/DNA10MIX_undiluted.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      472 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/woody_hosts/expected/DNA15MIX.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3131 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/examples/woody_hosts/metadata.tsv
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2007 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/examples/woody_hosts/run.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      381 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/examples/woody_hosts/setup.sh
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/requirements-ext.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      353 2023-06-02 14:20:09.000000 thapbi_pict-1.0.1/requirements.txt
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:50.000000 thapbi_pict-1.0.1/scripts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      204 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/scripts/README.rst
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2394 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/scripts/blast_to_fasta.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3305 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/scripts/gg_to_sintax.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1003 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/scripts/make_nr.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      559 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/scripts/make_nr_ctrl_a.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1102 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/scripts/md5.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5549 2022-07-15 14:45:53.000000 thapbi_pict-1.0.1/scripts/missed_refs.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     7693 2023-06-02 14:20:09.000000 thapbi_pict-1.0.1/scripts/plot_reduction.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    16418 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/scripts/pooling.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)    11772 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/scripts/rst_doc_test.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3629 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/scripts/sample_filter.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1107 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/scripts/swarm2usearch.py
+-rwxr-xr-x   0 pcock    (896600025) pcock    (896600025)     1045 2022-10-25 13:52:24.000000 thapbi_pict-1.0.1/scripts/swarm_to_usearch.py
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3222 2023-04-06 15:07:14.000000 thapbi_pict-1.0.1/scripts/unknowns.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       38 2023-07-26 11:33:00.000000 thapbi_pict-1.0.1/setup.cfg
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4040 2023-06-02 14:20:09.000000 thapbi_pict-1.0.1/setup.py
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:51.000000 thapbi_pict-1.0.1/tests/
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:52.000000 thapbi_pict-1.0.1/tests/assess/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      325 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/ex1.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      400 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/ex1.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex1.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      258 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex1a.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       32 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex1a.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      380 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/ex2.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      369 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex2.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      151 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex2.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      321 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/ex3.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      234 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex3.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       71 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex3.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      383 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/ex4.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      311 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex4.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      107 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/ex4.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      319 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/fp.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/fp.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       74 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/fp.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      173 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/meta.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      638 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/samples.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      378 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/samples.confusion.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/samples.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2278 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/seven.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      195 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/assess/unclassified.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      214 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/unclassified.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       79 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/assess/unclassified.known.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6757 2023-06-02 14:45:19.000000 thapbi_pict-1.0.1/tests/ceil-no-limit.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:53.000000 thapbi_pict-1.0.1/tests/classifier/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      826 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2307 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2319 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2331 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2343 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1902 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2263 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2295 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1118 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4305 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4329 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4353 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4377 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3691 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4237 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4281 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      703 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      830 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/corner_cases_query.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      587 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary_query.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary_query.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary_query.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary_query.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      232 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary_query.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      382 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary_query.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      396 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classifier/genus_boundary_query.onebp.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:53.000000 thapbi_pict-1.0.1/tests/classify/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1548 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1614 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      124 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.meta.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1533 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1732 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.reads.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.samples.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1371 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.substr.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1244 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      210 2022-03-09 12:53:03.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-etc.meta.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5335 2022-03-09 12:53:03.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-etc.reads.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      962 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/classify/P-infestans-etc.samples.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4187 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/hmm_trim.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4199 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/hmm_trim.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3822 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/classify/hmm_trim.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3992 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/hmm_trim.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4172 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/hmm_trim.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3925 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/classify/hmm_trim.tally.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:53.000000 thapbi_pict-1.0.1/tests/conflicts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2137 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/conflicts/default.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      248 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/conflicts/dup_seqs.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:53.000000 thapbi_pict-1.0.1/tests/curated-import/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1135 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/curated-import/dup_seqs.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:53.000000 thapbi_pict-1.0.1/tests/edit-graph/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      619 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/edit-graph/DNAMIX_S95_L001.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3811 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/edit-graph/DNAMIX_S95_L001.xgmml
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/marker_clash/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      601 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2725 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2835 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2747 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2702 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.NotITS1.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2616 2022-02-15 12:09:34.000000 thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      266 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/marker_clash/Phytophthora_cinnamomi.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      600 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/marker_clash/conflicts.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6865 2023-06-02 14:45:17.000000 thapbi_pict-1.0.1/tests/master.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      662 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/multi_marker/README.rst
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/16S/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/16S/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/ITS2/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      206 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/ITS2/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-16S/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      446 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-16S/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-COI/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      223 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-COI/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-cyt-b/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      569 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-rbcL/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      395 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-rbcL/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/rbcL/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/rbcL/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:54.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/trnL-P6-loop/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      302 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/trnL-P6-loop/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/trnL-UAA/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      211 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/multi_marker/intermediate/trnL-UAA/EM_1_sample.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/multi_marker/raw_data/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    35070 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    47717 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/multi_marker/summary/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1172 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/multi_marker/summary/pooled.reads.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      173 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/multi_marker/summary/pooled.samples.onebp.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/ncbi-import/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    62168 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/ncbi-import/20th_Century_ITS1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    76127 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1058 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/ncbi-import/hybrid.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5646 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/ncbi-import/multiple_hmm.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/nematodes/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1207 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/nematodes/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4660 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/nematodes/sample_R1.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     6783 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/nematodes/sample_R2.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      483 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/nematodes/sample_flip_a10.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      190 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/nematodes/sample_noflip_a10.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/pipeline/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2567 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/pipeline/thapbi-pict.reads.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      926 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/pipeline/thapbi-pict.samples.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2113 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/pipeline/thapbi-pict.tally.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/pooling/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1722 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/pooling/example.pooled.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4999 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/pooling/example.samples.onebp.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:55.000000 thapbi_pict-1.0.1/tests/prepare-reads/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      405 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/prepare-reads/6e847180a4da6eed316e1fb98b21218f.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2613 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1911 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/prepare-reads/DNAMIX_S95_L001.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2021-04-07 19:03:04.000000 thapbi_pict-1.0.1/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      429 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/prepare-reads/SRR6303948_sample_default.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3434 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/prepare-reads/SRR6303948_sample_primers.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:57.000000 thapbi_pict-1.0.1/tests/read-correction/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2409 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/read-correction/AA.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/read-correction/AA.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      113 2023-04-06 15:07:15.000000 thapbi_pict-1.0.1/tests/read-correction/AA.usearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      989 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/AA.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2541 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/ACGT.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1043 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/ACGT.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      698 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/ACGT.usearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1158 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/ACGT.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      775 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Brassica.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Brassica.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      389 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Brassica.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4588 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Phytophthora_cinnamomi.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      545 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2664 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8036 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Rhabditis.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Rhabditis.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4689 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/Rhabditis.vsearch.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2476 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/chimeras.before.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2772 2023-02-08 13:36:24.000000 thapbi_pict-1.0.1/tests/read-correction/chimeras.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2253 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/read-correction/chimeras.unoise.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2698 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/tests/read-correction/chimeras.vsearch.fasta
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:57.000000 thapbi_pict-1.0.1/tests/reads/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      561 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       76 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq.md5
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   580693 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz.md5
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)   679862 2020-09-11 17:49:04.000000 thapbi_pict-1.0.1/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       66 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/SRR6303948_sample_1.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/SRR6303948_sample_1.fastq.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)   126392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/SRR6303948_sample_2.fastq
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       60 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/SRR6303948_sample_2.fastq.md5
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      812 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/ena_submit.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      878 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/ena_submit_custom.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      147 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/reads/metadata.tsv
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1908 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/run_tests.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:57.000000 thapbi_pict-1.0.1/tests/sample-tally/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1971 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/sample-tally/DNAMIX_S95_L001.tally.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:58.000000 thapbi_pict-1.0.1/tests/summary/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      550 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/summary/assess-meta.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      392 2022-02-15 12:09:35.000000 thapbi_pict-1.0.1/tests/summary/assess.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      434 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary/classify-meta-req.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      457 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary/classify-meta-req.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      455 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary/classify-meta-req.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary/classify-meta-req.swarm.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary/classify-meta-req.swarmid.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      838 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/summary/classify-meta.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      465 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/summary/classify-meta.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      849 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/summary/classify-meta.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      284 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary/classify-meta.swarm.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      355 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary/classify-meta.swarmid.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      738 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/summary/classify.blast.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      365 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/summary/classify.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      749 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/summary/classify.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      188 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary/classify.swarm.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      259 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary/classify.swarmid.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:59.000000 thapbi_pict-1.0.1/tests/summary_meta/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1456 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary_meta/A1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1147 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/A1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      823 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary_meta/A2.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      630 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/A2.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      674 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary_meta/B1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      666 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/B1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      677 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary_meta/B1r.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      667 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/B1r.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary_meta/C1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/C1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      728 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary_meta/X1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      673 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/X1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      385 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/summary_meta/Y1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      386 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/Y1.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      138 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/metadata.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2953 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/summary-q.reads.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      947 2022-04-14 14:33:41.000000 thapbi_pict-1.0.1/tests/summary_meta/summary-q.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1021 2022-05-18 10:46:39.000000 thapbi_pict-1.0.1/tests/summary_meta/summary-qu.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1306 2022-05-18 10:46:39.000000 thapbi_pict-1.0.1/tests/summary_meta/summary-u.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3324 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/summary_meta/summary.reads.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1228 2022-04-14 14:33:42.000000 thapbi_pict-1.0.1/tests/summary_meta/summary.samples.1s3g.tsv
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:32:59.000000 thapbi_pict-1.0.1/tests/synthetic_controls/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11536 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11679 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     2838 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10447 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     9803 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/synthetic_controls/single-plate.ITS1.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10950 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-A.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    11366 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-B.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12065 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-C.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    12310 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-D.fasta
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3475 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/test_assess.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1240 2023-04-06 15:07:16.000000 thapbi_pict-1.0.1/tests/test_build_db.sh
+-rw-r--r--   0 pcock    (896600025) pcock    (896600025)   862238 2023-06-02 14:41:16.000000 thapbi_pict-1.0.1/tests/test_case2.fasta
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4980 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_classify.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1106 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/test_conflicts.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6941 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_curated-import.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3681 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_denoise.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1636 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_dump.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2267 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_edit-graph.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     1225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/test_ena-submit.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      991 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_fasta-nr.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3155 2022-07-08 11:55:38.000000 thapbi_pict-1.0.1/tests/test_load-tax.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     3297 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/test_marker_clash.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4096 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_multi_marker.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     9683 2022-07-08 11:55:38.000000 thapbi_pict-1.0.1/tests/test_ncbi-import.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4302 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_pipeline.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)      872 2022-04-15 14:20:11.000000 thapbi_pict-1.0.1/tests/test_pooling.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4966 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_prepare-reads.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     2263 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_sample-tally.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     4890 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_summary.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     6127 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_synthetic_controls.sh
+-rwxrwxr-x   0 pcock    (896600025) pcock    (896600025)     5659 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/test_woody_hosts.sh
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:33:00.000000 thapbi_pict-1.0.1/tests/woody_hosts/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1800 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/woody_hosts/DNA_MIXES.assess.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      681 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/woody_hosts/README.rst
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    26225 2022-02-15 12:09:36.000000 thapbi_pict-1.0.1/tests/woody_hosts/all.fasta
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    59744 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/woody_hosts/all.identity.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    60810 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/woody_hosts/all.onebp.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    58076 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/woody_hosts/all.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    36279 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/tests/woody_hosts/denoise.tally.tsv
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    10457 2022-02-15 12:09:37.000000 thapbi_pict-1.0.1/tests/woody_hosts/intermediate.tar.bz2
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:33:00.000000 thapbi_pict-1.0.1/thapbi_pict/
+-rw-r--r--   0 pcock    (896600025) pcock    (896600025)  1445888 2023-07-26 11:18:44.000000 thapbi_pict-1.0.1/thapbi_pict/ITS1_DB.sqlite
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     1031 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/thapbi_pict/__init__.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    70598 2023-06-02 14:20:09.000000 thapbi_pict-1.0.1/thapbi_pict/__main__.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    24519 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/thapbi_pict/assess.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    30403 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/thapbi_pict/classify.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4186 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/thapbi_pict/conflicts.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    28994 2023-04-06 15:07:17.000000 thapbi_pict-1.0.1/thapbi_pict/db_import.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     4854 2022-12-15 14:48:39.000000 thapbi_pict-1.0.1/thapbi_pict/db_orm.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21182 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/thapbi_pict/denoise.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     7725 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/dump.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    23538 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/edit_graph.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5997 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/ena_submit.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     3031 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/fasta_nr.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    32329 2023-05-19 09:46:34.000000 thapbi_pict-1.0.1/thapbi_pict/prepare.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21736 2023-07-26 11:16:38.000000 thapbi_pict-1.0.1/thapbi_pict/sample_tally.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    33294 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/summary.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    15147 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/taxdump.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    37237 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/utils.py
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     5981 2023-04-06 15:07:18.000000 thapbi_pict-1.0.1/thapbi_pict/versions.py
+drwxrwxr-x   0 pcock    (896600025) pcock    (896600025)        0 2023-07-26 11:33:00.000000 thapbi_pict-1.0.1/thapbi_pict.egg-info/
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)     8184 2023-07-26 11:32:40.000000 thapbi_pict-1.0.1/thapbi_pict.egg-info/PKG-INFO
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)    21001 2023-07-26 11:32:41.000000 thapbi_pict-1.0.1/thapbi_pict.egg-info/SOURCES.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)        1 2023-07-26 11:32:40.000000 thapbi_pict-1.0.1/thapbi_pict.egg-info/dependency_links.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       58 2023-07-26 11:32:40.000000 thapbi_pict-1.0.1/thapbi_pict.egg-info/entry_points.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)      110 2023-07-26 11:32:40.000000 thapbi_pict-1.0.1/thapbi_pict.egg-info/requires.txt
+-rw-rw-r--   0 pcock    (896600025) pcock    (896600025)       12 2023-07-26 11:32:40.000000 thapbi_pict-1.0.1/thapbi_pict.egg-info/top_level.txt
```

### Comparing `thapbi_pict-1.0.0/.flake8` & `thapbi_pict-1.0.1/.flake8`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/.zenodo.json` & `thapbi_pict-1.0.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/CHANGELOG.rst` & `thapbi_pict-1.0.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Release History
 ===============
 
 ======= ========== ============================================================================
 Version Date       Notes
 ======= ========== ============================================================================
+v1.0.1  2023-07-26 Fixed some rare corner-case read-corrections in ``unoise-l`` mode.
 v1.0.0  2023-05-19 Minor documentation changes, linked to Cock *et al.* (2023) preprint.
 v0.14.1 2023-03-13 Optional BIOM output using the ``biom-format`` Python library.
 v0.14.0 2023-03-02 Offers UNOISE read-correction, built-in or invoking USEARCH or VSEARCH.
 v0.13.6 2022-12-28 Factional abundance threshold in ``sample-tally`` was not strict enough.
 v0.13.5 2022-12-21 Misc small fixes and documentation updates.
 v0.13.4 2022-12-07 Support abundance thresholding in the ``sample-tally`` step. Log controls.
 v0.13.3 2022-11-25 Using new ``sample-tally`` command in pipeline, not ``fasta-nr``.
```

### Comparing `thapbi_pict-1.0.0/CONTRIBUTING.rst` & `thapbi_pict-1.0.1/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     $ cd database
     $ ./build_ITS1_DB.sh
     $ cd ..
     $ cp database/ITS1_DB.sqlite thapbi_pict/ITS1_DB.sqlite
     $ chmod a-w thapbi_pict/ITS1_DB.sqlite
 
-Assuming your default Python is at least version 3.6, to install the tool and
+Assuming your default Python is at least version 3.7, to install the tool and
 automatically get our Python dependencies:
 
 .. code:: console
 
     $ pip install .
 
 If your system defaults to Python 2, try ``pip3 install .`` or
```

### Comparing `thapbi_pict-1.0.0/INSTALL.rst` & `thapbi_pict-1.0.1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/LICENSE.rst` & `thapbi_pict-1.0.1/LICENSE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright 2018-2022, The James Hutton Institute, UK.
+Copyright 2018-2023, The James Hutton Institute, UK.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `thapbi_pict-1.0.0/MANIFEST.in` & `thapbi_pict-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/PKG-INFO` & `thapbi_pict-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thapbi_pict
-Version: 1.0.0
+Version: 1.0.1
 Summary: THAPBI Phytophthora ITS1 Classifier Tool (PICT).
 Home-page: https://github.com/peterjc/thapbi-pict
 Download-URL: https://github.com/peterjc/thapbi-pict
 Author: Peter Cock
 Author-email: peter.cock@hutton.ac.uk
 Project-URL: Documentation, https://thapbi-pict.readthedocs.io/
 Project-URL: Source, https://github.com/peterjc/thapbi-pict/
@@ -14,21 +14,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4529395.svg
    :alt: Zenodo DOI
    :target: https://doi.org/10.5281/zenodo.4529395
 .. image:: https://img.shields.io/github/license/peterjc/thapbi-pict.svg?label=License
@@ -133,17 +131,17 @@
 
 The documentation includes more detailed discussion of the sample datasets
 in the ``examples/`` folder (which are based on published datasets).
 
 Citation
 --------
 
-If you use THAPBI PICT in your work, please cite this manuscript (currently
-only available as a preprint), and give details of the version and any
-non-default settings used in your methods:
+If you use THAPBI PICT in your work, please cite this manuscript (to appear in
+the journal *PeerJ* but currently only available as a preprint), and give
+details of the version and any non-default settings used in your methods:
 
     Cock *et al.* (2023) "THAPBI PICT - a fast, cautious, and accurate
     metabarcoding analysis pipeline" *bioRxiv*
     https://doi.org/10.1101/2023.03.24.534090
 
 You can also cite the software specifically via Zenodo which offers version
 specific DOIs as well as https://doi.org/10.5281/zenodo.4529395 which is for
```

### Comparing `thapbi_pict-1.0.0/README.rst` & `thapbi_pict-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,17 @@
 
 The documentation includes more detailed discussion of the sample datasets
 in the ``examples/`` folder (which are based on published datasets).
 
 Citation
 --------
 
-If you use THAPBI PICT in your work, please cite this manuscript (currently
-only available as a preprint), and give details of the version and any
-non-default settings used in your methods:
+If you use THAPBI PICT in your work, please cite this manuscript (to appear in
+the journal *PeerJ* but currently only available as a preprint), and give
+details of the version and any non-default settings used in your methods:
 
     Cock *et al.* (2023) "THAPBI PICT - a fast, cautious, and accurate
     metabarcoding analysis pipeline" *bioRxiv*
     https://doi.org/10.1101/2023.03.24.534090
 
 You can also cite the software specifically via Zenodo which offers version
 specific DOIs as well as https://doi.org/10.5281/zenodo.4529395 which is for
```

### Comparing `thapbi_pict-1.0.0/database/2022-09-16_ITS1_Oomycota_obs.fasta` & `thapbi_pict-1.0.1/database/2022-09-16_ITS1_Oomycota_obs.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/2022-09-16_ITS1_Oomycota_w32.fasta` & `thapbi_pict-1.0.1/database/2022-09-16_ITS1_Oomycota_w32.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/ITS1_DB.fasta` & `thapbi_pict-1.0.1/database/ITS1_DB.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/ITS1_DB.sql` & `thapbi_pict-1.0.1/database/ITS1_DB.sql`

 * *Files 0% similar despite different names*

```diff
@@ -5,100 +5,100 @@
 	name VARCHAR(100), 
 	uri VARCHAR(200), 
 	md5 VARCHAR(32), 
 	notes VARCHAR(1000), 
 	PRIMARY KEY (id), 
 	UNIQUE (md5)
 );
-INSERT INTO data_source VALUES(1,'Import of controls.fasta','controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(83,'Import of 2022-09-16_ITS1_Oomycota_obs.fasta','2022-09-16_ITS1_Oomycota_obs.fasta','f63b69f776310b434e21248ca50963eb','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(84,'Import of 2022-09-16_ITS1_Oomycota_w32.fasta','2022-09-16_ITS1_Oomycota_w32.fasta','25b4cdf16f0e969575497273babdee09','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','c1c5fbc28b6082b829e54fb5f36d69b0','ITS1 imported with thapbi_pict v1.0.0');
+INSERT INTO data_source VALUES(1,'Import of controls.fasta','controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(83,'Import of 2022-09-16_ITS1_Oomycota_obs.fasta','2022-09-16_ITS1_Oomycota_obs.fasta','f63b69f776310b434e21248ca50963eb','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(84,'Import of 2022-09-16_ITS1_Oomycota_w32.fasta','2022-09-16_ITS1_Oomycota_w32.fasta','25b4cdf16f0e969575497273babdee09','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','c1c5fbc28b6082b829e54fb5f36d69b0','ITS1 imported with thapbi_pict v1.0.1');
 CREATE TABLE taxonomy (
 	id INTEGER NOT NULL, 
 	ncbi_taxid INTEGER, 
 	genus VARCHAR(100) NOT NULL, 
 	species VARCHAR(100) NOT NULL, 
 	PRIMARY KEY (id)
 );
```

### Comparing `thapbi_pict-1.0.0/database/Nothophytophthora_ITS1_curated.fasta` & `thapbi_pict-1.0.1/database/Nothophytophthora_ITS1_curated.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/Phytophthora_ITS1_curated.fasta` & `thapbi_pict-1.0.1/database/Phytophthora_ITS1_curated.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/README.rst` & `thapbi_pict-1.0.1/database/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/build_ITS1_DB.sh` & `thapbi_pict-1.0.1/database/build_ITS1_DB.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/controls.fasta` & `thapbi_pict-1.0.1/database/controls.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/2019-Pp2_S176_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/2019-Pp2_S176_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/RG161_S139_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/RG161_S139_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP10-P-aln-G06_S78_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP1218_S174_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP1218_S174_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP1220_S151_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP1220_S151_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP1222_S187_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP1222_S187_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP179_S177_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP179_S177_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP390_S129_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP390_S129_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SCRP9-P-aln-F06_S66_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/SRCP1221_S175_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/SRCP1221_S175_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T-30-4-1-A01_S1_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T-30-4-1-A01_S1_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T-30-4-2-B01_S13_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T-30-4-2-B01_S13_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T-30-4-2-F02_S62_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T-30-4-2-F02_S62_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T-30-4-2-F09_S69_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T-30-4-2-F09_S69_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T-30-4-3-C01_S25_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T-30-4-3-C01_S25_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T-30-4-3-G02_S74_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T-30-4-3-G02_S74_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T-30-4-3-G09_S81_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T-30-4-3-G09_S81_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/database/single_isolates/WL54_S128_L001.fasta` & `thapbi_pict-1.0.1/database/single_isolates/WL54_S128_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/README.rst` & `thapbi_pict-1.0.1/examples/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/PRJEB18620.tsv` & `thapbi_pict-1.0.1/examples/endangered_species/PRJEB18620.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/metadata.tsv` & `thapbi_pict-1.0.1/examples/endangered_species/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/raw_download/MD5SUM.txt` & `thapbi_pict-1.0.1/examples/endangered_species/raw_download/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/16S.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/ITS2.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/ITS2.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/Mini-16S.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/Mini-16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/Mini-COI.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/Mini-COI.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/Mini-cyt-b.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/Mini-cyt-b.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/Mini-rbcL.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/Mini-rbcL.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/trnL-P6-loop.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/trnL-P6-loop.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/references/trnL-UAA.fasta` & `thapbi_pict-1.0.1/examples/endangered_species/references/trnL-UAA.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/run.sh` & `thapbi_pict-1.0.1/examples/endangered_species/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/endangered_species/setup.sh` & `thapbi_pict-1.0.1/examples/endangered_species/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/PRJNA574765.tsv` & `thapbi_pict-1.0.1/examples/fecal_sequel/PRJNA574765.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/README.rst` & `thapbi_pict-1.0.1/examples/fecal_sequel/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/curated_bats.fasta` & `thapbi_pict-1.0.1/examples/fecal_sequel/curated_bats.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/metadata.tsv` & `thapbi_pict-1.0.1/examples/fecal_sequel/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/observed_3_bats.fasta` & `thapbi_pict-1.0.1/examples/fecal_sequel/observed_3_bats.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.1/examples/fecal_sequel/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/run.sh` & `thapbi_pict-1.0.1/examples/fecal_sequel/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fecal_sequel/setup.sh` & `thapbi_pict-1.0.1/examples/fecal_sequel/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/ITS1.fasta` & `thapbi_pict-1.0.1/examples/fungal_mock/ITS1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/ITS2.fasta` & `thapbi_pict-1.0.1/examples/fungal_mock/ITS2.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/PRJNA377530.tsv` & `thapbi_pict-1.0.1/examples/fungal_mock/PRJNA377530.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/metadata_AL1.tsv` & `thapbi_pict-1.0.1/examples/fungal_mock/metadata_AL1.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/metadata_AL2.tsv` & `thapbi_pict-1.0.1/examples/fungal_mock/metadata_AL2.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/raw_data/AL2/MD5SUM.txt` & `thapbi_pict-1.0.1/examples/fungal_mock/raw_data/AL2/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/run.sh` & `thapbi_pict-1.0.1/examples/fungal_mock/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/fungal_mock/setup.sh` & `thapbi_pict-1.0.1/examples/fungal_mock/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/great_lakes/MOL16S.fasta` & `thapbi_pict-1.0.1/examples/great_lakes/MOL16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/great_lakes/PRJNA379165.tsv` & `thapbi_pict-1.0.1/examples/great_lakes/PRJNA379165.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/great_lakes/SPH16S.fasta` & `thapbi_pict-1.0.1/examples/great_lakes/SPH16S.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/great_lakes/metadata.tsv` & `thapbi_pict-1.0.1/examples/great_lakes/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/great_lakes/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.1/examples/great_lakes/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/great_lakes/run.sh` & `thapbi_pict-1.0.1/examples/great_lakes/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/great_lakes/setup.sh` & `thapbi_pict-1.0.1/examples/great_lakes/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/PRJNA417859.tsv` & `thapbi_pict-1.0.1/examples/recycled_water/PRJNA417859.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta` & `thapbi_pict-1.0.1/examples/recycled_water/Redekar_et_al_2019_sup_table_3.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv` & `thapbi_pict-1.0.1/examples/recycled_water/Redekar_et_al_2019_sup_table_3.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/make_meta.py` & `thapbi_pict-1.0.1/examples/recycled_water/make_meta.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/metadata.tsv` & `thapbi_pict-1.0.1/examples/recycled_water/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.1/examples/recycled_water/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/run.sh` & `thapbi_pict-1.0.1/examples/recycled_water/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/recycled_water/setup.sh` & `thapbi_pict-1.0.1/examples/recycled_water/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/soil_nematodes/PRJEB27581.tsv` & `thapbi_pict-1.0.1/examples/soil_nematodes/PRJEB27581.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/soil_nematodes/metadata.tsv` & `thapbi_pict-1.0.1/examples/soil_nematodes/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/soil_nematodes/raw_data/MD5SUM.txt` & `thapbi_pict-1.0.1/examples/soil_nematodes/raw_data/MD5SUM.txt`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/soil_nematodes/run.sh` & `thapbi_pict-1.0.1/examples/soil_nematodes/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/soil_nematodes/setup.sh` & `thapbi_pict-1.0.1/examples/soil_nematodes/setup.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/woody_hosts/metadata.tsv` & `thapbi_pict-1.0.1/examples/woody_hosts/metadata.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/examples/woody_hosts/run.sh` & `thapbi_pict-1.0.1/examples/woody_hosts/run.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/blast_to_fasta.py` & `thapbi_pict-1.0.1/scripts/blast_to_fasta.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/gg_to_sintax.py` & `thapbi_pict-1.0.1/scripts/gg_to_sintax.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/make_nr.py` & `thapbi_pict-1.0.1/scripts/make_nr.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/make_nr_ctrl_a.py` & `thapbi_pict-1.0.1/scripts/make_nr_ctrl_a.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/md5.py` & `thapbi_pict-1.0.1/scripts/md5.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/missed_refs.py` & `thapbi_pict-1.0.1/scripts/missed_refs.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/pooling.py` & `thapbi_pict-1.0.1/scripts/pooling.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/rst_doc_test.py` & `thapbi_pict-1.0.1/scripts/rst_doc_test.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/sample_filter.py` & `thapbi_pict-1.0.1/scripts/sample_filter.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/swarm2usearch.py` & `thapbi_pict-1.0.1/scripts/swarm2usearch.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/swarm_to_usearch.py` & `thapbi_pict-1.0.1/scripts/swarm_to_usearch.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/scripts/unknowns.py` & `thapbi_pict-1.0.1/scripts/unknowns.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/setup.py` & `thapbi_pict-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018-2022 by Peter Cock, The James Hutton Institute.
+# Copyright 2018-2023 by Peter Cock, The James Hutton Institute.
 # All rights reserved.
 # This file is part of the THAPBI Phytophthora ITS1 Classifier Tool (PICT),
 # and is released under the "MIT License Agreement". Please see the LICENSE
 # file that should have been included as part of this package.
 """setuptools based setup script for THAPBI PICT.
 
 This uses setuptools which is now the standard python mechanism for installing
@@ -42,17 +42,17 @@
     sys.exit(
         "We need the Python library setuptools to be installed. "
         "Try running: python -m ensurepip"
     )
 
 
 # Make sure we have the right Python version.
-if sys.version_info[:2] < (3, 6):
+if sys.version_info[:2] < (3, 7):
     sys.exit(
-        "THAPBI PICT requires Python 3.6 or later. "
+        "THAPBI PICT requires Python 3.7 or later. "
         "Python %d.%d detected.\n" % sys.version_info[:2]
     )
 
 # We define the version number in thapbi_pict/__init__.py
 # Here we can't use "import thapbi_pict" then "thapbi_pict.__version__"
 # as that would tell us the version already installed (if any).
 __version__ = "Undefined"
@@ -92,22 +92,20 @@
         "Intended Audience :: Science/Research",
         "License :: Freely Distributable",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     entry_points={"console_scripts": ["thapbi_pict = thapbi_pict.__main__:main"]},
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "biopython",
         "cutadapt >=4.0",
         "matplotlib",
```

### Comparing `thapbi_pict-1.0.0/tests/assess/samples.assess.tsv` & `thapbi_pict-1.0.1/tests/assess/samples.assess.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/assess/seven.fasta` & `thapbi_pict-1.0.1/tests/assess/seven.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang.fasta` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s2g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s3g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s4g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.1s5g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.fasta` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.identity.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_bilorbang_query.onebp.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_bilorbang_query.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica.fasta` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s2g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s3g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s4g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.1s5g.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.fasta` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.identity.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/P_vulcanica_query.onebp.tsv` & `thapbi_pict-1.0.1/tests/classifier/P_vulcanica_query.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s2g.tsv` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s3g.tsv` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s4g.tsv` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.1s5g.tsv` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.blast.tsv` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.fasta` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.identity.tsv` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/corner_cases_query.onebp.tsv` & `thapbi_pict-1.0.1/tests/classifier/corner_cases_query.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classifier/genus_boundary.fasta` & `thapbi_pict-1.0.1/tests/classifier/genus_boundary.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.1s3g.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.blast.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.fasta` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.identity.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.onebp.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.reads.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.reads.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.substr.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.substr.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-T30-4.tally.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-T30-4.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-etc.reads.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-etc.reads.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/P-infestans-etc.samples.tsv` & `thapbi_pict-1.0.1/tests/classify/P-infestans-etc.samples.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/hmm_trim.1s3g.tsv` & `thapbi_pict-1.0.1/tests/classify/hmm_trim.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/hmm_trim.blast.tsv` & `thapbi_pict-1.0.1/tests/classify/hmm_trim.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/hmm_trim.fasta` & `thapbi_pict-1.0.1/tests/classify/hmm_trim.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/hmm_trim.identity.tsv` & `thapbi_pict-1.0.1/tests/classify/hmm_trim.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/hmm_trim.onebp.tsv` & `thapbi_pict-1.0.1/tests/classify/hmm_trim.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/classify/hmm_trim.tally.tsv` & `thapbi_pict-1.0.1/tests/classify/hmm_trim.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/conflicts/default.tsv` & `thapbi_pict-1.0.1/tests/conflicts/default.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/curated-import/dup_seqs.fasta` & `thapbi_pict-1.0.1/tests/curated-import/dup_seqs.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/edit-graph/DNAMIX_S95_L001.tsv` & `thapbi_pict-1.0.1/tests/edit-graph/DNAMIX_S95_L001.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/edit-graph/DNAMIX_S95_L001.xgmml` & `thapbi_pict-1.0.1/tests/edit-graph/DNAMIX_S95_L001.xgmml`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s2g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s4g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.1s5g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.ITS1.substr.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.NotITS1.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.NotITS1.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/GBLOCK-example.fasta` & `thapbi_pict-1.0.1/tests/marker_clash/GBLOCK-example.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/marker_clash/conflicts.tsv` & `thapbi_pict-1.0.1/tests/marker_clash/conflicts.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/multi_marker/README.rst` & `thapbi_pict-1.0.1/tests/multi_marker/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta` & `thapbi_pict-1.0.1/tests/multi_marker/intermediate/Mini-cyt-b/EM_1_sample.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz` & `thapbi_pict-1.0.1/tests/multi_marker/raw_data/EM_1_sample_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz` & `thapbi_pict-1.0.1/tests/multi_marker/raw_data/EM_1_sample_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/multi_marker/summary/pooled.reads.onebp.tsv` & `thapbi_pict-1.0.1/tests/multi_marker/summary/pooled.reads.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/ncbi-import/20th_Century_ITS1.fasta` & `thapbi_pict-1.0.1/tests/ncbi-import/20th_Century_ITS1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta` & `thapbi_pict-1.0.1/tests/ncbi-import/20th_Century_ITS1_Peronosporaceae.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/ncbi-import/hybrid.fasta` & `thapbi_pict-1.0.1/tests/ncbi-import/hybrid.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/ncbi-import/multiple_hmm.fasta` & `thapbi_pict-1.0.1/tests/ncbi-import/multiple_hmm.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/nematodes/README.rst` & `thapbi_pict-1.0.1/tests/nematodes/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/nematodes/sample_R1.fastq.gz` & `thapbi_pict-1.0.1/tests/nematodes/sample_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/nematodes/sample_R2.fastq.gz` & `thapbi_pict-1.0.1/tests/nematodes/sample_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/pipeline/thapbi-pict.reads.onebp.tsv` & `thapbi_pict-1.0.1/tests/pipeline/thapbi-pict.reads.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/pipeline/thapbi-pict.samples.onebp.tsv` & `thapbi_pict-1.0.1/tests/pipeline/thapbi-pict.samples.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/pipeline/thapbi-pict.tally.tsv` & `thapbi_pict-1.0.1/tests/pipeline/thapbi-pict.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/pooling/example.pooled.tsv` & `thapbi_pict-1.0.1/tests/pooling/example.pooled.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/pooling/example.samples.onebp.tsv` & `thapbi_pict-1.0.1/tests/pooling/example.samples.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta` & `thapbi_pict-1.0.1/tests/prepare-reads/DNAMIX_S95_L001-a2-head.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/prepare-reads/DNAMIX_S95_L001.fasta` & `thapbi_pict-1.0.1/tests/prepare-reads/DNAMIX_S95_L001.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv` & `thapbi_pict-1.0.1/tests/prepare-reads/DNAMIX_S95_L001.swarmid.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/prepare-reads/SRR6303948_sample_primers.fasta` & `thapbi_pict-1.0.1/tests/prepare-reads/SRR6303948_sample_primers.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/AA.before.fasta` & `thapbi_pict-1.0.1/tests/read-correction/AA.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/AA.unoise.fasta` & `thapbi_pict-1.0.1/tests/read-correction/AA.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/AA.vsearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/AA.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/ACGT.before.fasta` & `thapbi_pict-1.0.1/tests/read-correction/ACGT.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/ACGT.unoise.fasta` & `thapbi_pict-1.0.1/tests/read-correction/ACGT.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/ACGT.usearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/ACGT.usearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/ACGT.vsearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/ACGT.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Brassica.before.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Brassica.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Phytophthora_cinnamomi.before.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Phytophthora_cinnamomi.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Phytophthora_cinnamomi.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Phytophthora_cinnamomi.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.usearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Phytophthora_lacustris_vs_riparia.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Rhabditis.before.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Rhabditis.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Rhabditis.unoise.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Rhabditis.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/Rhabditis.vsearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/Rhabditis.vsearch.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/chimeras.before.fasta` & `thapbi_pict-1.0.1/tests/read-correction/chimeras.before.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/chimeras.fasta` & `thapbi_pict-1.0.1/tests/read-correction/chimeras.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/chimeras.unoise.fasta` & `thapbi_pict-1.0.1/tests/read-correction/chimeras.unoise.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/read-correction/chimeras.vsearch.fasta` & `thapbi_pict-1.0.1/tests/read-correction/chimeras.vsearch.fasta`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 TTTCCGTAGGTGAACCTGCGGAAGGATCATTACCACACCTAAAAAACTTTTCACGTGAACCGTATCAACCCTTTTAGTTGGGGGTCTTGCTTTTTTTGCGAGCCCTATCATGGCGAATGTTTGGACTTCGGTCTGGGCTAGTAGCTTTTTGTTTTAAACCCATTCTACAATACTGATTATACT
 >3d3fa2fd6fe0f183cad80771f5950b27_1362333
 TTTCCGTAGGTGAACCTGCGGAAGGATCATTACCACACCTAAAAAACTTTCCACGTGAACCGTATCAACCCATTTAGTTGGGGGCTTGTCCTGGTGGCTGGCTGTCGATGTCAAAGTTGACGGCTGCTGCTGTGTGGCGGGCCCTATCATGGCGAGCGTTTGGGTCCCTCTCGGGGGAACTGAGCCAGTAGCCCTTTTCTTTTAAACCCATTCTTGAATACTGAATATACT
 >dcd6316eb77be50ee344fbeca6e005c7_1148143
 TTTCCGTAGGTGAACCTGCGGAAGGATCATTACCACACCTAAAAAACTTTCCACGTGAACCGTATCAAAACCCTTAGTTGGGGGCTTCTGTTCGGCTGGCTTCGGCTGGCTGGGCGGCGGCTCTATCATGGCGAGCGCTTGAGCCTTCGGGTCTGAGCTAGTAGCCCACTTTTTAAACCCATTCCTAAATACTGAATATACT
 >d9e6de1308a8ac1448de351747d023c0_72646 chimera 972db44c016a166de86a2bacab3f4226/3d3fa2fd6fe0f183cad80771f5950b27
 TTTCCGTAGGTGAACCTGCGGAAGGATCATTACCACACCTAAAAAACTTTCCACGTGAACCGTATCAACCCACTTAGTTGGGGGCTAGTCCCGGCGGCTGGCTGTCGATGTCAAAGTTGACGGCTGCTGCTGTGTGGCGGGCCCTATCATGGCGAGCGTTTGGGTCCCTCTCGGGGGAACTGAGCCAGTAGCCCTTTTCTTTTAAACCCATTCTTGAATACTGAATATACT
->b5a466daa1cb779bb0d0dbfa39d49cb6_1617 chimera 6e847180a4da6eed316e1fb98b21218f/af3282a9797a70b6922e29e68c0b2bdc
+>b5a466daa1cb779bb0d0dbfa39d49cb6_1617
 TTTCCGTAGGTGAACCTGCGGAAGGATCATTACCACACCTAAAAAACTTTTCACGTGAACCGTATCAACCCTTTTAGTTGGGGGTCTTGCTTTTTTTGCGAGCCCTATCATGGCGAATGTTTGGACTTCGGTCTGGGCTAGTAGCTTTTTGTTTTAAACCCATTCCTAATTACTGAATATACT
 >0984333c38352fd1333ab5faf4c760ef_856 chimera 6e847180a4da6eed316e1fb98b21218f/af3282a9797a70b6922e29e68c0b2bdc
 TTTCCGTAGGTGAACCTGCGGAAGGATCATTACCACACCTAAAAAACTTTTCACGTGAACCGTATCAACCCTTTTAGTTGGGGGTCTTGCTTTTTTTGCGAGCCCTATCATGGCGAATGTTTGGACTTCGGTCTGGGCTAGTAGCGTATTTTTTAAACCCATTCCTAATTACTGAATATACT
 >3e602b47c64db19b5c4d8bdc29a833b1_667 chimera 32159de6cbb6df37d084e31c37c30e7b/dcd6316eb77be50ee344fbeca6e005c7
 TTTCCGTAGGTGAACCTGCGGAAGGATCATTACCACACCTAAAAAACTTTCCACGTGAACCGTATCAAAACCCTTTTATTGGGGGCTTCTGTCTGGTCTGGCTTCGGCTGGATTGGGTGGCGGCTCTATCATGGCGAGCGCTTGAGCCTTCGGGTCTGAGCTAGTAGCCCACTTTTTAAACCCATTCCTAAATACTGAATATACT
```

### Comparing `thapbi_pict-1.0.0/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq` & `thapbi_pict-1.0.1/tests/reads/6e847180a4da6eed316e1fb98b21218f_R1.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq` & `thapbi_pict-1.0.1/tests/reads/6e847180a4da6eed316e1fb98b21218f_R2.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz` & `thapbi_pict-1.0.1/tests/reads/DNAMIX_S95_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz` & `thapbi_pict-1.0.1/tests/reads/DNAMIX_S95_L001_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/reads/SRR6303948_sample_1.fastq` & `thapbi_pict-1.0.1/tests/reads/SRR6303948_sample_1.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/reads/SRR6303948_sample_2.fastq` & `thapbi_pict-1.0.1/tests/reads/SRR6303948_sample_2.fastq`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/reads/ena_submit.tsv` & `thapbi_pict-1.0.1/tests/reads/ena_submit.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/reads/ena_submit_custom.tsv` & `thapbi_pict-1.0.1/tests/reads/ena_submit_custom.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/run_tests.sh` & `thapbi_pict-1.0.1/tests/run_tests.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/sample-tally/DNAMIX_S95_L001.tally.tsv` & `thapbi_pict-1.0.1/tests/sample-tally/DNAMIX_S95_L001.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary/assess-meta.identity.tsv` & `thapbi_pict-1.0.1/tests/summary/assess-meta.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary/classify-meta.blast.tsv` & `thapbi_pict-1.0.1/tests/summary/classify-meta.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary/classify-meta.onebp.tsv` & `thapbi_pict-1.0.1/tests/summary/classify-meta.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary/classify.blast.tsv` & `thapbi_pict-1.0.1/tests/summary/classify.blast.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary/classify.onebp.tsv` & `thapbi_pict-1.0.1/tests/summary/classify.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/A1.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/A1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/A1.fasta` & `thapbi_pict-1.0.1/tests/summary_meta/A1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/A2.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/A2.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/A2.fasta` & `thapbi_pict-1.0.1/tests/summary_meta/A2.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/B1.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/B1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/B1.fasta` & `thapbi_pict-1.0.1/tests/summary_meta/B1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/B1r.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/B1r.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/B1r.fasta` & `thapbi_pict-1.0.1/tests/summary_meta/B1r.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/C1.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/C1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/C1.fasta` & `thapbi_pict-1.0.1/tests/summary_meta/C1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/X1.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/X1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/X1.fasta` & `thapbi_pict-1.0.1/tests/summary_meta/X1.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/summary-q.reads.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/summary-q.reads.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/summary-q.samples.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/summary-q.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/summary-qu.samples.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/summary-qu.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/summary-u.samples.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/summary-u.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/summary.reads.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/summary.reads.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/summary_meta/summary.samples.1s3g.tsv` & `thapbi_pict-1.0.1/tests/summary_meta/summary.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.1s3g.tsv` & `thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv` & `thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.reads.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv` & `thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.samples.1s3g.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/report.ITS1.tally.tsv` & `thapbi_pict-1.0.1/tests/synthetic_controls/report.ITS1.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/single-plate.ITS1.tally.tsv` & `thapbi_pict-1.0.1/tests/synthetic_controls/single-plate.ITS1.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-A.fasta` & `thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-A.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-B.fasta` & `thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-B.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-C.fasta` & `thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-C.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/synthetic_controls/spike-in-D.fasta` & `thapbi_pict-1.0.1/tests/synthetic_controls/spike-in-D.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_assess.sh` & `thapbi_pict-1.0.1/tests/test_assess.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_build_db.sh` & `thapbi_pict-1.0.1/tests/test_build_db.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_classify.sh` & `thapbi_pict-1.0.1/tests/test_classify.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_conflicts.sh` & `thapbi_pict-1.0.1/tests/test_conflicts.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_curated-import.sh` & `thapbi_pict-1.0.1/tests/test_curated-import.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_denoise.sh` & `thapbi_pict-1.0.1/tests/test_denoise.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_dump.sh` & `thapbi_pict-1.0.1/tests/test_dump.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_edit-graph.sh` & `thapbi_pict-1.0.1/tests/test_edit-graph.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_ena-submit.sh` & `thapbi_pict-1.0.1/tests/test_ena-submit.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_fasta-nr.sh` & `thapbi_pict-1.0.1/tests/test_fasta-nr.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_load-tax.sh` & `thapbi_pict-1.0.1/tests/test_load-tax.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_marker_clash.sh` & `thapbi_pict-1.0.1/tests/test_marker_clash.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_multi_marker.sh` & `thapbi_pict-1.0.1/tests/test_multi_marker.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_ncbi-import.sh` & `thapbi_pict-1.0.1/tests/test_ncbi-import.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_pipeline.sh` & `thapbi_pict-1.0.1/tests/test_pipeline.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_pooling.sh` & `thapbi_pict-1.0.1/tests/test_pooling.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_prepare-reads.sh` & `thapbi_pict-1.0.1/tests/test_prepare-reads.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_sample-tally.sh` & `thapbi_pict-1.0.1/tests/test_sample-tally.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_summary.sh` & `thapbi_pict-1.0.1/tests/test_summary.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_synthetic_controls.sh` & `thapbi_pict-1.0.1/tests/test_synthetic_controls.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/test_woody_hosts.sh` & `thapbi_pict-1.0.1/tests/test_woody_hosts.sh`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/DNA_MIXES.assess.tsv` & `thapbi_pict-1.0.1/tests/woody_hosts/DNA_MIXES.assess.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/README.rst` & `thapbi_pict-1.0.1/tests/woody_hosts/README.rst`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/all.fasta` & `thapbi_pict-1.0.1/tests/woody_hosts/all.fasta`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/all.identity.tsv` & `thapbi_pict-1.0.1/tests/woody_hosts/all.identity.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/all.onebp.tsv` & `thapbi_pict-1.0.1/tests/woody_hosts/all.onebp.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/all.tally.tsv` & `thapbi_pict-1.0.1/tests/woody_hosts/all.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/denoise.tally.tsv` & `thapbi_pict-1.0.1/tests/woody_hosts/denoise.tally.tsv`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/tests/woody_hosts/intermediate.tar.bz2` & `thapbi_pict-1.0.1/tests/woody_hosts/intermediate.tar.bz2`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/ITS1_DB.sqlite` & `thapbi_pict-1.0.1/thapbi_pict/ITS1_DB.sqlite`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -5,100 +5,100 @@
 	name VARCHAR(100), 
 	uri VARCHAR(200), 
 	md5 VARCHAR(32), 
 	notes VARCHAR(1000), 
 	PRIMARY KEY (id), 
 	UNIQUE (md5)
 );
-INSERT INTO data_source VALUES(1,'Import of controls.fasta','controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(83,'Import of 2022-09-16_ITS1_Oomycota_obs.fasta','2022-09-16_ITS1_Oomycota_obs.fasta','f63b69f776310b434e21248ca50963eb','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(84,'Import of 2022-09-16_ITS1_Oomycota_w32.fasta','2022-09-16_ITS1_Oomycota_w32.fasta','25b4cdf16f0e969575497273babdee09','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.0');
-INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','c1c5fbc28b6082b829e54fb5f36d69b0','ITS1 imported with thapbi_pict v1.0.0');
+INSERT INTO data_source VALUES(1,'Import of controls.fasta','controls.fasta','edb7776a3eb1b0bf999aca6cc8069ea0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(2,'Import of 2019-BL-1B_S117_L001.fasta','single_isolates/2019-BL-1B_S117_L001.fasta','410868d1b3a20dae9588e2dec224d35d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(3,'Import of 2019-Pp2_S176_L001.fasta','single_isolates/2019-Pp2_S176_L001.fasta','635eba28bca958be156600f5a76fa130','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(4,'Import of 75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','single_isolates/75-BT3-1gDNA-P-austrocedrae-F08_S68_L001.fasta','b9d033fb512a938bbd43a9d37a02617a','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(5,'Import of 76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','single_isolates/76-GA3-1gDNA-P-austrocedrae-G08_S80_L001.fasta','a0f23279ec301b6e24fbd917bca8f9d2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(6,'Import of 78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','single_isolates/78-CPB-DNA-from-FR-dil-1-100-P-obscura-H08_S92_L001.fasta','24e99e17cc8762f1f3a3be3b70ab8251','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(7,'Import of 88069-P-infestans-56-A04_S4_L001.fasta','single_isolates/88069-P-infestans-56-A04_S4_L001.fasta','0c3feb4c0fe4dbcee2a8211e45c88c0b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(8,'Import of P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','single_isolates/P-Europaea-DNA-from-FR-dil-1-100-F07_S67_L001.fasta','be94bad04e61973e3cedafcbee01049c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(9,'Import of P-cinnamomi-82-1-10-A07_S7_L001.fasta','single_isolates/P-cinnamomi-82-1-10-A07_S7_L001.fasta','e908d7662bf813cbbd1579bab316a2cc','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(10,'Import of P-foliorum_S165_L001.fasta','single_isolates/P-foliorum_S165_L001.fasta','ef558628310ffd3f7ab3b453456817f1','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(11,'Import of Pd2c_S105_L001.fasta','single_isolates/Pd2c_S105_L001.fasta','48cd9b09775236178a0e605caa41bd7c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(12,'Import of RG161_S139_L001.fasta','single_isolates/RG161_S139_L001.fasta','ce517ab8e7df28177f0d0d3f158c5306','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(13,'Import of SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-C03_S27_L001.fasta','f8969263fa5826630533a64c813e2622','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(14,'Import of SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-1-G01_S73_L001.fasta','46ad4dde36e46288c54f50aa539aac1f','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(15,'Import of SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D03_S39_L001.fasta','3713ec1a19429c90b78022103c55b4e2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(16,'Import of SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-D10_S46_L001.fasta','868c7b450a4c7bc23654eb5c3887518b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(17,'Import of SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-2-H01_S85_L001.fasta','2af51b23a7044a5bac99cbc22d2f69a5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(18,'Import of SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-A02_S2_L001.fasta','542a75fb4f1200fb53f85b8295721ced','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(19,'Import of SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E03_S51_L001.fasta','a11ec91a4bb7ab5783f89cdacb64acc5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(20,'Import of SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','single_isolates/SCRP-1161-P-austrocedrae-3-E10_S58_L001.fasta','7f77d2ca72611ab2fbc097df1ebf0498','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(21,'Import of SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','single_isolates/SCRP-1163-P-gonapodyides-C06_S30_L001.fasta','e3becd9bca1b9dae7d64b57bac23d5f2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(22,'Import of SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','single_isolates/SCRP-1170-P-Erythroseptica-B08_S20_L001.fasta','ab5969cfa74cbdfae2e8709c6e8a1db2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(23,'Import of SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','single_isolates/SCRP-1171-P-Erythroseptica-C08_S32_L001.fasta','5e4b1918da6bddba2762de9d43d42229','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(24,'Import of SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','single_isolates/SCRP-1197-P-nicotianae-50-or-51-C04_S28_L001.fasta','0930f783ab98db5c23d4258a638b238f','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(25,'Import of SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-D01_S37_L001.fasta','2cccb1400e24c869165229914a18c522','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(26,'Import of SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-1-H02_S86_L001.fasta','52691ec02b9f2c0e06aba8e34def7dae','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(27,'Import of SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A03_S3_L001.fasta','4a9fee9d3ea2d3e6fee66422dea7bb1a','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(28,'Import of SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-A10_S10_L001.fasta','fdf9cbab00b6ef0f2c1e49899c933c5e','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(29,'Import of SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-2-E01_S49_L001.fasta','c5b212be82d798ce53d8e8abf866c6a8','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(30,'Import of SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B03_S15_L001.fasta','85a836986733ee22e41de822b4e53a09','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(31,'Import of SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-B10_S22_L001.fasta','66dc12b09af8d0ab08b974b6c52956bf','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(32,'Import of SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','single_isolates/SCRP-734-P-pseudosyringae-3-F01_S61_L001.fasta','ee1d2a67f92a04c637636511acc02ab0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(33,'Import of SCRP10-P-aln-G06_S78_L001.fasta','single_isolates/SCRP10-P-aln-G06_S78_L001.fasta','f8f27981a37a487e1519569b4e435b60','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(34,'Import of SCRP1022-P-capsici-40-B05_S17_L001.fasta','single_isolates/SCRP1022-P-capsici-40-B05_S17_L001.fasta','de4e34757e41d78cd06e0971ec4f5f48','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(35,'Import of SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','single_isolates/SCRP1161-P-austrocedrae-1-20-1-C10_S34_L001.fasta','08c99d3effea5a8d7bd23ed7042c27d1','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(36,'Import of SCRP1162-P-austrocedrae-E08_S56_L001.fasta','single_isolates/SCRP1162-P-austrocedrae-E08_S56_L001.fasta','c4bb3e46150402c1e226f0a1905ea1a4','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(37,'Import of SCRP1218_S174_L001.fasta','single_isolates/SCRP1218_S174_L001.fasta','40c5346460c7092a496554815167bc0a','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(38,'Import of SCRP1220_S151_L001.fasta','single_isolates/SCRP1220_S151_L001.fasta','20457e003ea03927c65e4a502da9910e','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(39,'Import of SCRP1222_S187_L001.fasta','single_isolates/SCRP1222_S187_L001.fasta','3250d35908ce49b9ec60660f6c170c33','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(40,'Import of SCRP1226_S186_L001.fasta','single_isolates/SCRP1226_S186_L001.fasta','d29f93bed44dbc54d419e9601a31ef0c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(41,'Import of SCRP1227_S103_L001.fasta','single_isolates/SCRP1227_S103_L001.fasta','e60694b4ef3d691de374936234e377f0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(42,'Import of SCRP165-P-citricola-T-60-D05_S41_L001.fasta','single_isolates/SCRP165-P-citricola-T-60-D05_S41_L001.fasta','3879365d7d1df03d7196fa2decaa68f2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(43,'Import of SCRP179_S177_L001.fasta','single_isolates/SCRP179_S177_L001.fasta','f658223ca78a1d1f1013abcc387f9b00','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(44,'Import of SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','single_isolates/SCRP207-P-Cryptogea-72-or-73-A08_S8_L001.fasta','5a677701dd0859de85bf4b312334ff9b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(45,'Import of SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','single_isolates/SCRP23-P-boehmeriae-1-B09_S21_L001.fasta','e0717d26d51db4824192dd5efca69f4d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(46,'Import of SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','single_isolates/SCRP231-P-cajani-71-1-10-C07_S31_L001.fasta','51feea1bd7f7ad00bfa1ba1511adb456','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(47,'Import of SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','single_isolates/SCRP333-P-rubi-race-3-45-E07_S55_L001.fasta','e5cb0b82772fa9c9eaad1c47316bee02','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(48,'Import of SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','single_isolates/SCRP35-1-or-2-P-cactorum-CAC17-R222-E04_S52_L001.fasta','f3a196ad5363cb2c98aa6957d6883ac7','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(49,'Import of SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','single_isolates/SCRP37-P-cactorum-CAC19-145H-F04_S64_L001.fasta','2ef825ce0e519fa051c3188aa22828a7','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(50,'Import of SCRP371-P-idaei-41-A05_S5_L001.fasta','single_isolates/SCRP371-P-idaei-41-A05_S5_L001.fasta','bd71cd2dc3f11e28bf1f60a06377b35b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(51,'Import of SCRP372-P-idaei-47-H04_S88_L001.fasta','single_isolates/SCRP372-P-idaei-47-H04_S88_L001.fasta','c5ffdbf050c1bea2f9e054bbd35d4cbc','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(52,'Import of SCRP377-P-ilicis-62-E05_S53_L001.fasta','single_isolates/SCRP377-P-ilicis-62-E05_S53_L001.fasta','aa05088fdddbcdef3efa42d63b8f762c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(53,'Import of SCRP386-P-iranica-48-D04_S40_L001.fasta','single_isolates/SCRP386-P-iranica-48-D04_S40_L001.fasta','d057c13577581d15d1071c1791406044','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(54,'Import of SCRP388-P-castaneae-44-H05_S89_L001.fasta','single_isolates/SCRP388-P-castaneae-44-H05_S89_L001.fasta','73903eca1d478b0ef7af0f34c3bb55ac','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(55,'Import of SCRP390_S129_L001.fasta','single_isolates/SCRP390_S129_L001.fasta','9311bd8dea14d0d9937bfa6e9866e25e','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(56,'Import of SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','single_isolates/SCRP417-1-OR-2-P-megasperma-B06_S18_L001.fasta','c0a24e66621635578470beb91eced8ff','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(57,'Import of SCRP420-P-megasperma-66-A06_S6_L001.fasta','single_isolates/SCRP420-P-megasperma-66-A06_S6_L001.fasta','5acf6c06b4d62f75a6e123db53a6296c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(58,'Import of SCRP455-P-melonis-70-B07_S19_L001.fasta','single_isolates/SCRP455-P-melonis-70-B07_S19_L001.fasta','4b0bf6de70eb3d7f579886718b79c628','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(59,'Import of SCRP474-P-palmivora-11-F05_S65_L001.fasta','single_isolates/SCRP474-P-palmivora-11-F05_S65_L001.fasta','3befac09d8878973c82e7eb44fcfa3d0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(60,'Import of SCRP526-P-palmivora-64A-G05_S77_L001.fasta','single_isolates/SCRP526-P-palmivora-64A-G05_S77_L001.fasta','f8ca44626ff7db82d9058334cbc24cea','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(61,'Import of SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','single_isolates/SCRP56-P-cactorum-CH97-46-G04_S76_L001.fasta','eb4672cd94ded5acded4804cb58fac98','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(62,'Import of SCRP607-P-fallax-12-A09_S9_L001.fasta','single_isolates/SCRP607-P-fallax-12-A09_S9_L001.fasta','eee190f0dcd5ef525330aa6749178139','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(63,'Import of SCRP645-P-inundata-68-D06_S42_L001.fasta','single_isolates/SCRP645-P-inundata-68-D06_S42_L001.fasta','c3fb81d5717bde4e7c02724b14aa91b5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(64,'Import of SCRP660-P-syringae-83-H07_S91_L001.fasta','single_isolates/SCRP660-P-syringae-83-H07_S91_L001.fasta','0d64fab90e2d9adb856694021488ccb0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(65,'Import of SCRP660_S153_L001.fasta','single_isolates/SCRP660_S153_L001.fasta','f3d25ef3e862f31f1f8db427c41a14a2','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(66,'Import of SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','single_isolates/SCRP71-P-cambivora-69-cam5-H06_S90_L001.fasta','c5dc489ab31a75f6c71f358693c6f7e5','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(67,'Import of SCRP722_S141_L001.fasta','single_isolates/SCRP722_S141_L001.fasta','4c872ee9200a34b28e7875ead4824085','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(68,'Import of SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','single_isolates/SCRP734-1-or-2-P-pseudosyringae-1-H09_S93_L001.fasta','74999328eb896c5a45fc0312555198cb','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(69,'Import of SCRP893-P-sojae-22-D07_S43_L001.fasta','single_isolates/SCRP893-P-sojae-22-D07_S43_L001.fasta','6fa60abf7f948991beb77b07ee6c2d83','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(70,'Import of SCRP9-P-aln-F06_S66_L001.fasta','single_isolates/SCRP9-P-aln-F06_S66_L001.fasta','c75bffcc1dbe0796d93ce8a94260e480','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(71,'Import of SRCP1221_S175_L001.fasta','single_isolates/SRCP1221_S175_L001.fasta','54911ef6e9117cbbd553c59aa227bc33','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(72,'Import of T-30-4-1-A01_S1_L001.fasta','single_isolates/T-30-4-1-A01_S1_L001.fasta','80c04900062c2ba8e982b2fb637f51f3','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(73,'Import of T-30-4-1-E02_S50_L001.fasta','single_isolates/T-30-4-1-E02_S50_L001.fasta','34c531f18befe1491edcbc07ec012e4d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(74,'Import of T-30-4-2-B01_S13_L001.fasta','single_isolates/T-30-4-2-B01_S13_L001.fasta','f9fc3f1112d2884a014b3ffdc2aa30da','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(75,'Import of T-30-4-2-F02_S62_L001.fasta','single_isolates/T-30-4-2-F02_S62_L001.fasta','8adbc9331abd7ee1773c7e0d3f905be9','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(76,'Import of T-30-4-2-F09_S69_L001.fasta','single_isolates/T-30-4-2-F09_S69_L001.fasta','83a1a21c498a999507a8ec35c86417b0','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(77,'Import of T-30-4-3-C01_S25_L001.fasta','single_isolates/T-30-4-3-C01_S25_L001.fasta','f6e61f47db1ba63aecc7d0734931542b','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(78,'Import of T-30-4-3-G02_S74_L001.fasta','single_isolates/T-30-4-3-G02_S74_L001.fasta','491646427d79cb86f4e5197e3e4708da','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(79,'Import of T-30-4-3-G09_S81_L001.fasta','single_isolates/T-30-4-3-G09_S81_L001.fasta','de47994e2847642ce2f866cc7effe56d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(80,'Import of T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','single_isolates/T30-4-P-infestans-55-1-20-1-E09_S57_L001.fasta','f5a8a74f793605f8ae25dd951a6fb5e9','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(81,'Import of WL54_S128_L001.fasta','single_isolates/WL54_S128_L001.fasta','23ea6eb01b59cb5325acfc772383f218','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(82,'Import of WL77_S152_L001.fasta','single_isolates/WL77_S152_L001.fasta','8793ff33cef54442371a8943b666df7c','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(83,'Import of 2022-09-16_ITS1_Oomycota_obs.fasta','2022-09-16_ITS1_Oomycota_obs.fasta','f63b69f776310b434e21248ca50963eb','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(84,'Import of 2022-09-16_ITS1_Oomycota_w32.fasta','2022-09-16_ITS1_Oomycota_w32.fasta','25b4cdf16f0e969575497273babdee09','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(85,'Import of Nothophytophthora_ITS1_curated.fasta','Nothophytophthora_ITS1_curated.fasta','a8ce79c75a0e7cf55d5c32322c75789d','ITS1 imported with thapbi_pict v1.0.1');
+INSERT INTO data_source VALUES(86,'Import of Phytophthora_ITS1_curated.fasta','Phytophthora_ITS1_curated.fasta','c1c5fbc28b6082b829e54fb5f36d69b0','ITS1 imported with thapbi_pict v1.0.1');
 CREATE TABLE taxonomy (
 	id INTEGER NOT NULL, 
 	ncbi_taxid INTEGER, 
 	genus VARCHAR(100) NOT NULL, 
 	species VARCHAR(100) NOT NULL, 
 	PRIMARY KEY (id)
 );
```

### Comparing `thapbi_pict-1.0.0/thapbi_pict/__init__.py` & `thapbi_pict-1.0.1/thapbi_pict/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 The `tool documentation <https://thapbi-pict.readthedocs.io/>`_ is
 hosted by `Read The Docs <https://readthedocs.org/>`_, generated
 automatically from the ``docs/`` folder of the `software repository
 <https://github.com/peterjc/thapbi-pict/>`_ and the *"docstrings"*
 within the source code which document the Python API.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `thapbi_pict-1.0.0/thapbi_pict/__main__.py` & `thapbi_pict-1.0.1/thapbi_pict/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1576,15 +1576,15 @@
         help="Minimum total abundance for sequences. "
         "Applied after per-sample thresholds. Default 0 (not used).",
     )
     subcommand_parser.add_argument("--minlen", **ARG_MIN_LENGTH)
     subcommand_parser.add_argument("--maxlen", **ARG_MAX_LENGTH)
     subcommand_parser.add_argument("--denoise", **ARG_DENOISE)
     subcommand_parser.add_argument("-α", "--unoise_alpha", **ARG_UNOISE_ALPHA)
-    subcommand_parser.add_argument("-𝛾", "--unoise_gamma", **ARG_UNOISE_GAMMA)
+    subcommand_parser.add_argument("-γ", "--unoise_gamma", **ARG_UNOISE_GAMMA)
     subcommand_parser.add_argument("--temp", **ARG_TEMPDIR)
     subcommand_parser.add_argument("--cpu", **ARG_CPU)
     subcommand_parser.add_argument("-v", "--verbose", **ARG_VERBOSE)
     subcommand_parser.set_defaults(func=sample_tally)
 
     # classify
     subcommand_parser = subparsers.add_parser(
```

### Comparing `thapbi_pict-1.0.0/thapbi_pict/assess.py` & `thapbi_pict-1.0.1/thapbi_pict/assess.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/classify.py` & `thapbi_pict-1.0.1/thapbi_pict/classify.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/conflicts.py` & `thapbi_pict-1.0.1/thapbi_pict/conflicts.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/db_import.py` & `thapbi_pict-1.0.1/thapbi_pict/db_import.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/db_orm.py` & `thapbi_pict-1.0.1/thapbi_pict/db_orm.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/denoise.py` & `thapbi_pict-1.0.1/thapbi_pict/denoise.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
             # Don't need to calculate all the distances:
             for choice, dist, _index in extract_iter(
                 query,
                 high_abundance_centroids,
                 scorer=Levenshtein.distance,
                 score_cutoff=cutoff,
             ):
+                # UNOISE merges query into centroid if skew(M,C) <= beta(d),
+                #   (query abundance) / (centroid abundance) <= 1 / 2**(alpha*dist +1)
+                #   (query abundance) * 2**(alpha*dist + 1) <= centroid abundance
                 if a * 2 ** (unoise_alpha * dist + 1) <= counts[choice]:
                     centroids[choice].add(query)
                     if debug:
                         sys.stderr.write(
                             f"DEBUG: unoise-agc C:{md5seq(choice)}_{counts[choice]} "
                             f"<-- Q:{md5seq(query)}_{a} dist {dist}\n"
                         )
@@ -111,14 +114,15 @@
                 [
                     (dist, choice)
                     for (choice, dist, _index) in extract(
                         query,
                         high_abundance_centroids,
                         scorer=Levenshtein.distance,
                         score_cutoff=cutoff,
+                        limit=None,
                     )
                     if a * 2 ** (unoise_alpha * dist + 1) <= counts[choice]
                 ],
                 key=lambda x: (x[0], counts[x[1]], x[1]),
             )
             if candidates:
                 if debug:
@@ -166,15 +170,14 @@
 
     Assumes v10 or v11 (or later if the command line API is the same).
     Parses the four columns tabbed output.
 
     Returns a dict mapping input sequences to centroid sequences, and a dict
     of MD5 checksums of any sequences flagged as chimeras.
     """
-    debug = True
     check_tools(["usearch"], debug)
 
     if tmp_dir:
         # Up to the user to remove the files
         tmp_obj = None
         shared_tmp = tmp_dir
     else:
@@ -430,14 +433,18 @@
     abundance_based=False,
     tmp_dir=None,
     debug=False,
     cpu=0,
 ):
     """Apply builtin UNOISE algorithm or invoke an external tool like VSEARCH.
 
+    Argument algorithm is a string, "unoise-l" for our reimplementation of the
+    UNOISE2 algorithm, or "usearch" or "vsearch" to invoke those tools at the
+    command line.
+
     Argument counts is an (unsorted) dict of sequences (for the same amplicon
     marker) as keys, with their total abundance counts as values.
 
     Returns a dict mapping input sequences to centroid sequences, and dict of
     any chimeras detected (empty for some algorithms).
     """
     start = time()
```

### Comparing `thapbi_pict-1.0.0/thapbi_pict/dump.py` & `thapbi_pict-1.0.1/thapbi_pict/dump.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/edit_graph.py` & `thapbi_pict-1.0.1/thapbi_pict/edit_graph.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/ena_submit.py` & `thapbi_pict-1.0.1/thapbi_pict/ena_submit.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/fasta_nr.py` & `thapbi_pict-1.0.1/thapbi_pict/fasta_nr.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/prepare.py` & `thapbi_pict-1.0.1/thapbi_pict/prepare.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/sample_tally.py` & `thapbi_pict-1.0.1/thapbi_pict/sample_tally.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 import gzip
 import os
 import sys
 from collections import Counter
 from collections import defaultdict
 from math import ceil
+from time import time
 
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 
 from .denoise import read_correction
 from .prepare import load_fasta_header
 from .prepare import load_marker_defs
 from .utils import abundance_from_read_name
@@ -48,16 +49,17 @@
     cpu=0,
 ):
     """Implement the ``thapbi_pict sample-tally`` command.
 
     Arguments min_length and max_length are applied while loading the input
     per-sample FASTA files.
 
-    Set argument denoise=True for our reimplementation of the UNOISE2 read
-    correction / denoising algorithm.
+    Argument algorithm is a string, "-" for no read correction (denoising),
+    "unoise-l" for our reimplementation of the UNOISE2 algorithm, or "usearch"
+    or "vsearch" to invoke those tools at the command line.
 
     Arguments min_abundance and min_abundance_fraction are applied per-sample
     (after denoising if being used), increased by pool if negative or
     synthetic controls are given respectively. Comma separated string argument
     spike_genus is treated case insensitively.
     """
     if isinstance(inputs, str):
@@ -100,15 +102,14 @@
         spikes = marker_def["spike_kmers"]
         del marker_def
     del marker_definitions
     assert marker
 
     totals = Counter()
     counts = Counter()
-    sample_counts = Counter()
     sample_cutadapt = {}  # before any thresholds
     samples = set()
     sample_pool = {}
     sample_headers = {}
     for filename in inputs:
         # Assuming FASTA for now
         if debug:
@@ -138,28 +139,29 @@
         with open(filename) as handle:
             for _, seq in SimpleFastaParser(handle):
                 seq = seq.upper()
                 if min_length <= len(seq) <= max_length:
                     a = abundance_from_read_name(_.split(None, 1)[0])
                     totals[seq] += a
                     counts[seq, sample] += a
-                    sample_counts[sample] += a
 
     if totals:
         sys.stderr.write(
             f"Loaded {len(totals)} unique sequences from {sum(totals.values())}"
             f" in total within length range, max abundance {max(totals.values())}\n"
         )
     else:
         sys.stderr.write("WARNING: Loaded zero sequences within length range\n")
 
     chimeras = {}
     if denoise_algorithm != "-":
         if debug:
-            f"DEBUG: Starting read-correction with {denoise_algorithm}...\n"
+            sys.stderr.write(
+                f"DEBUG: Starting read-correction with {denoise_algorithm}...\n"
+            )
         corrections, chimeras = read_correction(
             denoise_algorithm,
             totals,
             unoise_alpha=unoise_alpha,
             unoise_gamma=unoise_gamma,
             tmp_dir=tmp_dir,
             debug=debug,
@@ -189,17 +191,20 @@
             )
         counts = new_counts
         totals = new_totals
         del new_totals, new_counts, corrections
 
     # Drop entries so low in abundance that they'll never be accepted, nor
     # increase the pool threshold. Drop before bothering to check if spikes.
-    # Note factor of 0.5 due to heuristic below for threshold adjustment.
+    # Note factor of 0.5 due to heuristic below for threshold adjustment
+    # (things slightly below the absolute threshold might still contribut to
+    # raising the max non-spike in counts and this the automatic fractional
+    # threshold)
     ultra_low = ceil(0.5 * min_abundance)
-    if ultra_low:
+    if ultra_low > 1:
         if debug:
             sys.stderr.write("DEBUG: Dropping ultra low abundance entries\n")
         new_counts = defaultdict(int)
         new_totals = defaultdict(int)
         before = len(totals)
         del totals
         while counts:
@@ -218,39 +223,53 @@
         del new_totals, new_counts
 
     pool_absolute_threshold = {}
     pool_fraction_threshold = {}
     max_spike_abundance = {sample: 0 for sample in samples}  # exporting in metadata
     max_non_spike_abundance = {sample: 0 for sample in samples}  # exporting in metadata
     if spikes:
+        if debug:
+            sys.stderr.write(
+                "DEBUG: About to identify spike-in synthetic sequences...\n"
+            )
+        start = time()
         for seq in totals:
             # Calling is_spike_in is relatively expensive, but will be of less
             # interest on the tail end low abundance samples.
             # Should we sort totals by count?
             assert totals[seq] >= ultra_low, seq
+            if totals[seq] < min(max_spike_abundance.values()) and totals[seq] < min(
+                max_non_spike_abundance.values()
+            ):
+                # Note counts[seq, sample] <= totals[seq] so will not be able to exceed
+                continue
             if any(
                 min(max_spike_abundance[sample], max_non_spike_abundance[sample])
                 < counts[seq, sample]
                 for sample in samples
             ):
                 # This could raise the max (non-)spike-in abundance
                 if is_spike_in(seq, spikes):
                     for sample in samples:
                         if max_spike_abundance[sample] < counts[seq, sample]:
                             max_spike_abundance[sample] = counts[seq, sample]
                 else:
                     for sample in samples:
                         if max_non_spike_abundance[sample] < counts[seq, sample]:
                             max_non_spike_abundance[sample] = counts[seq, sample]
+        time_spike_tagging = time() - start
+        if debug:
+            sys.stderr.write(
+                f"DEBUG: Spent {time_spike_tagging:0.1f}s tagging spike-in sequences.\n"
+            )
     else:
         for (_, sample), a in counts.items():
             max_non_spike_abundance[sample] = max(max_non_spike_abundance[sample], a)
-    if debug:
-        sys.stderr.write("DEBUG: Finished tagging spike-in sequences.\n")
 
+    start = time()
     sample_threshold = {}
     if controls:
         if debug:
             sys.stderr.write("DEBUG: Applying dynamic abundance thresholds...\n")
         for sample in controls:
             pool = sample_pool[sample]
             a = max_non_spike_abundance[sample]
@@ -329,18 +348,20 @@
             int(sample_headers[sample].get("threshold", 0)),
             pool_absolute_threshold.get(pool, min_abundance),
             ceil(
                 sample_cutadapt[sample]
                 * pool_fraction_threshold.get(pool, min_abundance_fraction)
             ),
         )
-        if debug:
+        if debug and not controls:
             sys.stderr.write(
                 f"DEBUG: {sample} in pool {pool} gets threshold {threshold}\n"
             )
+    del pool_absolute_threshold
+    del pool_fraction_threshold
 
     new_counts = defaultdict(int)
     new_totals = defaultdict(int)
     before = len(totals)
     del totals
     while counts:
         (seq, sample), a = counts.popitem()
@@ -367,14 +388,20 @@
             f"Total abundance threshold {total_min_abundance} reduced unique "
             f"ASVs from {len(totals)} to {len(new_totals)}.\n"
         )
         counts = new_counts
         totals = new_totals
         del new_totals, new_counts
 
+    if debug:
+        time_thresholds = time() - start
+        sys.stderr.write(
+            f"DEBUG: Spent {time_thresholds:0.1f}s on abundance thresholds\n"
+        )
+
     if chimeras:
         # Filter the chimeras list to drop low abundance entries
         # Would be better to call VSEARCH chimera detection here?
         chimeras = {
             md5seq(seq): chimeras[md5seq(seq)]
             for seq in totals
             if md5seq(seq) in chimeras
@@ -396,27 +423,31 @@
     values = sorted(
         ((count, seq) for seq, count in totals.items()),
         # (sort by marker), then put the highest abundance entries first:
         key=lambda x: (-x[0], x[1]),
     )
     del totals
 
+    if debug:
+        sys.stderr.write("DEBUG: Sorted, about to start output...\n")
+
     # TODO - avoid double definition here and in summary code:
     stats_fields = (
         "Raw FASTQ",
         "Flash",
         "Cutadapt",
         "Threshold pool",
         "Threshold",
         "Control",
         "Max non-spike",
         "Max spike-in",
         "Singletons",
     )
 
+    start = time()
     if output == "-":
         if fasta == "-":
             sys.exit("ERROR: Don't use stdout for both TSV and FASTA output.")
         if gzipped:
             raise ValueError("Does not support gzipped output to stdout.")
         out_handle = sys.stdout
     elif gzipped:
@@ -498,15 +529,17 @@
     elif fasta and gzipped:
         fasta_handle = gzip.open(fasta, "wt")
     elif fasta:
         fasta_handle = open(fasta, "w")
     else:
         fasta_handle = None
     for count, seq in values:
-        data = "\t".join(str(counts[seq, sample]) for sample in samples)
+        # This is the last time we'll use the counts[seq, *] values,
+        # so use pop to gradually reduce the data held in memory.
+        data = "\t".join(str(counts.pop((seq, sample), 0)) for sample in samples)
         md5 = md5seq(seq)
         if md5 in chimeras:
             out_handle.write(
                 f"{marker}/{md5}_{count}\t{data}\t{seq}\t{chimeras[md5]}\n"
             )
         elif chimeras:
             # Empty field
@@ -522,7 +555,10 @@
                 fasta_handle.write(f">{md5}_{count} chimera {chimeras[md5]}\n{seq}\n")
             else:
                 fasta_handle.write(f">{md5}_{count}\n{seq}\n")
     if output != "-":
         out_handle.close()
     if fasta and fasta != "-":
         fasta_handle.close()
+    if debug:
+        time_output = time() - start
+        sys.stderr.write(f"DEBUG: Spent {time_output:0.1f}s writing output files\n")
```

### Comparing `thapbi_pict-1.0.0/thapbi_pict/summary.py` & `thapbi_pict-1.0.1/thapbi_pict/summary.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/taxdump.py` & `thapbi_pict-1.0.1/thapbi_pict/taxdump.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/utils.py` & `thapbi_pict-1.0.1/thapbi_pict/utils.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict/versions.py` & `thapbi_pict-1.0.1/thapbi_pict/versions.py`

 * *Files identical despite different names*

### Comparing `thapbi_pict-1.0.0/thapbi_pict.egg-info/PKG-INFO` & `thapbi_pict-1.0.1/thapbi_pict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thapbi-pict
-Version: 1.0.0
+Version: 1.0.1
 Summary: THAPBI Phytophthora ITS1 Classifier Tool (PICT).
 Home-page: https://github.com/peterjc/thapbi-pict
 Download-URL: https://github.com/peterjc/thapbi-pict
 Author: Peter Cock
 Author-email: peter.cock@hutton.ac.uk
 Project-URL: Documentation, https://thapbi-pict.readthedocs.io/
 Project-URL: Source, https://github.com/peterjc/thapbi-pict/
@@ -14,21 +14,19 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4529395.svg
    :alt: Zenodo DOI
    :target: https://doi.org/10.5281/zenodo.4529395
 .. image:: https://img.shields.io/github/license/peterjc/thapbi-pict.svg?label=License
@@ -133,17 +131,17 @@
 
 The documentation includes more detailed discussion of the sample datasets
 in the ``examples/`` folder (which are based on published datasets).
 
 Citation
 --------
 
-If you use THAPBI PICT in your work, please cite this manuscript (currently
-only available as a preprint), and give details of the version and any
-non-default settings used in your methods:
+If you use THAPBI PICT in your work, please cite this manuscript (to appear in
+the journal *PeerJ* but currently only available as a preprint), and give
+details of the version and any non-default settings used in your methods:
 
     Cock *et al.* (2023) "THAPBI PICT - a fast, cautious, and accurate
     metabarcoding analysis pipeline" *bioRxiv*
     https://doi.org/10.1101/2023.03.24.534090
 
 You can also cite the software specifically via Zenodo which offers version
 specific DOIs as well as https://doi.org/10.5281/zenodo.4529395 which is for
```

### Comparing `thapbi_pict-1.0.0/thapbi_pict.egg-info/SOURCES.txt` & `thapbi_pict-1.0.1/thapbi_pict.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -203,23 +203,27 @@
 scripts/README.rst
 scripts/blast_to_fasta.py
 scripts/gg_to_sintax.py
 scripts/make_nr.py
 scripts/make_nr_ctrl_a.py
 scripts/md5.py
 scripts/missed_refs.py
+scripts/plot_reduction.py
 scripts/pooling.py
 scripts/rst_doc_test.py
 scripts/sample_filter.py
 scripts/swarm2usearch.py
 scripts/swarm_to_usearch.py
 scripts/unknowns.py
+tests/ceil-no-limit.fasta
+tests/master.fasta
 tests/run_tests.sh
 tests/test_assess.sh
 tests/test_build_db.sh
+tests/test_case2.fasta
 tests/test_classify.sh
 tests/test_conflicts.sh
 tests/test_curated-import.sh
 tests/test_denoise.sh
 tests/test_dump.sh
 tests/test_edit-graph.sh
 tests/test_ena-submit.sh
```

