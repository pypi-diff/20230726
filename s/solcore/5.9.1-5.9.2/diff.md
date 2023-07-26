# Comparing `tmp/solcore-5.9.1.tar.gz` & `tmp/solcore-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solcore-5.9.1.tar", last modified: Sat Feb 18 00:22:51 2023, max compression
+gzip compressed data, was "solcore-5.9.2.tar", last modified: Wed Jul 26 06:55:39 2023, max compression
```

## Comparing `solcore-5.9.1.tar` & `solcore-5.9.2.tar`

### file list

```diff
@@ -1,767 +1,779 @@
--rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 solcore-5.9.1/.all-contributorsrc
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 solcore-5.9.1/.devpy/cmds.py
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 solcore-5.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 solcore-5.9.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 solcore-5.9.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     4193 1970-01-01 00:00:00.000000 solcore-5.9.1/.github/workflows/build_deploy_wheels.yml
--rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 solcore-5.9.1/.github/workflows/test_unit_and_examples.yml
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 solcore-5.9.1/.gitignore
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 solcore-5.9.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0    11819 1970-01-01 00:00:00.000000 solcore-5.9.1/CHANGELOG.rst
--rwxr-xr-x   0        0        0     3215 1970-01-01 00:00:00.000000 solcore-5.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    10266 1970-01-01 00:00:00.000000 solcore-5.9.1/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     7651 1970-01-01 00:00:00.000000 solcore-5.9.1/GNU-LGPL.txt
--rwxr-xr-x   0        0        0      987 1970-01-01 00:00:00.000000 solcore-5.9.1/LICENSE.txt
--rw-r--r--   0        0        0    15488 1970-01-01 00:00:00.000000 solcore-5.9.1/README.md
--rw-r--r--   0        0        0       16 1970-01-01 00:00:00.000000 solcore-5.9.1/binder/apt.txt
--rw-r--r--   0        0        0       83 1970-01-01 00:00:00.000000 solcore-5.9.1/binder/postBuild
--rw-r--r--   0        0        0       68 1970-01-01 00:00:00.000000 solcore-5.9.1/binder/requirements.txt
--rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 solcore-5.9.1/build_tools/cibw_before_build_macos_arm.sh
--rw-r--r--   0        0        0      279 1970-01-01 00:00:00.000000 solcore-5.9.1/build_tools/x86_64-w64-arm64.ini
--rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/.nojekyll
--rwxr-xr-x   0        0        0     7057 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/Makefile
--rwxr-xr-x   0        0        0     6990 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/make.bat
--rw-r--r--   0        0        0    46736 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/Ag_GaAs_abs.png
--rw-r--r--   0        0        0    41012 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/Ag_k.png
--rw-r--r--   0        0        0    39380 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/Ag_n.png
--rwxr-xr-x   0        0        0    26706 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/DA_iv.png
--rwxr-xr-x   0        0        0   230604 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/DA_iv2.png
--rwxr-xr-x   0        0        0    31223 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/DA_qe.png
--rw-r--r--   0        0        0    20539 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/Diamond_nk.png
--rwxr-xr-x   0        0        0    21653 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/IV_param_dispersion.png
--rwxr-xr-x   0        0        0    16932 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/IV_solar_module.png
--rwxr-xr-x   0        0        0    24785 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/MJ_IV_optimal.png
--rwxr-xr-x   0        0        0    31579 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/MJ_efficiency_map.png
--rwxr-xr-x   0        0        0    59203 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/MJ_with_rad_coupling.png
--rwxr-xr-x   0        0        0   133711 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/MQW_LDOS.png
--rwxr-xr-x   0        0        0    24594 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/PDD_IV.png
--rwxr-xr-x   0        0        0    29250 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/PDD_carrier_density.png
--rwxr-xr-x   0        0        0    23275 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/PDD_qe.png
--rwxr-xr-x   0        0        0    82016 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/RAT_of_ARC.png
--rw-r--r--   0        0        0    18901 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/SiGeSn_nk.png
--rwxr-xr-x   0        0        0    71549 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/Single_QW.png
--rwxr-xr-x   0        0        0    14165 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/circular_mask_IV.png
--rwxr-xr-x   0        0        0    15138 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/circular_mask_V1_3.png
--rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/custom_materials_example.rst
--rwxr-xr-x   0        0        0    26589 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/eff_mass_fit.png
--rwxr-xr-x   0        0        0     5883 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_3J_with_DA_solver.rst
--rwxr-xr-x   0        0        0     1936 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_K_and_effective_mass.rst
--rwxr-xr-x   0        0        0     3305 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_MJ_efficiency_map.rst
--rwxr-xr-x   0        0        0     4056 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_PDD_solver.rst
--rwxr-xr-x   0        0        0     1771 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_QWs.rst
--rwxr-xr-x   0        0        0     2756 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_RAT_of_ARC.rst
--rwxr-xr-x   0        0        0     1780 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_light_sources.rst
--rw-r--r--   0        0        0     7098 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_optics_comparison.rst
--rwxr-xr-x   0        0        0     2157 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_pv_module.rst
--rwxr-xr-x   0        0        0     3574 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_quasi3D_cell.rst
--rwxr-xr-x   0        0        0     4345 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_radiative_coupling.rst
--rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_substrate.rst
--rwxr-xr-x   0        0        0     1333 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/example_tunnel_junction.rst
--rwxr-xr-x   0        0        0    27377 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/iv.jpg
--rwxr-xr-x   0        0        0    60710 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/iv_params.jpg
--rwxr-xr-x   0        0        0    19120 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/kp.png
--rwxr-xr-x   0        0        0    67440 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/ls_compare.png
--rwxr-xr-x   0        0        0    91514 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/ls_smarts.png
--rwxr-xr-x   0        0        0     1789 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/main.rst
--rw-r--r--   0        0        0   241086 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/optmodelcomp.png
--rwxr-xr-x   0        0        0    48407 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/qe.jpg
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/refractiveindex_info_db_example.rst
--rwxr-xr-x   0        0        0    14175 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/square_mask_IV.png
--rwxr-xr-x   0        0        0    10565 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/square_mask_V1_3.png
--rw-r--r--   0        0        0    41375 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/substrate_Adepth.png
--rw-r--r--   0        0        0    38834 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/substrate_RAT.png
--rwxr-xr-x   0        0        0    35316 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/tunnel_junction.png
--rwxr-xr-x   0        0        0    14884 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Examples/tutorial.rst
--rwxr-xr-x   0        0        0   196433 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Infographics.jpg
--rwxr-xr-x   0        0        0      987 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Installation/Solcore_on_MacOSX.md
--rwxr-xr-x   0        0        0     6255 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Installation/Solcore_on_Windows.md
--rwxr-xr-x   0        0        0     2400 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Installation/compilation.md
--rwxr-xr-x   0        0        0     8821 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Installation/installation.rst
--rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Installation/s4_installation.md
--rwxr-xr-x   0        0        0     8458 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Optics/material_optics.rst
--rwxr-xr-x   0        0        0      446 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Optics/optics.rst
--rwxr-xr-x   0        0        0      575 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Optics/other_methods.rst
--rwxr-xr-x   0        0        0    63532 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Optics/qw_absorption.png
--rwxr-xr-x   0        0        0     4566 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Optics/qw_absorption.rst
--rwxr-xr-x   0        0        0     4766 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Optics/rcwa.rst
--rwxr-xr-x   0        0        0     2022 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Optics/tmm.rst
--rwxr-xr-x   0        0        0     3359 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/QM/Schrodinger.rst
--rwxr-xr-x   0        0        0    18880 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Quasi3D/pv_module.png
--rwxr-xr-x   0        0        0     1731 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Quasi3D/pv_panel.rst
--rwxr-xr-x   0        0        0     5959 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Quasi3D/quasi3D.rst
--rwxr-xr-x   0        0        0   349548 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Quasi3D/quasi3Dimg.png
--rwxr-xr-x   0        0        0      968 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Quasi3D/spice.rst
--rwxr-xr-x   0        0        0    14080 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/ASC.rst
--rwxr-xr-x   0        0        0     2867 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/DDsolver.rst
--rwxr-xr-x   0        0        0     7222 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/DeviceStructure.rst
--rwxr-xr-x   0        0        0    20467 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/DriftDiffusionUtilities.rst
--rwxr-xr-x   0        0        0    34419 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/EQandSC.png
--rwxr-xr-x   0        0        0    35846 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/IV.png
--rwxr-xr-x   0        0        0    23374 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/LightIV.png
--rwxr-xr-x   0        0        0    88937 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/MeshDescription.svg
--rwxr-xr-x   0        0        0    34343 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/QE.png
--rwxr-xr-x   0        0        0    25790 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/QWunit.png
--rwxr-xr-x   0        0        0    84327 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/iv_mj.png
--rwxr-xr-x   0        0        0    20187 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/mesh.png
--rwxr-xr-x   0        0        0    43163 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/Figures/qe_mj.png
--rwxr-xr-x   0        0        0    12211 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/QWunit.rst
--rwxr-xr-x   0        0        0     5869 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/TwoDiode.rst
--rwxr-xr-x   0        0        0     4293 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/depletion.rst
--rwxr-xr-x   0        0        0     1513 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/detailed_balance.rst
--rwxr-xr-x   0        0        0     7377 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/multijunction_iv.rst
--rwxr-xr-x   0        0        0     7943 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Solvers/solving_solar_cells.rst
--rwxr-xr-x   0        0        0     2394 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Structures/structure.rst
--rwxr-xr-x   0        0        0     4764 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Systems/Materials.rst
--rwxr-xr-x   0        0        0     4616 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Systems/NewMats.rst
--rwxr-xr-x   0        0        0      256 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Systems/Units.rst
--rwxr-xr-x   0        0        0    46832 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Systems/eg_vs_lattice_constant.png
--rwxr-xr-x   0        0        0      284 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/Systems/systems.rst
--rw-r--r--   0        0        0   186465 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/_static/header.png
--rwxr-xr-x   0        0        0    10247 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/conf.py
--rwxr-xr-x   0        0        0     1240 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/index.rst
--rwxr-xr-x   0        0        0     3309 1970-01-01 00:00:00.000000 solcore-5.9.1/docs/source/spectral/spectral.rst
--rwxr-xr-x   0        0        0     1810 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Absorption_profile_AlGaAs_GaAs_structure.py
--rwxr-xr-x   0        0        0     1498 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Light_sources_examples.py
--rwxr-xr-x   0        0        0     3867 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/MJ_solar_cell_PDD_solver.py
--rwxr-xr-x   0        0        0     4716 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/MJ_solar_cell_using_DA.py
--rwxr-xr-x   0        0        0     3359 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/MJ_solar_cell_with_radiative_coupling.py
--rwxr-xr-x   0        0        0     1678 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Materials_Eg_vs_lattice_constant.py
--rwxr-xr-x   0        0        0     4236 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Optical_constants_CPPB_model.py
--rwxr-xr-x   0        0        0     2154 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Optical_constants_RAT_of_ARC.py
--rwxr-xr-x   0        0        0     1561 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Optical_constants_RAT_of_ITO_films.py
--rwxr-xr-x   0        0        0     3585 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Optical_constants_ellipsometry_modelling.py
--rwxr-xr-x   0        0        0     1660 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Optical_constants_ellipsometry_modelling_2.py
--rwxr-xr-x   0        0        0     1919 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Optical_constants_using_SOPRA_db.py
--rwxr-xr-x   0        0        0     4175 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Optics_comparison_of_models.py
--rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/PV_module_calculator.ipynb
--rwxr-xr-x   0        0        0     1827 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/PV_module_calculator.py
--rwxr-xr-x   0        0        0     2718 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Quasi3D_3J_solar_Cell.py
--rwxr-xr-x   0        0        0     2198 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Schrodinger_QW_absorption.py
--rwxr-xr-x   0        0        0     1452 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Schrodinger_QW_and_MQW.py
--rwxr-xr-x   0        0        0     1091 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/Tunnel_junction.py
--rw-r--r--   0        0        0     5653 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.ipynb
--rwxr-xr-x   0        0        0     2756 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.py
--rw-r--r--   0        0        0    14530 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_tutorial.ipynb
--rwxr-xr-x   0        0        0     7250 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_tutorial.py
--rw-r--r--   0        0        0    26801 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/differential_evolution_4Jcell.ipynb
--rw-r--r--   0        0        0    20116 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/differential_evolution_4Jcell.py
--rw-r--r--   0        0        0     8346 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/differential_evolution_ARC.ipynb
--rw-r--r--   0        0        0     5673 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/advanced_examples/differential_evolution_ARC.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/coherency_example.py
--rw-r--r--   0        0        0     6826 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/coherency_example_2.py
--rwxr-xr-x   0        0        0     2401 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/custom_materials_example.py
--rwxr-xr-x   0        0        0     3247 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/AlInP_nk.csv
--rwxr-xr-x   0        0        0     3684 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/GaInP_nk.csv
--rwxr-xr-x   0        0        0     1485 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/Ge-Palik.csv
--rwxr-xr-x   0        0        0     6758 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/Ge_nk.csv
--rwxr-xr-x   0        0        0     4963 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/MgF-ZnS_AR.csv
--rwxr-xr-x   0        0        0     6062 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/MgF_nk.csv
--rwxr-xr-x   0        0        0     1008 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/Palik_GaAs_Eps1.csv
--rwxr-xr-x   0        0        0     1692 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/Palik_GaAs_Eps2.csv
--rwxr-xr-x   0        0        0     3730 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/SiCx_nk.csv
--rwxr-xr-x   0        0        0    11488 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/SiGeSn_k.txt
--rwxr-xr-x   0        0        0    11406 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/SiGeSn_n.txt
--rwxr-xr-x   0        0        0      572 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/SiGeSn_params.txt
--rwxr-xr-x   0        0        0     7760 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/ZnS_nk.csv
--rwxr-xr-x   0        0        0    48480 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/ge_ellipsometry_data.dat
--rw-r--r--   0        0        0    24952 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/ge_g_sigesn_edge_nk.mat
--rw-r--r--   0        0        0    24957 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/ge_g_sigesn_nk.mat
--rwxr-xr-x   0        0        0     5239 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/in01gaas.csv
--rwxr-xr-x   0        0        0     2793 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/masks_cl.png
--rwxr-xr-x   0        0        0     3973 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/masks_illumination.png
--rwxr-xr-x   0        0        0      278 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/data/masks_sq.png
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/external_optics.py
--rwxr-xr-x   0        0        0     1597 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/kp_fit_effective_masses.py
--rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Absorption_profile_AlGaAs_GaAs_structure.ipynb
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Light_sources_examples.ipynb
--rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/MJ_solar_cell_PDD_solver.ipynb
--rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/MJ_solar_cell_using_DA.ipynb
--rw-r--r--   0        0        0     4754 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/MJ_solar_cell_with_radiative_coupling.ipynb
--rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Materials_eg_vs_lattice_constant.ipynb
--rw-r--r--   0        0        0     7148 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Optical_constants_CPPB_model.ipynb
--rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Optical_constants_RAT_of_ARC.ipynb
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Optical_constants_RAT_of_ITO_films.ipynb
--rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Optical_constants_ellipsometry_modelling.ipynb
--rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Optical_constants_ellipsometry_modelling_2.ipynb
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Optical_constants_using_SOPRA_db.ipynb
--rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Optics_comparison_of_models.ipynb
--rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/PDD_1Junction.ipynb
--rwxr-xr-x   0        0        0     7187 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/QW_Absorption.ipynb
--rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Quasi3D_3J_solar_Cell.ipynb
--rw-r--r--   0        0        0     5085 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Schrodinger_QW_absorption.ipynb
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Schrodinger_QW_and_MQW.ipynb
--rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/Tunnel_junction.ipynb
--rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/coherency_example.ipynb
--rw-r--r--   0        0        0    11693 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/coherency_example_2.ipynb
--rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/custom_materials_example.ipynb
--rw-r--r--   0        0        0    13578 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/external_optics.ipynb
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/kp_fit_effective_masses.ipynb
--rw-r--r--   0        0        0     5922 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/refractiveindex_info_db_example.ipynb
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/simple_rcwa.ipynb
--rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/notebooks/substrate_example.ipynb
--rwxr-xr-x   0        0        0     3607 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/refractiveindex_info_db_example.py
--rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/simple_rcwa.py
--rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 solcore-5.9.1/examples/substrate_example.py
--rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 solcore-5.9.1/meson.build
--rw-r--r--   0        0        0      244 1970-01-01 00:00:00.000000 solcore-5.9.1/meson_options.txt
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 solcore-5.9.1/pyproject.toml
--rwxr-xr-x   0        0        0     1812 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/__init__.py
--rwxr-xr-x   0        0        0      871 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/__init__.py
--rwxr-xr-x   0        0        0    17220 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/absorption_QW.py
--rwxr-xr-x   0        0        0     7526 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/adachi_alpha.py
--rwxr-xr-x   0        0        0    29393 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/cppm/Custom_CPPB.py
--rwxr-xr-x   0        0        0     4337 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/cppm/Custom_CPPB_MaterialParamaters.txt
--rwxr-xr-x   0        0        0       36 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/cppm/__init__.py
--rwxr-xr-x   0        0        0    15170 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/dielectric_constant_models.py
--rwxr-xr-x   0        0        0     1622 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/kramers_kronig.py
--rwxr-xr-x   0        0        0     4642 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/nk_db.py
--rwxr-xr-x   0        0        0    25092 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/rigorous_coupled_wave.py
--rwxr-xr-x   0        0        0    14233 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/sopra_db.py
--rwxr-xr-x   0        0        0    45986 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/tmm_core_vec.py
--rwxr-xr-x   0        0        0    29836 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/absorption_calculator/transfer_matrix.py
--rwxr-xr-x   0        0        0    10061 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/analytic_solar_cells/IV.py
--rwxr-xr-x   0        0        0    19030 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/analytic_solar_cells/QE.py
--rwxr-xr-x   0        0        0      417 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/analytic_solar_cells/__init__.py
--rwxr-xr-x   0        0        0    26456 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/analytic_solar_cells/depletion_approximation.py
--rwxr-xr-x   0        0        0     8490 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/analytic_solar_cells/detailed_balance.py
--rwxr-xr-x   0        0        0    22602 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/analytic_solar_cells/diode_equation.py
--rwxr-xr-x   0        0        0     7192 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/analytic_solar_cells/tunnel_junctions.py
--rwxr-xr-x   0        0        0    20354 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/config_tools.py
--rwxr-xr-x   0        0        0      300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/constants.py
--rwxr-xr-x   0        0        0     3624 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/crystals.py
--rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/data_analysis_tools/__init__.py
--rwxr-xr-x   0        0        0    18413 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/data_analysis_tools/ellipsometry_analysis.py
--rwxr-xr-x   0        0        0     3027 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/graphing/Colours.txt
--rwxr-xr-x   0        0        0     4762 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/graphing/Custom_Colours.py
--rwxr-xr-x   0        0        0       48 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/graphing/__init__.py
--rwxr-xr-x   0        0        0    10242 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/graphing/graph.py
--rwxr-xr-x   0        0        0     4506 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/graphing/graph_lines.py
--rwxr-xr-x   0        0        0      555 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/graphing/graph_support.py
--rwxr-xr-x   0        0        0    14088 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/interpolate.py
--rwxr-xr-x   0        0        0     7260 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/light_source/SPCTRAL_si_units.txt
--rwxr-xr-x   0        0        0      234 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/light_source/__init__.py
--rwxr-xr-x   0        0        0    79378 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/light_source/astmg173.csv
--rwxr-xr-x   0        0        0    22224 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/light_source/light_source.py
--rwxr-xr-x   0        0        0    14482 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/light_source/smarts.py
--rwxr-xr-x   0        0        0     9255 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/light_source/spectral2.py
--rwxr-xr-x   0        0        0      876 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Adachi/binaries.txt
--rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Adachi/ternaries.txt
--rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlAs-Material/k.txt
--rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlAs-Material/n.txt
--rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/__init__.py
--rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.000_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.099_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.198_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.315_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.419_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.491_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.590_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.700_AlGaAs_k.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.804_AlGaAs_k.txt
--rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/1.000_AlGaAs_k.txt
--rwxr-xr-x   0        0        0     5267 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/critical_points.txt
--rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.000_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.099_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.198_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.315_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.419_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.491_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.590_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.700_AlGaAs_n.txt
--rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.804_AlGaAs_n.txt
--rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/1.000_AlGaAs_n.txt
--rwxr-xr-x   0        0        0     2928 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/critical_points.txt
--rwxr-xr-x   0        0        0      857 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/__init__.py
--rwxr-xr-x   0        0        0     8103 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/k/0.000_AlInP_k.txt
--rwxr-xr-x   0        0        0    15376 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/k/0.530_AlInP_k.txt
--rwxr-xr-x   0        0        0      413 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/k/1.000_AlInP_k.txt
--rwxr-xr-x   0        0        0      996 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/k/critical_points.txt
--rwxr-xr-x   0        0        0     8200 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/n/0.000_AlInP_n.txt
--rwxr-xr-x   0        0        0    30000 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/n/0.530_AlInP_n.txt
--rwxr-xr-x   0        0        0      919 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/n/1.000_AlInP_n.txt
--rwxr-xr-x   0        0        0      471 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/AlInP-Material/n/critical_points.txt
--rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAs-Material/k.txt
--rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAs-Material/n.txt
--rwxr-xr-x   0        0        0      239 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAsP-Material/__init__.py
--rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAsP-Material/k/0.000_GaAsP_k.txt
--rwxr-xr-x   0        0        0     8200 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAsP-Material/k/1.000_GaAsP_k.txt
--rwxr-xr-x   0        0        0      888 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAsP-Material/k/critical_points.txt
--rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAsP-Material/n/0.000_GaAsP_n.txt
--rwxr-xr-x   0        0        0     8250 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAsP-Material/n/1.000_GaAsP_n.txt
--rwxr-xr-x   0        0        0      491 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaAsP-Material/n/critical_points.txt
--rwxr-xr-x   0        0        0      472 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/__init__.py
--rwxr-xr-x   0        0        0     8250 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/k/0.000_GaInP_k.txt
--rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/k/0.490_GaInP_k.txt
--rwxr-xr-x   0        0        0     8103 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/k/1.000_GaInP_k.txt
--rwxr-xr-x   0        0        0     1055 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/k/critical_points.txt
--rwxr-xr-x   0        0        0     8250 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/n/0.000_GaInP_n.txt
--rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/n/0.490_GaInP_n.txt
--rwxr-xr-x   0        0        0     8200 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/n/1.000_GaInP_n.txt
--rwxr-xr-x   0        0        0      627 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaInP-Material/n/critical_points.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaSb-Material/k.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/GaSb-Material/n.txt
--rw-r--r--   0        0        0     6606 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Ge-Material/k.txt
--rw-r--r--   0        0        0     6281 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Ge-Material/n.txt
--rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/__init__.py
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.000_Strained_InGaAs_k.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.100_Strained_InGaAs_k.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.200_Strained_InGaAs_k.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.240_Strained_InGaAs_k.txt
--rwxr-xr-x   0        0        0     2686 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/k/critical_points.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.000_Strained_InGaAs_n.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.100_Strained_InGaAs_n.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.200_Strained_InGaAs_n.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.240_Strained_InGaAs_n.txt
--rwxr-xr-x   0        0        0     2075 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaAs-Material/n/critical_points.txt
--rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/__init__.py
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.000_InGaSb_K.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.100_InGaSb_K.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.300_InGaSb_K.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.500_InGaSb_K.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.700_InGaSb_K.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.900_InGaSb_K.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/1.000_InGaSb_K.txt
--rwxr-xr-x   0        0        0     3274 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/k/critical_points.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.000_InGaSb_N.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.100_InGaSb_N.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.300_InGaSb_N.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.500_InGaSb_N.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.700_InGaSb_N.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.900_InGaSb_N.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/1.000_InGaSb_N.txt
--rwxr-xr-x   0        0        0     4776 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InGaSb-Material/n/critical_points.txt
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InP-Material/info.txt
--rw-r--r--   0        0        0   113600 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InP-Material/k.txt
--rw-r--r--   0        0        0   113600 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InP-Material/n.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InSb-Material/k.txt
--rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/InSb-Material/n.txt
--rwxr-xr-x   0        0        0     1122 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Levinshtein/GroupIV.txt
--rwxr-xr-x   0        0        0     2877 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/7059.MAT
--rwxr-xr-x   0        0        0     5843 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/AG.MAT
--rwxr-xr-x   0        0        0      162 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/AIR.MAT
--rwxr-xr-x   0        0        0     6133 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/AL.MAT
--rwxr-xr-x   0        0        0     1347 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/AL2O3.MAT
--rwxr-xr-x   0        0        0     2652 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/AL2O3P.MAT
--rwxr-xr-x   0        0        0     4832 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS.MAT
--rwxr-xr-x   0        0        0    10196 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS028T.MAT
--rwxr-xr-x   0        0        0    10199 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS052T.MAT
--rwxr-xr-x   0        0        0    10202 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS072T.MAT
--rwxr-xr-x   0        0        0    10205 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS098T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS125T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS152T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS178T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS204T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS228T.MAT
--rwxr-xr-x   0        0        0    10214 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS305T.MAT
--rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS331T.MAT
--rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS361T.MAT
--rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS390T.MAT
--rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS421T.MAT
--rwxr-xr-x   0        0        0    10226 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS445T.MAT
--rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS469T.MAT
--rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS499T.MAT
--rwxr-xr-x   0        0        0    10232 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS527T.MAT
--rwxr-xr-x   0        0        0    10235 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS552T.MAT
--rwxr-xr-x   0        0        0    10244 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS578T.MAT
--rwxr-xr-x   0        0        0    10247 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS602T.MAT
--rwxr-xr-x   0        0        0    10250 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS626T.MAT
--rwxr-xr-x   0        0        0    10196 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS028T.MAT
--rwxr-xr-x   0        0        0    10199 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS052T.MAT
--rwxr-xr-x   0        0        0    10202 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS072T.MAT
--rwxr-xr-x   0        0        0    10205 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS098T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS125T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS152T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS178T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS204T.MAT
--rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS228T.MAT
--rwxr-xr-x   0        0        0    10214 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS305T.MAT
--rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS331T.MAT
--rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS361T.MAT
--rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS390T.MAT
--rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS421T.MAT
--rwxr-xr-x   0        0        0    10226 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS445T.MAT
--rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS469T.MAT
--rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS499T.MAT
--rwxr-xr-x   0        0        0    10232 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS527T.MAT
--rwxr-xr-x   0        0        0    10235 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS552T.MAT
--rwxr-xr-x   0        0        0    10244 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS578T.MAT
--rwxr-xr-x   0        0        0    10247 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS602T.MAT
--rwxr-xr-x   0        0        0    10250 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS626T.MAT
--rwxr-xr-x   0        0        0     6285 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALCU.MAT
--rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS00.MAT
--rwxr-xr-x   0        0        0    10634 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS10.MAT
--rwxr-xr-x   0        0        0     4832 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS100.MAT
--rwxr-xr-x   0        0        0    10643 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS20.MAT
--rwxr-xr-x   0        0        0    10631 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS30.MAT
--rwxr-xr-x   0        0        0    10613 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS40.MAT
--rwxr-xr-x   0        0        0    10631 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS50.MAT
--rwxr-xr-x   0        0        0    10628 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS60.MAT
--rwxr-xr-x   0        0        0    10619 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS70.MAT
--rwxr-xr-x   0        0        0    10610 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS80.MAT
--rwxr-xr-x   0        0        0     4832 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS90.MAT
--rwxr-xr-x   0        0        0    15051 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP00.MAT
--rwxr-xr-x   0        0        0    15048 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP10.MAT
--rwxr-xr-x   0        0        0    15105 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP100.MAT
--rwxr-xr-x   0        0        0    15060 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP30.MAT
--rwxr-xr-x   0        0        0    15075 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP60.MAT
--rwxr-xr-x   0        0        0    15084 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP70.MAT
--rwxr-xr-x   0        0        0     2517 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALON.MAT
--rwxr-xr-x   0        0        0     5044 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALSB.MAT
--rwxr-xr-x   0        0        0     5362 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALSI.MAT
--rwxr-xr-x   0        0        0     5353 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ALSITI.MAT
--rwxr-xr-x   0        0        0     4680 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ARACHI.MAT
--rwxr-xr-x   0        0        0    14411 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ASI.MAT
--rwxr-xr-x   0        0        0     5269 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/AU.MAT
--rwxr-xr-x   0        0        0     8360 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/BAF2.MAT
--rwxr-xr-x   0        0        0     2652 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/BK7.MAT
--rwxr-xr-x   0        0        0     2652 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CAF2.MAT
--rwxr-xr-x   0        0        0     2763 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CARBAM.MAT
--rwxr-xr-x   0        0        0     3102 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CCL4.MAT
--rwxr-xr-x   0        0        0     5870 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CDSE.MAT
--rwxr-xr-x   0        0        0     4383 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CDTE.MAT
--rwxr-xr-x   0        0        0     3102 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CO.MAT
--rwxr-xr-x   0        0        0     1122 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/COR7059.MAT
--rwxr-xr-x   0        0        0     1887 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/COSI2-4.MAT
--rwxr-xr-x   0        0        0     5554 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CO_2.MAT
--rwxr-xr-x   0        0        0     4680 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CR.MAT
--rwxr-xr-x   0        0        0     2881 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CR3SI.MAT
--rwxr-xr-x   0        0        0     2824 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CR5SI3.MAT
--rwxr-xr-x   0        0        0     6326 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CRSI2EL2.MAT
--rwxr-xr-x   0        0        0     5734 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CU.MAT
--rwxr-xr-x   0        0        0     3666 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CU2O.MAT
--rwxr-xr-x   0        0        0     3654 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/CUO.MAT
--rwxr-xr-x   0        0        0     4980 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/DIAM.MAT
--rwxr-xr-x   0        0        0     2280 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/FESI2EL1.MAT
--rwxr-xr-x   0        0        0     6342 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/FESI2EL2.MAT
--rwxr-xr-x   0        0        0     2343 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/FESI2EPI.MAT
--rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS.MAT
--rwxr-xr-x   0        0        0    10377 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS031T.MAT
--rwxr-xr-x   0        0        0    10374 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS041T.MAT
--rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS060T.MAT
--rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS081T.MAT
--rwxr-xr-x   0        0        0    14621 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS100.MAT
--rwxr-xr-x   0        0        0    10368 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS103T.MAT
--rwxr-xr-x   0        0        0    14618 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS111.MAT
--rwxr-xr-x   0        0        0    10365 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS126T.MAT
--rwxr-xr-x   0        0        0    10362 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS150T.MAT
--rwxr-xr-x   0        0        0    10359 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS175T.MAT
--rwxr-xr-x   0        0        0    10356 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS199T.MAT
--rwxr-xr-x   0        0        0    10353 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS224T.MAT
--rwxr-xr-x   0        0        0    10350 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS249T.MAT
--rwxr-xr-x   0        0        0    10347 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS273T.MAT
--rwxr-xr-x   0        0        0    10344 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS297T.MAT
--rwxr-xr-x   0        0        0    10341 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS320T.MAT
--rwxr-xr-x   0        0        0    10338 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS344T.MAT
--rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS367T.MAT
--rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS391T.MAT
--rwxr-xr-x   0        0        0    10332 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS415T.MAT
--rwxr-xr-x   0        0        0    10329 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS443T.MAT
--rwxr-xr-x   0        0        0    10326 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS465T.MAT
--rwxr-xr-x   0        0        0    10323 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS488T.MAT
--rwxr-xr-x   0        0        0    10320 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS515T.MAT
--rwxr-xr-x   0        0        0    10317 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS546T.MAT
--rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS579T.MAT
--rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS603T.MAT
--rwxr-xr-x   0        0        0    10305 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS634T.MAT
--rwxr-xr-x   0        0        0     4857 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAASO.MAT
--rwxr-xr-x   0        0        0     2202 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAASOX.MAT
--rwxr-xr-x   0        0        0    10377 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS031T.MAT
--rwxr-xr-x   0        0        0    10374 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS041T.MAT
--rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS060T.MAT
--rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS081T.MAT
--rwxr-xr-x   0        0        0    10368 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS103T.MAT
--rwxr-xr-x   0        0        0    10365 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS126T.MAT
--rwxr-xr-x   0        0        0    10362 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS150T.MAT
--rwxr-xr-x   0        0        0    10359 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS175T.MAT
--rwxr-xr-x   0        0        0    10356 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS199T.MAT
--rwxr-xr-x   0        0        0    10353 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS224T.MAT
--rwxr-xr-x   0        0        0    10350 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS249T.MAT
--rwxr-xr-x   0        0        0    10347 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS273T.MAT
--rwxr-xr-x   0        0        0    10344 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS297T.MAT
--rwxr-xr-x   0        0        0    10341 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS320T.MAT
--rwxr-xr-x   0        0        0    10338 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS344T.MAT
--rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS367T.MAT
--rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS391T.MAT
--rwxr-xr-x   0        0        0    10332 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS415T.MAT
--rwxr-xr-x   0        0        0    10329 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS443T.MAT
--rwxr-xr-x   0        0        0    10326 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS465T.MAT
--rwxr-xr-x   0        0        0    10323 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS488T.MAT
--rwxr-xr-x   0        0        0    10320 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS515T.MAT
--rwxr-xr-x   0        0        0    10317 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS546T.MAT
--rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS579T.MAT
--rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS603T.MAT
--rwxr-xr-x   0        0        0    10305 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS634T.MAT
--rwxr-xr-x   0        0        0    10320 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAP.MAT
--rwxr-xr-x   0        0        0    14900 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAP100.MAT
--rwxr-xr-x   0        0        0     2175 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GAPOX.MAT
--rwxr-xr-x   0        0        0     4503 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GASB.MAT
--rwxr-xr-x   0        0        0     2226 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GASBOX.MAT
--rwxr-xr-x   0        0        0     5224 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GE.MAT
--rwxr-xr-x   0        0        0    14363 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/GE100.MAT
--rwxr-xr-x   0        0        0     4227 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/H2O.MAT
--rwxr-xr-x   0        0        0     2517 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/HFO2.MAT
--rwxr-xr-x   0        0        0     8965 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/HFSI2.MAT
--rwxr-xr-x   0        0        0     6146 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE00.MAT
--rwxr-xr-x   0        0        0     6182 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE20.MAT
--rwxr-xr-x   0        0        0     6197 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE30.MAT
--rwxr-xr-x   0        0        0     7374 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INAS.MAT
--rwxr-xr-x   0        0        0     2220 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INASOX.MAT
--rwxr-xr-x   0        0        0    10574 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGAAS.MAT
--rwxr-xr-x   0        0        0     5675 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB00.MAT
--rwxr-xr-x   0        0        0     5672 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB10.MAT
--rwxr-xr-x   0        0        0     5720 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB100.MAT
--rwxr-xr-x   0        0        0     5672 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB30.MAT
--rwxr-xr-x   0        0        0     5678 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB50.MAT
--rwxr-xr-x   0        0        0     5690 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB70.MAT
--rwxr-xr-x   0        0        0     5708 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB90.MAT
--rwxr-xr-x   0        0        0     5245 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INP.MAT
--rwxr-xr-x   0        0        0     2223 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INPOX.MAT
--rwxr-xr-x   0        0        0     9397 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INSB.MAT
--rwxr-xr-x   0        0        0     2292 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/INSBOX.MAT
--rwxr-xr-x   0        0        0     5674 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/IR.MAT
--rwxr-xr-x   0        0        0     2022 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/IR3SI5E.MAT
--rwxr-xr-x   0        0        0     2382 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/IR3SI5P.MAT
--rwxr-xr-x   0        0        0     3060 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ITO2.MAT
--rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/KCL.MAT
--rwxr-xr-x   0        0        0     2382 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/LASF9.MAT
--rwxr-xr-x   0        0        0     1113 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/LI.MAT
--rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/LIF.MAT
--rwxr-xr-x   0        0        0    43469 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/List_Of_Files.xlsx
--rwxr-xr-x   0        0        0    47376 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/List_Of_Files_Updated_PDF.pdf
--rwxr-xr-x   0        0        0     1347 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/MGF2.MAT
--rwxr-xr-x   0        0        0    11252 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/MO.MAT
--rwxr-xr-x   0        0        0     1707 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/MOSI2-A.MAT
--rwxr-xr-x   0        0        0     1707 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/MOSI2-B.MAT
--rwxr-xr-x   0        0        0     5566 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/NBSI-A.MAT
--rwxr-xr-x   0        0        0     5569 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/NBSI-B.MAT
--rwxr-xr-x   0        0        0     5600 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/NI.MAT
--rwxr-xr-x   0        0        0     2746 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/NI2SI.MAT
--rwxr-xr-x   0        0        0     2750 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/NI3SI.MAT
--rwxr-xr-x   0        0        0     2750 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/NISI.MAT
--rwxr-xr-x   0        0        0     5600 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/OS.MAT
--rwxr-xr-x   0        0        0     5393 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/PBS.MAT
--rwxr-xr-x   0        0        0     4884 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/PBSE.MAT
--rwxr-xr-x   0        0        0     5682 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/PD.MAT
--rwxr-xr-x   0        0        0     3288 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/PD2SI-A.MAT
--rwxr-xr-x   0        0        0     3290 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/PD2SI-B.MAT
--rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/PT.MAT
--rwxr-xr-x   0        0        0    14570 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/P_SIAS.MAT
--rwxr-xr-x   0        0        0    14546 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/P_SIUD.MAT
--rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS00.MAT
--rwxr-xr-x   0        0        0     5831 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS10.MAT
--rwxr-xr-x   0        0        0     5444 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS20.MAT
--rwxr-xr-x   0        0        0    13233 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS24.MAT
--rwxr-xr-x   0        0        0     5662 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESI1-75.MAT
--rwxr-xr-x   0        0        0     5224 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE100.MAT
--rwxr-xr-x   0        0        0     6858 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE11.MAT
--rwxr-xr-x   0        0        0     1971 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE22.MAT
--rwxr-xr-x   0        0        0     1965 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE39.MAT
--rwxr-xr-x   0        0        0     1959 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE51.MAT
--rwxr-xr-x   0        0        0     1956 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE64.MAT
--rwxr-xr-x   0        0        0     1953 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE75.MAT
--rwxr-xr-x   0        0        0     1947 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE83.MAT
--rwxr-xr-x   0        0        0     1947 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE91.MAT
--rwxr-xr-x   0        0        0     5301 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RH.MAT
--rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS0.MAT
--rwxr-xr-x   0        0        0     5831 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS10.MAT
--rwxr-xr-x   0        0        0     5444 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS20.MAT
--rwxr-xr-x   0        0        0    13233 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS24.MAT
--rwxr-xr-x   0        0        0     2382 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SF11.MAT
--rwxr-xr-x   0        0        0    14806 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SI100_2.MAT
--rwxr-xr-x   0        0        0    14806 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SI110.MAT
--rwxr-xr-x   0        0        0    14806 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SI111.MAT
--rwxr-xr-x   0        0        0     6739 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SI3N4.MAT
--rwxr-xr-x   0        0        0     2640 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIAM1.MAT
--rwxr-xr-x   0        0        0     2454 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIAM2.MAT
--rwxr-xr-x   0        0        0     9988 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIC.MAT
--rwxr-xr-x   0        0        0     6181 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T02.MAT
--rwxr-xr-x   0        0        0     6175 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T10.MAT
--rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T15.MAT
--rwxr-xr-x   0        0        0     6172 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T20.MAT
--rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T25.MAT
--rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T30.MAT
--rwxr-xr-x   0        0        0     6169 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T35.MAT
--rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T40.MAT
--rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T45.MAT
--rwxr-xr-x   0        0        0    17004 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR.MAT
--rwxr-xr-x   0        0        0     6181 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T020.MAT
--rwxr-xr-x   0        0        0     6175 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T100.MAT
--rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T150.MAT
--rwxr-xr-x   0        0        0     6172 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T200.MAT
--rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T250.MAT
--rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T300.MAT
--rwxr-xr-x   0        0        0     6169 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T350.MAT
--rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T400.MAT
--rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T450.MAT
--rwxr-xr-x   0        0        0    14447 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_GE.MAT
--rwxr-xr-x   0        0        0    14297 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE11.MAT
--rwxr-xr-x   0        0        0    14336 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE20.MAT
--rwxr-xr-x   0        0        0    14366 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE28.MAT
--rwxr-xr-x   0        0        0    14492 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE65.MAT
--rwxr-xr-x   0        0        0    14549 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE85.MAT
--rwxr-xr-x   0        0        0    14567 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE98.MAT
--rwxr-xr-x   0        0        0    14459 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI.MAT
--rwxr-xr-x   0        0        0     2622 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIO.MAT
--rwxr-xr-x   0        0        0     3327 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIO2.MAT
--rwxr-xr-x   0        0        0     5149 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION0.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION20.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION40.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION60.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION80.MAT
--rwxr-xr-x   0        0        0     5149 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION00.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION20.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION40.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION60.MAT
--rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION80.MAT
--rwxr-xr-x   0        0        0     5771 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIOP.MAT
--rwxr-xr-x   0        0        0     4725 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY.MAT
--rwxr-xr-x   0        0        0     5765 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY10.MAT
--rwxr-xr-x   0        0        0     5756 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY20.MAT
--rwxr-xr-x   0        0        0     5756 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY30.MAT
--rwxr-xr-x   0        0        0     5747 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY40.MAT
--rwxr-xr-x   0        0        0     5729 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY50.MAT
--rwxr-xr-x   0        0        0     5714 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY60.MAT
--rwxr-xr-x   0        0        0     5708 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY70.MAT
--rwxr-xr-x   0        0        0     5693 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY80.MAT
--rwxr-xr-x   0        0        0     5687 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY90.MAT
--rwxr-xr-x   0        0        0     4776 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPORE.MAT
--rwxr-xr-x   0        0        0    15495 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/SOPRA_DB_Updated.csv
--rwxr-xr-x   0        0        0     5840 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS00.MAT
--rwxr-xr-x   0        0        0     5834 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS10.MAT
--rwxr-xr-x   0        0        0     5825 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS20.MAT
--rwxr-xr-x   0        0        0     5822 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS24.MAT
--rwxr-xr-x   0        0        0     4833 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG0.MAT
--rwxr-xr-x   0        0        0     4824 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG06.MAT
--rwxr-xr-x   0        0        0     4818 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG12.MAT
--rwxr-xr-x   0        0        0     4812 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG17.MAT
--rwxr-xr-x   0        0        0     4803 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG22.MAT
--rwxr-xr-x   0        0        0    11076 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TA.MAT
--rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TAOX1.MAT
--rwxr-xr-x   0        0        0     5600 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TAOX2.MAT
--rwxr-xr-x   0        0        0     9536 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TASI2-A.MAT
--rwxr-xr-x   0        0        0     9551 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TASI2-B.MAT
--rwxr-xr-x   0        0        0     4983 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TEST.MAT
--rwxr-xr-x   0        0        0     4634 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/THF4.MAT
--rwxr-xr-x   0        0        0     4680 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TI.MAT
--rwxr-xr-x   0        0        0     3234 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TINI.MAT
--rwxr-xr-x   0        0        0     6161 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TIO2.MAT
--rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TIO2B.MAT
--rwxr-xr-x   0        0        0     9739 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/TISI-A.MAT
--rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/V.MAT
--rwxr-xr-x   0        0        0     3273 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/VOID.MAT
--rwxr-xr-x   0        0        0     4554 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/VSI2-A.MAT
--rwxr-xr-x   0        0        0     4554 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/VSI2-B.MAT
--rwxr-xr-x   0        0        0    11122 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/W.MAT
--rwxr-xr-x   0        0        0     3669 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/WSI2-A.MAT
--rwxr-xr-x   0        0        0     3654 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/WSI2-B.MAT
--rwxr-xr-x   0        0        0     5249 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/Y2O3.MAT
--rwxr-xr-x   0        0        0    20559 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE00.MAT
--rwxr-xr-x   0        0        0    20550 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE10.MAT
--rwxr-xr-x   0        0        0    20475 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE100.MAT
--rwxr-xr-x   0        0        0    20535 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE30.MAT
--rwxr-xr-x   0        0        0    20517 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE50.MAT
--rwxr-xr-x   0        0        0    20499 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE70.MAT
--rwxr-xr-x   0        0        0    20481 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE90.MAT
--rwxr-xr-x   0        0        0     4926 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSCUB.MAT
--rwxr-xr-x   0        0        0     5320 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSE.MAT
--rwxr-xr-x   0        0        0    21345 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE0.MAT
--rwxr-xr-x   0        0        0    21342 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE1.MAT
--rwxr-xr-x   0        0        0    21564 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE10.MAT
--rwxr-xr-x   0        0        0    21354 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE3.MAT
--rwxr-xr-x   0        0        0    21384 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE5.MAT
--rwxr-xr-x   0        0        0    21438 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE7.MAT
--rwxr-xr-x   0        0        0    21513 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE9.MAT
--rwxr-xr-x   0        0        0     2877 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZRO2.MAT
--rwxr-xr-x   0        0        0      717 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/ZRSI2.MAT
--rwxr-xr-x   0        0        0      195 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/SOPRA_DB/compounds.txt
--rwxr-xr-x   0        0        0      534 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Si-Material/info.txt
--rwxr-xr-x   0        0        0     2203 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Si-Material/k.txt
--rwxr-xr-x   0        0        0     2203 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Si-Material/n.txt
--rwxr-xr-x   0        0        0     7099 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Vurgaftman/binaries.txt
--rwxr-xr-x   0        0        0     2849 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/Vurgaftman/ternaries.txt
--rwxr-xr-x   0        0        0       40 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/__init__.py
--rwxr-xr-x   0        0        0    15884 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/mobility.py
--rwxr-xr-x   0        0        0     3752 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/mobility_parameters.json
--rwxr-xr-x   0        0        0       35 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/refractiveindex_info_DB/__init__.py
--rwxr-xr-x   0        0        0    17507 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/refractiveindex_info_DB/dbmaterial.py
--rwxr-xr-x   0        0        0    15811 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_data/refractiveindex_info_DB/dboperations.py
--rwxr-xr-x   0        0        0       96 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_system/__init__.py
--rwxr-xr-x   0        0        0     2913 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_system/create_new_material.py
--rwxr-xr-x   0        0        0     7578 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_system/critical_point_interpolate.py
--rwxr-xr-x   0        0        0     7040 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_system/critical_point_picker.py
--rwxr-xr-x   0        0        0    18225 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/material_system/material_system.py
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/meson.build
--rwxr-xr-x   0        0        0      381 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/optics/__init__.py
--rwxr-xr-x   0        0        0    10132 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/optics/beer_lambert.py
--rwxr-xr-x   0        0        0     2435 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/optics/external_optics.py
--rwxr-xr-x   0        0        0     7272 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/optics/rcwa.py
--rwxr-xr-x   0        0        0     7597 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/optics/tmm.py
--rw-r--r--   0        0        0       44 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/optimization/__init__.py
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/optimization/differential_evolution.py
--rwxr-xr-x   0        0        0       45 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/parameter_system/__init__.py
--rwxr-xr-x   0        0        0     1366 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/parameter_system/calculable_parameters.txt
--rwxr-xr-x   0        0        0     7730 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/parameter_system/parameter_system.py
--rwxr-xr-x   0        0        0    85017 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/poisson_drift_diffusion/DDmodel-current.f95
--rwxr-xr-x   0        0        0    12628 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/poisson_drift_diffusion/DeviceStructure.py
--rwxr-xr-x   0        0        0    20236 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/poisson_drift_diffusion/DriftDiffusionUtilities.py
--rwxr-xr-x   0        0        0    20729 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/poisson_drift_diffusion/QWunit.py
--rwxr-xr-x   0        0        0      442 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/poisson_drift_diffusion/__init__.py
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/poisson_drift_diffusion/meson.build
--rwxr-xr-x   0        0        0      169 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/__init__.py
--rwxr-xr-x   0        0        0    15768 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/graphics.py
--rwxr-xr-x   0        0        0      329 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/heterostructure_alignment.py
--rwxr-xr-x   0        0        0     8293 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/high_level_kp_QW.py
--rwxr-xr-x   0        0        0    22253 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/kp_QW.py
--rwxr-xr-x   0        0        0    17433 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/kp_bulk.py
--rwxr-xr-x   0        0        0     8987 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/potential_utilities.py
--rwxr-xr-x   0        0        0     6720 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/strain.py
--rwxr-xr-x   0        0        0    13892 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/quantum_mechanics/structure_utilities.py
--rw-r--r--   0        0        0    10861 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/registries.py
--rwxr-xr-x   0        0        0     2989 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/science_tracker.py
--rwxr-xr-x   0        0        0     4504 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/singleton.py
--rwxr-xr-x   0        0        0     1989 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/smooth.py
--rwxr-xr-x   0        0        0     6520 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/solar_cell.py
--rwxr-xr-x   0        0        0    14521 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/solar_cell_solver.py
--rwxr-xr-x   0        0        0     1286 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/solcore_config.txt
--rwxr-xr-x   0        0        0     2592 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/source_managed_class.py
--rwxr-xr-x   0        0        0      141 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/spice/__init__.py
--rwxr-xr-x   0        0        0     7514 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/spice/pv_module_solver.py
--rwxr-xr-x   0        0        0    14639 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/spice/quasi_3D_solver.py
--rwxr-xr-x   0        0        0     3615 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/spice/spice.py
--rwxr-xr-x   0        0        0     1026 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/state.py
--rwxr-xr-x   0        0        0     7934 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/strain_balancing.py
--rwxr-xr-x   0        0        0     8123 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/structure.py
--rwxr-xr-x   0        0        0      928 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/units_system/Default_units.txt
--rwxr-xr-x   0        0        0       37 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/units_system/__init__.py
--rwxr-xr-x   0        0        0    15404 1970-01-01 00:00:00.000000 solcore-5.9.1/solcore/units_system/units_system.py
--rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/__init__.py
--rw-r--r--   0        0        0     6445 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/conftest.py
--rwxr-xr-x   0        0        0     1483 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/Ge-Palik.csv
--rwxr-xr-x   0        0        0     4963 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/MgF-ZnS_AR.csv
--rw-r--r--   0        0        0    11488 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/SiGeSn_k.txt
--rw-r--r--   0        0        0    11406 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/SiGeSn_n.txt
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/SiGeSn_params.txt
--rw-r--r--   0        0        0     3437 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/absorption_profile.txt
--rwxr-xr-x   0        0        0     4082 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/alinp.csv
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/database_materials.txt
--rwxr-xr-x   0        0        0     5239 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/in01gaas.csv
--rwxr-xr-x   0        0        0     4855 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/in048ga052p.csv
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/data/substrate_presence_profile.csv
--rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/mock_ddModel.py
--rwxr-xr-x   0        0        0     6400 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test__pdd.py
--rwxr-xr-x   0        0        0     9056 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_absorption.py
--rwxr-xr-x   0        0        0      415 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_basics.py
--rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_config_tools.py
--rw-r--r--   0        0        0    41131 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_depletion_approximation.py
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_dielectric_constant.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_examples.py
--rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_light_source.py
--rw-r--r--   0        0        0    13063 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_optics.py
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_optimization.py
--rwxr-xr-x   0        0        0     7196 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_qm.py
--rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_registries.py
--rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_solar_cell_solver.py
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_state.py
--rw-r--r--   0        0        0     7016 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_structure.py
--rw-r--r--   0        0        0    68002 1970-01-01 00:00:00.000000 solcore-5.9.1/tests/test_tmm_core_vec.py
--rw-r--r--   0        0        0    26246 1970-01-01 00:00:00.000000 solcore-5.9.1/PKG-INFO
+-rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 solcore-5.9.2/.all-contributorsrc
+-rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 solcore-5.9.2/.devpy/cmds.py
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 solcore-5.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 solcore-5.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 solcore-5.9.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     4226 1970-01-01 00:00:00.000000 solcore-5.9.2/.github/workflows/build_deploy_wheels.yml
+-rw-r--r--   0        0        0     4973 1970-01-01 00:00:00.000000 solcore-5.9.2/.github/workflows/test_unit_and_examples.yml
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 solcore-5.9.2/.gitignore
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 solcore-5.9.2/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0    11819 1970-01-01 00:00:00.000000 solcore-5.9.2/CHANGELOG.rst
+-rwxr-xr-x   0        0        0     3215 1970-01-01 00:00:00.000000 solcore-5.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    10266 1970-01-01 00:00:00.000000 solcore-5.9.2/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     7651 1970-01-01 00:00:00.000000 solcore-5.9.2/GNU-LGPL.txt
+-rwxr-xr-x   0        0        0      987 1970-01-01 00:00:00.000000 solcore-5.9.2/LICENSE.txt
+-rw-r--r--   0        0        0    15488 1970-01-01 00:00:00.000000 solcore-5.9.2/README.md
+-rw-r--r--   0        0        0       98 1970-01-01 00:00:00.000000 solcore-5.9.2/binder/apt.txt
+-rw-r--r--   0        0        0       99 1970-01-01 00:00:00.000000 solcore-5.9.2/binder/postBuild
+-rw-r--r--   0        0        0       68 1970-01-01 00:00:00.000000 solcore-5.9.2/binder/requirements.txt
+-rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 solcore-5.9.2/build_tools/cibw_before_build_macos_arm.sh
+-rw-r--r--   0        0        0      279 1970-01-01 00:00:00.000000 solcore-5.9.2/build_tools/x86_64-w64-arm64.ini
+-rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/.nojekyll
+-rwxr-xr-x   0        0        0     7057 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/Makefile
+-rwxr-xr-x   0        0        0     6990 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/make.bat
+-rw-r--r--   0        0        0    46736 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/Ag_GaAs_abs.png
+-rw-r--r--   0        0        0    41012 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/Ag_k.png
+-rw-r--r--   0        0        0    39380 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/Ag_n.png
+-rwxr-xr-x   0        0        0    26706 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/DA_iv.png
+-rwxr-xr-x   0        0        0   230604 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/DA_iv2.png
+-rwxr-xr-x   0        0        0    31223 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/DA_qe.png
+-rw-r--r--   0        0        0    20539 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/Diamond_nk.png
+-rwxr-xr-x   0        0        0    21653 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/IV_param_dispersion.png
+-rwxr-xr-x   0        0        0    16932 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/IV_solar_module.png
+-rwxr-xr-x   0        0        0    24785 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/MJ_IV_optimal.png
+-rwxr-xr-x   0        0        0    31579 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/MJ_efficiency_map.png
+-rwxr-xr-x   0        0        0    59203 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/MJ_with_rad_coupling.png
+-rwxr-xr-x   0        0        0   133711 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/MQW_LDOS.png
+-rwxr-xr-x   0        0        0    24594 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/PDD_IV.png
+-rwxr-xr-x   0        0        0    29250 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/PDD_carrier_density.png
+-rwxr-xr-x   0        0        0    23275 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/PDD_qe.png
+-rwxr-xr-x   0        0        0    82016 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/RAT_of_ARC.png
+-rw-r--r--   0        0        0    18901 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/SiGeSn_nk.png
+-rwxr-xr-x   0        0        0    71549 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/Single_QW.png
+-rwxr-xr-x   0        0        0    14165 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/circular_mask_IV.png
+-rwxr-xr-x   0        0        0    15138 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/circular_mask_V1_3.png
+-rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/custom_materials_example.rst
+-rwxr-xr-x   0        0        0    26589 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/eff_mass_fit.png
+-rwxr-xr-x   0        0        0     5883 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_3J_with_DA_solver.rst
+-rwxr-xr-x   0        0        0     1936 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_K_and_effective_mass.rst
+-rwxr-xr-x   0        0        0     3305 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_MJ_efficiency_map.rst
+-rwxr-xr-x   0        0        0     4056 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_PDD_solver.rst
+-rwxr-xr-x   0        0        0     1771 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_QWs.rst
+-rwxr-xr-x   0        0        0     2756 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_RAT_of_ARC.rst
+-rwxr-xr-x   0        0        0     1780 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_light_sources.rst
+-rw-r--r--   0        0        0     7098 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_optics_comparison.rst
+-rwxr-xr-x   0        0        0     2157 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_pv_module.rst
+-rwxr-xr-x   0        0        0     3574 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_quasi3D_cell.rst
+-rwxr-xr-x   0        0        0     4345 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_radiative_coupling.rst
+-rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_substrate.rst
+-rwxr-xr-x   0        0        0     1333 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/example_tunnel_junction.rst
+-rwxr-xr-x   0        0        0    27377 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/iv.jpg
+-rwxr-xr-x   0        0        0    60710 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/iv_params.jpg
+-rwxr-xr-x   0        0        0    19120 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/kp.png
+-rwxr-xr-x   0        0        0    67440 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/ls_compare.png
+-rwxr-xr-x   0        0        0    91514 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/ls_smarts.png
+-rwxr-xr-x   0        0        0     1789 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/main.rst
+-rw-r--r--   0        0        0   241086 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/optmodelcomp.png
+-rwxr-xr-x   0        0        0    48407 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/qe.jpg
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/refractiveindex_info_db_example.rst
+-rwxr-xr-x   0        0        0    14175 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/square_mask_IV.png
+-rwxr-xr-x   0        0        0    10565 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/square_mask_V1_3.png
+-rw-r--r--   0        0        0    41375 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/substrate_Adepth.png
+-rw-r--r--   0        0        0    38834 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/substrate_RAT.png
+-rwxr-xr-x   0        0        0    35316 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/tunnel_junction.png
+-rwxr-xr-x   0        0        0    14884 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Examples/tutorial.rst
+-rwxr-xr-x   0        0        0   196433 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Infographics.jpg
+-rwxr-xr-x   0        0        0      987 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Installation/Solcore_on_MacOSX.md
+-rwxr-xr-x   0        0        0     6255 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Installation/Solcore_on_Windows.md
+-rwxr-xr-x   0        0        0     2400 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Installation/compilation.md
+-rwxr-xr-x   0        0        0     9390 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Installation/installation.rst
+-rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Installation/s4_installation.md
+-rwxr-xr-x   0        0        0     8458 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Optics/material_optics.rst
+-rwxr-xr-x   0        0        0      446 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Optics/optics.rst
+-rwxr-xr-x   0        0        0      575 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Optics/other_methods.rst
+-rwxr-xr-x   0        0        0    63532 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Optics/qw_absorption.png
+-rwxr-xr-x   0        0        0     4566 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Optics/qw_absorption.rst
+-rwxr-xr-x   0        0        0     4766 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Optics/rcwa.rst
+-rwxr-xr-x   0        0        0     2022 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Optics/tmm.rst
+-rwxr-xr-x   0        0        0     3359 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/QM/Schrodinger.rst
+-rwxr-xr-x   0        0        0    18880 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Quasi3D/pv_module.png
+-rwxr-xr-x   0        0        0     1731 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Quasi3D/pv_panel.rst
+-rwxr-xr-x   0        0        0     5959 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Quasi3D/quasi3D.rst
+-rwxr-xr-x   0        0        0   349548 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Quasi3D/quasi3Dimg.png
+-rwxr-xr-x   0        0        0      968 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Quasi3D/spice.rst
+-rwxr-xr-x   0        0        0    14080 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/ASC.rst
+-rwxr-xr-x   0        0        0     2867 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/DDsolver.rst
+-rwxr-xr-x   0        0        0     7222 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/DeviceStructure.rst
+-rwxr-xr-x   0        0        0    20467 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/DriftDiffusionUtilities.rst
+-rwxr-xr-x   0        0        0    34419 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/EQandSC.png
+-rwxr-xr-x   0        0        0    35846 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/IV.png
+-rwxr-xr-x   0        0        0    23374 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/LightIV.png
+-rwxr-xr-x   0        0        0    88937 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/MeshDescription.svg
+-rwxr-xr-x   0        0        0    34343 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/QE.png
+-rwxr-xr-x   0        0        0    25790 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/QWunit.png
+-rwxr-xr-x   0        0        0    84327 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/iv_mj.png
+-rwxr-xr-x   0        0        0    20187 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/mesh.png
+-rwxr-xr-x   0        0        0    43163 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/Figures/qe_mj.png
+-rwxr-xr-x   0        0        0    12211 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/QWunit.rst
+-rwxr-xr-x   0        0        0     5869 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/TwoDiode.rst
+-rwxr-xr-x   0        0        0     4293 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/depletion.rst
+-rwxr-xr-x   0        0        0     1513 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/detailed_balance.rst
+-rwxr-xr-x   0        0        0     7377 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/multijunction_iv.rst
+-rwxr-xr-x   0        0        0     7945 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Solvers/solving_solar_cells.rst
+-rwxr-xr-x   0        0        0     2394 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Structures/structure.rst
+-rwxr-xr-x   0        0        0     4764 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Systems/Materials.rst
+-rwxr-xr-x   0        0        0     4616 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Systems/NewMats.rst
+-rwxr-xr-x   0        0        0      256 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Systems/Units.rst
+-rwxr-xr-x   0        0        0    46832 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Systems/eg_vs_lattice_constant.png
+-rwxr-xr-x   0        0        0      284 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/Systems/systems.rst
+-rw-r--r--   0        0        0   186465 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/_static/header.png
+-rwxr-xr-x   0        0        0    10247 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/conf.py
+-rwxr-xr-x   0        0        0     1321 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/index.rst
+-rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/publications.rst
+-rwxr-xr-x   0        0        0     3309 1970-01-01 00:00:00.000000 solcore-5.9.2/docs/source/spectral/spectral.rst
+-rwxr-xr-x   0        0        0     1810 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Absorption_profile_AlGaAs_GaAs_structure.py
+-rwxr-xr-x   0        0        0     1498 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Light_sources_examples.py
+-rwxr-xr-x   0        0        0     3867 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/MJ_solar_cell_PDD_solver.py
+-rwxr-xr-x   0        0        0     5168 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/MJ_solar_cell_external_reflectance.py
+-rwxr-xr-x   0        0        0     6885 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/MJ_solar_cell_using_DA.py
+-rwxr-xr-x   0        0        0     3359 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/MJ_solar_cell_with_radiative_coupling.py
+-rwxr-xr-x   0        0        0     1678 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Materials_Eg_vs_lattice_constant.py
+-rwxr-xr-x   0        0        0     4236 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Optical_constants_CPPB_model.py
+-rwxr-xr-x   0        0        0     2154 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Optical_constants_RAT_of_ARC.py
+-rwxr-xr-x   0        0        0     1561 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Optical_constants_RAT_of_ITO_films.py
+-rwxr-xr-x   0        0        0     3585 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Optical_constants_ellipsometry_modelling.py
+-rwxr-xr-x   0        0        0     1660 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Optical_constants_ellipsometry_modelling_2.py
+-rwxr-xr-x   0        0        0     1919 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Optical_constants_using_SOPRA_db.py
+-rwxr-xr-x   0        0        0     4175 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Optics_comparison_of_models.py
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/PV_module_calculator.ipynb
+-rwxr-xr-x   0        0        0     1827 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/PV_module_calculator.py
+-rwxr-xr-x   0        0        0     2718 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Quasi3D_3J_solar_Cell.py
+-rwxr-xr-x   0        0        0     2198 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Schrodinger_QW_absorption.py
+-rwxr-xr-x   0        0        0     1452 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Schrodinger_QW_and_MQW.py
+-rwxr-xr-x   0        0        0     1091 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/Tunnel_junction.py
+-rw-r--r--   0        0        0     5653 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.ipynb
+-rwxr-xr-x   0        0        0     2756 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.py
+-rw-r--r--   0        0        0    14530 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_tutorial.ipynb
+-rwxr-xr-x   0        0        0     7250 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_tutorial.py
+-rw-r--r--   0        0        0    26801 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/differential_evolution_4Jcell.ipynb
+-rw-r--r--   0        0        0    20116 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/differential_evolution_4Jcell.py
+-rw-r--r--   0        0        0     8346 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/differential_evolution_ARC.ipynb
+-rw-r--r--   0        0        0     5673 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/advanced_examples/differential_evolution_ARC.py
+-rw-r--r--   0        0        0    14136 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/analytic_depletion_approximation.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/coherency_example.py
+-rw-r--r--   0        0        0     6826 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/coherency_example_2.py
+-rwxr-xr-x   0        0        0     2401 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/custom_materials_example.py
+-rwxr-xr-x   0        0        0     3247 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/AlInP_nk.csv
+-rwxr-xr-x   0        0        0     3684 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/GaInP_nk.csv
+-rwxr-xr-x   0        0        0     1485 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/Ge-Palik.csv
+-rwxr-xr-x   0        0        0     6758 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/Ge_nk.csv
+-rwxr-xr-x   0        0        0     4963 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/MgF-ZnS_AR.csv
+-rwxr-xr-x   0        0        0     6062 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/MgF_nk.csv
+-rwxr-xr-x   0        0        0     1008 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/Palik_GaAs_Eps1.csv
+-rwxr-xr-x   0        0        0     1692 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/Palik_GaAs_Eps2.csv
+-rwxr-xr-x   0        0        0     3730 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/SiCx_nk.csv
+-rwxr-xr-x   0        0        0    11488 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/SiGeSn_k.txt
+-rwxr-xr-x   0        0        0    11406 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/SiGeSn_n.txt
+-rwxr-xr-x   0        0        0      572 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/SiGeSn_params.txt
+-rwxr-xr-x   0        0        0     7760 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/ZnS_nk.csv
+-rwxr-xr-x   0        0        0    48480 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/ge_ellipsometry_data.dat
+-rw-r--r--   0        0        0    24952 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/ge_g_sigesn_edge_nk.mat
+-rw-r--r--   0        0        0    24957 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/ge_g_sigesn_nk.mat
+-rwxr-xr-x   0        0        0     5239 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/in01gaas.csv
+-rwxr-xr-x   0        0        0     2793 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/masks_cl.png
+-rwxr-xr-x   0        0        0     3973 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/masks_illumination.png
+-rwxr-xr-x   0        0        0      278 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/data/masks_sq.png
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/external_optics.py
+-rwxr-xr-x   0        0        0     1597 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/kp_fit_effective_masses.py
+-rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Absorption_profile_AlGaAs_GaAs_structure.ipynb
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Light_sources_examples.ipynb
+-rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/MJ_solar_cell_PDD_solver.ipynb
+-rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/MJ_solar_cell_using_DA.ipynb
+-rw-r--r--   0        0        0     4754 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/MJ_solar_cell_with_radiative_coupling.ipynb
+-rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Materials_eg_vs_lattice_constant.ipynb
+-rw-r--r--   0        0        0     7148 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Optical_constants_CPPB_model.ipynb
+-rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Optical_constants_RAT_of_ARC.ipynb
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Optical_constants_RAT_of_ITO_films.ipynb
+-rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Optical_constants_ellipsometry_modelling.ipynb
+-rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Optical_constants_ellipsometry_modelling_2.ipynb
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Optical_constants_using_SOPRA_db.ipynb
+-rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Optics_comparison_of_models.ipynb
+-rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/PDD_1Junction.ipynb
+-rwxr-xr-x   0        0        0     7187 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/QW_Absorption.ipynb
+-rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Quasi3D_3J_solar_Cell.ipynb
+-rw-r--r--   0        0        0     5085 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Schrodinger_QW_absorption.ipynb
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Schrodinger_QW_and_MQW.ipynb
+-rw-r--r--   0        0        0     2399 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/Tunnel_junction.ipynb
+-rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/coherency_example.ipynb
+-rw-r--r--   0        0        0    11693 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/coherency_example_2.ipynb
+-rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/custom_materials_example.ipynb
+-rw-r--r--   0        0        0    13578 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/external_optics.ipynb
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/kp_fit_effective_masses.ipynb
+-rw-r--r--   0        0        0     5922 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/refractiveindex_info_db_example.ipynb
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/simple_rcwa.ipynb
+-rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/notebooks/substrate_example.ipynb
+-rwxr-xr-x   0        0        0     3607 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/refractiveindex_info_db_example.py
+-rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/simple_rcwa.py
+-rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 solcore-5.9.2/examples/substrate_example.py
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 solcore-5.9.2/meson.build
+-rw-r--r--   0        0        0      244 1970-01-01 00:00:00.000000 solcore-5.9.2/meson_options.txt
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 solcore-5.9.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1812 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/__init__.py
+-rwxr-xr-x   0        0        0      871 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/__init__.py
+-rwxr-xr-x   0        0        0    17220 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/absorption_QW.py
+-rwxr-xr-x   0        0        0     7526 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/adachi_alpha.py
+-rwxr-xr-x   0        0        0    29393 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/cppm/Custom_CPPB.py
+-rwxr-xr-x   0        0        0     4337 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/cppm/Custom_CPPB_MaterialParamaters.txt
+-rwxr-xr-x   0        0        0       36 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/cppm/__init__.py
+-rwxr-xr-x   0        0        0    15170 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/dielectric_constant_models.py
+-rwxr-xr-x   0        0        0     1622 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/kramers_kronig.py
+-rwxr-xr-x   0        0        0     4642 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/nk_db.py
+-rwxr-xr-x   0        0        0    25092 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/rigorous_coupled_wave.py
+-rwxr-xr-x   0        0        0    14233 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/sopra_db.py
+-rwxr-xr-x   0        0        0    45986 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/tmm_core_vec.py
+-rwxr-xr-x   0        0        0    32049 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/absorption_calculator/transfer_matrix.py
+-rwxr-xr-x   0        0        0    10061 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/analytic_solar_cells/IV.py
+-rwxr-xr-x   0        0        0    19030 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/analytic_solar_cells/QE.py
+-rwxr-xr-x   0        0        0      417 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/analytic_solar_cells/__init__.py
+-rwxr-xr-x   0        0        0    34145 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/analytic_solar_cells/depletion_approximation.py
+-rwxr-xr-x   0        0        0     8490 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/analytic_solar_cells/detailed_balance.py
+-rwxr-xr-x   0        0        0    22602 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/analytic_solar_cells/diode_equation.py
+-rwxr-xr-x   0        0        0     7192 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/analytic_solar_cells/tunnel_junctions.py
+-rwxr-xr-x   0        0        0    20354 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/config_tools.py
+-rwxr-xr-x   0        0        0      300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/constants.py
+-rwxr-xr-x   0        0        0     3624 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/crystals.py
+-rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/data_analysis_tools/__init__.py
+-rwxr-xr-x   0        0        0    18413 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/data_analysis_tools/ellipsometry_analysis.py
+-rwxr-xr-x   0        0        0     3027 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/graphing/Colours.txt
+-rwxr-xr-x   0        0        0     4762 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/graphing/Custom_Colours.py
+-rwxr-xr-x   0        0        0       48 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/graphing/__init__.py
+-rwxr-xr-x   0        0        0    10242 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/graphing/graph.py
+-rwxr-xr-x   0        0        0     4506 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/graphing/graph_lines.py
+-rwxr-xr-x   0        0        0      555 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/graphing/graph_support.py
+-rwxr-xr-x   0        0        0    14088 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/interpolate.py
+-rwxr-xr-x   0        0        0     7260 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/light_source/SPCTRAL_si_units.txt
+-rwxr-xr-x   0        0        0      234 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/light_source/__init__.py
+-rwxr-xr-x   0        0        0    79378 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/light_source/astmg173.csv
+-rwxr-xr-x   0        0        0    22224 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/light_source/light_source.py
+-rwxr-xr-x   0        0        0    14482 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/light_source/smarts.py
+-rwxr-xr-x   0        0        0     9255 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/light_source/spectral2.py
+-rwxr-xr-x   0        0        0      876 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Adachi/binaries.txt
+-rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Adachi/ternaries.txt
+-rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlAs-Material/k.txt
+-rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlAs-Material/n.txt
+-rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/__init__.py
+-rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.000_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.099_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.198_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.315_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.419_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.491_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.590_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.700_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.804_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/1.000_AlGaAs_k.txt
+-rwxr-xr-x   0        0        0     5267 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/critical_points.txt
+-rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.000_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.099_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.198_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.315_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.419_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.491_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.590_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.700_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0    11300 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.804_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0     5150 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/1.000_AlGaAs_n.txt
+-rwxr-xr-x   0        0        0     2928 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/critical_points.txt
+-rwxr-xr-x   0        0        0      857 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/__init__.py
+-rwxr-xr-x   0        0        0     8103 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/k/0.000_AlInP_k.txt
+-rwxr-xr-x   0        0        0    15376 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/k/0.530_AlInP_k.txt
+-rwxr-xr-x   0        0        0      413 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/k/1.000_AlInP_k.txt
+-rwxr-xr-x   0        0        0      996 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/k/critical_points.txt
+-rwxr-xr-x   0        0        0     8200 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/n/0.000_AlInP_n.txt
+-rwxr-xr-x   0        0        0    30000 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/n/0.530_AlInP_n.txt
+-rwxr-xr-x   0        0        0      919 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/n/1.000_AlInP_n.txt
+-rwxr-xr-x   0        0        0      471 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/AlInP-Material/n/critical_points.txt
+-rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAs-Material/k.txt
+-rwxr-xr-x   0        0        0     5550 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAs-Material/n.txt
+-rwxr-xr-x   0        0        0      239 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAsP-Material/__init__.py
+-rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAsP-Material/k/0.000_GaAsP_k.txt
+-rwxr-xr-x   0        0        0     8200 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAsP-Material/k/1.000_GaAsP_k.txt
+-rwxr-xr-x   0        0        0      888 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAsP-Material/k/critical_points.txt
+-rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAsP-Material/n/0.000_GaAsP_n.txt
+-rwxr-xr-x   0        0        0     8250 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAsP-Material/n/1.000_GaAsP_n.txt
+-rwxr-xr-x   0        0        0      491 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaAsP-Material/n/critical_points.txt
+-rwxr-xr-x   0        0        0      472 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/__init__.py
+-rwxr-xr-x   0        0        0     8250 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/k/0.000_GaInP_k.txt
+-rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/k/0.490_GaInP_k.txt
+-rwxr-xr-x   0        0        0     8103 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/k/1.000_GaInP_k.txt
+-rwxr-xr-x   0        0        0     1055 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/k/critical_points.txt
+-rwxr-xr-x   0        0        0     8250 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/n/0.000_GaInP_n.txt
+-rwxr-xr-x   0        0        0     4900 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/n/0.490_GaInP_n.txt
+-rwxr-xr-x   0        0        0     8200 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/n/1.000_GaInP_n.txt
+-rwxr-xr-x   0        0        0      627 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaInP-Material/n/critical_points.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaSb-Material/k.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/GaSb-Material/n.txt
+-rw-r--r--   0        0        0     6606 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Ge-Material/k.txt
+-rw-r--r--   0        0        0     6281 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Ge-Material/n.txt
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/000_InGaAs.txt
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/010_InGaAs.txt
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/024_InGaAs.txt
+-rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/035_InGaAs.txt
+-rw-r--r--   0        0        0     5478 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/053_InGaAs.txt
+-rw-r--r--   0        0        0     5523 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/075_InGaAs.txt
+-rw-r--r--   0        0        0     5523 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/100_InGaAs.txt
+-rw-r--r--   0        0        0    40283 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/InGaAs_comp copy.txt
+-rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/__init__.py
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.000_Strained_InGaAs_k.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.100_Strained_InGaAs_k.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.200_Strained_InGaAs_k.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.240_Strained_InGaAs_k.txt
+-rwxr-xr-x   0        0        0     2686 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/k/critical_points.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.000_Strained_InGaAs_n.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.100_Strained_InGaAs_n.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.200_Strained_InGaAs_n.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.240_Strained_InGaAs_n.txt
+-rwxr-xr-x   0        0        0     2075 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/n/critical_points.txt
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaAs-Material/test.py
+-rwxr-xr-x   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/__init__.py
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.000_InGaSb_K.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.100_InGaSb_K.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.300_InGaSb_K.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.500_InGaSb_K.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.700_InGaSb_K.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.900_InGaSb_K.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/1.000_InGaSb_K.txt
+-rwxr-xr-x   0        0        0     3274 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/k/critical_points.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.000_InGaSb_N.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.100_InGaSb_N.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.300_InGaSb_N.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.500_InGaSb_N.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.700_InGaSb_N.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.900_InGaSb_N.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/1.000_InGaSb_N.txt
+-rwxr-xr-x   0        0        0     4776 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InGaSb-Material/n/critical_points.txt
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InP-Material/info.txt
+-rw-r--r--   0        0        0   113600 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InP-Material/k.txt
+-rw-r--r--   0        0        0   113600 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InP-Material/n.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InSb-Material/k.txt
+-rwxr-xr-x   0        0        0     6050 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/InSb-Material/n.txt
+-rwxr-xr-x   0        0        0     1122 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Levinshtein/GroupIV.txt
+-rwxr-xr-x   0        0        0     2877 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/7059.MAT
+-rwxr-xr-x   0        0        0     5843 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/AG.MAT
+-rwxr-xr-x   0        0        0      162 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/AIR.MAT
+-rwxr-xr-x   0        0        0     6133 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/AL.MAT
+-rwxr-xr-x   0        0        0     1347 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/AL2O3.MAT
+-rwxr-xr-x   0        0        0     2652 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/AL2O3P.MAT
+-rwxr-xr-x   0        0        0     4832 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS.MAT
+-rwxr-xr-x   0        0        0    10196 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS028T.MAT
+-rwxr-xr-x   0        0        0    10199 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS052T.MAT
+-rwxr-xr-x   0        0        0    10202 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS072T.MAT
+-rwxr-xr-x   0        0        0    10205 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS098T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS125T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS152T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS178T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS204T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS228T.MAT
+-rwxr-xr-x   0        0        0    10214 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS305T.MAT
+-rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS331T.MAT
+-rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS361T.MAT
+-rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS390T.MAT
+-rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS421T.MAT
+-rwxr-xr-x   0        0        0    10226 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS445T.MAT
+-rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS469T.MAT
+-rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS499T.MAT
+-rwxr-xr-x   0        0        0    10232 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS527T.MAT
+-rwxr-xr-x   0        0        0    10235 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS552T.MAT
+-rwxr-xr-x   0        0        0    10244 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS578T.MAT
+-rwxr-xr-x   0        0        0    10247 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS602T.MAT
+-rwxr-xr-x   0        0        0    10250 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS626T.MAT
+-rwxr-xr-x   0        0        0    10196 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS028T.MAT
+-rwxr-xr-x   0        0        0    10199 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS052T.MAT
+-rwxr-xr-x   0        0        0    10202 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS072T.MAT
+-rwxr-xr-x   0        0        0    10205 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS098T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS125T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS152T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS178T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS204T.MAT
+-rwxr-xr-x   0        0        0    10208 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS228T.MAT
+-rwxr-xr-x   0        0        0    10214 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS305T.MAT
+-rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS331T.MAT
+-rwxr-xr-x   0        0        0    10217 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS361T.MAT
+-rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS390T.MAT
+-rwxr-xr-x   0        0        0    10220 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS421T.MAT
+-rwxr-xr-x   0        0        0    10226 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS445T.MAT
+-rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS469T.MAT
+-rwxr-xr-x   0        0        0    10229 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS499T.MAT
+-rwxr-xr-x   0        0        0    10232 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS527T.MAT
+-rwxr-xr-x   0        0        0    10235 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS552T.MAT
+-rwxr-xr-x   0        0        0    10244 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS578T.MAT
+-rwxr-xr-x   0        0        0    10247 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS602T.MAT
+-rwxr-xr-x   0        0        0    10250 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS626T.MAT
+-rwxr-xr-x   0        0        0     6285 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALCU.MAT
+-rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS00.MAT
+-rwxr-xr-x   0        0        0    10634 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS10.MAT
+-rwxr-xr-x   0        0        0     4832 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS100.MAT
+-rwxr-xr-x   0        0        0    10643 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS20.MAT
+-rwxr-xr-x   0        0        0    10631 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS30.MAT
+-rwxr-xr-x   0        0        0    10613 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS40.MAT
+-rwxr-xr-x   0        0        0    10631 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS50.MAT
+-rwxr-xr-x   0        0        0    10628 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS60.MAT
+-rwxr-xr-x   0        0        0    10619 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS70.MAT
+-rwxr-xr-x   0        0        0    10610 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS80.MAT
+-rwxr-xr-x   0        0        0     4832 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS90.MAT
+-rwxr-xr-x   0        0        0    15051 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP00.MAT
+-rwxr-xr-x   0        0        0    15048 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP10.MAT
+-rwxr-xr-x   0        0        0    15105 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP100.MAT
+-rwxr-xr-x   0        0        0    15060 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP30.MAT
+-rwxr-xr-x   0        0        0    15075 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP60.MAT
+-rwxr-xr-x   0        0        0    15084 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP70.MAT
+-rwxr-xr-x   0        0        0     2517 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALON.MAT
+-rwxr-xr-x   0        0        0     5044 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALSB.MAT
+-rwxr-xr-x   0        0        0     5362 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALSI.MAT
+-rwxr-xr-x   0        0        0     5353 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ALSITI.MAT
+-rwxr-xr-x   0        0        0     4680 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ARACHI.MAT
+-rwxr-xr-x   0        0        0    14411 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ASI.MAT
+-rwxr-xr-x   0        0        0     5269 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/AU.MAT
+-rwxr-xr-x   0        0        0     8360 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/BAF2.MAT
+-rwxr-xr-x   0        0        0     2652 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/BK7.MAT
+-rwxr-xr-x   0        0        0     2652 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CAF2.MAT
+-rwxr-xr-x   0        0        0     2763 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CARBAM.MAT
+-rwxr-xr-x   0        0        0     3102 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CCL4.MAT
+-rwxr-xr-x   0        0        0     5870 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CDSE.MAT
+-rwxr-xr-x   0        0        0     4383 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CDTE.MAT
+-rwxr-xr-x   0        0        0     3102 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CO.MAT
+-rwxr-xr-x   0        0        0     1122 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/COR7059.MAT
+-rwxr-xr-x   0        0        0     1887 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/COSI2-4.MAT
+-rwxr-xr-x   0        0        0     5554 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CO_2.MAT
+-rwxr-xr-x   0        0        0     4680 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CR.MAT
+-rwxr-xr-x   0        0        0     2881 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CR3SI.MAT
+-rwxr-xr-x   0        0        0     2824 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CR5SI3.MAT
+-rwxr-xr-x   0        0        0     6326 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CRSI2EL2.MAT
+-rwxr-xr-x   0        0        0     5734 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CU.MAT
+-rwxr-xr-x   0        0        0     3666 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CU2O.MAT
+-rwxr-xr-x   0        0        0     3654 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/CUO.MAT
+-rwxr-xr-x   0        0        0     4980 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/DIAM.MAT
+-rwxr-xr-x   0        0        0     2280 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/FESI2EL1.MAT
+-rwxr-xr-x   0        0        0     6342 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/FESI2EL2.MAT
+-rwxr-xr-x   0        0        0     2343 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/FESI2EPI.MAT
+-rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS.MAT
+-rwxr-xr-x   0        0        0    10377 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS031T.MAT
+-rwxr-xr-x   0        0        0    10374 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS041T.MAT
+-rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS060T.MAT
+-rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS081T.MAT
+-rwxr-xr-x   0        0        0    14621 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS100.MAT
+-rwxr-xr-x   0        0        0    10368 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS103T.MAT
+-rwxr-xr-x   0        0        0    14618 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS111.MAT
+-rwxr-xr-x   0        0        0    10365 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS126T.MAT
+-rwxr-xr-x   0        0        0    10362 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS150T.MAT
+-rwxr-xr-x   0        0        0    10359 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS175T.MAT
+-rwxr-xr-x   0        0        0    10356 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS199T.MAT
+-rwxr-xr-x   0        0        0    10353 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS224T.MAT
+-rwxr-xr-x   0        0        0    10350 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS249T.MAT
+-rwxr-xr-x   0        0        0    10347 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS273T.MAT
+-rwxr-xr-x   0        0        0    10344 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS297T.MAT
+-rwxr-xr-x   0        0        0    10341 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS320T.MAT
+-rwxr-xr-x   0        0        0    10338 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS344T.MAT
+-rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS367T.MAT
+-rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS391T.MAT
+-rwxr-xr-x   0        0        0    10332 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS415T.MAT
+-rwxr-xr-x   0        0        0    10329 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS443T.MAT
+-rwxr-xr-x   0        0        0    10326 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS465T.MAT
+-rwxr-xr-x   0        0        0    10323 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS488T.MAT
+-rwxr-xr-x   0        0        0    10320 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS515T.MAT
+-rwxr-xr-x   0        0        0    10317 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS546T.MAT
+-rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS579T.MAT
+-rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS603T.MAT
+-rwxr-xr-x   0        0        0    10305 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS634T.MAT
+-rwxr-xr-x   0        0        0     4857 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAASO.MAT
+-rwxr-xr-x   0        0        0     2202 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAASOX.MAT
+-rwxr-xr-x   0        0        0    10377 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS031T.MAT
+-rwxr-xr-x   0        0        0    10374 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS041T.MAT
+-rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS060T.MAT
+-rwxr-xr-x   0        0        0    10371 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS081T.MAT
+-rwxr-xr-x   0        0        0    10368 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS103T.MAT
+-rwxr-xr-x   0        0        0    10365 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS126T.MAT
+-rwxr-xr-x   0        0        0    10362 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS150T.MAT
+-rwxr-xr-x   0        0        0    10359 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS175T.MAT
+-rwxr-xr-x   0        0        0    10356 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS199T.MAT
+-rwxr-xr-x   0        0        0    10353 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS224T.MAT
+-rwxr-xr-x   0        0        0    10350 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS249T.MAT
+-rwxr-xr-x   0        0        0    10347 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS273T.MAT
+-rwxr-xr-x   0        0        0    10344 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS297T.MAT
+-rwxr-xr-x   0        0        0    10341 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS320T.MAT
+-rwxr-xr-x   0        0        0    10338 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS344T.MAT
+-rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS367T.MAT
+-rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS391T.MAT
+-rwxr-xr-x   0        0        0    10332 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS415T.MAT
+-rwxr-xr-x   0        0        0    10329 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS443T.MAT
+-rwxr-xr-x   0        0        0    10326 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS465T.MAT
+-rwxr-xr-x   0        0        0    10323 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS488T.MAT
+-rwxr-xr-x   0        0        0    10320 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS515T.MAT
+-rwxr-xr-x   0        0        0    10317 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS546T.MAT
+-rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS579T.MAT
+-rwxr-xr-x   0        0        0    10311 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS603T.MAT
+-rwxr-xr-x   0        0        0    10305 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS634T.MAT
+-rwxr-xr-x   0        0        0    10320 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAP.MAT
+-rwxr-xr-x   0        0        0    14900 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAP100.MAT
+-rwxr-xr-x   0        0        0     2175 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GAPOX.MAT
+-rwxr-xr-x   0        0        0     4503 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GASB.MAT
+-rwxr-xr-x   0        0        0     2226 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GASBOX.MAT
+-rwxr-xr-x   0        0        0     5224 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GE.MAT
+-rwxr-xr-x   0        0        0    14363 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/GE100.MAT
+-rwxr-xr-x   0        0        0     4227 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/H2O.MAT
+-rwxr-xr-x   0        0        0     2517 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/HFO2.MAT
+-rwxr-xr-x   0        0        0     8965 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/HFSI2.MAT
+-rwxr-xr-x   0        0        0     6146 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE00.MAT
+-rwxr-xr-x   0        0        0     6182 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE20.MAT
+-rwxr-xr-x   0        0        0     6197 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE30.MAT
+-rwxr-xr-x   0        0        0     7374 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INAS.MAT
+-rwxr-xr-x   0        0        0     2220 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INASOX.MAT
+-rwxr-xr-x   0        0        0    10574 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGAAS.MAT
+-rwxr-xr-x   0        0        0     5675 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB00.MAT
+-rwxr-xr-x   0        0        0     5672 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB10.MAT
+-rwxr-xr-x   0        0        0     5720 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB100.MAT
+-rwxr-xr-x   0        0        0     5672 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB30.MAT
+-rwxr-xr-x   0        0        0     5678 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB50.MAT
+-rwxr-xr-x   0        0        0     5690 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB70.MAT
+-rwxr-xr-x   0        0        0     5708 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB90.MAT
+-rwxr-xr-x   0        0        0     5245 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INP.MAT
+-rwxr-xr-x   0        0        0     2223 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INPOX.MAT
+-rwxr-xr-x   0        0        0     9397 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INSB.MAT
+-rwxr-xr-x   0        0        0     2292 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/INSBOX.MAT
+-rwxr-xr-x   0        0        0     5674 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/IR.MAT
+-rwxr-xr-x   0        0        0     2022 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/IR3SI5E.MAT
+-rwxr-xr-x   0        0        0     2382 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/IR3SI5P.MAT
+-rwxr-xr-x   0        0        0     3060 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ITO2.MAT
+-rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/KCL.MAT
+-rwxr-xr-x   0        0        0     2382 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/LASF9.MAT
+-rwxr-xr-x   0        0        0     1113 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/LI.MAT
+-rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/LIF.MAT
+-rwxr-xr-x   0        0        0    43469 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/List_Of_Files.xlsx
+-rwxr-xr-x   0        0        0    47376 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/List_Of_Files_Updated_PDF.pdf
+-rwxr-xr-x   0        0        0     1347 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/MGF2.MAT
+-rwxr-xr-x   0        0        0    11252 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/MO.MAT
+-rwxr-xr-x   0        0        0     1707 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/MOSI2-A.MAT
+-rwxr-xr-x   0        0        0     1707 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/MOSI2-B.MAT
+-rwxr-xr-x   0        0        0     5566 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/NBSI-A.MAT
+-rwxr-xr-x   0        0        0     5569 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/NBSI-B.MAT
+-rwxr-xr-x   0        0        0     5600 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/NI.MAT
+-rwxr-xr-x   0        0        0     2746 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/NI2SI.MAT
+-rwxr-xr-x   0        0        0     2750 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/NI3SI.MAT
+-rwxr-xr-x   0        0        0     2750 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/NISI.MAT
+-rwxr-xr-x   0        0        0     5600 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/OS.MAT
+-rwxr-xr-x   0        0        0     5393 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/PBS.MAT
+-rwxr-xr-x   0        0        0     4884 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/PBSE.MAT
+-rwxr-xr-x   0        0        0     5682 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/PD.MAT
+-rwxr-xr-x   0        0        0     3288 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/PD2SI-A.MAT
+-rwxr-xr-x   0        0        0     3290 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/PD2SI-B.MAT
+-rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/PT.MAT
+-rwxr-xr-x   0        0        0    14570 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/P_SIAS.MAT
+-rwxr-xr-x   0        0        0    14546 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/P_SIUD.MAT
+-rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS00.MAT
+-rwxr-xr-x   0        0        0     5831 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS10.MAT
+-rwxr-xr-x   0        0        0     5444 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS20.MAT
+-rwxr-xr-x   0        0        0    13233 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS24.MAT
+-rwxr-xr-x   0        0        0     5662 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESI1-75.MAT
+-rwxr-xr-x   0        0        0     5224 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE100.MAT
+-rwxr-xr-x   0        0        0     6858 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE11.MAT
+-rwxr-xr-x   0        0        0     1971 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE22.MAT
+-rwxr-xr-x   0        0        0     1965 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE39.MAT
+-rwxr-xr-x   0        0        0     1959 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE51.MAT
+-rwxr-xr-x   0        0        0     1956 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE64.MAT
+-rwxr-xr-x   0        0        0     1953 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE75.MAT
+-rwxr-xr-x   0        0        0     1947 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE83.MAT
+-rwxr-xr-x   0        0        0     1947 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE91.MAT
+-rwxr-xr-x   0        0        0     5301 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RH.MAT
+-rwxr-xr-x   0        0        0     5233 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS0.MAT
+-rwxr-xr-x   0        0        0     5831 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS10.MAT
+-rwxr-xr-x   0        0        0     5444 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS20.MAT
+-rwxr-xr-x   0        0        0    13233 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS24.MAT
+-rwxr-xr-x   0        0        0     2382 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SF11.MAT
+-rwxr-xr-x   0        0        0    14806 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SI100_2.MAT
+-rwxr-xr-x   0        0        0    14806 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SI110.MAT
+-rwxr-xr-x   0        0        0    14806 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SI111.MAT
+-rwxr-xr-x   0        0        0     6739 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SI3N4.MAT
+-rwxr-xr-x   0        0        0     2640 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIAM1.MAT
+-rwxr-xr-x   0        0        0     2454 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIAM2.MAT
+-rwxr-xr-x   0        0        0     9988 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIC.MAT
+-rwxr-xr-x   0        0        0     6181 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T02.MAT
+-rwxr-xr-x   0        0        0     6175 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T10.MAT
+-rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T15.MAT
+-rwxr-xr-x   0        0        0     6172 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T20.MAT
+-rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T25.MAT
+-rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T30.MAT
+-rwxr-xr-x   0        0        0     6169 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T35.MAT
+-rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T40.MAT
+-rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T45.MAT
+-rwxr-xr-x   0        0        0    17004 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR.MAT
+-rwxr-xr-x   0        0        0     6181 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T020.MAT
+-rwxr-xr-x   0        0        0     6175 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T100.MAT
+-rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T150.MAT
+-rwxr-xr-x   0        0        0     6172 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T200.MAT
+-rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T250.MAT
+-rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T300.MAT
+-rwxr-xr-x   0        0        0     6169 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T350.MAT
+-rwxr-xr-x   0        0        0     6166 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T400.MAT
+-rwxr-xr-x   0        0        0     6163 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T450.MAT
+-rwxr-xr-x   0        0        0    14447 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_GE.MAT
+-rwxr-xr-x   0        0        0    14297 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE11.MAT
+-rwxr-xr-x   0        0        0    14336 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE20.MAT
+-rwxr-xr-x   0        0        0    14366 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE28.MAT
+-rwxr-xr-x   0        0        0    14492 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE65.MAT
+-rwxr-xr-x   0        0        0    14549 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE85.MAT
+-rwxr-xr-x   0        0        0    14567 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE98.MAT
+-rwxr-xr-x   0        0        0    14459 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI.MAT
+-rwxr-xr-x   0        0        0     2622 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIO.MAT
+-rwxr-xr-x   0        0        0     3327 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIO2.MAT
+-rwxr-xr-x   0        0        0     5149 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION0.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION20.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION40.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION60.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION80.MAT
+-rwxr-xr-x   0        0        0     5149 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION00.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION20.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION40.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION60.MAT
+-rwxr-xr-x   0        0        0     5155 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION80.MAT
+-rwxr-xr-x   0        0        0     5771 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIOP.MAT
+-rwxr-xr-x   0        0        0     4725 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY.MAT
+-rwxr-xr-x   0        0        0     5765 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY10.MAT
+-rwxr-xr-x   0        0        0     5756 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY20.MAT
+-rwxr-xr-x   0        0        0     5756 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY30.MAT
+-rwxr-xr-x   0        0        0     5747 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY40.MAT
+-rwxr-xr-x   0        0        0     5729 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY50.MAT
+-rwxr-xr-x   0        0        0     5714 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY60.MAT
+-rwxr-xr-x   0        0        0     5708 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY70.MAT
+-rwxr-xr-x   0        0        0     5693 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY80.MAT
+-rwxr-xr-x   0        0        0     5687 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY90.MAT
+-rwxr-xr-x   0        0        0     4776 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPORE.MAT
+-rwxr-xr-x   0        0        0    15495 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/SOPRA_DB_Updated.csv
+-rwxr-xr-x   0        0        0     5840 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS00.MAT
+-rwxr-xr-x   0        0        0     5834 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS10.MAT
+-rwxr-xr-x   0        0        0     5825 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS20.MAT
+-rwxr-xr-x   0        0        0     5822 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS24.MAT
+-rwxr-xr-x   0        0        0     4833 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG0.MAT
+-rwxr-xr-x   0        0        0     4824 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG06.MAT
+-rwxr-xr-x   0        0        0     4818 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG12.MAT
+-rwxr-xr-x   0        0        0     4812 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG17.MAT
+-rwxr-xr-x   0        0        0     4803 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG22.MAT
+-rwxr-xr-x   0        0        0    11076 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TA.MAT
+-rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TAOX1.MAT
+-rwxr-xr-x   0        0        0     5600 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TAOX2.MAT
+-rwxr-xr-x   0        0        0     9536 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TASI2-A.MAT
+-rwxr-xr-x   0        0        0     9551 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TASI2-B.MAT
+-rwxr-xr-x   0        0        0     4983 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TEST.MAT
+-rwxr-xr-x   0        0        0     4634 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/THF4.MAT
+-rwxr-xr-x   0        0        0     4680 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TI.MAT
+-rwxr-xr-x   0        0        0     3234 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TINI.MAT
+-rwxr-xr-x   0        0        0     6161 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TIO2.MAT
+-rwxr-xr-x   0        0        0    10335 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TIO2B.MAT
+-rwxr-xr-x   0        0        0     9739 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/TISI-A.MAT
+-rwxr-xr-x   0        0        0     5140 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/V.MAT
+-rwxr-xr-x   0        0        0     3273 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/VOID.MAT
+-rwxr-xr-x   0        0        0     4554 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/VSI2-A.MAT
+-rwxr-xr-x   0        0        0     4554 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/VSI2-B.MAT
+-rwxr-xr-x   0        0        0    11122 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/W.MAT
+-rwxr-xr-x   0        0        0     3669 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/WSI2-A.MAT
+-rwxr-xr-x   0        0        0     3654 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/WSI2-B.MAT
+-rwxr-xr-x   0        0        0     5249 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/Y2O3.MAT
+-rwxr-xr-x   0        0        0    20559 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE00.MAT
+-rwxr-xr-x   0        0        0    20550 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE10.MAT
+-rwxr-xr-x   0        0        0    20475 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE100.MAT
+-rwxr-xr-x   0        0        0    20535 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE30.MAT
+-rwxr-xr-x   0        0        0    20517 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE50.MAT
+-rwxr-xr-x   0        0        0    20499 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE70.MAT
+-rwxr-xr-x   0        0        0    20481 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE90.MAT
+-rwxr-xr-x   0        0        0     4926 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSCUB.MAT
+-rwxr-xr-x   0        0        0     5320 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSE.MAT
+-rwxr-xr-x   0        0        0    21345 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE0.MAT
+-rwxr-xr-x   0        0        0    21342 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE1.MAT
+-rwxr-xr-x   0        0        0    21564 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE10.MAT
+-rwxr-xr-x   0        0        0    21354 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE3.MAT
+-rwxr-xr-x   0        0        0    21384 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE5.MAT
+-rwxr-xr-x   0        0        0    21438 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE7.MAT
+-rwxr-xr-x   0        0        0    21513 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE9.MAT
+-rwxr-xr-x   0        0        0     2877 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZRO2.MAT
+-rwxr-xr-x   0        0        0      717 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/ZRSI2.MAT
+-rwxr-xr-x   0        0        0      195 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/SOPRA_DB/compounds.txt
+-rwxr-xr-x   0        0        0      534 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Si-Material/info.txt
+-rwxr-xr-x   0        0        0     2203 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Si-Material/k.txt
+-rwxr-xr-x   0        0        0     2203 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Si-Material/n.txt
+-rwxr-xr-x   0        0        0     7099 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Vurgaftman/binaries.txt
+-rwxr-xr-x   0        0        0     2849 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/Vurgaftman/ternaries.txt
+-rwxr-xr-x   0        0        0       40 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/__init__.py
+-rwxr-xr-x   0        0        0    15884 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/mobility.py
+-rwxr-xr-x   0        0        0     3752 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/mobility_parameters.json
+-rwxr-xr-x   0        0        0       35 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/refractiveindex_info_DB/__init__.py
+-rwxr-xr-x   0        0        0    17507 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/refractiveindex_info_DB/dbmaterial.py
+-rwxr-xr-x   0        0        0    15811 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_data/refractiveindex_info_DB/dboperations.py
+-rwxr-xr-x   0        0        0       96 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_system/__init__.py
+-rwxr-xr-x   0        0        0     2913 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_system/create_new_material.py
+-rwxr-xr-x   0        0        0     7578 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_system/critical_point_interpolate.py
+-rwxr-xr-x   0        0        0     7040 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_system/critical_point_picker.py
+-rwxr-xr-x   0        0        0    18225 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/material_system/material_system.py
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/meson.build
+-rwxr-xr-x   0        0        0      381 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/optics/__init__.py
+-rwxr-xr-x   0        0        0    10132 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/optics/beer_lambert.py
+-rwxr-xr-x   0        0        0     2435 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/optics/external_optics.py
+-rwxr-xr-x   0        0        0     7481 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/optics/rcwa.py
+-rwxr-xr-x   0        0        0     7806 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/optics/tmm.py
+-rw-r--r--   0        0        0       44 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/optimization/__init__.py
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/optimization/differential_evolution.py
+-rwxr-xr-x   0        0        0       45 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/parameter_system/__init__.py
+-rwxr-xr-x   0        0        0     1366 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/parameter_system/calculable_parameters.txt
+-rwxr-xr-x   0        0        0     7730 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/parameter_system/parameter_system.py
+-rwxr-xr-x   0        0        0    85017 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/poisson_drift_diffusion/DDmodel-current.f95
+-rwxr-xr-x   0        0        0    12628 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/poisson_drift_diffusion/DeviceStructure.py
+-rwxr-xr-x   0        0        0    20236 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/poisson_drift_diffusion/DriftDiffusionUtilities.py
+-rwxr-xr-x   0        0        0    20729 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/poisson_drift_diffusion/QWunit.py
+-rwxr-xr-x   0        0        0      442 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/poisson_drift_diffusion/__init__.py
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/poisson_drift_diffusion/meson.build
+-rwxr-xr-x   0        0        0      169 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/__init__.py
+-rwxr-xr-x   0        0        0    15768 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/graphics.py
+-rwxr-xr-x   0        0        0      329 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/heterostructure_alignment.py
+-rwxr-xr-x   0        0        0     8293 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/high_level_kp_QW.py
+-rwxr-xr-x   0        0        0    22253 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/kp_QW.py
+-rwxr-xr-x   0        0        0    17433 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/kp_bulk.py
+-rwxr-xr-x   0        0        0     8987 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/potential_utilities.py
+-rwxr-xr-x   0        0        0     6720 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/strain.py
+-rwxr-xr-x   0        0        0    13892 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/quantum_mechanics/structure_utilities.py
+-rw-r--r--   0        0        0    10861 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/registries.py
+-rwxr-xr-x   0        0        0     2989 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/science_tracker.py
+-rwxr-xr-x   0        0        0     4504 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/singleton.py
+-rwxr-xr-x   0        0        0     1989 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/smooth.py
+-rwxr-xr-x   0        0        0     6520 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/solar_cell.py
+-rwxr-xr-x   0        0        0    14521 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/solar_cell_solver.py
+-rwxr-xr-x   0        0        0     1286 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/solcore_config.txt
+-rwxr-xr-x   0        0        0     2592 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/source_managed_class.py
+-rwxr-xr-x   0        0        0      141 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/spice/__init__.py
+-rwxr-xr-x   0        0        0     7514 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/spice/pv_module_solver.py
+-rwxr-xr-x   0        0        0    14639 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/spice/quasi_3D_solver.py
+-rwxr-xr-x   0        0        0     3615 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/spice/spice.py
+-rwxr-xr-x   0        0        0     1026 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/state.py
+-rwxr-xr-x   0        0        0     7934 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/strain_balancing.py
+-rwxr-xr-x   0        0        0     8123 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/structure.py
+-rwxr-xr-x   0        0        0      928 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/units_system/Default_units.txt
+-rwxr-xr-x   0        0        0       37 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/units_system/__init__.py
+-rwxr-xr-x   0        0        0    15404 1970-01-01 00:00:00.000000 solcore-5.9.2/solcore/units_system/units_system.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     6445 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/conftest.py
+-rwxr-xr-x   0        0        0     1483 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/Ge-Palik.csv
+-rwxr-xr-x   0        0        0     4963 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/MgF-ZnS_AR.csv
+-rw-r--r--   0        0        0    11488 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/SiGeSn_k.txt
+-rw-r--r--   0        0        0    11406 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/SiGeSn_n.txt
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/SiGeSn_params.txt
+-rw-r--r--   0        0        0     3437 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/absorption_profile.txt
+-rwxr-xr-x   0        0        0     4082 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/alinp.csv
+-rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/database_materials.txt
+-rwxr-xr-x   0        0        0     5239 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/in01gaas.csv
+-rwxr-xr-x   0        0        0     4855 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/in048ga052p.csv
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/data/substrate_presence_profile.csv
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/mock_ddModel.py
+-rwxr-xr-x   0        0        0     6400 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test__pdd.py
+-rwxr-xr-x   0        0        0     9056 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_absorption.py
+-rwxr-xr-x   0        0        0      415 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_basics.py
+-rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_config_tools.py
+-rw-r--r--   0        0        0    45293 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_depletion_approximation.py
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_dielectric_constant.py
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_examples.py
+-rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_light_source.py
+-rw-r--r--   0        0        0    13063 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_optics.py
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_optimization.py
+-rwxr-xr-x   0        0        0     7196 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_qm.py
+-rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_registries.py
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_solar_cell_solver.py
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_state.py
+-rw-r--r--   0        0        0     7016 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_structure.py
+-rw-r--r--   0        0        0    68002 1970-01-01 00:00:00.000000 solcore-5.9.2/tests/test_tmm_core_vec.py
+-rw-r--r--   0        0        0    26254 1970-01-01 00:00:00.000000 solcore-5.9.2/PKG-INFO
```

### Comparing `solcore-5.9.1/.all-contributorsrc` & `solcore-5.9.2/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/.devpy/cmds.py` & `solcore-5.9.2/.devpy/cmds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 from devpy import util
-from devpy.cmds.util import get_site_packages, set_pythonpath, run
+from devpy.cmds.meson import _get_site_packages
 
 
 @click.command()
 @click.option(
     "-test-dep", is_flag=True, help="If to install test dependecies"
 )
 @click.option(
@@ -21,27 +21,27 @@
     doc_dep: bool
         Flag for installing the documentation dependencies
 
     """
     config = util.get_config()
     default_dependencies = config["project"]['dependencies']
     print("Installing dependencies", default_dependencies)
-    run(
+    util.run(
         ["pip", "install"] + list(default_dependencies),
     )
     if test_dep:
         test_dependencies = config["project.optional-dependencies"]['test']
         print("Installing test-dependencies", test_dependencies)
-        run(
+        util.run(
             ["pip", "install"] + list(test_dependencies),
         )
     if doc_dep:
         doc_dependencies = config["project.optional-dependencies"]['doc']
         print("Installing doc-dependencies", doc_dependencies)
-        run(
+        util.run(
             ["pip", "install"] + list(doc_dependencies),
         )
 
 
 @click.command()
 @click.option(
     "--build-dir", default="build", help="Build directory; default is `$PWD/build`"
@@ -56,13 +56,13 @@
     ----------
     build_dir: str
         Path of the build directory default is `$PWD/build`"
     codecov_args: bool
         codecov parameters
     """
 
-    site_path = get_site_packages(build_dir)
+    site_path = _get_site_packages()
 
-    run(
+    util.run(
         ["codecov"] + list(codecov_args),
         cwd=site_path,
-    )
+    )
```

### Comparing `solcore-5.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `solcore-5.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/.github/ISSUE_TEMPLATE/feature_request.md` & `solcore-5.9.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/.github/ISSUE_TEMPLATE/question.md` & `solcore-5.9.2/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/.github/workflows/build_deploy_wheels.yml` & `solcore-5.9.2/.github/workflows/build_deploy_wheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: 3.8
 
       - name: install-rtools needed for windows
         if: ${{ runner.os == 'Windows' }}
         run: |
-          choco install rtools --no-progress
+          choco install rtools --version=4.0.0.20220206 --no-progress --force
           echo "c:\rtools40\ucrt64\bin;" >> $env:GITHUB_PATH
 
       - name: Install cibuildwheel
         run: python -m pip install cibuildwheel==2.11.4
 
       - name: Build Solcore
         if: >-
```

### Comparing `solcore-5.9.1/.github/workflows/test_unit_and_examples.yml` & `solcore-5.9.2/.github/workflows/test_unit_and_examples.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: install-rtools
         if: matrix.os == 'windows-latest'
         run: |
-          choco install rtools --no-progress
+          choco install rtools --version=4.0.0.20220206 --no-progress --force
           echo "c:\rtools40\ucrt64\bin;" >> $env:GITHUB_PATH
 
       - name: Install system dependencies in Linux
         if: matrix.os == 'ubuntu-latest'
         run: |
           sudo apt-get update
           sudo apt install -y gfortran ngspice python3-tk libboost-all-dev libopenblas-dev libfftw3-dev libsuitesparse-dev
@@ -49,35 +49,43 @@
 
       - name: Install system dependencies in Windows
         if: matrix.os == 'windows-latest'
         run: choco install ngspice
 
       - name: Install Python dependecies
         run: |
-          pip install pytest meson-python ninja cython numpy git+https://github.com/scientific-python/devpy
+          pip install pytest meson-python ninja cython numpy git+https://github.com/scientific-python/devpy@v0.1
           python3 -m devpy install-dependencies -test-dep
 
       - name: Install S4
         if: matrix.os != 'windows-latest'
         run: |
+          pip install wheel
           git clone https://github.com/phoebe-p/S4
           cd S4
           make S4_pyext
           cd ..
           rm -rf S4    
 
       - name: Build solcore
         run: |
           python -m devpy build -- -Dwith_pdd=true -Dinstall_test=true
 
-      - name: Unit and functional tests
+      - name: Unit and functional tests (MacOS and Linux)
+        if: matrix.os != 'windows-latest'
         env:
           SOLCORE_SPICE: ngspice
         run: |
-          python -m devpy test -- -r a -v --cov=solcore/ --ignore solcore/tests/test_examples.py -n "auto"
+          python -m devpy test -- -r a -v --cov=solcore/ --ignore=solcore/tests/test_examples.py -n "auto" 
+
+      - name: Unit and functional tests (Windows)
+        if: matrix.os == 'windows-latest'
+        run: |
+          cd D:\a\solcore5\solcore5\build-install\usr\Lib\site-packages
+          python -m pytest -r a -v --ignore=solcore/tests/test_examples.py 
 
       - name: Codecov
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
         run: |
           python -m pip install codecov
           python -m devpy codecov 
@@ -100,15 +108,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: install-rtools
         if: matrix.os == 'windows-latest'
         run: |
-          choco install rtools --no-progress
+          choco install rtools --version=4.0.0.20220206 --no-progress --force
           echo "c:\rtools40\ucrt64\bin;" >> $env:GITHUB_PATH
 
       - name: Install system dependencies in Linux
         if: matrix.os == 'ubuntu-latest'
         run: |
           sudo apt-get update
           sudo apt install -y gfortran ngspice python3-tk libboost-all-dev libopenblas-dev libfftw3-dev libsuitesparse-dev
@@ -121,20 +129,21 @@
 
 #      - name: Install system dependencies in Windows
 #        if: matrix.os == 'windows-latest'
 #        run: choco install ngspice
 
       - name: Install Python dependecies
         run: |
-          pip install pytest meson-python ninja cython numpy git+https://github.com/scientific-python/devpy
+          pip install pytest meson-python ninja cython numpy git+https://github.com/scientific-python/devpy@v0.1
           python3 -m devpy install-dependencies -test-dep
 
       - name: Install S4
         if: matrix.os != 'windows-latest'
         run: |
+          pip install wheel
           git clone https://github.com/phoebe-p/S4
           cd S4
           make S4_pyext
           cd ..
           rm -rf S4    
 
       - name: Build solcore
@@ -144,11 +153,11 @@
       - name: Unit and functional tests (MacOS and Linux)
         if: matrix.os != 'windows-latest'
         env:
           SOLCORE_SPICE: ngspice
         run: |
           python -m devpy test -- -r a -v solcore/tests/test_examples.py -n "auto"
 
-      - name: Unit and functional tests (Windows)
-        if: matrix.os == 'windows-latest'
-        run: |
-          python -m devpy test -- -r a -v solcore/tests/test_examples.py -n "auto"
+#      - name: Unit and functional tests (Windows)
+#        if: matrix.os == 'windows-latest'
+#        run: |
+#          python -m devpy test -- -r a -v solcore/tests/test_examples.py
```

### Comparing `solcore-5.9.1/.gitignore` & `solcore-5.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/CHANGELOG.rst` & `solcore-5.9.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/CODE_OF_CONDUCT.md` & `solcore-5.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/CONTRIBUTING.md` & `solcore-5.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/GNU-LGPL.txt` & `solcore-5.9.2/GNU-LGPL.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/LICENSE.txt` & `solcore-5.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/README.md` & `solcore-5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/build_tools/cibw_before_build_macos_arm.sh` & `solcore-5.9.2/build_tools/cibw_before_build_macos_arm.sh`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/Makefile` & `solcore-5.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/make.bat` & `solcore-5.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/Ag_GaAs_abs.png` & `solcore-5.9.2/docs/source/Examples/Ag_GaAs_abs.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/Ag_k.png` & `solcore-5.9.2/docs/source/Examples/Ag_k.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/Ag_n.png` & `solcore-5.9.2/docs/source/Examples/Ag_n.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/DA_iv.png` & `solcore-5.9.2/docs/source/Examples/DA_iv.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/DA_iv2.png` & `solcore-5.9.2/docs/source/Examples/DA_iv2.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/DA_qe.png` & `solcore-5.9.2/docs/source/Examples/DA_qe.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/Diamond_nk.png` & `solcore-5.9.2/docs/source/Examples/Diamond_nk.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/IV_param_dispersion.png` & `solcore-5.9.2/docs/source/Examples/IV_param_dispersion.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/IV_solar_module.png` & `solcore-5.9.2/docs/source/Examples/IV_solar_module.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/MJ_IV_optimal.png` & `solcore-5.9.2/docs/source/Examples/MJ_IV_optimal.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/MJ_efficiency_map.png` & `solcore-5.9.2/docs/source/Examples/MJ_efficiency_map.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/MJ_with_rad_coupling.png` & `solcore-5.9.2/docs/source/Examples/MJ_with_rad_coupling.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/MQW_LDOS.png` & `solcore-5.9.2/docs/source/Examples/MQW_LDOS.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/PDD_IV.png` & `solcore-5.9.2/docs/source/Examples/PDD_IV.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/PDD_carrier_density.png` & `solcore-5.9.2/docs/source/Examples/PDD_carrier_density.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/PDD_qe.png` & `solcore-5.9.2/docs/source/Examples/PDD_qe.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/RAT_of_ARC.png` & `solcore-5.9.2/docs/source/Examples/RAT_of_ARC.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/SiGeSn_nk.png` & `solcore-5.9.2/docs/source/Examples/SiGeSn_nk.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/Single_QW.png` & `solcore-5.9.2/docs/source/Examples/Single_QW.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/circular_mask_IV.png` & `solcore-5.9.2/docs/source/Examples/circular_mask_IV.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/circular_mask_V1_3.png` & `solcore-5.9.2/docs/source/Examples/circular_mask_V1_3.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/custom_materials_example.rst` & `solcore-5.9.2/docs/source/Examples/custom_materials_example.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/eff_mass_fit.png` & `solcore-5.9.2/docs/source/Examples/eff_mass_fit.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_3J_with_DA_solver.rst` & `solcore-5.9.2/docs/source/Examples/example_3J_with_DA_solver.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_K_and_effective_mass.rst` & `solcore-5.9.2/docs/source/Examples/example_K_and_effective_mass.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_MJ_efficiency_map.rst` & `solcore-5.9.2/docs/source/Examples/example_MJ_efficiency_map.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_PDD_solver.rst` & `solcore-5.9.2/docs/source/Examples/example_PDD_solver.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_QWs.rst` & `solcore-5.9.2/docs/source/Examples/example_QWs.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_RAT_of_ARC.rst` & `solcore-5.9.2/docs/source/Examples/example_RAT_of_ARC.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_light_sources.rst` & `solcore-5.9.2/docs/source/Examples/example_light_sources.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_optics_comparison.rst` & `solcore-5.9.2/docs/source/Examples/example_optics_comparison.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_pv_module.rst` & `solcore-5.9.2/docs/source/Examples/example_pv_module.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_quasi3D_cell.rst` & `solcore-5.9.2/docs/source/Examples/example_quasi3D_cell.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_radiative_coupling.rst` & `solcore-5.9.2/docs/source/Examples/example_radiative_coupling.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_substrate.rst` & `solcore-5.9.2/docs/source/Examples/example_substrate.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/example_tunnel_junction.rst` & `solcore-5.9.2/docs/source/Examples/example_tunnel_junction.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/iv.jpg` & `solcore-5.9.2/docs/source/Examples/iv.jpg`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/iv_params.jpg` & `solcore-5.9.2/docs/source/Examples/iv_params.jpg`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/kp.png` & `solcore-5.9.2/docs/source/Examples/kp.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/ls_compare.png` & `solcore-5.9.2/docs/source/Examples/ls_compare.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/ls_smarts.png` & `solcore-5.9.2/docs/source/Examples/ls_smarts.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/main.rst` & `solcore-5.9.2/docs/source/Examples/main.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/optmodelcomp.png` & `solcore-5.9.2/docs/source/Examples/optmodelcomp.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/qe.jpg` & `solcore-5.9.2/docs/source/Examples/qe.jpg`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/refractiveindex_info_db_example.rst` & `solcore-5.9.2/docs/source/Examples/refractiveindex_info_db_example.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/square_mask_IV.png` & `solcore-5.9.2/docs/source/Examples/square_mask_IV.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/square_mask_V1_3.png` & `solcore-5.9.2/docs/source/Examples/square_mask_V1_3.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/substrate_Adepth.png` & `solcore-5.9.2/docs/source/Examples/substrate_Adepth.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/substrate_RAT.png` & `solcore-5.9.2/docs/source/Examples/substrate_RAT.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/tunnel_junction.png` & `solcore-5.9.2/docs/source/Examples/tunnel_junction.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Examples/tutorial.rst` & `solcore-5.9.2/docs/source/Examples/tutorial.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Infographics.jpg` & `solcore-5.9.2/docs/source/Infographics.jpg`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Installation/Solcore_on_MacOSX.md` & `solcore-5.9.2/docs/source/Installation/Solcore_on_MacOSX.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Installation/Solcore_on_Windows.md` & `solcore-5.9.2/docs/source/Installation/Solcore_on_Windows.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Installation/compilation.md` & `solcore-5.9.2/docs/source/Installation/compilation.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Installation/installation.rst` & `solcore-5.9.2/docs/source/Installation/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,43 @@
 
 Trying Solcore
 ^^^^^^^^^^^^^^
 
 You can try Solcore without installing anything in your computer by using the online service `MyBinder.org <https://mybinder.org/>`_. To do so, just click in the following badge:
 
 .. image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/qpv-research-group/solcore5/devel
+ :target: https://mybinder.org/v2/gh/qpv-research-group/solcore5/develop
 
 It might take a few minutes to start the server. Be patient! Once launched, this service offers a full-feature Jupyter server with Solcore and all its dependencies installed on it. You can use it to try different features and run the examples shipped with Solcore, but it is not recommended for production: resources in MyBinder are limited and the execution depends on a reliable internet connexion.
 
 Once you are ready to install it in your own machine, go to the next section.
 
 Installing Solcore
 ^^^^^^^^^^^^^^^^^^
 The only requirement for installing Solcore is having Python version 3.7 or higher (Python 3.8 or higher if you are installing
 on a MacOS device with an ARM/Apple M1 chip). Installing Solcore (version 5.9 onwards) should be as easy as running the
 following command in your terminal::
 
     pip install solcore
 
-This will download Solcore form the PyPI repository and install the package within the active Python environment. Depending
+This will download Solcore from the PyPI repository and install the package within the
+active Python environment. Depending
 on your operating system/Python installation you may need to use `pip3` instead of `pip`. And that's all! Solcore should
 be available to be used as with any Python package::
 
     >>> import solcore
 
+Note that the above should install the Fortran-based Poisson drift-diffusion (PDD)
+solver, without requiring local compilation (i.e. you do not need to have Fortran
+compiler installed on your computer -- see further details below). If you would like to
+install Solcore without
+the PDD solver, you can do so by running::
+
+    pip install solcore --config-setting=setup-args="-Dwith_pdd=false"
+
 Installation details
 ^^^^^^^^^^^^^^^^^^^^
 
 Solcore is written mostly in Python, but the Poisson-Drift-diffusion (PDD) solver is written in Fortran to make it more efficient,
 and the RCWA (rigorous coupled-wave analysis) solver uses the package `S4 <https://web.stanford.edu/group/fan/S4/>`_ which
 is written in C++. Solcore uses pre-built
 binary wheels for the PDD solver to make installation as easy as possible (these are built for Windows, Linux, and MacOS,
@@ -47,25 +56,29 @@
 Alternatively, you can `download the source from the Solcore GitHub repository <https://github.com/qpv-research-group/solcore5>`_,
 either using `git clone` or as a zip file using one of the links on the right. If you want to install it, unpack it and
 run from the directory where *pyproject.toml* is located::
 
     pip install .
 
 This will compile the PDD solver locally, so you will need to have a
-:doc:`a suitable Fortran compiler (only needed for the PDD solver) <compilation>`.
+:doc:`a suitable Fortran compiler (only needed for the PDD solver) <compilation>`. If
+you wish to install Solcore from source without compiling the PDD solver, you can do so by running::
+
+    pip install . --config-setting=setup-args="-Dwith_pdd=false"
 
 
 Installing in development mode
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you are planning to develop Solcore further, you may want to have all the files in an accessible place (as opposed to
 the default installation location for pip), while still being able to use the package from other places and examples, so
 that if you make changes to the solcore5 folder those changes will be reflected in installed versions of the package.
 To achieve this, you need to install Solcore in editable/development mode. Download or clone the source from the
-`Solcore GitHub repository <https://github.com/dalonsoa/solcore5>`_ as above, make sure the dependencies are installed
+`Solcore GitHub repository <https://github.com/dalonsoa/solcore5>`_ as above, and make
+sure the dependencies are installed
 (the easiest way to do this is to run `pip install solcore`, which will install Solcore with dependencies as usual,
 followed by `pip uninstall solcore`). In the folder where *pyproject.toml* is located run::
 
     pip install meson-python==0.13.0rc0 cython ninja
     pip install -e . --no-build-isolation --no-deps
 
 If you are developing Solcore using Git/GitHub, we recommend you use *pre-commit* to do a few things before committing changes
```

### Comparing `solcore-5.9.1/docs/source/Installation/s4_installation.md` & `solcore-5.9.2/docs/source/Installation/s4_installation.md`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Optics/material_optics.rst` & `solcore-5.9.2/docs/source/Optics/material_optics.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Optics/other_methods.rst` & `solcore-5.9.2/docs/source/Optics/other_methods.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Optics/qw_absorption.png` & `solcore-5.9.2/docs/source/Optics/qw_absorption.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Optics/qw_absorption.rst` & `solcore-5.9.2/docs/source/Optics/qw_absorption.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Optics/rcwa.rst` & `solcore-5.9.2/docs/source/Optics/rcwa.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Optics/tmm.rst` & `solcore-5.9.2/docs/source/Optics/tmm.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/QM/Schrodinger.rst` & `solcore-5.9.2/docs/source/QM/Schrodinger.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Quasi3D/pv_module.png` & `solcore-5.9.2/docs/source/Quasi3D/pv_module.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Quasi3D/pv_panel.rst` & `solcore-5.9.2/docs/source/Quasi3D/pv_panel.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Quasi3D/quasi3D.rst` & `solcore-5.9.2/docs/source/Quasi3D/quasi3D.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Quasi3D/quasi3Dimg.png` & `solcore-5.9.2/docs/source/Quasi3D/quasi3Dimg.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Quasi3D/spice.rst` & `solcore-5.9.2/docs/source/Quasi3D/spice.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/ASC.rst` & `solcore-5.9.2/docs/source/Solvers/ASC.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/DDsolver.rst` & `solcore-5.9.2/docs/source/Solvers/DDsolver.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/DeviceStructure.rst` & `solcore-5.9.2/docs/source/Solvers/DeviceStructure.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/DriftDiffusionUtilities.rst` & `solcore-5.9.2/docs/source/Solvers/DriftDiffusionUtilities.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/EQandSC.png` & `solcore-5.9.2/docs/source/Solvers/Figures/EQandSC.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/IV.png` & `solcore-5.9.2/docs/source/Solvers/Figures/IV.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/LightIV.png` & `solcore-5.9.2/docs/source/Solvers/Figures/LightIV.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/MeshDescription.svg` & `solcore-5.9.2/docs/source/Solvers/Figures/MeshDescription.svg`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/QE.png` & `solcore-5.9.2/docs/source/Solvers/Figures/QE.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/QWunit.png` & `solcore-5.9.2/docs/source/Solvers/Figures/QWunit.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/iv_mj.png` & `solcore-5.9.2/docs/source/Solvers/Figures/iv_mj.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/mesh.png` & `solcore-5.9.2/docs/source/Solvers/Figures/mesh.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/Figures/qe_mj.png` & `solcore-5.9.2/docs/source/Solvers/Figures/qe_mj.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/QWunit.rst` & `solcore-5.9.2/docs/source/Solvers/QWunit.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/TwoDiode.rst` & `solcore-5.9.2/docs/source/Solvers/TwoDiode.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/depletion.rst` & `solcore-5.9.2/docs/source/Solvers/depletion.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/detailed_balance.rst` & `solcore-5.9.2/docs/source/Solvers/detailed_balance.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/multijunction_iv.rst` & `solcore-5.9.2/docs/source/Solvers/multijunction_iv.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Solvers/solving_solar_cells.rst` & `solcore-5.9.2/docs/source/Solvers/solving_solar_cells.rst`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     - **pol** = 'u'
 
 - :doc:`Detailed balance solver options <detailed_balance>`
     - **db_mode** = 'boltzmann'
         If the Boltzmann approximation should be used in the detailed balance solver. Any other choice will result in using the full Plank equation, which will be slower, in general.
 
 - :doc:`Depletion approximation solver options <depletion>`
-    - **da_mode** = 'bvp'
+    - **da_mode** = 'green'
         Selects the numerical approximation method for the drift-diffusion equation in the depletion approximation solver. Possible values are “bvp” for numerical solution using the `solve_bvp` method of the `scipy.integrate` module or 'green' for a semi-analytic solution using Green's functions. The latter is expected to be faster. 
 
 - :doc:`Poisson-drift diffusion solver options <DriftDiffusionUtilities>`
     Check the PDD section for details on this parameters.
 
     - Mesh control
         - **meshpoints** = -400
```

### Comparing `solcore-5.9.1/docs/source/Structures/structure.rst` & `solcore-5.9.2/docs/source/Structures/structure.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Systems/Materials.rst` & `solcore-5.9.2/docs/source/Systems/Materials.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Systems/NewMats.rst` & `solcore-5.9.2/docs/source/Systems/NewMats.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/Systems/eg_vs_lattice_constant.png` & `solcore-5.9.2/docs/source/Systems/eg_vs_lattice_constant.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/_static/header.png` & `solcore-5.9.2/docs/source/_static/header.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/docs/source/conf.py` & `solcore-5.9.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # print(solcore_root)
 #
 # sys.path.append(solcore_root)
 # default_config = os.path.join(solcore_root, 'solcore', 'solcore_config.txt')
 # config = ConfigParser()
 # config.read([default_config, ])
 # __version__ = config.get('Configuration', 'version')
-__version__ = '5.9.1'
+__version__ = '5.9.2'
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration ------------------------------------------------
```

### Comparing `solcore-5.9.1/docs/source/index.rst` & `solcore-5.9.2/docs/source/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 .. image:: _static/header.png
     :align: center
 
 :literal:`Solcore` was born as a modular set of tools, written (almost) entirely in Python 3, to address some of the task we had to solve more often, such as fitting dark IV curves or luminescence decays. With time, however,  it has evolved as a complete semiconductor solver able of modelling the optical and electrical properties of a wide range of solar cells, from quantum well devices to multi-junction solar cells. A compact description of Solcore's functionality and physics can be found in the open access publication:
 
 `D. Alonso-Álvarez, T. Wilson, P. Pearce, M. Führer, D. Farrell, N. Ekins-Daukes, Journal of Computational Electronics (2018) <https://doi.org/10.1007/s10825-018-1171-3>`_.
 
-Please, cite this article if you find Solcore useful for your research.
+Please, cite this article if you find Solcore useful for your research. A list of papers
+which have used Solcore can be found :ref:`here<publications>`.
 
 .. image:: Infographics.jpg
     :align: center
 
 
 Contents:
 ---------
```

### Comparing `solcore-5.9.1/docs/source/spectral/spectral.rst` & `solcore-5.9.2/docs/source/spectral/spectral.rst`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Absorption_profile_AlGaAs_GaAs_structure.py` & `solcore-5.9.2/examples/Absorption_profile_AlGaAs_GaAs_structure.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Light_sources_examples.py` & `solcore-5.9.2/examples/Light_sources_examples.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/MJ_solar_cell_PDD_solver.py` & `solcore-5.9.2/examples/MJ_solar_cell_PDD_solver.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/MJ_solar_cell_using_DA.py` & `solcore-5.9.2/examples/MJ_solar_cell_external_reflectance.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,63 +11,73 @@
 
 def this_dir_file(f):
     return "data/" + f
 
 # We need to build the solar cell layer by layer.
 # We start from the AR coating. In this case, we load it from an an external file
 refl_nm = np.loadtxt(this_dir_file("MgF-ZnS_AR.csv"), unpack=True, delimiter=",")
-ref = interp1d(x=siUnits(refl_nm[0], "nm"), y=refl_nm[1], bounds_error=False, fill_value=0)
+ref = interp1d(x=siUnits(refl_nm[0], "nm"), y=refl_nm[1],
+               bounds_error=False, fill_value=0)
 
 # TOP CELL - GaInP
-# Now we build the top cell, which requires the n and p sides of GaInP and a window layer.
-# We also load the absorption coefficient from an external file. We also add some extra parameters needed for the
-# calculation such as the minority carriers diffusion lengths
+# Now we build the top cell, which requires the n and p sides of GaInP and a window
+# layer. We also load the absorption coefficient from an external file. We also add
+# some extra parameters needed for the calculation such as the minority carriers
+# diffusion lengths
 AlInP = material("AlInP")
 InGaP = material("GaInP")
 window_material = AlInP(Al=0.52)
-top_cell_n_material = InGaP(In=0.49, Nd=siUnits(2e18, "cm-3"), hole_diffusion_length=si("200nm"))
-top_cell_p_material = InGaP(In=0.49, Na=siUnits(1e17, "cm-3"), electron_diffusion_length=si("1um"))
+top_cell_n_material = InGaP(In=0.49, Nd=siUnits(2e18, "cm-3"),
+                            hole_diffusion_length=si("200nm"))
+top_cell_p_material = InGaP(In=0.49, Na=siUnits(1e17, "cm-3"),
+                            electron_diffusion_length=si("1um"))
 
 all_materials.append(window_material)
 all_materials.append(top_cell_n_material)
 all_materials.append(top_cell_p_material)
 
 # MID CELL  - InGaAs
-# We add manually the absorption coefficient of InGaAs since the one contained in the database doesn't cover
-# enough range, keeping in mind that the data has to be provided as a function that takes wavelengths (m) as input and
+# We add manually the absorption coefficient of InGaAs since the one contained in the
+# database doesn't cover enough range, keeping in mind that the data has to be
+# provided as a function that takes wavelengths (m) as input and
 # returns absorption (1/m)
 InGaAs = material("InGaAs")
 InGaAs_alpha = np.loadtxt(this_dir_file("in01gaas.csv"), unpack=True, delimiter=",")
-InGaAs.alpha = interp1d(x=1240e-9 / InGaAs_alpha[0][::-1], y=InGaAs_alpha[1][::-1], bounds_error=False, fill_value=0)
+InGaAs.alpha = interp1d(x=1240e-9 / InGaAs_alpha[0][::-1],
+                        y=InGaAs_alpha[1][::-1], bounds_error=False, fill_value=0)
 
-mid_cell_n_material = InGaAs(In=0.01, Nd=siUnits(3e18, "cm-3"), hole_diffusion_length=si("500nm"))
-mid_cell_p_material = InGaAs(In=0.01, Na=siUnits(1e17, "cm-3"), electron_diffusion_length=si("5um"))
+mid_cell_n_material = InGaAs(In=0.01, Nd=siUnits(3e18, "cm-3"),
+                             hole_diffusion_length=si("500nm"))
+mid_cell_p_material = InGaAs(In=0.01, Na=siUnits(1e17, "cm-3"),
+                             electron_diffusion_length=si("5um"))
 
 all_materials.append(mid_cell_n_material)
 all_materials.append(mid_cell_p_material)
 
 # BOTTOM CELL - Ge
 Ge = material("Ge")
 
 bot_cell_n_material = Ge(Nd=siUnits(2e18, "cm-3"), hole_diffusion_length=si("800nm"))
 bot_cell_p_material = Ge(Na=siUnits(1e17, "cm-3"), electron_diffusion_length=si("50um"))
 
 all_materials.append(bot_cell_n_material)
 all_materials.append(bot_cell_p_material)
 
-# We add some other properties to the materials, assumed the same in all cases, for simplicity.
-# If different, we should have added them above in the definition of the materials.
+# We add some other properties to the materials, assumed the same in all cases, for
+# simplicity. If different, we should have added them above in the definition of the
+# materials.
 for mat in all_materials:
     mat.hole_mobility = 5e-2
     mat.electron_mobility = 3.4e-3
     mat.hole_mobility = 3.4e-3
     mat.electron_mobility = 5e-2
 
-# And, finally, we put everything together, adding also the surface recombination velocities. We also add some shading
-# due to the metallisation of the cell = 8%, and indicate it has an area of 0.7x0.7 mm2 (converted to m2)
+# And, finally, we put everything together, adding also the surface recombination
+# velocities. We also add some shading due to the metallisation of the cell = 8%,
+# and indicate it has an area of 0.7x0.7 mm2 (converted to m2)
 solar_cell = SolarCell(
     [
         Junction([Layer(si("25nm"), material=window_material, role='window'),
                   Layer(si("100nm"), material=top_cell_n_material, role='emitter'),
                   Layer(si("600nm"), material=top_cell_p_material, role='base'),
                   ], sn=1, sp=1, kind='DA'),
         Junction([Layer(si("200nm"), material=mid_cell_n_material, role='emitter'),
@@ -75,29 +85,34 @@
                   ], sn=1, sp=1, kind='DA'),
         Junction([Layer(si("400nm"), material=bot_cell_n_material, role='emitter'),
                   Layer(si("100um"), material=bot_cell_p_material, role='base'),
                   ], sn=1, sp=1, kind='DA'),
     ], reflectivity=ref, shading=0.08, cell_area=0.7 * 0.7 / 1e4)
 
 wl = np.linspace(300, 1800, 700) * 1e-9
-solar_cell_solver(solar_cell, 'qe', user_options={'wavelength': wl})
+solar_cell_solver(solar_cell, 'qe', user_options={'wavelength': wl,
+                                                  'da_mode': 'green'})
 
 plt.figure(1)
 plt.plot(wl * 1e9, solar_cell[0].eqe(wl) * 100, 'b', label='GaInP')
 plt.plot(wl * 1e9, solar_cell[1].eqe(wl) * 100, 'g', label='InGaAs')
 plt.plot(wl * 1e9, solar_cell[2].eqe(wl) * 100, 'r', label='Ge')
 
 plt.legend()
 plt.ylim(0, 100)
 plt.ylabel('EQE (%)')
 plt.xlabel('Wavelength (nm)')
 plt.show()
 
 V = np.linspace(0, 3, 300)
-solar_cell_solver(solar_cell, 'iv', user_options={'voltages': V, 'light_iv': True, 'wavelength': wl})
+solar_cell_solver(solar_cell, 'iv', user_options={'voltages': V,
+                                                  'light_iv': True,
+                                                  'wavelength': wl,
+                                                  'da_mode': 'green'
+                                                  })
 
 plt.figure(2)
 plt.plot(V, solar_cell.iv['IV'][1], 'k', linewidth=3, label='Total')
 plt.plot(V, -solar_cell[0].iv(V), 'b', label='GaInP')
 plt.plot(V, -solar_cell[1].iv(V), 'g', label='InGaAs')
 plt.plot(V, -solar_cell[2].iv(V), 'r', label='Ge')
```

### Comparing `solcore-5.9.1/examples/MJ_solar_cell_with_radiative_coupling.py` & `solcore-5.9.2/examples/MJ_solar_cell_with_radiative_coupling.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Materials_Eg_vs_lattice_constant.py` & `solcore-5.9.2/examples/Materials_Eg_vs_lattice_constant.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Optical_constants_CPPB_model.py` & `solcore-5.9.2/examples/Optical_constants_CPPB_model.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Optical_constants_RAT_of_ARC.py` & `solcore-5.9.2/examples/Optical_constants_RAT_of_ARC.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Optical_constants_RAT_of_ITO_films.py` & `solcore-5.9.2/examples/Optical_constants_RAT_of_ITO_films.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Optical_constants_ellipsometry_modelling.py` & `solcore-5.9.2/examples/Optical_constants_ellipsometry_modelling.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Optical_constants_ellipsometry_modelling_2.py` & `solcore-5.9.2/examples/Optical_constants_ellipsometry_modelling_2.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Optical_constants_using_SOPRA_db.py` & `solcore-5.9.2/examples/Optical_constants_using_SOPRA_db.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Optics_comparison_of_models.py` & `solcore-5.9.2/examples/Optics_comparison_of_models.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/PV_module_calculator.ipynb` & `solcore-5.9.2/examples/PV_module_calculator.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/PV_module_calculator.py` & `solcore-5.9.2/examples/PV_module_calculator.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Quasi3D_3J_solar_Cell.py` & `solcore-5.9.2/examples/Quasi3D_3J_solar_Cell.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Schrodinger_QW_absorption.py` & `solcore-5.9.2/examples/Schrodinger_QW_absorption.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Schrodinger_QW_and_MQW.py` & `solcore-5.9.2/examples/Schrodinger_QW_and_MQW.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/Tunnel_junction.py` & `solcore-5.9.2/examples/Tunnel_junction.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.ipynb` & `solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.py` & `solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_3J_efficiency_map.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_tutorial.ipynb` & `solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/MJ_solar_cell_tutorial.py` & `solcore-5.9.2/examples/advanced_examples/MJ_solar_cell_tutorial.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/differential_evolution_4Jcell.ipynb` & `solcore-5.9.2/examples/advanced_examples/differential_evolution_4Jcell.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/differential_evolution_4Jcell.py` & `solcore-5.9.2/examples/advanced_examples/differential_evolution_4Jcell.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/differential_evolution_ARC.ipynb` & `solcore-5.9.2/examples/advanced_examples/differential_evolution_ARC.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/advanced_examples/differential_evolution_ARC.py` & `solcore-5.9.2/examples/advanced_examples/differential_evolution_ARC.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/coherency_example.py` & `solcore-5.9.2/examples/coherency_example.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/coherency_example_2.py` & `solcore-5.9.2/examples/coherency_example_2.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/custom_materials_example.py` & `solcore-5.9.2/examples/custom_materials_example.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/AlInP_nk.csv` & `solcore-5.9.2/examples/data/AlInP_nk.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/GaInP_nk.csv` & `solcore-5.9.2/examples/data/GaInP_nk.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/Ge-Palik.csv` & `solcore-5.9.2/examples/data/Ge-Palik.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/Ge_nk.csv` & `solcore-5.9.2/examples/data/Ge_nk.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/MgF-ZnS_AR.csv` & `solcore-5.9.2/examples/data/MgF-ZnS_AR.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/MgF_nk.csv` & `solcore-5.9.2/examples/data/MgF_nk.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/Palik_GaAs_Eps1.csv` & `solcore-5.9.2/examples/data/Palik_GaAs_Eps1.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/Palik_GaAs_Eps2.csv` & `solcore-5.9.2/examples/data/Palik_GaAs_Eps2.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/SiCx_nk.csv` & `solcore-5.9.2/examples/data/SiCx_nk.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/SiGeSn_k.txt` & `solcore-5.9.2/examples/data/SiGeSn_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/SiGeSn_n.txt` & `solcore-5.9.2/examples/data/SiGeSn_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/SiGeSn_params.txt` & `solcore-5.9.2/examples/data/SiGeSn_params.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/ZnS_nk.csv` & `solcore-5.9.2/examples/data/ZnS_nk.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/ge_ellipsometry_data.dat` & `solcore-5.9.2/examples/data/ge_ellipsometry_data.dat`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/ge_g_sigesn_edge_nk.mat` & `solcore-5.9.2/examples/data/ge_g_sigesn_edge_nk.mat`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/ge_g_sigesn_nk.mat` & `solcore-5.9.2/examples/data/ge_g_sigesn_nk.mat`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/in01gaas.csv` & `solcore-5.9.2/examples/data/in01gaas.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/masks_cl.png` & `solcore-5.9.2/examples/data/masks_cl.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/data/masks_illumination.png` & `solcore-5.9.2/examples/data/masks_illumination.png`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/external_optics.py` & `solcore-5.9.2/examples/external_optics.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/kp_fit_effective_masses.py` & `solcore-5.9.2/examples/kp_fit_effective_masses.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Absorption_profile_AlGaAs_GaAs_structure.ipynb` & `solcore-5.9.2/examples/notebooks/Absorption_profile_AlGaAs_GaAs_structure.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Light_sources_examples.ipynb` & `solcore-5.9.2/examples/notebooks/Light_sources_examples.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/MJ_solar_cell_PDD_solver.ipynb` & `solcore-5.9.2/examples/notebooks/MJ_solar_cell_PDD_solver.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/MJ_solar_cell_using_DA.ipynb` & `solcore-5.9.2/examples/notebooks/MJ_solar_cell_using_DA.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/MJ_solar_cell_with_radiative_coupling.ipynb` & `solcore-5.9.2/examples/notebooks/MJ_solar_cell_with_radiative_coupling.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Materials_eg_vs_lattice_constant.ipynb` & `solcore-5.9.2/examples/notebooks/Materials_eg_vs_lattice_constant.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Optical_constants_CPPB_model.ipynb` & `solcore-5.9.2/examples/notebooks/Optical_constants_CPPB_model.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Optical_constants_RAT_of_ARC.ipynb` & `solcore-5.9.2/examples/notebooks/Optical_constants_RAT_of_ARC.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Optical_constants_RAT_of_ITO_films.ipynb` & `solcore-5.9.2/examples/notebooks/Optical_constants_RAT_of_ITO_films.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Optical_constants_ellipsometry_modelling.ipynb` & `solcore-5.9.2/examples/notebooks/Optical_constants_ellipsometry_modelling.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Optical_constants_ellipsometry_modelling_2.ipynb` & `solcore-5.9.2/examples/notebooks/Optical_constants_ellipsometry_modelling_2.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Optical_constants_using_SOPRA_db.ipynb` & `solcore-5.9.2/examples/notebooks/Optical_constants_using_SOPRA_db.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Optics_comparison_of_models.ipynb` & `solcore-5.9.2/examples/notebooks/Optics_comparison_of_models.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/PDD_1Junction.ipynb` & `solcore-5.9.2/examples/notebooks/PDD_1Junction.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/QW_Absorption.ipynb` & `solcore-5.9.2/examples/notebooks/QW_Absorption.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Quasi3D_3J_solar_Cell.ipynb` & `solcore-5.9.2/examples/notebooks/Quasi3D_3J_solar_Cell.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Schrodinger_QW_absorption.ipynb` & `solcore-5.9.2/examples/notebooks/Schrodinger_QW_absorption.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Schrodinger_QW_and_MQW.ipynb` & `solcore-5.9.2/examples/notebooks/Schrodinger_QW_and_MQW.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/Tunnel_junction.ipynb` & `solcore-5.9.2/examples/notebooks/Tunnel_junction.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/coherency_example.ipynb` & `solcore-5.9.2/examples/notebooks/coherency_example.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/coherency_example_2.ipynb` & `solcore-5.9.2/examples/notebooks/coherency_example_2.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/custom_materials_example.ipynb` & `solcore-5.9.2/examples/notebooks/custom_materials_example.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/external_optics.ipynb` & `solcore-5.9.2/examples/notebooks/external_optics.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/kp_fit_effective_masses.ipynb` & `solcore-5.9.2/examples/notebooks/kp_fit_effective_masses.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/refractiveindex_info_db_example.ipynb` & `solcore-5.9.2/examples/notebooks/refractiveindex_info_db_example.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/simple_rcwa.ipynb` & `solcore-5.9.2/examples/notebooks/simple_rcwa.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/notebooks/substrate_example.ipynb` & `solcore-5.9.2/examples/notebooks/substrate_example.ipynb`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/refractiveindex_info_db_example.py` & `solcore-5.9.2/examples/refractiveindex_info_db_example.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/simple_rcwa.py` & `solcore-5.9.2/examples/simple_rcwa.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/examples/substrate_example.py` & `solcore-5.9.2/examples/substrate_example.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/pyproject.toml` & `solcore-5.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics",
     ]
 dependencies = [
-    "numpy",
+    "numpy>=1.21.0",
     "matplotlib",
     "scipy",
     "tmm",
     "natsort",
     "regex",
     "cycler",
     "pyyaml",
@@ -63,15 +63,15 @@
 
 dev = ["pre-commit"]
 
 [tool.devpy]
 package = 'solcore'
 
 [tool.devpy.commands]
-"Build" = ["devpy.build", "devpy.test"]
+"Build" = ["devpy.cmds.meson.build", "devpy.cmds.meson.test"]
 "Extensions" = ['.devpy/cmds.py:codecov', '.devpy/cmds.py:install_dependencies']
 
 [tool.pytest.ini_options]
 addopts = "--cov=solcore --cov-report=html:htmlcov -p no:warnings -n \"auto\" -v"
 
 [tool.isort]
 line_length = 88
```

### Comparing `solcore-5.9.1/solcore/__init__.py` & `solcore-5.9.2/solcore/__init__.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/__init__.py` & `solcore-5.9.2/solcore/absorption_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/absorption_QW.py` & `solcore-5.9.2/solcore/absorption_calculator/absorption_QW.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/adachi_alpha.py` & `solcore-5.9.2/solcore/absorption_calculator/adachi_alpha.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/cppm/Custom_CPPB.py` & `solcore-5.9.2/solcore/absorption_calculator/cppm/Custom_CPPB.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/cppm/Custom_CPPB_MaterialParamaters.txt` & `solcore-5.9.2/solcore/absorption_calculator/cppm/Custom_CPPB_MaterialParamaters.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/dielectric_constant_models.py` & `solcore-5.9.2/solcore/absorption_calculator/dielectric_constant_models.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/kramers_kronig.py` & `solcore-5.9.2/solcore/absorption_calculator/kramers_kronig.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/nk_db.py` & `solcore-5.9.2/solcore/absorption_calculator/nk_db.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/rigorous_coupled_wave.py` & `solcore-5.9.2/solcore/absorption_calculator/rigorous_coupled_wave.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/sopra_db.py` & `solcore-5.9.2/solcore/absorption_calculator/sopra_db.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/tmm_core_vec.py` & `solcore-5.9.2/solcore/absorption_calculator/tmm_core_vec.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/absorption_calculator/transfer_matrix.py` & `solcore-5.9.2/solcore/absorption_calculator/transfer_matrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-""" This module serves as interface between solcore structures (junctions, layers, materials...) and the
-transfer matrix package developed by Steven Byrnes and included in the PyPi repository.
+""" This module serves as interface between solcore structures (junctions, layers,
+materials...) and the transfer matrix package developed by Steven Byrnes and included in
+the PyPi repository.
 
 """
 import numpy as np
 import solcore
 
 from warnings import warn
 from collections.abc import Hashable
@@ -13,24 +14,28 @@
 from solcore.absorption_calculator import tmm_core_vec as tmm
 from functools import lru_cache, wraps
 
 degree = np.pi / 180
 
 
 def np_cache(function):
-    """This function was taken from https://stackoverflow.com/questions/52331944/cache-decorator-for-numpy-arrays/52332109#52332109
-    
-    Creates a cacheable version of a function which takes a 1D numpy array as input, by using a wrapping function
-    which converts the array to a tuple. It returns a function which returns the same output as the input function,
-    but can be cached, avoiding a bottleneck when optical constants in a material are looked up repeatedly.
-    
-    If the input argument is hashable already - eg. a single float number - then the function is not chached and is returned "as is".
+    """This function was taken from
+    https://stackoverflow.com/questions/52331944/cache-decorator-for-numpy-arrays/52332109#52332109 # noqa: E501
+
+    Creates a cacheable version of a function which takes a 1D numpy array as input, by
+    using a wrapping function which converts the array to a tuple. It returns a
+    function which returns the same output as the input function, but can be cached,
+    avoiding a bottleneck when optical constants in a material are looked up repeatedly.
+
+    If the input argument is hashable already - eg. a single float number - then the
+    function is not chached and is returned "as is".
 
     :param: function: the function of which a cacheable version is to be created
     :return: wrapper: the cacheable version of the function"""
+
     @lru_cache()
     def cached_wrapper(hashable_array):
         array = np.array(hashable_array)
         return function(array)
 
     @wraps(function)
     def wrapper(array):
@@ -43,70 +48,88 @@
     wrapper.cache_info = cached_wrapper.cache_info
     wrapper.cache_clear = cached_wrapper.cache_clear
 
     return wrapper
 
 
 class OptiStack(object):
-    """ Class that contains an optical structure: a sequence of layers with a thickness and a complex refractive index.
+    """Class that contains an optical structure: a sequence of layers with a thickness
+    and a complex refractive index.
 
-    It serves as an intermediate step between solcore layers and materials and the stack of thicknesses and
-    and n and k values necessary to run calculations involving TMM. When creating an OptiStack object, the thicknesses
-    of all the layers forming the Solcore structure and the optical data of the materials of the layers are extracted
+    It serves as an intermediate step between solcore layers and materials and the
+    stack of thicknesses and n and k values necessary to run calculations involving TMM.
+    When creating an OptiStack object, the thicknesses of all the layers forming the
+    Solcore structure and the optical data of the materials of the layers are extracted
     and arranged in such a way they can be easily and fastly read by the TMM functions.
 
-    In addition to a solcore structure with Layers, it can also take a list where each element represent a layer
-    written as a list and contains the layer thickness and the dielectrical model, the raw n and k data as a function
+    In addition to a solcore structure with Layers, it can also take a list where each
+    element represent a layer written as a list and contains the layer thickness and
+    the dielectrical model, the raw n and k data as a function
     of wavelengths, or a whole Device structure as the type used in the PDD model.
 
     In summary, this class acepts:
 
         - A solcore structure with layers
         - A list where each element is [thickness, DielectricModel]
         - A list where each element is [thickness, wavelength, n, k]
         - A list mixing the above:
             [ [thickness, DielectricModel],
               [thickness, wavelength, n, k],
               solcore.Layer,
               solcore.Layer ]
 
-    This allows for maximum flexibility when creating the optical model, allowing to construct the stack with
-    experimental data, modelled data and known material properties from the database.
-
-    Yet anther way of defining the layers mixes experimental data with a DielectricModel within the same layer but in
-    spectrally distinct regions. The syntaxis for the layer is:
+    This allows for maximum flexibility when creating the optical model, allowing to
+    construct the stack with experimental data, modelled data and known material
+    properties from the database.
+
+    Yet anther way of defining the layers mixes experimental data with a DielectricModel
+    within the same layer but in spectrally distinct regions. The syntaxis for the
+    layer is:
 
     layer = [thickness, wavelength, n, k, DielectricModel, mixing]
 
-    where mixing is a list containing three elements: [the mixing point (nm), the mixing width (nm),  zero or one]
-    depending if the mixing function should be increasing with the wavelength or decreasing. If increasing (zero), the
-    Dielectric model will be used at long wavelengths and the experimental data at short wavelengths. If decreasing
-    (one) the oposite is done. The mixing point and mixing width control how smooth is the transition between one and
-    the other type of data.
-
-    Extra layers such as he semi-infinite, air-like first and last medium, and a back highly absorbing layer are
-    included at runtime to fulfill the requirements of the TMM solver or to solve some of its limitations.
+    where mixing is a list containing three elements:
+    [the mixing point (nm), the mixing width (nm),  zero or one]
+    depending if the mixing function should be increasing with the wavelength or
+    decreasing. If increasing (zero), the Dielectric model will be used at long
+    wavelengths and the experimental data at short wavelengths. If decreasing (one)
+    the oposite is done. The mixing point and mixing width control how smooth is the
+    transition between one and the other type of data.
+
+    Extra layers such as he semi-infinite, air-like first and last medium, and a back
+    highly absorbing layer are included at runtime to fulfill the requirements of the
+    TMM solver or to solve some of its limitations.
     """
 
-    def __init__(self, structure=(), no_back_reflection=False, substrate=None, incidence=None, **kwargs):
-        """ Class constructor. It takes a Solcore structure and extract the thickness and optical data from the
-        Layers and the materials. Option is given to indicate if the reflexion from the back of the structure must be
-        supressed, usefull for ellipsometry calculations. This is done by creating an artificial highly absorbing but
-        not reflecting layer just at the back.
-
-        Alternativelly, it can take simply a list of [thickness, DielectricModel] or [thickness, wavelength, n, k] for
-        each layer accounting for the refractive index of the layers. The three options can be mixed for maximum
-        flexibility.
+    def __init__(
+        self,
+        structure=(),
+        no_back_reflection=False,
+        substrate=None,
+        incidence=None,
+        **kwargs,
+    ):
+        """Class constructor. It takes a Solcore structure and extract the thickness
+        and optical data from the Layers and the materials. Option is given to
+        indicate if the reflection from the back of the structure must be suppressed,
+        useful for ellipsometry calculations. This is done by creating an artificial
+        highly absorbing but not reflecting layer just at the back.
+
+        Alternatively, it can take simply a list of [thickness, DielectricModel] or
+        [thickness, wavelength, n, k] for each layer accounting for the refractive
+        index of the layers. The three options can be mixed for maximum flexibility.
 
         :param structure: A list with one or more layers.
-        :param no_back_reflection: If reflection from the back must be suppressed. Default=False.
-        :param substrate: a semi-infinite transmission medium. Note that if no_back_reflection is set to True,
-        adding a substrate won't make any difference.
-        :param incidence: a semi-infinite transmission medium. Note that add things may happen if
-        this material is absorbing
+        :param no_back_reflection: If reflection from the back must be suppressed.
+            Default=False.
+        :param substrate: a semi-infinite transmission medium. Note that if
+            no_back_reflection is set to True, adding a substrate won't make any
+         difference.
+        :param incidence: a semi-infinite incidence medium. Note that add things may
+            happen if this material is absorbing
         """
 
         self.widths = []
         self.n_data = []
         self.k_data = []
         self.models = []
         self.layers = []
@@ -114,542 +137,725 @@
         self.incidence = incidence
 
         self.num_layers = 0
         self.add_layers(structure)
 
         self.no_back_reflection = no_back_reflection
 
-        if 'no_back_reflexion' in kwargs:
-            warn('The no_back_reflexion warning is deprecated. Use no_back_reflection instead.', FutureWarning)
-            self.no_back_reflection = kwargs['no_back_reflexion']
+        if "no_back_reflexion" in kwargs:
+            warn(
+                "The no_back_reflexion warning is deprecated. "
+                "Use no_back_reflection instead.",
+                FutureWarning,
+            )
+            self.no_back_reflection = kwargs["no_back_reflexion"]
 
     def get_indices(self, wl):
-        """ Returns the complex refractive index of the stack.
+        """Returns the complex refractive index of the stack.
 
         :param wl: Wavelength of the light in nm.
-        :return: A list with the complex refractive index of each layer, including the semi-infinite front and back
-        layers and, opionally, the back absorbing layer used to suppress back surface relfexion.
+        :return: A list with the complex refractive index of each layer, including the
+        semi-infinite front and back layers and, opionally, the back absorbing layer
+        used to suppress back surface relfexion.
         """
 
         out = []
-        wl_m = solcore.si(wl, 'nm')
+        wl_m = solcore.si(wl, "nm")
 
-        if hasattr(self, 'n_sub'):
-            n1 = self.n_sub(wl_m) + self.k_sub(wl_m)*1.0j
+        if hasattr(self, "n_sub"):
+            n1 = self.n_sub(wl_m) + self.k_sub(wl_m) * 1.0j
         else:
-            if hasattr(wl, 'size'):
+            if hasattr(wl, "size"):
                 n1 = np.ones_like(wl, dtype=complex)
             else:
                 n1 = 1
 
         # incidence medium!
-        if hasattr(self, 'n_sup'):
-            n0 = self.n_sup(wl_m) #+ self.k_sup(wl_m)*1.0j ignore complex part for now to avoid errors
+        if hasattr(self, "n_sup"):
+            n0 = self.n_sup(
+                wl_m
+            )  # + self.k_sup(wl_m)*1.0j ignore complex part for now to avoid errors
         else:
-            if hasattr(wl, 'size'):
+            if hasattr(wl, "size"):
                 n0 = np.ones_like(wl, dtype=complex)
             else:
                 n0 = 1
 
         for i in range(self.num_layers):
             out.append(self.n_data[i](wl_m) + self.k_data[i](wl_m) * 1.0j)
 
         # substrate irrelevant if no_back_reflection = True
         if self.no_back_reflection:
-            return [n0] + out + [self.n_data[-1](wl_m) + self._k_absorbing(wl_m) * 1.0j, n1] # look at last entry in stack,
+            return (
+                [n0]
+                + out
+                + [self.n_data[-1](wl_m) + self._k_absorbing(wl_m) * 1.0j, n1]
+            )  # look at last entry in stack,
             # make high;y absorbing layer based on it.
 
         else:
-
             return [n0] + out + [n1]
 
-
     def get_widths(self):
-        """ Returns the widths of the layers of the stack.
+        """Returns the widths of the layers of the stack.
 
-        :return: A list with the widths each layer, including the semi-infinite front and back layers and, opionally,
-        the back absorbing layer used to suppress back surface relfexion, defined as 1 mm thick.
+        :return: A list with the widths each layer, including the semi-infinite front
+        and back layers and, opionally, the back absorbing layer used to suppress
+        back surface relfection, defined as 1 mm thick.
         """
 
         if self.no_back_reflection:
             return [np.inf] + self.widths + [1e6, np.inf]
         else:
             return [np.inf] + self.widths + [np.inf]
 
     def _k_absorbing(self, wl):
-        """ k value of the back highly absorbing layer. It is the maximum between the bottom layer of the stack or a
-        finite, small value that will absorb all light within the absorbing layer thickness.
+        """k value of the back highly absorbing layer. It is the maximum between the
+        bottom layer of the stack or a finite, small value that will absorb all light
+        within the absorbing layer thickness.
 
         :param wl: Wavelength of the light in nm.
         :return: The k value at each wavelength.
         """
         return np.maximum(wl / 1e-3, self.k_data[-1](wl))
 
     @staticmethod
     def _k_dummy(wl):
-        """ Dummy k value to be used with the dielectric model, which produces the refractive index as a complex
-        number.
+        """Dummy k value to be used with the dielectric model, which produces the
+        refractive index as a complex number.
 
         :param wl: Wavelength of the light in nm.
         :return: The k value at each wavelength... set to zero.
         """
-        return 0.
+        return 0.0
 
     def add_layers(self, layers):
-        """ Generic function to add layers to the OptiStack. Internally, it calls add_solcore_layer,
-        add_modelled_layer or add_raw_nk_layer.
+        """Generic function to add layers to the OptiStack. Internally, it calls
+        add_solcore_layer, add_modelled_layer or add_raw_nk_layer.
 
-        :param layers: A list with the layers to add (even if it is just one layer) It can be one or more and it can
-        mixed, Solcore-based and modelled layers.
+        :param layers: A list with the layers to add (even if it is just one layer)
+            It can be one or more and it can be mixed, Solcore-based and modelled
+            layers.
         :return: None
         """
         try:
-            # If the input is a whole device structure, we get just the layers information
+            # If the input is a whole device structure, we get just the layers
+            # information
             if type(layers) is dict:
                 layers = ToStructure(layers)
 
             if self.substrate is not None:
                 self.n_sub = self.substrate.n
                 self.k_sub = self.substrate.k
 
             if self.incidence is not None:
                 self.n_sup = self.incidence.n
                 self.k_sup = self.incidence.k
 
             for layer in layers:
                 self.layers.append(layer)
-                if 'Layer' in str(type(layer)):
+                if "Layer" in str(type(layer)):
                     self._add_solcore_layer(layer)
-                elif 'DielectricConstantModel' in str(type(layer[1])):
+                elif "DielectricConstantModel" in str(type(layer[1])):
                     self._add_modelled_layer(layer)
                 else:
                     self._add_raw_nk_layer(layer)
 
                 self.num_layers += 1
 
         except Exception as err:
-            print('Error when adding a new layer to the OptiStack. {}'.format(err))
+            print("Error when adding a new layer to the OptiStack. {}".format(err))
 
     def remove_layer(self, idx):
-        """ Removes layer with index idx from the OptiStack
+        """Removes layer with index idx from the OptiStack
 
         :param idx: Index of the layer to remove
         :return: None
         """
         if idx >= self.num_layers:
-            print('Error when removing layers. idx must be: 0 <= idx <= {}.'.format(self.num_layers - 1))
+            print(
+                "Error when removing layers. idx must be: 0 <= idx <= {}.".format(
+                    self.num_layers - 1
+                )
+            )
             return
 
         self.widths.pop(idx)
         self.models.pop(idx)
         self.n_data.pop(idx)
         self.k_data.pop(idx)
         self.num_layers -= 1
 
     def swap_layers(self, idx1, idx2):
-        """ Swaps two layers in the OptiStack.
+        """Swaps two layers in the OptiStack.
 
         :param idx1: The index of one of the layers.
         :param idx2: The index of the other.
         :return: None
         """
         if idx1 >= self.num_layers or idx2 >= self.num_layers:
-            print('Error when removing layers. idx must be: 0 <= idx1, idx2 <= {}.'.format(self.num_layers - 1))
+            print(
+                "Error when removing layers. idx must be: 0 <= idx1, idx2 <= {}.".
+                format(self.num_layers - 1)
+            )
             return
 
         self.widths[idx1], self.widths[idx2] = self.widths[idx2], self.widths[idx1]
         self.models[idx1], self.models[idx2] = self.models[idx2], self.models[idx1]
         self.n_data[idx1], self.n_data[idx2] = self.n_data[idx2], self.n_data[idx1]
         self.k_data[idx1], self.k_data[idx2] = self.k_data[idx2], self.k_data[idx1]
 
-
     def set_widths(self, widths):
         """Changes the widths of the layers in the stack.
 
         :param: widths: a list or array of widths, length equal to the number of layers
         :return: None"""
 
         if type(widths) is np.ndarray:
             widths = widths.tolist()
 
-        assert len(widths) == self.num_layers, \
-            'Error: The list of widths must have as many elements (now {}) as the ' \
-        'number of layers (now {}).'.format(len(widths), self.num_layers)
+        assert len(widths) == self.num_layers, (
+            "Error: The list of widths must have as many elements (now {}) as the "
+            "number of layers (now {}).".format(len(widths), self.num_layers)
+        )
 
         self.widths = widths
 
-
     def _add_solcore_layer(self, layer):
-        """ Adds a Solcore layer to the end (bottom) of the stack, extracting its thickness and n and k data.
+        """Adds a Solcore layer to the end (bottom) of the stack, extracting its
+        thickness and n and k data.
 
         :param layer: The Solcore layer
         :return: None
         """
-        self.widths.append(solcore.asUnit(layer.width, 'nm'))
+        self.widths.append(solcore.asUnit(layer.width, "nm"))
         self.models.append([])
         self.n_data.append(np_cache(layer.material.n))
         self.k_data.append(np_cache(layer.material.k))
 
-
     def _add_modelled_layer(self, layer):
-        """ Adds a layer to the end (bottom) of the stack. The layer must be defined as a list containing the layer
-        thickness in nm and a dielectric model.
+        """Adds a layer to the end (bottom) of the stack. The layer must be defined as
+        a list containing the layer thickness in nm and a dielectric model.
 
         :param layer: The new layer to add as [thickness, DielectricModel]
         :return: None
         """
         self.widths.append(layer[0])
         self.models.append(layer[1])
         self.n_data.append(np_cache(self.models[-1].n_and_k))
         self.k_data.append(np_cache(self._k_dummy))
 
     def _add_raw_nk_layer(self, layer):
-        """ Adds a layer to the end (bottom) of the stack. The layer must be defined as a list containing the layer
-        thickness in nm, the wavelength, the n and the k data as array-like objects.
+        """Adds a layer to the end (bottom) of the stack. The layer must be defined as
+        a list containing the layer thickness in nm, the wavelength, the n and the k
+        data as array-like objects.
 
         :param layer: The new layer to add as [thickness, wavelength, n, k]
         :return: None
         """
-        # We make sure that the wavelengths are increasing, revering the arrays otherwise.
+        # We make sure that the wavelengths are increasing, reversing the arrays
+        # otherwise.
         if layer[1][0] > layer[1][-1]:
             layer[1] = layer[1][::-1]
             layer[2] = layer[2][::-1]
             layer[3] = layer[3][::-1]
 
         self.widths.append(layer[0])
 
         if len(layer) >= 5:
             self.models.append(layer[4])
-            c = solcore.si(layer[5][0], 'nm')
-            w = solcore.si(layer[5][1], 'nm')
+            c = solcore.si(layer[5][0], "nm")
+            w = solcore.si(layer[5][1], "nm")
             d = layer[5][2]  # = 0 for increasing, =1 for decreasing
 
             def mix(x):
-
                 out = 1 + np.exp(-(x - c) / w)
                 out = d + (-1) ** d * 1 / out
 
                 return out
 
-            n_data = np_cache(lambda x: self.models[-1].n_and_k(x) * mix(x) + (1 - mix(x)) * interp1d(
-                x=solcore.si(layer[1], 'nm'), y=layer[2], fill_value=layer[2][-1])(x))
-            k_data = np_cache(lambda x: interp1d(x=solcore.si(layer[1], 'nm'), y=layer[3], fill_value=layer[3][-1])(x))
+            n_data = np_cache(
+                lambda x: self.models[-1].n_and_k(x) * mix(x)
+                + (1 - mix(x))
+                * interp1d(
+                    x=solcore.si(layer[1], "nm"), y=layer[2], fill_value=layer[2][-1]
+                )(x)
+            )
+            k_data = np_cache(
+                lambda x: interp1d(
+                    x=solcore.si(layer[1], "nm"), y=layer[3], fill_value=layer[3][-1]
+                )(x)
+            )
 
             self.n_data.append(n_data)
             self.k_data.append(k_data)
 
         else:
             self.models.append([])
-            self.n_data.append(np_cache(interp1d(x=solcore.si(layer[1], 'nm'), y=layer[2], fill_value=layer[2][-1])))
-            self.k_data.append(np_cache(interp1d(x=solcore.si(layer[1], 'nm'), y=layer[3], fill_value=layer[3][-1])))
-
-
-def calculate_rat(structure, wavelength, angle=0, pol='u',
-                  coherent=True, coherency_list=None, no_back_reflection=True, **kwargs):
-    """ Calculates the reflected, absorbed and transmitted intensity of the structure for the wavelengths and angles
-    defined.
+            self.n_data.append(
+                np_cache(
+                    interp1d(
+                        x=solcore.si(layer[1], "nm"),
+                        y=layer[2],
+                        fill_value=layer[2][-1],
+                    )
+                )
+            )
+            self.k_data.append(
+                np_cache(
+                    interp1d(
+                        x=solcore.si(layer[1], "nm"),
+                        y=layer[3],
+                        fill_value=layer[3][-1],
+                    )
+                )
+            )
+
+
+def calculate_rat(
+    structure,
+    wavelength,
+    angle=0,
+    pol="u",
+    coherent=True,
+    coherency_list=None,
+    no_back_reflection=True,
+    **kwargs,
+):
+    """Calculates the reflected, absorbed and transmitted intensity of the structure
+    for the wavelengths and angles defined.
 
-    :param structure: A solcore Structure object with layers and materials or a OptiStack object.
+    :param structure: A solcore Structure object with layers and materials or a
+        OptiStack object.
     :param wavelength: Wavelengths (in nm) in which calculate the data. An array.
-    :param angle: Angle (in degrees) of the incident light. Default: 0 (normal incidence).
+    :param angle: Angle (in degrees) of the incident light.
+        Default: 0 (normal incidence).
     :param pol: Polarisation of the light: 's', 'p' or 'u'. Default: 'u' (unpolarised).
-    :param coherent: If the light is coherent or not. If not, a coherency list must be added.
-    :param coherency_list: A list indicating in which layers light should be treated as coeherent ('c') and in which
-    incoherent ('i'). It needs as many elements as layers in the structure.
-    :param no_back_reflection: If reflexion from the back must be supressed. Default=True.
+    :param coherent: If the light is coherent or not. If not, a coherency list
+        must be added.
+    :param coherency_list: A list indicating in which layers light should be treated as
+        coherent ('c') and in which incoherent ('i'). It needs as many elements as
+        layers in the structure.
+    :param no_back_reflection: If reflection from the back must be supressed.
+        Default=True.
     :return: A dictionary with the R, A and T at the specified wavelengths and angle.
     """
     num_wl = len(wavelength)
 
-    if 'no_back_reflexion' in kwargs:
-        warn('The no_back_reflexion argument is deprecated. Use no_back_reflection instead.', FutureWarning)
-        no_back_reflection = kwargs['no_back_reflexion']
+    if "no_back_reflexion" in kwargs:
+        warn(
+            "The no_back_reflexion argument is deprecated. "
+            "Use no_back_reflection instead.",
+            FutureWarning,
+        )
+        no_back_reflection = kwargs["no_back_reflexion"]
 
-    if 'OptiStack' in str(type(structure)):
+    if "OptiStack" in str(type(structure)):
         stack = structure
         stack.no_back_reflection = no_back_reflection
     else:
         stack = OptiStack(structure, no_back_reflection=no_back_reflection)
 
     if not coherent:
         if coherency_list is not None:
-            assert len(coherency_list) == stack.num_layers, \
-                'Error: The coherency list must have as many elements (now {}) as the ' \
-                'number of layers (now {}).'.format(len(coherency_list), stack.num_layers)
+            assert len(coherency_list) == stack.num_layers, (
+                "Error: The coherency list must have as many elements (now {}) as the "
+                "number of layers (now {}).".format(
+                    len(coherency_list), stack.num_layers
+                )
+            )
 
             if stack.no_back_reflection:
-                coherency_list = ['i'] + coherency_list + ['i', 'i']
+                coherency_list = ["i"] + coherency_list + ["i", "i"]
             else:
-                coherency_list = ['i'] + coherency_list + ['i']
+                coherency_list = ["i"] + coherency_list + ["i"]
 
         else:
-            raise Exception('Error: For incoherent or partly incoherent calculations you must supply the '
-                            'coherency_list parameter with as many elements as the number of layers in the '
-                            'structure')
+            raise Exception(
+                "Error: For incoherent or partly incoherent calculations you must "
+                "supply the coherency_list parameter with as many elements as the "
+                "number of layers in the structure"
+            )
+
+    output = {
+        "R": np.zeros(num_wl),
+        "A": np.zeros(num_wl),
+        "T": np.zeros(num_wl),
+        "all_p": [],
+        "all_s": [],
+        "out": [],
+        "out_s": [],
+        "out_p": [],
+        "A_per_layer_s": [],
+        "A_per_layer_p": [],
+    }
 
-    output = {'R': np.zeros(num_wl), 'A': np.zeros(num_wl), 'T': np.zeros(num_wl), 'all_p': [], 'all_s': [], 'out': [],
-              'out_s': [], 'out_p': [],  'A_per_layer_s': [], 'A_per_layer_p': []}
-
-    if pol in 'sp':
+    if pol in "sp":
         if coherent:
-            out = tmm.coh_tmm(pol, stack.get_indices(wavelength), stack.get_widths(), angle * degree, wavelength)
+            out = tmm.coh_tmm(
+                pol,
+                stack.get_indices(wavelength),
+                stack.get_widths(),
+                angle * degree,
+                wavelength,
+            )
             A_per_layer = tmm.absorp_in_each_layer(out)
-            output['R'] = out['R']
-            output['A'] = 1 - out['R'] - out['T']
-            output['T'] = out['T']
-            output['A_per_layer'] = A_per_layer
-            output['out'] = out
-        else:
-            out = tmm.inc_tmm(pol, stack.get_indices(wavelength), stack.get_widths(), coherency_list, angle * degree, wavelength)
+            output["R"] = out["R"]
+            output["A"] = 1 - out["R"] - out["T"]
+            output["T"] = out["T"]
+            output["A_per_layer"] = A_per_layer
+            output["out"] = out
+        else:
+            out = tmm.inc_tmm(
+                pol,
+                stack.get_indices(wavelength),
+                stack.get_widths(),
+                coherency_list,
+                angle * degree,
+                wavelength,
+            )
             A_per_layer = np.array(tmm.inc_absorp_in_each_layer(out))
-            output['R'] = out['R']
-            output['A'] = 1 - out['R'] - out['T']
-            output['T'] = out['T']
-            output['A_per_layer'] = A_per_layer
-            output['out'] = out
+            output["R"] = out["R"]
+            output["A"] = 1 - out["R"] - out["T"]
+            output["T"] = out["T"]
+            output["A_per_layer"] = A_per_layer
+            output["out"] = out
     else:
         if coherent:
-            out_p = tmm.coh_tmm('p', stack.get_indices(wavelength), stack.get_widths(), angle * degree, wavelength)
-            out_s = tmm.coh_tmm('s', stack.get_indices(wavelength), stack.get_widths(), angle * degree, wavelength)
+            out_p = tmm.coh_tmm(
+                "p",
+                stack.get_indices(wavelength),
+                stack.get_widths(),
+                angle * degree,
+                wavelength,
+            )
+            out_s = tmm.coh_tmm(
+                "s",
+                stack.get_indices(wavelength),
+                stack.get_widths(),
+                angle * degree,
+                wavelength,
+            )
             A_per_layer_p = tmm.absorp_in_each_layer(out_p)
             A_per_layer_s = tmm.absorp_in_each_layer(out_s)
-            output['R'] = 0.5 * (out_p['R'] + out_s['R'])
-            output['T'] = 0.5 * (out_p['T'] + out_s['T'])
-            output['A'] = 1 - output['R'] - output['T']
-            output['A_per_layer'] = 0.5*(A_per_layer_p + A_per_layer_s)
-
-            output['out_s'] = out_s
-            output['out_p'] = out_p
-            output['A_per_layer_s'] = A_per_layer_s
-            output['A_per_layer_p'] = A_per_layer_p
-
-        else:
-
-
-            out_p = tmm.inc_tmm('p', stack.get_indices(wavelength), stack.get_widths(), coherency_list, angle * degree, wavelength)
-            out_s = tmm.inc_tmm('s', stack.get_indices(wavelength), stack.get_widths(), coherency_list, angle * degree, wavelength)
+            output["R"] = 0.5 * (out_p["R"] + out_s["R"])
+            output["T"] = 0.5 * (out_p["T"] + out_s["T"])
+            output["A"] = 1 - output["R"] - output["T"]
+            output["A_per_layer"] = 0.5 * (A_per_layer_p + A_per_layer_s)
+
+            output["out_s"] = out_s
+            output["out_p"] = out_p
+            output["A_per_layer_s"] = A_per_layer_s
+            output["A_per_layer_p"] = A_per_layer_p
+
+        else:
+            out_p = tmm.inc_tmm(
+                "p",
+                stack.get_indices(wavelength),
+                stack.get_widths(),
+                coherency_list,
+                angle * degree,
+                wavelength,
+            )
+            out_s = tmm.inc_tmm(
+                "s",
+                stack.get_indices(wavelength),
+                stack.get_widths(),
+                coherency_list,
+                angle * degree,
+                wavelength,
+            )
 
             A_per_layer_p = np.array(tmm.inc_absorp_in_each_layer(out_p))
             A_per_layer_s = np.array(tmm.inc_absorp_in_each_layer(out_s))
 
-            output['R'] = 0.5 * (out_p['R'] + out_s['R'])
-            output['T'] = 0.5 * (out_p['T'] + out_s['T'])
-            output['A'] = 1 - output['R'] - output['T']
-            output['all_p'] = out_p['power_entering_list']
-            output['all_s'] = out_s['power_entering_list']
-            output['A_per_layer'] = 0.5*(A_per_layer_p + A_per_layer_s)
-
-            output['out_s'] = out_s
-            output['out_p'] = out_p
-            output['A_per_layer_s'] =  A_per_layer_s
-            output['A_per_layer_p'] = A_per_layer_p
-
+            output["R"] = 0.5 * (out_p["R"] + out_s["R"])
+            output["T"] = 0.5 * (out_p["T"] + out_s["T"])
+            output["A"] = 1 - output["R"] - output["T"]
+            output["all_p"] = out_p["power_entering_list"]
+            output["all_s"] = out_s["power_entering_list"]
+            output["A_per_layer"] = 0.5 * (A_per_layer_p + A_per_layer_s)
+
+            output["out_s"] = out_s
+            output["out_p"] = out_p
+            output["A_per_layer_s"] = A_per_layer_s
+            output["A_per_layer_p"] = A_per_layer_p
 
     return output
 
 
-def calculate_ellipsometry(structure, wavelength, angle, no_back_reflection=True, **kwargs):
-    """ Calculates the ellipsometric parameters psi and delta. It can only deal with coherent light and the whole stack
-    (including back surface) is considered, so caution must be taken when comparing the simulated results with
-    experiments where the back surface is rough or layers are thick and coherent light propagation makes no sense.
-
-    The optional argument no_back_reflection can be included to add an extra layer on the back absorbing all light that
-    reaches that position without any reflexion, to remove the reflexion from the back surface.
+def calculate_ellipsometry(
+    structure, wavelength, angle, no_back_reflection=True, **kwargs
+):
+    """Calculates the ellipsometric parameters psi and delta. It can only deal with
+    coherent light and the whole stack (including back surface) is considered,
+    so caution must be taken when comparing the simulated results with experiments
+    where the back surface is rough or layers are thick and coherent light propagation
+    makes no sense.
+
+    The optional argument no_back_reflection can be included to add an extra layer on
+    the back absorbing all light that reaches that position without any reflection,
+    to remove the reflection from the back surface.
 
     :param structure: A solcore structure with layers and materials.
     :param wavelength: Wavelengths (in nm) in which calculate the data. An array.
-    :param angle: A tupple or list with the angles (in degrees) in which to calculate the data.
-    :param no_back_reflection: If reflexion from the back must be suppressed. Default=True.
-    :return: A dictionary with psi and delta at the specified wavelengths and angles (2D arrays).
+    :param angle: A tupple or list with the angles (in degrees) in which to calculate
+        the data.
+    :param no_back_reflection: If reflection from the back must be suppressed.
+        Default=True.
+    :return: A dictionary with psi and delta at the specified wavelengths and angles
+        (2D arrays).
     """
 
-    if 'no_back_reflexion' in kwargs:
-        warn('The no_back_reflexion argument is deprecated. Use no_back_reflection instead.', FutureWarning)
-        no_back_reflection = kwargs['no_back_reflexion']
+    if "no_back_reflexion" in kwargs:
+        warn(
+            "The no_back_reflexion argument is deprecated. "
+            "Use no_back_reflection instead.",
+            FutureWarning,
+        )
+        no_back_reflection = kwargs["no_back_reflexion"]
 
     num_wl = len(wavelength)
     num_ang = len(angle)
 
-    if 'OptiStack' in str(type(structure)):
+    if "OptiStack" in str(type(structure)):
         stack = structure
         stack.no_back_reflection = no_back_reflection
     else:
-        if hasattr(structure, 'substrate'):
+        if hasattr(structure, "substrate"):
             substrate = structure.substrate
         else:
             substrate = None
-        stack = OptiStack(structure, no_back_reflection=no_back_reflection, substrate=substrate)
+        stack = OptiStack(
+            structure, no_back_reflection=no_back_reflection, substrate=substrate
+        )
 
-    output = {'psi': np.zeros((num_wl, num_ang)), 'Delta': np.zeros((num_wl, num_ang))}
+    output = {"psi": np.zeros((num_wl, num_ang)), "Delta": np.zeros((num_wl, num_ang))}
 
     for i, ang in enumerate(angle):
-        out = tmm.ellips(stack.get_indices(wavelength), stack.get_widths(), ang * degree, wavelength)
-        output['psi'][:, i] = out['psi'] / degree
+        out = tmm.ellips(
+            stack.get_indices(wavelength), stack.get_widths(), ang * degree, wavelength
+        )
+        output["psi"][:, i] = out["psi"] / degree
 
         # We revere the sign of Delta in order to use Woollam sign convention
-        output['Delta'][:, i] = -out['Delta'] / degree
+        output["Delta"][:, i] = -out["Delta"] / degree
 
-        output['Delta'][:, i] = np.where(output['Delta'][:, i] > 0, -output['Delta'][:, i], output['Delta'][:, i])
-        output['Delta'][:, i] = np.where(output['Delta'][:, i] < 180, 180 - output['Delta'][:, i],
-                                         output['Delta'][:, i])
+        output["Delta"][:, i] = np.where(
+            output["Delta"][:, i] > 0, -output["Delta"][:, i], output["Delta"][:, i]
+        )
+        output["Delta"][:, i] = np.where(
+            output["Delta"][:, i] < 180,
+            180 - output["Delta"][:, i],
+            output["Delta"][:, i],
+        )
 
     return output
 
 
-
-def calculate_absorption_profile(structure, wavelength, z_limit=None, steps_size=2, dist=None,
-                                   no_back_reflection=True, angle=0, pol = 'u',
-                                 coherent=True, coherency_list=None, zero_threshold=1e-6, RAT_out=None, **kwargs):
-    """ It calculates the absorbed energy density within the material. From the documentation:
-
-    'In principle this has units of [power]/[volume], but we can express it as a multiple of incoming light power
-    density on the material, which has units [power]/[area], so that absorbed energy density has units of 1/[length].'
-
-    Integrating this absorption profile in the whole stack gives the same result that the absorption obtained with
-    calculate_rat as long as the spacial mesh (controlled by steps_thinest_layer) is fine enough. If the structure is
-    very thick and the mesh not thin enough, the calculation might diverge at short wavelengths.
+def calculate_absorption_profile(
+    structure,
+    wavelength,
+    z_limit=None,
+    steps_size=2,
+    dist=None,
+    no_back_reflection=True,
+    angle=0,
+    pol="u",
+    coherent=True,
+    coherency_list=None,
+    zero_threshold=1e-6,
+    RAT_out=None,
+    **kwargs,
+):
+    """It calculates the absorbed energy density within the material.
+    From the documentation:
+
+    'In principle this has units of [power]/[volume], but we can express it as a
+    multiple of incoming light power density on the material, which has units [
+    power]/[area], so that absorbed energy density has units of 1/[length].'
+
+    Integrating this absorption profile in the whole stack gives the same result that
+    the absorption obtained with calculate_rat as long as the spatial mesh (controlled
+    by steps_thinest_layer) is fine enough. If the structure is very thick and the
+    mesh not thin enough, the calculation might diverge at short wavelengths.
 
     :param structure: A solcore structure with layers and materials.
     :param wavelength: Wavelengths in which calculate the data (in nm). An array
     :param z_limit: Maximum value in the z direction
-    :param steps_size: if the dist is not specified, the step size in nm to use in the depth-dependent calculation
+    :param steps_size: if the dist is not specified, the step size in nm to use in the
+        depth-dependent calculation
     :param dist: the positions (in nm) at which to calculate depth-dependent absorption
-    :param no_back_reflection: whether to suppress reflections from the back interface (True) or not (False)
+    :param no_back_reflection: whether to suppress reflections from the back interface
+        (True) or not (False)
     :param angle: incidence of angle in degrees
     :param pol: polarization of incident light: 's', 'p' or 'u' (unpolarized)
-    :param coherent: True if all the layers are to be treated coherently, False otherwise
-    :param coherency_list: if coherent is False, a list of 'c' (coherent) or 'i' (incoherent) for each layer
-    :param zero_threshold: when the fraction of incident light absorbed in a layer is less than this value, the absorption
-    profile is completely set to zero for both coherent and incoherent calculations. This is applied on a wavelength-by-wavelength
-    basis and is intended to prevent errors where integrating a weak absorption profile in a layer over many points leads to
-    calculated EQE > total absorption in that layer.
+    :param coherent: True if all the layers are to be treated coherently,
+        False otherwise
+    :param coherency_list: if coherent is False, a list of 'c' (coherent) or
+        'i' (incoherent) for each layer
+    :param zero_threshold: when the fraction of incident light absorbed in a layer is
+        less than this value, the absorption profile is completely set to zero for
+        both coherent and incoherent calculations. This is applied on a
+        wavelength-by-wavelength basis and is intended to prevent errors where
+        integrating a weak absorption profile in a layer over many
+        points leads to calculated EQE > total absorption in that layer.
     :param RAT_out: output from calculate_rat for the same stack & options
-    :return: A dictionary containing the positions (in nm) and a 2D array with the absorption in the structure as a
-    function of the position and the wavelength.
+    :return: A dictionary containing the positions (in nm) and a 2D array with the
+        absorption in the structure as a function of the position and the wavelength.
     """
 
-    if 'no_back_reflexion' in kwargs:
-        warn('The no_back_reflexion warning is deprecated. Use no_back_reflection instead.', FutureWarning)
-        no_back_reflection = kwargs['no_back_reflexion']
+    if "no_back_reflexion" in kwargs:
+        warn(
+            "The no_back_reflexion warning is deprecated. "
+            "Use no_back_reflection instead.",
+            FutureWarning,
+        )
+        no_back_reflection = kwargs["no_back_reflexion"]
 
     if RAT_out is None:
         # R, A per layer, T not yet calculated, calculate now
-        RAT_out = calculate_rat(structure, wavelength, angle, pol=pol, coherent=coherent, coherency_list=coherency_list,
-                                no_back_reflection=no_back_reflection)
+        RAT_out = calculate_rat(
+            structure,
+            wavelength,
+            angle,
+            pol=pol,
+            coherent=coherent,
+            coherency_list=coherency_list,
+            no_back_reflection=no_back_reflection,
+        )
 
     num_wl = len(wavelength)
 
-    if 'OptiStack' in str(type(structure)):
+    if "OptiStack" in str(type(structure)):
         stack = structure
         stack.no_back_reflection = no_back_reflection
     else:
         stack = OptiStack(structure, no_back_reflection=no_back_reflection)
 
     if dist is None:
         if z_limit is None:
             z_limit = np.sum(np.array(stack.widths))
         dist = np.arange(0, z_limit, steps_size)
 
     if not coherent:
         if coherency_list is not None:
-
             if stack.no_back_reflection:
-                coherency_list = ['i'] + coherency_list + ['i', 'i']
+                coherency_list = ["i"] + coherency_list + ["i", "i"]
             else:
-                coherency_list = ['i'] + coherency_list + ['i']
+                coherency_list = ["i"] + coherency_list + ["i"]
 
         else:
-            raise Exception('Error: For incoherent or partly incoherent calculations you must supply the '
-                            'coherency_list parameter with as many elements as the number of layers in the '
-                            'structure')
+            raise Exception(
+                "Error: For incoherent or partly incoherent calculations you must "
+                "supply the coherency_list parameter with as many elements as the "
+                "number of layers in the structure"
+            )
 
-    output = {'position': dist, 'absorption': np.zeros((num_wl, len(dist)))}
+    output = {"position": dist, "absorption": np.zeros((num_wl, len(dist)))}
 
-    if pol in 'sp':
+    layer, d_in_layer = tmm.find_in_structure_with_inf(stack.get_widths(), dist)
 
+    if pol in "sp":
         if coherent:
-            A_per_layer = RAT_out['A_per_layer']
-            no_abs_in_layer = np.where(A_per_layer[:-1,:] < zero_threshold)
-            RAT_out['out']['vw_list'][no_abs_in_layer[0], no_abs_in_layer[1], :] = 0
-
-            layer, d_in_layer = tmm.find_in_structure_with_inf(stack.get_widths(), dist)
-            data = tmm.position_resolved(layer, d_in_layer, RAT_out['out'])
-            output['absorption'] = data['absor']
-
-        else:
-            layer, d_in_layer = tmm.find_in_structure_with_inf(stack.get_widths(), dist)
-            data = tmm.inc_position_resolved(layer, d_in_layer, RAT_out['out'], coherency_list,
-                                             4*np.pi*np.imag(stack.get_indices(wavelength))/wavelength, zero_threshold)
-            output['absorption'] = data
+            A_per_layer = RAT_out["A_per_layer"]
+            no_abs_in_layer = np.where(A_per_layer[:-1, :] < zero_threshold)
+            RAT_out["out"]["vw_list"][no_abs_in_layer[0], no_abs_in_layer[1], :] = 0
+
+            data = tmm.position_resolved(layer, d_in_layer, RAT_out["out"])
+            output["absorption"] = data["absor"]
+
+        else:
+            data = tmm.inc_position_resolved(
+                layer,
+                d_in_layer,
+                RAT_out["out"],
+                coherency_list,
+                4 * np.pi * np.imag(stack.get_indices(wavelength)) / wavelength,
+                zero_threshold,
+            )
+            output["absorption"] = data
 
     else:
-
-
-
         if coherent:
-
-            A_per_layer_s = RAT_out['A_per_layer_s']
-            A_per_layer_p = RAT_out['A_per_layer_p']
-            no_abs_in_layer_s = np.where(A_per_layer_s[:-1,:] < zero_threshold)
+            A_per_layer_s = RAT_out["A_per_layer_s"]
+            A_per_layer_p = RAT_out["A_per_layer_p"]
+            no_abs_in_layer_s = np.where(A_per_layer_s[:-1, :] < zero_threshold)
             no_abs_in_layer_p = np.where(A_per_layer_p[:-1, :] < zero_threshold)
-            RAT_out['out_s']['vw_list'][no_abs_in_layer_s[0], no_abs_in_layer_s[1], :] = 0
-            RAT_out['out_p']['vw_list'][no_abs_in_layer_p[0], no_abs_in_layer_p[1], :] = 0
-
-            layer, d_in_layer = tmm.find_in_structure_with_inf(stack.get_widths(), dist)
-
-            data_s = tmm.position_resolved(layer, d_in_layer, RAT_out['out_s'])
-            data_p = tmm.position_resolved(layer, d_in_layer, RAT_out['out_p'])
-
-            output['absorption'] = 0.5*(data_s['absor'] + data_p['absor'])
+            RAT_out["out_s"]["vw_list"][
+                no_abs_in_layer_s[0], no_abs_in_layer_s[1], :
+            ] = 0
+            RAT_out["out_p"]["vw_list"][
+                no_abs_in_layer_p[0], no_abs_in_layer_p[1], :
+            ] = 0
+
+            data_s = tmm.position_resolved(layer, d_in_layer, RAT_out["out_s"])
+            data_p = tmm.position_resolved(layer, d_in_layer, RAT_out["out_p"])
+
+            output["absorption"] = 0.5 * (data_s["absor"] + data_p["absor"])
 
         else:
 
-            layer, d_in_layer = tmm.find_in_structure_with_inf(stack.get_widths(), dist)
-            data_s = tmm.inc_position_resolved(layer, d_in_layer, RAT_out['out_s'], coherency_list,
-                                             4*np.pi*np.imag(stack.get_indices(wavelength))/wavelength, zero_threshold)
-            data_p = tmm.inc_position_resolved(layer, d_in_layer, RAT_out['out_p'], coherency_list,
-                                             4*np.pi*np.imag(stack.get_indices(wavelength))/wavelength, zero_threshold)
+            data_s = tmm.inc_position_resolved(
+                layer,
+                d_in_layer,
+                RAT_out["out_s"],
+                coherency_list,
+                4 * np.pi * np.imag(stack.get_indices(wavelength)) / wavelength,
+                zero_threshold,
+            )
+            data_p = tmm.inc_position_resolved(
+                layer,
+                d_in_layer,
+                RAT_out["out_p"],
+                coherency_list,
+                4 * np.pi * np.imag(stack.get_indices(wavelength)) / wavelength,
+                zero_threshold,
+            )
 
-            output['absorption'] = 0.5*(data_s + data_p)
+            output["absorption"] = 0.5 * (data_s + data_p)
 
     return output
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import matplotlib.pyplot as plt
     from solcore import material, si
     from solcore.structure import Layer, Structure
 
-    GaAs = material('GaAs')(T=300)
-    InGaAs = material('InGaAs')(T=300, In=0.1)
-
-    my_structure = Structure([
-        Layer(si(3000, 'nm'), material=InGaAs),
-        Layer(si(30, 'um'), material=GaAs),
+    GaAs = material("GaAs")(T=300)
+    InGaAs = material("InGaAs")(T=300, In=0.1)
 
-    ])
+    my_structure = Structure(
+        [
+            Layer(si(3000, "nm"), material=InGaAs),
+            Layer(si(30, "um"), material=GaAs),
+        ]
+    )
 
     wavelength = np.linspace(450, 1100, 300)
 
-    out = calculate_rat(my_structure, wavelength, coherent=True, no_back_reflection=False)
+    out = calculate_rat(
+        my_structure, wavelength, coherent=True, no_back_reflection=False
+    )
     # #
     # plt.plot(wavelength, out['R'], 'b', label='Reflexion')
     # plt.plot(wavelength, out['A'], 'r', label='Absorption')
     # plt.plot(wavelength, out['T'], 'g', label='Transmission')
     # plt.legend()
     # plt.show()
 
     angles = [60, 65, 70]
     out = calculate_ellipsometry(my_structure, wavelength, angle=angles)
     #
-    plt.plot(wavelength, out['psi'][:, 0], 'b', label='psi')
-    plt.plot(wavelength, out['Delta'][:, 0], 'r', label='Delta')
+    plt.plot(wavelength, out["psi"][:, 0], "b", label="psi")
+    plt.plot(wavelength, out["Delta"][:, 0], "r", label="Delta")
     for i in range(1, len(angles)):
-        plt.plot(wavelength, out['psi'][:, i], 'b')
-        plt.plot(wavelength, out['Delta'][:, i], 'r')
+        plt.plot(wavelength, out["psi"][:, i], "b")
+        plt.plot(wavelength, out["Delta"][:, i], "r")
     #
     # plt.legend()
 
     # out = calculate_absorption_profile_2(my_structure, wavelength, z_limit=3000)
     # # print(tuple(out['absorption'][0]))
     # # plt.plot(out['position'], out['absorption'][0])
     # A = np.zeros_like(wavelength)
```

### Comparing `solcore-5.9.1/solcore/analytic_solar_cells/IV.py` & `solcore-5.9.2/solcore/analytic_solar_cells/IV.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/analytic_solar_cells/QE.py` & `solcore-5.9.2/solcore/analytic_solar_cells/QE.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/analytic_solar_cells/depletion_approximation.py` & `solcore-5.9.2/solcore/analytic_solar_cells/depletion_approximation.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,116 +4,132 @@
 from functools import partial
 
 from solcore.constants import kb, q
 from solcore.science_tracker import science_reference
 from solcore.state import State
 from solcore.light_source import LightSource
 
+import warnings
+
 da_options = State()
-da_options.da_mode = 'bvp'
+da_options.da_mode = "green"
+
 
 def identify_layers(junction):
     # First we have to figure out if we are talking about a PN, NP, PIN or NIP junction
     # We search for the emitter and check if it is n-type or p-type
     idx = 0
-    pn_or_np = 'pn'
-    homojunction = True
+    pn_or_np = "pn"
+    # homojunction = True
 
     for layer in junction:
-        if layer.role.lower() != 'emitter':
+        if layer.role.lower() != "emitter":
             idx += 1
         else:
             Na = 0
             Nd = 0
-            if hasattr(layer.material, 'Na'): Na = layer.material.Na
-            if hasattr(layer.material, 'Nd'): Nd = layer.material.Nd
+            if hasattr(layer.material, "Na"):
+                Na = layer.material.Na
+            if hasattr(layer.material, "Nd"):
+                Nd = layer.material.Nd
             if Na < Nd:
                 pn_or_np = "np"
                 nRegion = junction[idx]
             else:
                 pRegion = junction[idx]
 
             id_top = idx
 
             break
 
     # Now we check for an intrinsic region and, if there is, for the base.
-    if junction[idx + 1].role.lower() == 'intrinsic':
+    if junction[idx + 1].role.lower() == "intrinsic":
         iRegion = junction[idx + 1]
 
-        if junction[idx + 2].role.lower() == 'base':
+        if junction[idx + 2].role.lower() == "base":
             if pn_or_np == "pn":
                 nRegion = junction[idx + 2]
 
             else:
                 pRegion = junction[idx + 2]
 
             id_bottom = idx + 2
-            homojunction = homojunction and nRegion.material.material_string == pRegion.material.material_string
-            homojunction = homojunction and nRegion.material.material_string == iRegion.material.material_string
+            # homojunction = (
+            #   homojunction
+            #   and nRegion.material.material_string == pRegion.material.material_string
+            # )
+            # homojunction = (
+            #   homojunction
+            #   and nRegion.material.material_string == iRegion.material.material_string
+            # )
 
         else:
-            raise RuntimeError(
-                'ERROR processing junctions: A layer following the "intrinsic" layer must be defined as '
-                '"base".')
+            raise RuntimeError("ERROR processing junctions: A layer following the "
+                               '"intrinsic" layer must be defined as "base".')
 
     # If there is no intrinsic region, we check directly the base
-    elif junction[idx + 1].role.lower() == 'base':
+    elif junction[idx + 1].role.lower() == "base":
         if pn_or_np == "pn":
             nRegion = junction[idx + 1]
 
         else:
             pRegion = junction[idx + 1]
 
         iRegion = None
 
         id_bottom = idx + 1
-        homojunction = homojunction and nRegion.material.material_string == pRegion.material.material_string
+        # homojunction = (
+        #     homojunction
+        #     and nRegion.material.material_string == pRegion.material.material_string
+        # )
 
     else:
-        raise RuntimeError(
-            'ERROR processing junctions: A layer following the "emitter" must be defined as "intrinsic"'
-            'or "base".')
+        raise RuntimeError('ERROR processing junctions: A layer following the '
+                           '"emitter" must be defined as "intrinsic" or "base".')
 
     # We assert that we are really working with an homojunction
-    assert homojunction, 'ERROR: The DA solver only works with homojunctions, for now.'
-
+    # assert homojunction, "ERROR: The DA solver only works with homojunctions,
+    # for now."
 
     return id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np
 
 
 def identify_parameters(junction, T, pRegion, nRegion, iRegion):
-
     kbT = kb * T
 
     xp = pRegion.width
     xn = nRegion.width
     xi = 0 if iRegion is None else iRegion.width
 
     sn = 0 if not hasattr(junction, "sn") else junction.sn
     sp = 0 if not hasattr(junction, "sp") else junction.sp
 
     # Now we have to get all the material parameters needed for the calculation
+    # labels for permittivity refer to the doping of the layer
     if hasattr(junction, "permittivity"):
-        es = junction.permittivity
+        es_n = junction.permittivity
+        es_p = junction.permittivity
     else:
-        es = nRegion.material.permittivity  # equal for n and p.  I hope.
+        es_n = nRegion.material.permittivity
+        es_p = pRegion.material.permittivity
 
-    # For the diffusion length, subscript n and p refer to the carriers, electrons and holes
+    # For the diffusion length, subscript n and p refer to the carriers,
+    # electrons and holes
     if hasattr(junction, "ln"):
         ln = junction.ln
     else:
         ln = pRegion.material.electron_diffusion_length
 
     if hasattr(junction, "lp"):
         lp = junction.lp
     else:
         lp = nRegion.material.hole_diffusion_length
 
-    # For the diffusion coefficient, n and p refer to the regions, n side and p side. Yeah, it's confusing...
+    # For the diffusion coefficient, n and p refer to the regions,
+    # n side and p side. Yeah, it's confusing...
     if hasattr(junction, "mup"):
         dp = junction.mup * kbT / q
     else:
         dp = pRegion.material.electron_mobility * kbT / q
 
     if hasattr(junction, "mun"):
         dn = junction.mun * kbT / q
@@ -121,47 +137,63 @@
         dn = nRegion.material.hole_mobility * kbT / q
 
     ni = nRegion.material.ni
 
     Na = pRegion.material.Na
     Nd = nRegion.material.Nd
 
-    return xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es
+    return xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es_n, es_p
 
 
 def iv_depletion(junction, options):
-    """ Calculates the IV curve of a junction object using the depletion approximation as described in J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003). The junction is then updated with an "iv" function that calculates the IV curve at any voltage.
+    """Calculates the IV curve of a junction object using the depletion approximation as
+    described in J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003).
+    The junction is then updated with an "iv" function that calculates the IV curve at
+    any voltage.
 
     :param junction: A junction object.
     :param options: Solver options.
     :return: None.
     """
 
-    science_reference('Depletion approximation',
-                      'J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003).')
+    science_reference(
+        "Depletion approximation",
+        "J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003).",
+    )
 
     junction.voltage = options.internal_voltages
     T = options.T
     kbT = kb * T
 
     id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(junction)
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es = identify_parameters(junction, T, pRegion, nRegion, iRegion)
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es_n, es_p = identify_parameters(
+        junction, T, pRegion, nRegion, iRegion
+    )
 
     niSquared = ni**2
 
-    Vbi = (kbT / q) * np.log(Nd * Na / niSquared) if not hasattr(junction, "Vbi") else junction.Vbi  # Jenny p146
+    Vbi = (
+        (kbT / q) * np.log(Nd * Na / niSquared)
+        if not hasattr(junction, "Vbi")
+        else junction.Vbi
+    )  # Jenny p146
 
-    #Na, Nd, ni, niSquared, xi, ln, lp, xn, xp, sn, sp, dn, dp, es, id_top, id_bottom, Vbi, pn_or_np = process_junction(junction, options)
+    R_shunt = min(junction.R_shunt, 1e14) if hasattr(junction, "R_shunt") else 1e14
 
-    R_shunt = min(junction.R_shunt, 1e14) if hasattr(junction, 'R_shunt') else 1e14
-
-    # And now we account for the possible applied voltage, which can be, at most, equal to Vbi
+    # And now we account for the possible applied voltage,
+    # which can be, at most, equal to Vbi
     V = np.where(junction.voltage < Vbi - 0.001, junction.voltage, Vbi - 0.001)
 
-    wn, wp = get_depletion_widths(junction, es, Vbi, V, Na, Nd, xi)
+    wn, wp = get_depletion_widths(junction, es_n, es_p, Vbi, V, Na, Nd, xi)
+
+    # if the depletion region is calculated to be wider than the width of the n/p
+    # region itself, the whole region is depleted:
+
+    wn[wn > xn] = xn
+    wp[wp > xp] = xp
 
     w = wn + wp + xi
 
     # Now it is time to calculate currents
     if pn_or_np == "pn":
         l_top, l_bottom = ln, lp
         x_top, x_bottom = xp, xn
@@ -174,142 +206,197 @@
         x_bottom, x_top = xp, xn
         w_bottom, w_top = wp, wn
         s_bottom, s_top = sp, sn
         d_bottom, d_top = dp, dn
         min_bot, min_top = niSquared / Na, niSquared / Nd
 
     JtopDark = get_j_dark(x_top, w_top, l_top, s_top, d_top, V, min_top, T)
-    JbotDark = get_j_dark(x_bottom, w_bottom, l_bottom, s_bottom, d_bottom, V, min_bot, T)
+    JbotDark = get_j_dark(
+        x_bottom, w_bottom, l_bottom, s_bottom, d_bottom, V, min_bot, T
+    )
 
-    # hereby we define the subscripts to refer to the layer in which the current is generated:
+    # hereby we define the subscripts to refer to the layer in which
+    # the current is generated:
     if pn_or_np == "pn":
         JnDark, JpDark = JbotDark, JtopDark
     else:
         JpDark, JnDark = JbotDark, JtopDark
 
-    # These might not be the right lifetimes. Actually, they are not as they include all recombination processes, not
-    # just SRH recombination, which is what the equation in Jenny, p159 refers to. Let´ leave them, for now.
-    lifetime_n = ln ** 2 / dn
-    lifetime_p = lp ** 2 / dp  # Jenny p163
-
-    # Here we use the full version of the SRH recombination term as calculated by Sah et al. Works for positive bias
-    # and moderately negative ones.
-
-    science_reference('SRH current term.',
-                      'C. T. Sah, R. N. Noyce, and W. Shockley, “Carrier Generation and Recombination in P-N Junctions and P-N Junction Characteristics,” presented at the Proceedings of the IRE, 1957, vol. 45, no. 9, pp. 1228–1243.')
+    # These might not be the right lifetimes. Actually, they are not as
+    # they include all recombination processes, not just SRH recombination,
+    # which is what the equation in Jenny, p159 refers to. Let´s leave them, for now.
+    lifetime_n = ln**2 / dn
+    lifetime_p = lp**2 / dp  # Jenny p163
+
+    # Here we use the full version of the SRH recombination term as calculated by
+    # Sah et al. Works for positive bias and moderately negative ones.
+
+    science_reference(
+        "SRH current term.",
+        "C. T. Sah, R. N. Noyce, and W. Shockley, “Carrier Generation and "
+        "Recombination in P-N Junctions and P-N Junction Characteristics,” presented "
+        "at the Proceedings of the IRE, 1957, vol. 45, no. 9, pp. 1228–1243.",
+    )
     Jrec = get_Jsrh(ni, V, Vbi, lifetime_p, lifetime_n, w, kbT)
 
     J_sc_top = 0
     J_sc_bot = 0
     J_sc_scr = 0
 
     if options.light_iv:
-
         widths = []
         for layer in junction:
             widths.append(layer.width)
 
         cum_widths = np.cumsum([0] + widths)
 
         g = junction.absorbed
         wl = options.wavelength
-        wl_sp, ph = options.light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+        wl_sp, ph = options.light_source.spectrum(
+            output_units="photon_flux_per_m", x=wl
+        )
         id_v0 = np.argmin(abs(V))
 
         # The contribution from the Emitter (top side).
         xa = cum_widths[id_top]
         xb = cum_widths[id_top + 1] - w_top[id_v0]
 
-        if options.da_mode == 'bvp':
-            deriv = get_J_sc_diffusion(xa, xb, g, d_top, l_top, min_top, s_top, wl, ph, side='top')
+        if options.da_mode == "bvp":
+            deriv = get_J_sc_diffusion(
+                xa, xb, g, d_top, l_top, min_top, s_top, wl, ph, side="top"
+            )
         else:
-            xbb = xb - (xb - xa)/1001.
-            deriv = get_J_sc_diffusion_green(xa, xbb, g, d_top, l_top, min_top, s_top, ph, side='top')
-            deriv = np.trapz(deriv, wl)
+            xbb = xb - (xb - xa) / 1001.0
+
+            zz = np.linspace(xa, xb, 1001, endpoint=False)
+            gg = ph * g(zz)
+            g_vs_z = np.trapz(gg, wl, axis=1)
+            g_vs_z[np.isnan(g_vs_z)] = 0
+            g_vs_z = interp1d(zz, g_vs_z, axis=0)
+
+            deriv = get_J_sc_diffusion_green(
+                xa, xbb, g_vs_z, d_top, l_top, s_top, 1, side="top"
+            )
+
         J_sc_top = q * d_top * abs(deriv)
 
         # The contribution from the Base (bottom side).
         xa = cum_widths[id_bottom] + w_bottom[id_v0]
         xb = cum_widths[id_bottom + 1]
-        if options.da_mode == 'bvp':
-            deriv = get_J_sc_diffusion(xa, xb, g, d_bottom, l_bottom, min_bot, s_bottom, wl, ph, side='bottom')
+        if options.da_mode == "bvp":
+            deriv = get_J_sc_diffusion(
+                xa, xb, g, d_bottom, l_bottom, min_bot, s_bottom, wl, ph, side="bottom"
+            )
         else:
-            xbb = xb - (xb - xa)/1001.
-            deriv = get_J_sc_diffusion_green(xa, xbb, g, d_bottom, l_bottom, min_bot, s_bottom, ph, side='bottom')
-            deriv = np.trapz(deriv, wl)
+            xbb = xb - (xb - xa) / 1001.0
+            zz = np.linspace(xa, xb, 1001, endpoint=False)
+            gg = ph * g(zz)
+            g_vs_z = np.trapz(gg, wl, axis=1)
+            g_vs_z[np.isnan(g_vs_z)] = 0
+            g_vs_z = interp1d(zz, g_vs_z, axis=0)
+
+            deriv = get_J_sc_diffusion_green(
+                xa, xbb, g_vs_z, d_bottom, l_bottom, s_bottom, 1, side="bottom"
+            )
+            # photogeneration is included in g_vs_z, so set ph=1
+
         J_sc_bot = q * d_bottom * abs(deriv)
 
         # The contribution from the SCR (includes the intrinsic region, if present).
         xa = cum_widths[id_top + 1] - w_top[id_v0]
         xb = cum_widths[id_bottom] + w_bottom[id_v0]
         J_sc_scr = q * get_J_sc_SCR(xa, xb, g, wl, ph)
 
     # And, finally, we output the currents
-    junction.current = Jrec + JnDark + JpDark + V / R_shunt - J_sc_top - J_sc_bot - J_sc_scr
-    junction.iv = interp1d(junction.voltage, junction.current, kind='linear', bounds_error=False, assume_sorted=True,
-                           fill_value=(junction.current[0], junction.current[-1]))
-    junction.region_currents = State({"Jn_dif": JnDark, "Jp_dif": JpDark, "Jscr_srh": Jrec,
-                                      "J_sc_top": J_sc_top, "J_sc_bot": J_sc_bot, "J_sc_scr": J_sc_scr})
+    junction.current = (
+        Jrec + JnDark + JpDark + V / R_shunt - J_sc_top - J_sc_bot - J_sc_scr
+    )
+    junction.iv = interp1d(
+        junction.voltage,
+        junction.current,
+        kind="linear",
+        bounds_error=False,
+        assume_sorted=True,
+        fill_value=(junction.current[0], junction.current[-1]),
+    )
+    junction.region_currents = State(
+        {
+            "Jn_dif": JnDark,
+            "Jp_dif": JpDark,
+            "Jscr_srh": Jrec,
+            "J_sc_top": J_sc_top,
+            "J_sc_bot": J_sc_bot,
+            "J_sc_scr": J_sc_scr,
+        }
+    )
 
 
-def get_j_dark(x, w, l, s, d, V, minority, T):
+def get_j_dark(x, w, L, s, d, V, minority, T):
     """
     :param x: width of top junction
     :param w: depletion width in top junction
-    :param l: diffusion length
+    :param L: diffusion length
     :param s: surface recombination velocity
     :param d: diffusion coefficient
     :param V: voltage
     :param minority: minority carrier density
     :param T: Temperature
 
     :return: J_top_dark
     """
     # We calculate some fractions
 
-    harg = (x - w) / l
+    harg = (x - w) / L
     sinh_harg = np.sinh(harg)
     cosh_harg = np.cosh(harg)
-    lsod = (l * s) / d
+    lsod = (L * s) / d
 
     # And then we are ready to calculate the different currents
     # Missing the voltage dependent part of these equations.
     # They should be 6.34 and 6.39, not 6.62 and 6.63
 
-    J_dark = (q * d * minority / l) * (np.exp(q * V / kb / T) - 1) * \
-                 ((lsod * cosh_harg + sinh_harg) / (lsod * sinh_harg + cosh_harg))
+    J_dark = (
+        (q * d * minority / L)
+        * (np.exp(q * V / kb / T) - 1)
+        * ((lsod * cosh_harg + sinh_harg) / (lsod * sinh_harg + cosh_harg))
+    )
 
     return J_dark
 
 
 def get_Jsrh(ni, V, Vbi, tp, tn, w, kbT, dEt=0):
-    science_reference('SRH current term.',
-                      'C. T. Sah, R. N. Noyce, and W. Shockley, “Carrier Generation and Recombination in P-N Junctions and P-N Junction Characteristics,” presented at the Proceedings of the IRE, 1957, vol. 45, no. 9, pp. 1228–1243.')
+    science_reference(
+        "SRH current term.",
+        "C. T. Sah, R. N. Noyce, and W. Shockley, “Carrier Generation and Recombination"
+        " in P-N Junctions and P-N Junction Characteristics,” presented at the "
+        "Proceedings of the IRE, 1957, vol. 45, no. 9, pp. 1228–1243.",
+    )
 
     out = np.zeros(V.shape)
 
     m = V >= -1120 * kbT / q
     out[m] = forward(ni, V[m], Vbi, tp, tn, w[m], kbT)
 
     return out
 
 
 def forward(ni, V, Vbi, tp, tn, w, kbT, dEt=0):
-    """ Equation 27 of Sah's paper. Strictly speaking, it is not valid for intermediate negative bias. """
+    """Equation 27 of Sah's paper. Strictly speaking, it is not valid for
+    intermediate negative bias."""
 
     J0 = 2 * q * ni * w / np.sqrt(tn * tp)
     f = factor(V, Vbi, tp, tn, kbT, dEt)
     out = J0 * np.sinh(q * V / (2 * kbT)) / (q * (Vbi - V) / kbT) * f
 
     return out
 
 
 def factor(V, Vbi, tp, tn, kbT, dEt=0):
-    """ The integral of Eq. 27 in Sah's paper. While it is coninuum (in principle) it has to be done in two parts.
-    (or three) """
+    """The integral of Eq. 27 in Sah's paper. While it is continuum (in principle) it
+    has to be done in two parts (or three)"""
     trap = q * dEt / kbT + np.log(tp / tn) / 2
     b = np.exp(-q * V / kbT / 2) * np.cosh(trap)
 
     z1 = np.sqrt(tp / tn) * np.exp(-q * (Vbi - V) / kbT / 2)
     z2 = np.sqrt(tp / tn) * np.exp(q * (Vbi - V) / kbT / 2)
 
     out = np.zeros(b.shape)
@@ -320,15 +407,15 @@
     bot = np.arctan((b[m] + z1[m]) / np.sqrt(1 - b[m] ** 2))
 
     out[m] = (top - bot) / np.sqrt(1 - b[m] ** 2)
 
     # For b values >= 1 and <=1e7
     m = (b >= 1) * (b <= 1e7)
     xx = b[m]
-    yy = np.sqrt(xx ** 2 - 1)
+    yy = np.sqrt(xx**2 - 1)
 
     top = np.log(abs(z2[m] - yy + xx) / abs(z2[m] + yy + xx))
     bot = np.log(abs(z1[m] - yy + xx) / abs(z1[m] + yy + xx))
 
     out[m] = (top - bot) / (2 * yy)
 
     # For b values > 1e7
@@ -338,15 +425,15 @@
     bot = np.log(z1[m]) - np.log(z1[m] + 2 * b[m])
 
     out[m] = (top - bot) / (2 * b[m])
 
     return out
 
 
-def get_J_sc_diffusion(xa, xb, g, D, L, y0, S, wl, ph, side='top'):
+def get_J_sc_diffusion(xa, xb, g, D, L, y0, S, wl, ph, side="top"):
     """
     :param xa:
     :param xb:
     :param g:
     :param D:
     :param L:
     :param y0:
@@ -354,202 +441,272 @@
     :param wl:
     :param ph:
     :param side:
 
     :return: out
     """
 
+    # see comments in get_J_sc_diffusion_vs_WL for details on how differential
+    # equations are solved
     zz = np.linspace(xa, xb, 1001, endpoint=False)
     gg = g(zz) * ph
 
     g_vs_z = np.trapz(gg, wl, axis=1)
 
     g_vs_z[np.isnan(g_vs_z)] = 0
 
-    A = lambda x: np.interp(x, zz, g_vs_z) / D + y0 / L ** 2
+    def A(x):
+        return np.interp(x, zz, g_vs_z) / D + y0 / L**2
 
     def fun(x, y):
         out1 = y[1]
-        out2 = y[0] / L ** 2 - A(x)
+        out2 = y[0] / L**2 - A(x)
         return np.vstack((out1, out2))
 
-    if side == 'top':
+    if side == "top":
+
         def bc(ya, yb):
             left = ya[1] - S / D * (ya[0] - y0)
-            right = yb[0]
+            right = yb[0] - y0
             return np.array([left, right])
+
     else:
+
         def bc(ya, yb):
-            left = ya[0]
-            right = yb[1] - S / D * (yb[0] - y0)
+            left = ya[0] - y0
+            right = yb[1] + S / D * (yb[0] - y0)
             return np.array([left, right])
 
     guess = y0 * np.ones((2, zz.size))
     guess[1] = np.zeros_like(guess[0])
 
-    solution = solve_bvp(fun, bc, zz, guess)
+    solution = solve_bvp(fun, bc, zz, guess, max_nodes=2 * zz.shape[0])
 
-    if side == 'top':
+    if side == "top":
         out = solution.y[1][-1]
     else:
         out = solution.y[1][0]
 
+    if solution.status != 0:
+        warnings.warn(
+            "Depletion approximation (DA) I-V calculation: "
+            "solve_bvp did not converge as expected",
+            RuntimeWarning,
+        )
+
     return out
 
 
 def _conv_exp_top(x, xa, xb, g, L, phoD):
-    """Convolution of the carrier generation rate with the approximate Green's function kernel at point x. To be used with the numerical integration routine to compute the minority carrier derivative on the top edge. This kernel approximates the original one when the diffusion length is 2 orders of magnitude higher than the junction width by assuming that sinh(x) = cosh(x) = .5 * exp(x).
+    """Convolution of the carrier generation rate with the approximate Green's function
+    kernel at point x. To be used with the numerical integration routine to compute the
+    minority carrier derivative on the top edge. This kernel approximates the original
+    one when the diffusion length is 2 orders of magnitude higher than the junction
+    width by assuming that sinh(x) = cosh(x) = .5 * exp(x).
 
     :param x: Coordinate in the junction (variable to be integrated).
     :param xa: Coordinate at the start the junction.
     :param xb: Coordinate at the end the junction.
     :param g: Carrier generation rate at point x (expected as function).
     :param L: Diffusion length.
     :param phoD: Light spectrum divided by the diffusion constant D.
     """
     xc = (xa - x) / L
-    xv = np.array([xa + xb - x, ])
+    xv = np.array(
+        [
+            xa + xb - x,
+        ]
+    )
     Pkern = -np.exp(xc)
     Gx = g(xv) * phoD
-    return Pkern*Gx
+    return Pkern * Gx
 
 
 def _conv_exp_bottom(x, xa, g, L, phoD):
-    """Convolution of the carrier generation rate with the approximate Green's function kernel at point x. To be used with the numerical integration routine to compute the minority carrier derivative on the bottom edge. This kernel approximates the original one when the diffusion length is 2 orders of magnitude higher than the junction width by assuming that sinh(x) = cosh(x) = .5 * exp(x).
+    """Convolution of the carrier generation rate with the approximate Green's function
+    kernel at point x. To be used with the numerical integration routine to compute the
+    minority carrier derivative on the bottom edge. This kernel approximates the
+    original one when the diffusion length is 2 orders of magnitude higher than
+    the junction width by assuming that sinh(x) = cosh(x) = .5 * exp(x).
 
     :param x: Coordinate in the junction (variable to be integrated).
     :param xa: Coordinate at the start the junction.
     :param g: Carrier generation rate at point x (expected as function).
     :param L: Diffusion length.
     :param phoD: Light spectrum divided by the diffusion constant D.
     """
     xc = (xa - x) / L
-    xv = np.array([x, ])
+    xv = np.array(
+        [
+            x,
+        ]
+    )
     Pkern = np.exp(xc)
     Gx = g(xv) * phoD
-    return Pkern*Gx
+    return Pkern * Gx
 
 
 def _conv_green_top(x, xa, xb, g, L, phoD, crvel):
-    """Convolution of the carrier generation rate with the Green's function kernel at point x. To be used with the numerical integration routine to compute the minority carrier derivative on the top edge.
+    """Convolution of the carrier generation rate with the Green's function kernel at
+    point x. To be used with the numerical integration routine to compute the minority
+    carrier derivative on the top edge.
 
     :param x: Coordinate in the junction (variable to be integrated).
     :param xa: Coordinate at the start the junction.
     :param xb: Coordinate at the end the junction.
     :param g: Carrier generation rate at point x (expected as function).
     :param L: Diffusion length.
     :param phoD: Light spectrum divided by the diffusion constant D.
-    :param crvel: Coefficient computed as S / D * L, with S the surface recombination velocity.
+    :param crvel: Coefficient computed as S / D * L, with S the surface recombination
+         velocity.
     """
     xc = (xb - x) / L
-    xv = np.array([xa + xb - x, ])
+    xv = np.array(
+        [
+            xa + xb - x,
+        ]
+    )
     Pkern = np.cosh(xc) + crvel * np.sinh(xc)
     Gx = g(xv) * phoD
-    return Pkern*Gx
+
+    return Pkern * Gx
 
 
 def _conv_green_bottom(x, xb, g, L, phoD, crvel):
-    """Convolution of the carrier generation rate with the Green's function kernel at point x. To be used with the numerical integration routine to compute the minority carrier derivative on the bottom edge.
+    """Convolution of the carrier generation rate with the Green's function kernel at
+    point x. To be used with the numerical integration routine to compute the minority
+    carrier derivative on the bottom edge.
 
     :param x: Coordinate in the junction (variable to be integrated).
     :param xb: Coordinate at the end the junction.
     :param g: Carrier generation rate at point x (expected as function).
     :param L: Diffusion length.
     :param phoD: Light spectrum divided by the diffusion constant D.
-    :param crvel: Coefficient computed as S / D * L, with S the surface recombination velocity.
+    :param crvel: Coefficient computed as S / D * L, with S the surface recombination
+        velocity.
     """
     xc = (xb - x) / L
-    xv = np.array([x, ])
+    xv = np.array(
+        [
+            x,
+        ]
+    )
     Pkern = np.cosh(xc) - crvel * np.sinh(xc)
     Gx = g(xv) * phoD
-    return Pkern*Gx
+    return Pkern * Gx
 
 
-def get_J_sc_diffusion_green(xa, xb, g, D, L, y0, S, ph, side='top'):
-    """Computes the derivative of the minority carrier concentration at the edge of the junction by approximating the convolution integral resulting from applying the Green's function method to the drift-diffusion equation.
+def get_J_sc_diffusion_green(xa, xb, g, D, L, S, ph, side="top"):
+    """Computes the derivative of the minority carrier concentration at the edge of the
+    junction by approximating the convolution integral resulting from applying the
+    Green's function method to the drift-diffusion equation.
 
     :param xa: Coordinate at the start the junction.
     :param xb: Coordinate at the end the junction.
     :param g: Carrier generation rate at point x (expected as function).
     :param D: Diffusion constant.
     :param L: Diffusion length.
     :param y0: Carrier equilibrium density.
     :param S: Surface recombination velocity.
     :param ph: Light spectrum.
     :param side: String to indicate the edge of interest. Either 'top' or 'bottom'.
 
-    :return: The derivative of the minority carrier concentration at the edge of the junction.
+    :return: The derivative of the minority carrier concentration at the edge of the
+        junction.
     """
 
-    science_reference('DA Green\'s function method.',
-                      'T. Vasileiou, J. M. Llorens, J. Buencuerpo, J. M. Ripalda, D. Izzo and L. Summerer, “Light absorption enhancement and radiation hardening for triple junction solar cell through bioinspired nanostructures,” Bioinspir. Biomim., vol. 16, no. 5, pp. 056010, 2021.')
+    science_reference(
+        "DA Green's function method.",
+        "T. Vasileiou, J. M. Llorens, J. Buencuerpo, J. M. Ripalda, D. Izzo and "
+        "L. Summerer, “Light absorption enhancement and radiation hardening for triple "
+        "junction solar cell through bioinspired nanostructures,” "
+        "Bioinspir. Biomim., vol. 16, no. 5, pp. 056010, 2021.",
+    )
 
     xbL = (xb - xa) / L
     crvel = S / D * L
     ph_over_D = ph / D
 
     # if L too low in comparison to junction width, avoid nan's
-    if xbL > 1.e2:
-        if side == 'top':
-            cadd = -y0 / L
-            fun = partial(_conv_exp_top, xa=xa, xb=xb, g=g,
-                          L=L, phoD=ph_over_D)
+    if xbL > 1.0e2:
+        if side == "top":
+            fun = partial(_conv_exp_top, xa=xa, xb=xb, g=g, L=L, phoD=ph_over_D)
         else:
-            cadd = y0 / L
-            fun = partial(_conv_exp_bottom, xa=xa, g=g,
-                          L=L, phoD=ph_over_D)
-        cp = 1.
+            fun = partial(_conv_exp_bottom, xa=xa, g=g, L=L, phoD=ph_over_D)
+        cp = 1.0
+
     else:
-        if side == 'top':
+        if side == "top":
             cp = -np.cosh(xbL) - crvel * np.sinh(xbL)
-            cadd = (np.sinh(xbL) + crvel * np.cosh(xbL)) * y0 / L
-            fun = partial(_conv_green_top, xa=xa, xb=xb, g=g,
-                          L=L, phoD=ph_over_D, crvel=crvel)
+
+            fun = partial(
+                _conv_green_top, xa=xa, xb=xb, g=g, L=L, phoD=ph_over_D, crvel=crvel
+            )
         else:
-            cp = np.cosh(xbL) - crvel * np.sinh(xbL)
-            cadd = (np.sinh(xbL) - crvel * np.cosh(xbL)) * y0 / L
-            fun = partial(_conv_green_bottom, xb=xb, g=g,
-                          L=L, phoD=ph_over_D, crvel=crvel)
+            cp = np.cosh(xbL) + crvel * np.sinh(xbL)
 
-    out, err = quad_vec(fun, xa, xb, epsrel=1.e-5)
-    return (out.squeeze() + cadd) / cp
+            fun = partial(
+                _conv_green_bottom, xb=xb, g=g, L=L, phoD=ph_over_D, crvel=-crvel
+            )
+
+    out, err = quad_vec(fun, xa, xb, epsrel=1.0e-5)
+    return out.squeeze() / cp
 
 
 def get_J_sc_SCR(xa, xb, g, wl, ph):
     zz = np.linspace(xa, xb, 1001, endpoint=False)
     gg = g(zz) * ph
     out = np.trapz(np.trapz(gg, wl, axis=1), zz)
 
     return out
 
 
 def qe_depletion(junction, options):
-    """ Calculates the QE curve of a junction object using the depletion approximation as described in J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003). The junction is then updated with an "iqe" and several "eqe" functions that calculates the QE curve at any wavelength.
+    """Calculates the QE curve of a junction object using the depletion approximation as
+    described in J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003).
+    The junction is then updated with an "iqe" and several "eqe" functions that
+    calculates the QE curve at any wavelength.
 
     :param junction: A junction object.
     :param options: Solver options.
     :return: None.
     """
 
-    science_reference('Depletion approximation',
-                      'J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003).')
-
+    science_reference(
+        "Depletion approximation",
+        "J. Nelson, “The Physics of Solar Cells”, Imperial College Press (2003).",
+    )
 
     # First we have to figure out if we are talking about a PN, NP, PIN or NIP junction
     T = options.T
     kbT = kb * T
 
     id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(junction)
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es = identify_parameters(junction, T, pRegion, nRegion, iRegion)
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es_n, es_p = identify_parameters(
+        junction, T, pRegion, nRegion, iRegion
+    )
+
+    niSquared = ni**2
+
+    Vbi = (
+        (kbT / q) * np.log(Nd * Na / niSquared)
+        if not hasattr(junction, "Vbi")
+        else junction.Vbi
+    )  # Jenny p146
+
+    wn, wp = get_depletion_widths(junction, es_n, es_p, Vbi, 0, Na, Nd, xi)
 
-    niSquared = ni ** 2
+    # if the depletion region is calculated to be wider than the width of the n/p
+    # region itself, the whole region is depleted:
 
-    Vbi = (kbT / q) * np.log(Nd * Na / niSquared) if not hasattr(junction, "Vbi") else junction.Vbi  # Jenny p146
+    if wn > xn:
+        wn = xn
 
-    wn, wp = get_depletion_widths(junction, es, Vbi, 0, Na, Nd, xi)
+    if wp > xp:
+        wp = xp
 
     # Now it is time to calculate currents
     if pn_or_np == "pn":
         l_top, l_bottom = ln, lp
         w_top, w_bottom = wp, wn
         s_top, s_bottom = sp, sn
         d_top, d_bottom = dp, dn
@@ -565,143 +722,344 @@
     for layer in junction:
         widths.append(layer.width)
 
     cum_widths = np.cumsum([0] + widths)
 
     g = junction.absorbed
     wl = options.wavelength
-    wl_sp, ph = LightSource(source_type='black body', x=wl, T=6000).spectrum(output_units='photon_flux_per_m', x=wl)
-
+    wl_sp, ph = LightSource(source_type="black body", x=wl, T=6000).spectrum(
+        output_units="photon_flux_per_m", x=wl
+    )
+    # wl_sp, ph = options.light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    ph = 1e10 * np.ones_like(ph)
     # The contribution from the Emitter (top side).
     xa = cum_widths[id_top]
     xb = cum_widths[id_top + 1] - w_top
 
-    if options.da_mode == 'bvp':
-        deriv = get_J_sc_diffusion_vs_WL(xa, xb, g, d_top, l_top, min_top, s_top, wl, ph, side='top')
+    if options.da_mode == "bvp":
+        deriv = get_J_sc_diffusion_vs_WL(
+            xa, xb, g, d_top, l_top, min_top, s_top, wl, ph, side="top"
+        )
     else:
-        xbb = xb - (xb - xa)/1001.
-        deriv = get_J_sc_diffusion_green(xa, xbb, g, d_top, l_top, min_top, s_top, ph, side='top')
-    j_sc_top = d_top * abs(deriv)
+        xbb = xb - (xb - xa) / 1001.0
+        deriv = get_J_sc_diffusion_green(
+            xa, xbb, g, d_top, l_top, s_top, ph, side="top"
+        )
 
+    j_sc_top = d_top * abs(deriv)
 
     # The contribution from the Base (bottom side).
     xa = cum_widths[id_bottom] + w_bottom
     xb = cum_widths[id_bottom + 1]
 
-    if options.da_mode == 'bvp':
-        deriv = get_J_sc_diffusion_vs_WL(xa, xb, g, d_bottom, l_bottom, min_bot, s_bottom, wl, ph, side='bottom')
+    if options.da_mode == "bvp":
+        deriv = get_J_sc_diffusion_vs_WL(
+            xa, xb, g, d_bottom, l_bottom, min_bot, s_bottom, wl, ph, side="bottom"
+        )
     else:
-        xbb = xb - (xb - xa)/1001.
-        deriv = get_J_sc_diffusion_green(xa, xbb, g, d_bottom, l_bottom, min_bot, s_bottom, ph, side='bottom')
+        xbb = xb - (xb - xa) / 1001.0
+        deriv = get_J_sc_diffusion_green(
+            xa, xbb, g, d_bottom, l_bottom, s_bottom, ph, side="bottom"
+        )
+
     j_sc_bot = d_bottom * abs(deriv)
 
     # The contribution from the SCR (includes the intrinsic region, if present).
     xa = cum_widths[id_top + 1] - w_top
     xb = cum_widths[id_bottom] + w_bottom
     j_sc_scr = get_J_sc_SCR_vs_WL(xa, xb, g, wl, ph)
 
     # The total light absorbed, but not necessarily collected, is:
     xa = cum_widths[id_top]
     xb = cum_widths[id_bottom + 1]
-    zz = np.linspace(xa, xb, 10001)
+    zz = np.linspace(xa, xb, 1001)
     gg = g(zz) * ph
     current_absorbed = np.trapz(gg, zz, axis=0)
 
+    # why does this happen sometimes?
+    # j_sc_top[j_sc_top < 0] = 0
+    # j_sc_bot[j_sc_bot < 0] = 0
+    # j_sc_scr[j_sc_scr < 0] = 0
+
     # Now, we put everything together
     j_sc = j_sc_top + j_sc_bot + j_sc_scr
 
     eqe = j_sc / ph
     eqe_emitter = j_sc_top / ph
     eqe_base = j_sc_bot / ph
     eqe_scr = j_sc_scr / ph
 
-    iqe =  j_sc / current_absorbed
-    iqe[np.isnan(iqe)] = 0 # if zero current_absorbed, get NaN in previous line; want 0 IQE
+    iqe = np.divide(j_sc, current_absorbed,
+                    out=np.zeros_like(j_sc), where=current_absorbed != 0)
 
     junction.iqe = interp1d(wl, iqe)
 
-    junction.eqe = interp1d(wl, eqe, kind='linear', bounds_error=False, assume_sorted=True,
-                            fill_value=(eqe[0], eqe[-1]))
-    junction.eqe_emitter = interp1d(wl, eqe_emitter, kind='linear', bounds_error=False, assume_sorted=True,
-                                    fill_value=(eqe_emitter[0], eqe_emitter[-1]))
-    junction.eqe_base = interp1d(wl, eqe_base, kind='linear', bounds_error=False, assume_sorted=True,
-                                 fill_value=(eqe_base[0], eqe_base[-1]))
-    junction.eqe_scr = interp1d(wl, eqe_scr, kind='linear', bounds_error=False, assume_sorted=True,
-                                fill_value=(eqe_scr[0], eqe_scr[-1]))
+    junction.eqe = interp1d(
+        wl,
+        eqe,
+        kind="linear",
+        bounds_error=False,
+        assume_sorted=True,
+        fill_value=(eqe[0], eqe[-1]),
+    )
+    junction.eqe_emitter = interp1d(
+        wl,
+        eqe_emitter,
+        kind="linear",
+        bounds_error=False,
+        assume_sorted=True,
+        fill_value=(eqe_emitter[0], eqe_emitter[-1]),
+    )
+    junction.eqe_base = interp1d(
+        wl,
+        eqe_base,
+        kind="linear",
+        bounds_error=False,
+        assume_sorted=True,
+        fill_value=(eqe_base[0], eqe_base[-1]),
+    )
+    junction.eqe_scr = interp1d(
+        wl,
+        eqe_scr,
+        kind="linear",
+        bounds_error=False,
+        assume_sorted=True,
+        fill_value=(eqe_scr[0], eqe_scr[-1]),
+    )
+    junction.qe = State(
+        {
+            "WL": wl,
+            "IQE": junction.iqe(wl),
+            "EQE": junction.eqe(wl),
+            "EQE_emitter": junction.eqe_emitter(wl),
+            "EQE_base": junction.eqe_base(wl),
+            "EQE_scr": junction.eqe_scr(wl),
+        }
+    )
 
-    junction.qe = State({'WL': wl, 'IQE': junction.iqe(wl), 'EQE': junction.eqe(wl), 'EQE_emitter': junction.eqe_emitter(wl),
-                         'EQE_base': junction.eqe_base(wl), 'EQE_scr': junction.eqe_scr(wl)})
 
 def get_J_sc_SCR_vs_WL(xa, xb, g, wl, ph):
     zz = np.linspace(xa, xb, 1001, endpoint=False)
     gg = g(zz) * ph
     out = np.trapz(gg, zz, axis=0)
 
     return out
 
 
-def get_J_sc_diffusion_vs_WL(xa, xb, g, D, L, y0, S, wl, ph, side='top'):
-    zz = np.linspace(xa, xb, 1001, endpoint=False) # excluding the last point - depending on the mesh/floating point errors, sometimes this is actually in the next layer
-    gg = g(zz) * ph
+def get_J_sc_diffusion_vs_WL(xa, xb, g, D, L, y0, S, wl, ph, side="top"):
+    zz = np.linspace(xa, xb, 1001, endpoint=False)
+    # excluding the last point - depending on the mesh/floating point errors,
+    # sometimes this is actually in the next layer
+
+    gg = g(zz) * ph  # generation rate * photon flux
+
     out = np.zeros_like(wl)
+    sol_success = np.zeros_like(wl)  # keep track of whether solve_bvp is converging
 
     for i in range(len(wl)):
-
-        if np.all(gg[:,i] == 0): # no reason to solve anything if no generation at this wavelength
+        if np.all(
+            gg[:, i] == 0
+        ):  # no reason to solve anything if no generation at this wavelength
             out[i] = 0
+            sol_success[i] = 0
 
         else:
-            A = lambda x: np.interp(x, zz, gg[:, i]) / D + y0 / L ** 2
+
+            def A(x):
+                return np.interp(x, zz, gg[:, i]) / D + y0 / L**2
+
+            # generation and n0/p0 term in differential equation
+            # (eq. 6.15 & 6.20 in Jenny Nelson, Physics of Solar Cells)
 
             def fun(x, y):
-                out1 = y[1]
-                out2 = y[0] / L ** 2 - A(x)
+                # differential equation (eq. 6.15 & 6.20 in Jenny Nelson,
+                # Physics of Solar Cells)
+                # solve_bvp solves equation of form:
+                # dy / dx = f(x, y, p), a <= x <= b
+                # in this case y = [n or p, dn/dx or dp/dx]
+                # y[0] = carrier concentration (n or p)
+                # y[1] = carrier concentration gradient (dn/dx or dp/dx)
+                out1 = y[1]  # by definition! dy/dx = dy/dx
+
+                out2 = y[0] / L**2 - A(x)
+                # actually solving the differential equation (6.15 & 6.20)
+
                 return np.vstack((out1, out2))
 
-            if side == 'top':
+            # boundary conditions for solve_bvp:
+            if side == "top":
+
                 def bc(ya, yb):
                     left = ya[1] - S / D * (ya[0] - y0)
-                    right = yb[0]
+                    # eq. 6.18 - b.c. at front of junction (surface recombination)
+
+                    right = yb[0] - y0
+                    # eq. 6.17 - b.c. edge of depletion region, top half of junction
+                    # added - y0 (generally very small so makes almost no difference)
                     return np.array([left, right])
+
             else:
+
                 def bc(ya, yb):
-                    left = ya[0]
-                    right = yb[1] - S / D * (yb[0] - y0)
+                    left = ya[0] - y0
+                    # eq. 6.21 - b.c. edge of depletion region, bottom half of junction
+                    # added - y0 (generally very small so makes almost no difference)
+
+                    right = yb[1] + S / D * (yb[0] - y0)
+                    # eq. 6.22 - b.c. at back of junction (surface recombination)
+                    # changed sign! Current is going the other way
                     return np.array([left, right])
 
             guess = y0 * np.ones((2, zz.size))
             guess[1] = np.zeros_like(guess[0])
-            solution = solve_bvp(fun, bc, zz, guess)
 
-            if side == 'top':
+            solution = solve_bvp(fun, bc, zz, guess, max_nodes=2 * zz.shape[0])
+            # increase max_nodes to avoid "too many mesh points" message
+
+            sol_success[i] = solution.status
+
+            if side == "top":
                 out[i] = solution.y[1][-1]
+                # current at edge of depletion region (top half of junction), eq. 6.33
             else:
                 out[i] = solution.y[1][0]
+                # current at edge of depletion region (bottom half of junction), eq 6.38
 
-    return out
+        # give a warning f any of the solution statuses are not 0 using warnings.warn:
+        if np.any(sol_success != 0):
+            warnings.warn(
+                "Depletion approximation (DA) EQE calculation: "
+                "solve_bvp did not converge as expected for some wavelengths",
+                RuntimeWarning,
+            )
 
+    return out
 
-def get_depletion_widths(junction, es, Vbi, V, Na, Nd, xi):
 
+def get_depletion_widths(junction, es_n, es_p, Vbi, V, Na, Nd, xi):
     if not hasattr(junction, "wp") or not hasattr(junction, "wn"):
-
-        if hasattr(junction, "depletion_approximation") and junction.depletion_approximation == "one-sided abrupt":
+        if (
+            hasattr(junction, "depletion_approximation")
+            and junction.depletion_approximation == "one-sided abrupt"
+        ):
             print("using one-sided abrupt junction approximation for depletion width")
             one_sided = True
         else:
             one_sided = False
 
-
         if one_sided:
-            science_reference("Sze abrupt junction approximation",
-                              "Sze: The Physics of Semiconductor Devices, 2nd edition, John Wiley & Sons, Inc (2007)")
-            wn = np.sqrt(2 * es * (Vbi - V) / (q * Nd))
-            wp = np.sqrt(2 * es * (Vbi - V) / (q * Na))
+            science_reference(
+                "Sze abrupt junction approximation",
+                "Sze: The Physics of Semiconductor Devices, "
+                "2nd edition, John Wiley & Sons, Inc (2007)",
+            )
+            wn = np.sqrt(2 * es_n * (Vbi - V) / (q * Nd))
+            wp = np.sqrt(2 * es_p * (Vbi - V) / (q * Na))
 
         else:
-            wn = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Nd / Na)
-            wp = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Na / Nd)
+            wn = (
+                -xi + np.sqrt(xi**2 + 2.0 * es_n * (Vbi - V) / q * (1 / Na + 1 / Nd))
+            ) / (1 + Nd / Na)
+            wp = (
+                -xi + np.sqrt(xi**2 + 2.0 * es_p * (Vbi - V) / q * (1 / Na + 1 / Nd))
+            ) / (1 + Na / Nd)
 
     wn = wn if not hasattr(junction, "wn") else junction.wn
     wp = wp if not hasattr(junction, "wp") else junction.wp
 
-    return wn, wp
+    return wn, wp
+
+
+# def iv_depletion_analytical(junction, options):
+#     """Calculates the IV curve of a junction object using the analytical solutions to
+#     the depletion approximation with Beer-Lambert absorption as described in e.g. J.
+#     Nelson, “The Physics of Solar Cells”, Imperial College Press (2003). Note that the
+#     equations used here are not exactly those from the book, as they contain typos.
+#     The junction is then updated with an "iv" function that calculates the IV curve at
+#     any voltage.
+#
+#     :param junction: A junction object.
+#     :param options: Solver options.
+#     :return: None.
+#     """
+#
+#     pass
+
+
+# def minority_carrier_top_analytical(x, L, alpha, xa, D, S, n0, A):
+#     aL = alpha * L
+#     a1 = -aL * np.exp(2 * alpha * (x + xa) + (2 * x / L)) + aL * np.exp(
+#         2 * alpha * (x + xa) + (2 * xa / L)
+#     )
+#
+#     a2 = np.exp(2 * alpha * x + alpha * xa + (xa / L)) - np.exp(
+#         alpha * x + 2 * alpha * xa + (x / L)
+#     )
+#
+#     a3 = np.exp(((aL + 1) * (2 * x + xa)) / L) - np.exp(((aL + 1) * (x + 2 * xa)) / L)
+#
+#     b1 = np.exp(((aL + 1) * (2 * x + xa)) / L) - np.exp(((aL + 1) * (x + 2 * xa)) / L)
+#
+#     b2 = np.exp(alpha * x + 2 * alpha * xa + (x / L)) - np.exp(
+#         2 * alpha * x + alpha * xa + (xa / L)
+#     )
+#
+#     b3 = -np.exp(2 * alpha * (x + xa) + (2 * x / L)) + np.exp(
+#         2 * alpha * (x + xa) + (2 * xa / L)
+#     )
+#
+#     numerator = (
+#         A
+#         * L**2
+#         * np.exp(-2 * alpha * (x + xa) - (x / L))
+#         * (D * (a1 + a2 + a3) + L * S * (b1 + b2 + b3))
+#     )
+#     denominator = (
+#         D
+#         * (alpha**2 * L**2 - 1)
+#         * (D * (np.exp(2 * xa / L) + 1) + L * S * (np.exp(2 * xa / L) - 1))
+#     )
+#     result = numerator / denominator + n0
+#
+#     return result
+
+
+# def minority_carrier_bottom_analytical(x, L, alpha, xb, D, S, p0, A):
+#     aL = alpha * L
+#     denominator = (
+#         D
+#         * (-1 + alpha**2 * L**2)
+#         * (D * (1 + np.exp((2 * xb) / L)) + (-1 + np.exp((2 * xb) / L)) * L * S)
+#     )
+#
+#     a1 = np.exp((2 * xb) / L + 2 * alpha * (x + xb)) - np.exp(
+#         (((1 + aL) * (x + 2 * xb)) / L)
+#     )
+#
+#     a2 = np.exp((2 * x) / L + 2 * alpha * (x + xb)) - np.exp(
+#         alpha * x + x / L + 2 * alpha * xb
+#     )
+#
+#     a3 = (
+#         alpha * np.exp(2 * alpha * x + alpha * xb + xb / L) * L
+#         - alpha * np.exp(((1 + aL) * (2 * x + xb)) / L) * L
+#     )
+#
+#     b1 = np.exp(((1 + aL) * (2 * x + xb)) / L) - np.exp(((1 + aL) * (x + 2 * xb)) / L)
+#
+#     b2 = +np.exp(alpha * x + x / L + 2 * alpha * xb) - np.exp(
+#         2 * alpha * x + alpha * xb + xb / L
+#     )
+#
+#     b3 = np.exp((2 * xb) / L + 2 * alpha * (x + xb)) - np.exp(
+#         (2 * x) / L + 2 * alpha * (x + xb)
+#     )
+#
+#     numerator = (
+#         A
+#         * np.exp(-(x / L) - 2 * alpha * (x + xb))
+#         * L**2
+#         * (D * (a1 + a2 + a3) + (b1 + b2 + b3) * L * S)
+#     )
+#
+#     p = p0 + numerator / denominator
+#     return p
```

### Comparing `solcore-5.9.1/solcore/analytic_solar_cells/detailed_balance.py` & `solcore-5.9.2/solcore/analytic_solar_cells/detailed_balance.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/analytic_solar_cells/diode_equation.py` & `solcore-5.9.2/solcore/analytic_solar_cells/diode_equation.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/analytic_solar_cells/tunnel_junctions.py` & `solcore-5.9.2/solcore/analytic_solar_cells/tunnel_junctions.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/config_tools.py` & `solcore-5.9.2/solcore/config_tools.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/crystals.py` & `solcore-5.9.2/solcore/crystals.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/data_analysis_tools/ellipsometry_analysis.py` & `solcore-5.9.2/solcore/data_analysis_tools/ellipsometry_analysis.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/graphing/Colours.txt` & `solcore-5.9.2/solcore/graphing/Colours.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/graphing/Custom_Colours.py` & `solcore-5.9.2/solcore/graphing/Custom_Colours.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/graphing/graph.py` & `solcore-5.9.2/solcore/graphing/graph.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/graphing/graph_lines.py` & `solcore-5.9.2/solcore/graphing/graph_lines.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/graphing/graph_support.py` & `solcore-5.9.2/solcore/graphing/graph_support.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/interpolate.py` & `solcore-5.9.2/solcore/interpolate.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/light_source/SPCTRAL_si_units.txt` & `solcore-5.9.2/solcore/light_source/SPCTRAL_si_units.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/light_source/astmg173.csv` & `solcore-5.9.2/solcore/light_source/astmg173.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/light_source/light_source.py` & `solcore-5.9.2/solcore/light_source/light_source.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/light_source/smarts.py` & `solcore-5.9.2/solcore/light_source/smarts.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/light_source/spectral2.py` & `solcore-5.9.2/solcore/light_source/spectral2.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Adachi/binaries.txt` & `solcore-5.9.2/solcore/material_data/Adachi/binaries.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlAs-Material/k.txt` & `solcore-5.9.2/solcore/material_data/AlAs-Material/k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlAs-Material/n.txt` & `solcore-5.9.2/solcore/material_data/AlAs-Material/n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.000_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.000_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.099_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.099_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.198_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.198_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.315_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.315_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.419_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.419_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.491_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.491_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.590_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.590_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.700_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.700_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/0.804_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/0.804_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/1.000_AlGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/1.000_AlGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/k/critical_points.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/k/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.000_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.000_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.099_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.099_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.198_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.198_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.315_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.315_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.419_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.419_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.491_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.491_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.590_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.590_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.700_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.700_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/0.804_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/0.804_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/1.000_AlGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/1.000_AlGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlGaAs-Material/n/critical_points.txt` & `solcore-5.9.2/solcore/material_data/AlGaAs-Material/n/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlInP-Material/__init__.py` & `solcore-5.9.2/solcore/material_data/AlInP-Material/__init__.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlInP-Material/k/0.000_AlInP_k.txt` & `solcore-5.9.2/solcore/material_data/AlInP-Material/k/0.000_AlInP_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlInP-Material/k/0.530_AlInP_k.txt` & `solcore-5.9.2/solcore/material_data/AlInP-Material/k/0.530_AlInP_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlInP-Material/k/critical_points.txt` & `solcore-5.9.2/solcore/material_data/AlInP-Material/k/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlInP-Material/n/0.000_AlInP_n.txt` & `solcore-5.9.2/solcore/material_data/AlInP-Material/n/0.000_AlInP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlInP-Material/n/0.530_AlInP_n.txt` & `solcore-5.9.2/solcore/material_data/AlInP-Material/n/0.530_AlInP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/AlInP-Material/n/1.000_AlInP_n.txt` & `solcore-5.9.2/solcore/material_data/AlInP-Material/n/1.000_AlInP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaAs-Material/k.txt` & `solcore-5.9.2/solcore/material_data/GaAs-Material/k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaAs-Material/n.txt` & `solcore-5.9.2/solcore/material_data/GaAs-Material/n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaAsP-Material/k/0.000_GaAsP_k.txt` & `solcore-5.9.2/solcore/material_data/GaAsP-Material/k/0.000_GaAsP_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaAsP-Material/k/1.000_GaAsP_k.txt` & `solcore-5.9.2/solcore/material_data/GaAsP-Material/k/1.000_GaAsP_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaAsP-Material/k/critical_points.txt` & `solcore-5.9.2/solcore/material_data/GaAsP-Material/k/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaAsP-Material/n/0.000_GaAsP_n.txt` & `solcore-5.9.2/solcore/material_data/GaAsP-Material/n/0.000_GaAsP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaAsP-Material/n/1.000_GaAsP_n.txt` & `solcore-5.9.2/solcore/material_data/GaAsP-Material/n/1.000_GaAsP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/k/0.000_GaInP_k.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/k/0.000_GaInP_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/k/0.490_GaInP_k.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/k/0.490_GaInP_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/k/1.000_GaInP_k.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/k/1.000_GaInP_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/k/critical_points.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/k/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/n/0.000_GaInP_n.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/n/0.000_GaInP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/n/0.490_GaInP_n.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/n/0.490_GaInP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/n/1.000_GaInP_n.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/n/1.000_GaInP_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaInP-Material/n/critical_points.txt` & `solcore-5.9.2/solcore/material_data/GaInP-Material/n/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaSb-Material/k.txt` & `solcore-5.9.2/solcore/material_data/GaSb-Material/k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/GaSb-Material/n.txt` & `solcore-5.9.2/solcore/material_data/GaSb-Material/n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Ge-Material/k.txt` & `solcore-5.9.2/solcore/material_data/Ge-Material/k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Ge-Material/n.txt` & `solcore-5.9.2/solcore/material_data/Ge-Material/n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.000_Strained_InGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.000_Strained_InGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.100_Strained_InGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.100_Strained_InGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.200_Strained_InGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.200_Strained_InGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/k/0.240_Strained_InGaAs_k.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/k/0.240_Strained_InGaAs_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/k/critical_points.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/k/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.000_Strained_InGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.000_Strained_InGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.100_Strained_InGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.100_Strained_InGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.200_Strained_InGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.200_Strained_InGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/n/0.240_Strained_InGaAs_n.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/n/0.240_Strained_InGaAs_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaAs-Material/n/critical_points.txt` & `solcore-5.9.2/solcore/material_data/InGaAs-Material/n/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.000_InGaSb_K.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.000_InGaSb_K.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.100_InGaSb_K.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.100_InGaSb_K.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.300_InGaSb_K.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.300_InGaSb_K.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.500_InGaSb_K.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.500_InGaSb_K.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.700_InGaSb_K.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.700_InGaSb_K.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/0.900_InGaSb_K.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/0.900_InGaSb_K.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/1.000_InGaSb_K.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/1.000_InGaSb_K.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/k/critical_points.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/k/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.000_InGaSb_N.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.000_InGaSb_N.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.100_InGaSb_N.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.100_InGaSb_N.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.300_InGaSb_N.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.300_InGaSb_N.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.500_InGaSb_N.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.500_InGaSb_N.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.700_InGaSb_N.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.700_InGaSb_N.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/0.900_InGaSb_N.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/0.900_InGaSb_N.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/1.000_InGaSb_N.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/1.000_InGaSb_N.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InGaSb-Material/n/critical_points.txt` & `solcore-5.9.2/solcore/material_data/InGaSb-Material/n/critical_points.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InP-Material/info.txt` & `solcore-5.9.2/solcore/material_data/InP-Material/info.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InP-Material/k.txt` & `solcore-5.9.2/solcore/material_data/InP-Material/k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InP-Material/n.txt` & `solcore-5.9.2/solcore/material_data/InP-Material/n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InSb-Material/k.txt` & `solcore-5.9.2/solcore/material_data/InSb-Material/k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/InSb-Material/n.txt` & `solcore-5.9.2/solcore/material_data/InSb-Material/n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Levinshtein/GroupIV.txt` & `solcore-5.9.2/solcore/material_data/Levinshtein/GroupIV.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/7059.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/7059.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/AG.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/AG.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/AL.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/AL.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/AL2O3.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/AL2O3.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/AL2O3P.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/AL2O3P.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS028T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS028T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS052T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS052T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS072T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS072T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS098T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS098T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS125T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS125T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS152T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS152T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS178T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS178T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS204T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS204T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS228T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS228T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS305T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS305T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS331T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS331T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS361T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS361T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS390T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS390T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS421T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS421T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS445T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS445T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS469T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS469T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS499T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS499T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS527T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS527T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS552T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS552T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS578T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS578T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS602T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS602T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS626T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS626T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS028T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS028T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS052T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS052T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS072T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS072T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS098T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS098T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS125T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS125T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS152T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS152T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS178T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS178T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS204T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS204T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS228T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS228T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS305T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS305T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS331T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS331T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS361T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS361T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS390T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS390T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS421T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS421T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS445T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS445T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS469T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS469T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS499T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS499T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS527T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS527T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS552T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS552T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS578T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS578T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS602T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS602T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALAS_T/ALAS626T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALAS_T/ALAS626T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALCU.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALCU.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS30.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS30.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS40.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS40.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS50.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS50.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS60.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS60.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS70.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS70.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS80.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS80.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS90.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAAS_AL/ALGAAS90.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP30.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP30.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP60.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP60.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP70.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALGAINP_AL/AGAINP70.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALON.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALON.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALSB.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALSB.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALSI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALSI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ALSITI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ALSITI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ARACHI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ARACHI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ASI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ASI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/AU.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/AU.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/BAF2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/BAF2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/BK7.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/BK7.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CAF2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CAF2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CARBAM.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CARBAM.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CCL4.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CCL4.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CDSE.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CDSE.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CDTE.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CDTE.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CO.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CO.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/COR7059.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/COR7059.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/COSI2-4.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/COSI2-4.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CO_2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CO_2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CR.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CR.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CR3SI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CR3SI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CR5SI3.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CR5SI3.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CRSI2EL2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CRSI2EL2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CU.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CU.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CU2O.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CU2O.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/CUO.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/CUO.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/DIAM.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/DIAM.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/FESI2EL1.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/FESI2EL1.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/FESI2EL2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/FESI2EL2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/FESI2EPI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/FESI2EPI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS031T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS031T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS041T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS041T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS060T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS060T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS081T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS081T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS103T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS103T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS111.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS111.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS126T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS126T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS150T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS150T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS175T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS175T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS199T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS199T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS224T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS224T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS249T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS249T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS273T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS273T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS297T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS297T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS320T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS320T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS344T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS344T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS367T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS367T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS391T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS391T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS415T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS415T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS443T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS443T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS465T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS465T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS488T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS488T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS515T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS515T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS546T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS546T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS579T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS579T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS603T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS603T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS634T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS634T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAASO.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAASO.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAASOX.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAASOX.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS031T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS031T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS041T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS041T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS060T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS060T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS081T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS081T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS103T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS103T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS126T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS126T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS150T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS150T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS175T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS175T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS199T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS199T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS224T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS224T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS249T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS249T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS273T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS273T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS297T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS297T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS320T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS320T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS344T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS344T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS367T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS367T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS391T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS391T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS415T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS415T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS443T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS443T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS465T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS465T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS488T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS488T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS515T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS515T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS546T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS546T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS579T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS579T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS603T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS603T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAAS_T/GAAS634T.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAAS_T/GAAS634T.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAP.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAP.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAP100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAP100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GAPOX.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GAPOX.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GASB.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GASB.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GASBOX.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GASBOX.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GE.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GE.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/GE100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/GE100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/H2O.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/H2O.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/HFO2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/HFO2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/HFSI2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/HFSI2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE30.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/HGCDTE_CD/HGCDTE30.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INAS.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INAS.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INASOX.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INASOX.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGAAS.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGAAS.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB30.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB30.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB50.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB50.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB70.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB70.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB90.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INGASB_GA/INGASB90.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INP.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INP.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INPOX.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INPOX.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INSB.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INSB.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/INSBOX.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/INSBOX.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/IR.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/IR.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/IR3SI5E.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/IR3SI5E.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/IR3SI5P.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/IR3SI5P.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ITO2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ITO2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/KCL.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/KCL.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/LASF9.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/LASF9.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/LI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/LI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/LIF.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/LIF.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/List_Of_Files.xlsx` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/List_Of_Files.xlsx`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/List_Of_Files_Updated_PDF.pdf` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/List_Of_Files_Updated_PDF.pdf`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/MGF2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/MGF2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/MO.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/MO.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/MOSI2-A.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/MOSI2-A.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/MOSI2-B.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/MOSI2-B.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/NBSI-A.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/NBSI-A.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/NBSI-B.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/NBSI-B.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/NI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/NI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/NI2SI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/NI2SI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/NI3SI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/NI3SI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/NISI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/NISI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/OS.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/OS.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/PBS.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/PBS.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/PBSE.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/PBSE.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/PD.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/PD.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/PD2SI-A.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/PD2SI-A.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/PD2SI-B.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/PD2SI-B.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/PT.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/PT.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/P_SIAS.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/P_SIAS.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/P_SIUD.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/P_SIUD.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS24.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/REINGAAS_IN/RINGAS24.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESI1-75.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESI1-75.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE11.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE11.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE22.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE22.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE39.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE39.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE51.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE51.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE64.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE64.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE75.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE75.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE83.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE83.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE91.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RESIGE_GE/RESIGE91.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RH.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RH.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS0.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS0.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/RINGAS24.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/RINGAS24.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SF11.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SF11.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SI100_2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SI100_2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SI110.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SI110.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SI111.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SI111.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SI3N4.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SI3N4.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIAM1.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIAM1.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIAM2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIAM2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIC.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIC.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T02.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T02.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T15.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T15.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T25.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T25.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T30.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T30.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T35.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T35.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T40.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T40.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR-T45.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR-T45.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T020.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T020.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T150.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T150.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T200.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T200.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T250.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T250.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T300.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T300.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T350.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T350.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T400.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T400.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SICR_T/SICR-T450.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SICR_T/SICR-T450.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_GE.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_GE.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE11.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE11.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE28.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE28.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE65.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE65.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE85.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE85.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE98.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI/SIGE98.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIGE_SI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIGE_SI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIO.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIO.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIO2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIO2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION0.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION0.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION40.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION40.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION60.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION60.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION80.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION80.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION40.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION40.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION60.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION60.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SION_N/SION80.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SION_N/SION80.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIOP.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIOP.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY30.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY30.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY40.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY40.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY50.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY50.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY60.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY60.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY70.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY70.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY80.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY80.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY90.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPOLY_X/SIPOLY90.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SIPORE.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SIPORE.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/SOPRA_DB_Updated.csv` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/SOPRA_DB_Updated.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS20.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS20.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS24.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STINGAAS_IN/SINGAS24.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG0.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG0.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG06.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG06.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG12.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG12.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG17.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG17.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG22.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/STSIGE_GE/STSG22.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TA.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TA.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TAOX1.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TAOX1.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TAOX2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TAOX2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TASI2-A.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TASI2-A.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TASI2-B.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TASI2-B.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TEST.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TEST.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/THF4.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/THF4.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TINI.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TINI.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TIO2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TIO2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TIO2B.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TIO2B.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/TISI-A.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/TISI-A.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/V.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/V.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/VOID.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/VOID.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/VSI2-A.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/VSI2-A.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/VSI2-B.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/VSI2-B.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/W.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/W.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/WSI2-A.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/WSI2-A.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/WSI2-B.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/WSI2-B.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/Y2O3.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/Y2O3.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE00.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE00.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE100.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE100.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE30.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE30.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE50.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE50.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE70.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE70.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE90.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNCDTE_CD/ZNCDTE90.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSCUB.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSCUB.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSE.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSE.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE0.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE0.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE1.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE1.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE10.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE10.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE3.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE3.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE5.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE5.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE7.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE7.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE9.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZNSETE_TE/ZNSETE9.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZRO2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZRO2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/SOPRA_DB/ZRSI2.MAT` & `solcore-5.9.2/solcore/material_data/SOPRA_DB/ZRSI2.MAT`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Si-Material/info.txt` & `solcore-5.9.2/solcore/material_data/Si-Material/info.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Si-Material/k.txt` & `solcore-5.9.2/solcore/material_data/Si-Material/k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Si-Material/n.txt` & `solcore-5.9.2/solcore/material_data/Si-Material/n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Vurgaftman/binaries.txt` & `solcore-5.9.2/solcore/material_data/Vurgaftman/binaries.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/Vurgaftman/ternaries.txt` & `solcore-5.9.2/solcore/material_data/Vurgaftman/ternaries.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/mobility.py` & `solcore-5.9.2/solcore/material_data/mobility.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/mobility_parameters.json` & `solcore-5.9.2/solcore/material_data/mobility_parameters.json`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/refractiveindex_info_DB/dbmaterial.py` & `solcore-5.9.2/solcore/material_data/refractiveindex_info_DB/dbmaterial.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_data/refractiveindex_info_DB/dboperations.py` & `solcore-5.9.2/solcore/material_data/refractiveindex_info_DB/dboperations.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_system/create_new_material.py` & `solcore-5.9.2/solcore/material_system/create_new_material.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_system/critical_point_interpolate.py` & `solcore-5.9.2/solcore/material_system/critical_point_interpolate.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_system/critical_point_picker.py` & `solcore-5.9.2/solcore/material_system/critical_point_picker.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/material_system/material_system.py` & `solcore-5.9.2/solcore/material_system/material_system.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/meson.build` & `solcore-5.9.2/solcore/meson.build`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/optics/beer_lambert.py` & `solcore-5.9.2/solcore/optics/beer_lambert.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/optics/external_optics.py` & `solcore-5.9.2/solcore/optics/external_optics.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/optics/rcwa.py` & `solcore-5.9.2/solcore/optics/rcwa.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,22 +182,25 @@
 
 def calculate_absorption_rcwa(tmm_out, initial=1):
     all_z = tmm_out["position"] * 1e-9
     all_abs = initial * tmm_out["absorption"] / 1e-9
 
     def diff_absorption(z):
         idx = all_z.searchsorted(z)
-        idx = np.where(idx <= len(all_z) - 2, idx, len(all_z) - 2)
-        try:
-            z1 = all_z[idx]
-            z2 = all_z[idx + 1]
+        idx = np.where(idx <= len(all_z) - 1, idx, len(all_z) - 1)
+        idx = np.where(idx > 0, idx, 1)
 
-            f = (z - z1) / (z2 - z1)
+        try:
+            z1 = all_z[idx - 1]
+            z2 = all_z[idx]
 
-            out = f * all_abs[:, idx] + (1 - f) * all_abs[:, idx + 1]
+            f = np.divide(z - z1, z2 - z1,
+                          out=np.zeros_like(z), where=np.abs(z2-z1) > 1e-12)
+            # this is to avoid divide by zero errors (|f| gets very large) when z1 = z2
+            out = (1-f) * all_abs[:, idx - 1] + f * all_abs[:, idx]
 
         except IndexError:
             out = all_abs[:, idx]
 
         return out
 
     all_absorbed = np.trapz(diff_absorption(all_z), all_z)
```

### Comparing `solcore-5.9.1/solcore/optics/tmm.py` & `solcore-5.9.2/solcore/optics/tmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,22 +187,25 @@
 
 def calculate_absorption_tmm(tmm_out, initial=1):
     all_z = tmm_out["position"] * 1e-9
     all_abs = initial * tmm_out["absorption"] / 1e-9
 
     def diff_absorption(z):
         idx = all_z.searchsorted(z)
-        idx = np.where(idx <= len(all_z) - 2, idx, len(all_z) - 2)
-        try:
-            z1 = all_z[idx]
-            z2 = all_z[idx + 1]
+        idx = np.where(idx <= len(all_z) - 1, idx, len(all_z) - 1)
+        idx = np.where(idx > 0, idx, 1)
 
-            f = (z - z1) / (z2 - z1)
+        try:
+            z1 = all_z[idx - 1]
+            z2 = all_z[idx]
 
-            out = f * all_abs[:, idx] + (1 - f) * all_abs[:, idx + 1]
+            f = np.divide(z - z1, z2 - z1,
+                          out=np.zeros_like(z), where=np.abs(z2-z1) > 1e-12)
+            # this is to avoid divide by zero errors (|f| gets very large) when z1 = z2
+            out = (1-f) * all_abs[:, idx - 1] + f * all_abs[:, idx]
 
         except IndexError:
             out = all_abs[:, idx]
 
         return out
 
     all_absorbed = np.trapz(diff_absorption(all_z), all_z)
```

### Comparing `solcore-5.9.1/solcore/optimization/differential_evolution.py` & `solcore-5.9.2/solcore/optimization/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/parameter_system/calculable_parameters.txt` & `solcore-5.9.2/solcore/parameter_system/calculable_parameters.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/parameter_system/parameter_system.py` & `solcore-5.9.2/solcore/parameter_system/parameter_system.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/poisson_drift_diffusion/DDmodel-current.f95` & `solcore-5.9.2/solcore/poisson_drift_diffusion/DDmodel-current.f95`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/poisson_drift_diffusion/DeviceStructure.py` & `solcore-5.9.2/solcore/poisson_drift_diffusion/DeviceStructure.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/poisson_drift_diffusion/DriftDiffusionUtilities.py` & `solcore-5.9.2/solcore/poisson_drift_diffusion/DriftDiffusionUtilities.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/poisson_drift_diffusion/QWunit.py` & `solcore-5.9.2/solcore/poisson_drift_diffusion/QWunit.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/quantum_mechanics/graphics.py` & `solcore-5.9.2/solcore/quantum_mechanics/graphics.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/quantum_mechanics/high_level_kp_QW.py` & `solcore-5.9.2/solcore/quantum_mechanics/high_level_kp_QW.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/quantum_mechanics/kp_QW.py` & `solcore-5.9.2/solcore/quantum_mechanics/kp_QW.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/quantum_mechanics/kp_bulk.py` & `solcore-5.9.2/solcore/quantum_mechanics/kp_bulk.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/quantum_mechanics/potential_utilities.py` & `solcore-5.9.2/solcore/quantum_mechanics/potential_utilities.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/quantum_mechanics/strain.py` & `solcore-5.9.2/solcore/quantum_mechanics/strain.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/quantum_mechanics/structure_utilities.py` & `solcore-5.9.2/solcore/quantum_mechanics/structure_utilities.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/registries.py` & `solcore-5.9.2/solcore/registries.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/science_tracker.py` & `solcore-5.9.2/solcore/science_tracker.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/singleton.py` & `solcore-5.9.2/solcore/singleton.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/smooth.py` & `solcore-5.9.2/solcore/smooth.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/solar_cell.py` & `solcore-5.9.2/solcore/solar_cell.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/solar_cell_solver.py` & `solcore-5.9.2/solcore/solar_cell_solver.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/solcore_config.txt` & `solcore-5.9.2/solcore/solcore_config.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [Configuration]
-version: 5.9.1
+version: 5.9.2
 welcome_message: 1
 verbose_loading: 1
 
 [Units]
 default: SOLCORE_ROOT/units_system/Default_units.txt
 
 [Parameters]
```

### Comparing `solcore-5.9.1/solcore/source_managed_class.py` & `solcore-5.9.2/solcore/source_managed_class.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/spice/pv_module_solver.py` & `solcore-5.9.2/solcore/spice/pv_module_solver.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/spice/quasi_3D_solver.py` & `solcore-5.9.2/solcore/spice/quasi_3D_solver.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/spice/spice.py` & `solcore-5.9.2/solcore/spice/spice.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/state.py` & `solcore-5.9.2/solcore/state.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/strain_balancing.py` & `solcore-5.9.2/solcore/strain_balancing.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/structure.py` & `solcore-5.9.2/solcore/structure.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/units_system/Default_units.txt` & `solcore-5.9.2/solcore/units_system/Default_units.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/solcore/units_system/units_system.py` & `solcore-5.9.2/solcore/units_system/units_system.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/conftest.py` & `solcore-5.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/Ge-Palik.csv` & `solcore-5.9.2/tests/data/Ge-Palik.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/MgF-ZnS_AR.csv` & `solcore-5.9.2/tests/data/MgF-ZnS_AR.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/SiGeSn_k.txt` & `solcore-5.9.2/tests/data/SiGeSn_k.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/SiGeSn_n.txt` & `solcore-5.9.2/tests/data/SiGeSn_n.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/SiGeSn_params.txt` & `solcore-5.9.2/tests/data/SiGeSn_params.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/absorption_profile.txt` & `solcore-5.9.2/tests/data/absorption_profile.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/alinp.csv` & `solcore-5.9.2/tests/data/alinp.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/database_materials.txt` & `solcore-5.9.2/tests/data/database_materials.txt`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/in01gaas.csv` & `solcore-5.9.2/tests/data/in01gaas.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/data/in048ga052p.csv` & `solcore-5.9.2/tests/data/in048ga052p.csv`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test__pdd.py` & `solcore-5.9.2/tests/test__pdd.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_absorption.py` & `solcore-5.9.2/tests/test_absorption.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         user_options={
             "wavelength": wavelength,
             "optics_method": "TMM",
             "no_back_reflection": False,
         },
     )
 
-    z_pos = np.linspace(0, my_structure.width, 10)
+    z_pos = np.linspace(0, my_structure.width, 50)
 
     profile_subs = my_structure[0].absorbed(z_pos)
 
     my_structure = SolarCell([Layer(si(700, "nm"), material=GaAs)])
 
     solar_cell_solver(
         my_structure,
```

### Comparing `solcore-5.9.1/tests/test_config_tools.py` & `solcore-5.9.2/tests/test_config_tools.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_depletion_approximation.py` & `solcore-5.9.2/tests/test_depletion_approximation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,156 +1,184 @@
-from pytest import approx, mark, raises
+from pytest import approx, raises
 import numpy as np
 from solcore.constants import kb, q, vacuum_permittivity
 
 
-
 def test_get_j_dark():
     from solcore.analytic_solar_cells.depletion_approximation import get_j_dark
 
     x = np.power(10, np.random.uniform(-8, -5))
     xi = np.power(10, np.random.uniform(-8, -5))
 
-    l = np.power(10, np.random.uniform(-9, -6))
+    L = np.power(10, np.random.uniform(-9, -6))
     s = np.power(10, np.random.uniform(1, 3))
     d = np.power(10, np.random.uniform(-5, 0))
-    Vbi = np.random.uniform(0.1,5)
+    Vbi = np.random.uniform(0.1, 5)
     minor = np.power(10, np.random.uniform(-7, -4))
-    T = np.random.uniform(0.1,400)
-    es = np.random.uniform(1,20)*vacuum_permittivity
+    T = np.random.uniform(0.1, 400)
+    es = np.random.uniform(1, 20) * vacuum_permittivity
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(22, 25))
 
     V = np.linspace(-6, 4, 20)
     V = np.where(V < Vbi - 0.001, V, Vbi - 0.001)
 
-    wn = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Nd / Na)
-    wp = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Na / Nd)
+    wn = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Nd / Na
+    )
+    wp = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Na / Nd
+    )
 
     w = wn + wp + xi
 
-    expected = (q*d*minor/l)*(np.exp(q*V/(kb*T))-1)*((((s*l)/d)*np.cosh((x-w)/l)+np.sinh((x-w)/l))/
-                                                  (((s*l)/d)*np.sinh((x-w)/l)+np.cosh((x-w)/l)))
+    expected = (
+        (q * d * minor / L)
+        * (np.exp(q * V / (kb * T)) - 1)
+        * (
+            (((s * L) / d) * np.cosh((x - w) / L) + np.sinh((x - w) / L))
+            / (((s * L) / d) * np.sinh((x - w) / L) + np.cosh((x - w) / L))
+        )
+    )
 
-    result = get_j_dark(x, w, l, s, d, V, minor, T)
+    result = get_j_dark(x, w, L, s, d, V, minor, T)
 
     assert result == approx(expected, nan_ok=True)
 
 
 def test_factor():
     from solcore.analytic_solar_cells.depletion_approximation import factor
-    T = np.random.uniform(0.1,400)
-    Vbi = np.random.uniform(0.1,5)
+
+    T = np.random.uniform(0.1, 400)
+    Vbi = np.random.uniform(0.1, 5)
     tp = np.power(10, np.random.uniform(-10, -5))
     tn = np.power(10, np.random.uniform(-10, -5))
     dEt = 0
 
-    kT = kb*T
+    kT = kb * T
     V = np.linspace(-6, 4, 20)
     V = np.where(V < Vbi - 0.001, V, Vbi - 0.001)
 
     m = V >= -1120 * kT / q
     V = V[m]
 
-    b= np.exp(-V*q/(2*kT))*np.cosh((q*dEt/kT)+(1/2)*np.log(tp/tn))
+    b = np.exp(-V * q / (2 * kT)) * np.cosh((q * dEt / kT) + (1 / 2) * np.log(tp / tn))
 
-    z1 = np.sqrt(tp/tn)*np.exp(-q*(Vbi - V)/(kT * 2))
-    z2 = np.sqrt(tp/tn)*np.exp(q*(Vbi - V)/(kT * 2))
+    z1 = np.sqrt(tp / tn) * np.exp(-q * (Vbi - V) / (kT * 2))
+    z2 = np.sqrt(tp / tn) * np.exp(q * (Vbi - V) / (kT * 2))
 
     expected = np.zeros(b.shape)
 
     # For b values < 1
     inds = b < 1  # use tan-1 formulation without issue
 
-    upper = np.arctan((b[inds]+z2[inds])/np.sqrt(1-b[inds]**2))
-    lower = np.arctan((b[inds]+z1[inds])/np.sqrt(1-b[inds]**2))
+    upper = np.arctan((b[inds] + z2[inds]) / np.sqrt(1 - b[inds] ** 2))
+    lower = np.arctan((b[inds] + z1[inds]) / np.sqrt(1 - b[inds] ** 2))
 
-    expected[inds] = (upper - lower)/np.sqrt(1-b[inds]**2)
+    expected[inds] = (upper - lower) / np.sqrt(1 - b[inds] ** 2)
 
     # for b values >=1, log formulation
     inds = (b >= 1) & (b <= 1e7)
 
-    upper = np.log(abs(z2[inds] + b[inds] - np.sqrt(b[inds]**2-1))) - \
-            np.log(abs(z2[inds] + b[inds] + np.sqrt(b[inds]**2-1)))
-
-    lower = np.log(abs(z1[inds] + b[inds] - np.sqrt(b[inds]**2-1))) - \
-            np.log(abs(z1[inds] + b[inds] + np.sqrt(b[inds]**2-1)))
-    expected[inds] = (upper - lower)/(2*np.sqrt(b[inds]**2 - 1))
+    upper = np.log(abs(z2[inds] + b[inds] - np.sqrt(b[inds] ** 2 - 1))) - np.log(
+        abs(z2[inds] + b[inds] + np.sqrt(b[inds] ** 2 - 1))
+    )
+
+    lower = np.log(abs(z1[inds] + b[inds] - np.sqrt(b[inds] ** 2 - 1))) - np.log(
+        abs(z1[inds] + b[inds] + np.sqrt(b[inds] ** 2 - 1))
+    )
+    expected[inds] = (upper - lower) / (2 * np.sqrt(b[inds] ** 2 - 1))
 
     # limit as b gets very large: sqrt(b**2-1) = b
 
     inds = b > 1e7
 
-    upper = np.log(z2[inds]) - np.log(z2[inds] + 2*b[inds])
-    lower = np.log(z1[inds]) - np.log(z1[inds] + 2*b[inds])
+    upper = np.log(z2[inds]) - np.log(z2[inds] + 2 * b[inds])
+    lower = np.log(z1[inds]) - np.log(z1[inds] + 2 * b[inds])
 
-    expected[inds] = (upper - lower) / (2*b[inds])
+    expected[inds] = (upper - lower) / (2 * b[inds])
 
     result = factor(V, Vbi, tp, tn, kT, dEt)
 
     assert result == approx(expected, nan_ok=True)
 
 
 def test_forward():
     from solcore.analytic_solar_cells.depletion_approximation import factor, forward
 
-    T = np.random.uniform(0.1,400)
-    Vbi = np.random.uniform(0.1,5)
+    T = np.random.uniform(0.1, 400)
+    Vbi = np.random.uniform(0.1, 5)
     tp = np.power(10, np.random.uniform(-10, -5))
     tn = np.power(10, np.random.uniform(-10, -5))
     dEt = 0
 
-    kT = kb*T
+    kT = kb * T
     V = np.linspace(-6, 4, 20)
     V = np.where(V < Vbi - 0.001, V, Vbi - 0.001)
 
     ni = np.power(10, np.random.uniform(2, 9))
-    es = np.random.uniform(1,20)*vacuum_permittivity
+    es = np.random.uniform(1, 20) * vacuum_permittivity
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(22, 25))
     xi = np.power(10, np.random.uniform(-8, -5))
 
     m = V >= -1120 * kT / q
     V = V[m]
 
-    wn = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Nd / Na)
-    wp = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Na / Nd)
+    wn = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Nd / Na
+    )
+    wp = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Na / Nd
+    )
 
     w = wn + wp + xi
 
     f_b = factor(V, Vbi, tp, tn, kT, dEt)
-    expected = 2 * q * ni * w / np.sqrt(tn * tp) * \
-          np.sinh(q*V / (2 * kT)) / (q * (Vbi - V) / kT) * f_b
+    expected = (
+        2
+        * q
+        * ni
+        * w
+        / np.sqrt(tn * tp)
+        * np.sinh(q * V / (2 * kT))
+        / (q * (Vbi - V) / kT)
+        * f_b
+    )
 
     result = forward(ni, V, Vbi, tp, tn, w, kT, dEt)
 
     assert result == approx(expected, nan_ok=True)
 
 
 def test_get_J_srh():
     from solcore.analytic_solar_cells.depletion_approximation import forward, get_Jsrh
 
-    T = np.random.uniform(0.1,400)
-    Vbi = np.random.uniform(0.1,5)
+    T = np.random.uniform(0.1, 400)
+    Vbi = np.random.uniform(0.1, 5)
     tp = np.power(10, np.random.uniform(-10, -5))
     tn = np.power(10, np.random.uniform(-10, -5))
     dEt = 0
 
-    kT = kb*T
+    kT = kb * T
     V = np.linspace(-6, 4, 20)
     V = np.where(V < Vbi - 0.001, V, Vbi - 0.001)
 
     ni = np.power(10, np.random.uniform(2, 9))
-    es = np.random.uniform(1,20)*vacuum_permittivity
+    es = np.random.uniform(1, 20) * vacuum_permittivity
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(22, 25))
     xi = np.power(10, np.random.uniform(-8, -5))
 
-    wn = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Nd / Na)
-    wp = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Na / Nd)
+    wn = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Nd / Na
+    )
+    wp = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Na / Nd
+    )
 
     w = wn + wp + xi
 
     expected = np.zeros(V.shape)
 
     inds = V >= -1120 * kT / q
     expected[inds] = forward(ni, V[inds], Vbi, tp, tn, w[inds], kT)
@@ -162,522 +190,600 @@
 
 def test_get_J_sc_diffusion_top():
     from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_diffusion
     from scipy.integrate import solve_bvp
     from solcore.interpolate import interp1d
     from solcore.light_source import LightSource
 
-    D = np.power(10, np.random.uniform(-5, 0)) # Diffusion coefficient
-    L = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    minority = np.power(10, np.random.uniform(-7, -4))# minority carrier density
-    s = np.power(10, np.random.uniform(0, 3)) # surface recombination velocity
+    D = np.power(10, np.random.uniform(-5, 0))  # Diffusion coefficient
+    L = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    minority = np.power(10, np.random.uniform(-7, -4))  # minority carrier density
+    s = np.power(10, np.random.uniform(0, 3))  # surface recombination velocity
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
-    wl = np.linspace(300, 1800, 50)*1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl = np.linspace(300, 1800, 50) * 1e-9
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
-    xa = xa_nm*1e-9
-    xb = np.random.uniform(xa_nm+1, 1100)*1e-9
+    xa = xa_nm * 1e-9
+    xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     dist = np.linspace(0, xb, 1000)
     alphas = np.linspace(1e8, 10, len(wl))
 
-    expn = np.exp(- alphas[:, None] * dist[None,:])
+    expn = np.exp(-alphas[:, None] * dist[None, :])
 
-    output = alphas[:, None]*expn
+    output = alphas[:, None] * expn
     output = output.T
-    gen_prof = interp1d(dist, output, axis = 0)
-
+    gen_prof = interp1d(dist, output, axis=0)
 
     zz = np.linspace(xa, xb, 1002)[:-1]
     gg = gen_prof(zz) * phg
 
     g_vs_z = np.trapz(gg, wl, axis=1)
 
-    A = lambda x: np.interp(x, zz, g_vs_z) / D + minority / L ** 2
+    def A(x):
+        return np.interp(x, zz, g_vs_z) / D + minority / L**2
 
     def fun(x, y):
         out1 = y[1]
-        out2 = y[0] / L ** 2 - A(x)
+        out2 = y[0] / L**2 - A(x)
         return np.vstack((out1, out2))
 
     def bc(ya, yb):
         left = ya[1] - s / D * (ya[0] - minority)
         right = yb[0]
         return np.array([left, right])
 
-
     guess = minority * np.ones((2, zz.size))
     guess[1] = np.zeros_like(guess[0])
 
-    solution = solve_bvp(fun, bc, zz, guess)
+    solution = solve_bvp(fun, bc, zz, guess, max_nodes=2 * zz.shape[0])
 
     expected = solution.y[1][-1]
 
-    result = get_J_sc_diffusion(xa, xb, gen_prof, D, L, minority, s, wl, phg, side='top')
+    result = get_J_sc_diffusion(
+        xa, xb, gen_prof, D, L, minority, s, wl, phg, side="top"
+    )
 
     assert result == approx(expected)
 
 
 def test_get_J_sc_diffusion_bottom():
     from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_diffusion
     from scipy.integrate import solve_bvp
     from solcore.interpolate import interp1d
     from solcore.light_source import LightSource
 
-    D = np.power(10, np.random.uniform(-5, 0)) # Diffusion coefficient
-    L = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    minority = np.power(10, np.random.uniform(-7, -4))# minority carrier density
-    s = np.power(10, np.random.uniform(0, 3)) # surface recombination velocity
+    D = np.power(10, np.random.uniform(-5, 0))  # Diffusion coefficient
+    L = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    minority = np.power(10, np.random.uniform(-7, -4))  # minority carrier density
+    s = np.power(10, np.random.uniform(0, 3))  # surface recombination velocity
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
-    wl = np.linspace(300, 1800, 50)*1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl = np.linspace(300, 1800, 50) * 1e-9
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
-    xa = xa_nm*1e-9
-    xb = np.random.uniform(xa_nm+1, 1100)*1e-9
+    xa = xa_nm * 1e-9
+    xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     dist = np.linspace(0, xb, 1000)
     alphas = np.linspace(1e8, 10, len(wl))
 
-    expn = np.exp(- alphas[:, None] * dist[None,:])
+    expn = np.exp(-alphas[:, None] * dist[None, :])
 
-    output = alphas[:, None]*expn
+    output = alphas[:, None] * expn
     output = output.T
-    gen_prof = interp1d(dist, output, axis = 0)
-
+    gen_prof = interp1d(dist, output, axis=0)
 
     zz = np.linspace(xa, xb, 1002)[:-1]
     gg = gen_prof(zz) * phg
 
     g_vs_z = np.trapz(gg, wl, axis=1)
 
-    A = lambda x: np.interp(x, zz, g_vs_z) / D + minority / L ** 2
+    def A(x):
+        return np.interp(x, zz, g_vs_z) / D + minority / L**2
 
     def fun(x, y):
         out1 = y[1]
-        out2 = y[0] / L ** 2 - A(x)
+        out2 = y[0] / L**2 - A(x)
         return np.vstack((out1, out2))
 
     def bc(ya, yb):
-        left = ya[0]
-        right = yb[1] - s / D * (yb[0] - minority)
+        left = ya[0] - minority
+        right = yb[1] + s / D * (yb[0] - minority)
         return np.array([left, right])
 
-
     guess = minority * np.ones((2, zz.size))
     guess[1] = np.zeros_like(guess[0])
 
-    solution = solve_bvp(fun, bc, zz, guess)
+    solution = solve_bvp(fun, bc, zz, guess, max_nodes=2 * zz.shape[0])
 
     expected = solution.y[1][0]
 
-    result = get_J_sc_diffusion(xa, xb, gen_prof, D, L, minority, s, wl, phg, side='bottom')
+    result = get_J_sc_diffusion(
+        xa, xb, gen_prof, D, L, minority, s, wl, phg, side="bottom"
+    )
 
     assert result == approx(expected)
 
 
 def test_get_J_sc_SCR():
     from solcore.light_source import LightSource
     from solcore.interpolate import interp1d
     from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_SCR
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
-    wl = np.linspace(300, 1800, 50)*1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl = np.linspace(300, 1800, 50) * 1e-9
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
-    xa = xa_nm*1e-9
-    xb = np.random.uniform(xa_nm+1, 1100)*1e-9
+    xa = xa_nm * 1e-9
+    xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     dist = np.linspace(0, xb, 1000)
     alphas = np.linspace(1e5, 10, len(wl))
 
-    expn = np.exp(- alphas[:, None] * dist[None,:])
+    expn = np.exp(-alphas[:, None] * dist[None, :])
 
-    output = alphas[:, None]*expn
+    output = alphas[:, None] * expn
     output = output.T
-    gen_prof = interp1d(dist, output, axis = 0)
+    gen_prof = interp1d(dist, output, axis=0)
 
     zz = np.linspace(xa, xb, 1002)[:-1]
     gg = gen_prof(zz) * phg
     expected = np.trapz(np.trapz(gg, wl, axis=1), zz)
 
     result = get_J_sc_SCR(xa, xb, gen_prof, wl, phg)
 
-    assert  expected == approx(result)
+    assert expected == approx(result)
 
 
 def test_get_J_sc_SCR_vs_WL():
     from solcore.light_source import LightSource
     from solcore.interpolate import interp1d
     from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_SCR_vs_WL
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
-    wl = np.linspace(300, 1800, 50)*1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl = np.linspace(300, 1800, 50) * 1e-9
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
-    xa = xa_nm*1e-9
-    xb = np.random.uniform(xa_nm+1, 1100)*1e-9
+    xa = xa_nm * 1e-9
+    xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     dist = np.linspace(0, xb, 1000)
     alphas = np.linspace(1e5, 10, len(wl))
 
-    expn = np.exp(- alphas[:, None] * dist[None,:])
+    expn = np.exp(-alphas[:, None] * dist[None, :])
 
-    output = alphas[:, None]*expn
+    output = alphas[:, None] * expn
     output = output.T
-    gen_prof = interp1d(dist, output, axis = 0)
+    gen_prof = interp1d(dist, output, axis=0)
 
     zz = np.linspace(xa, xb, 1002)[:-1]
     gg = gen_prof(zz) * phg
     expected = np.trapz(gg, zz, axis=0)
 
     result = get_J_sc_SCR_vs_WL(xa, xb, gen_prof, wl, phg)
 
-    assert  expected == approx(result)
+    assert expected == approx(result)
 
 
 def test_get_J_sc_diffusion_vs_WL_top():
-    from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_diffusion_vs_WL
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        get_J_sc_diffusion_vs_WL,
+    )
     from scipy.integrate import solve_bvp
     from solcore.interpolate import interp1d
     from solcore.light_source import LightSource
 
-    D = np.power(10, np.random.uniform(-5, 0)) # Diffusion coefficient
-    L = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    minority = np.power(10, np.random.uniform(-7, -4))# minority carrier density
-    s = np.power(10, np.random.uniform(0, 3)) # surface recombination velocity
+    D = np.power(10, np.random.uniform(-5, 0))  # Diffusion coefficient
+    L = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    minority = np.power(10, np.random.uniform(-7, -4))  # minority carrier density
+    s = np.power(10, np.random.uniform(0, 3))  # surface recombination velocity
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
-    wl = np.linspace(300, 1800, 50)*1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl = np.linspace(300, 1800, 50) * 1e-9
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
-    xa = xa_nm*1e-9
-    xb = np.random.uniform(xa_nm+1, 1100)*1e-9
+    xa = xa_nm * 1e-9
+    xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     dist = np.linspace(0, xb, 1000)
     alphas = np.linspace(1e8, 10, len(wl))
 
-    expn = np.exp(- alphas[:, None] * dist[None,:])
+    expn = np.exp(-alphas[:, None] * dist[None, :])
 
-    output = alphas[:, None]*expn
+    output = alphas[:, None] * expn
     output = output.T
-    gen_prof = interp1d(dist, output, axis = 0)
-
+    gen_prof = interp1d(dist, output, axis=0)
 
-    zz =  np.linspace(xa, xb, 1002)[:-1]
+    zz = np.linspace(xa, xb, 1002)[:-1]
     gg = gen_prof(zz) * phg
 
     expected = np.zeros_like(wl)
 
     for i in range(len(wl)):
-
-        if np.all(gg[:,i] == 0): # no reason to solve anything if no generation at this wavelength
+        if np.all(
+            gg[:, i] == 0
+        ):  # no reason to solve anything if no generation at this wavelength
             expected[i] = 0
 
-        A = lambda x: np.interp(x, zz, gg[:, i]) / D + minority / L ** 2
+        def A(x):
+            return np.interp(x, zz, gg[:, i]) / D + minority / L**2
 
         def fun(x, y):
             out1 = y[1]
-            out2 = y[0] / L ** 2 - A(x)
+            out2 = y[0] / L**2 - A(x)
             return np.vstack((out1, out2))
 
         def bc(ya, yb):
             left = ya[1] - s / D * (ya[0] - minority)
-            right = yb[0]
+            right = yb[0] - minority
             return np.array([left, right])
 
         guess = minority * np.ones((2, zz.size))
         guess[1] = np.zeros_like(guess[0])
-        solution = solve_bvp(fun, bc, zz, guess)
+        solution = solve_bvp(fun, bc, zz, guess, max_nodes=2 * zz.shape[0])
 
         expected[i] = solution.y[1][-1]
 
-    result = get_J_sc_diffusion_vs_WL(xa, xb, gen_prof, D, L, minority, s, wl, phg, side='top')
-
+    result = get_J_sc_diffusion_vs_WL(
+        xa, xb, gen_prof, D, L, minority, s, wl, phg, side="top"
+    )
 
     assert result == approx(expected)
 
 
 def test_get_J_sc_diffusion_vs_WL_bottom():
-    from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_diffusion_vs_WL
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        get_J_sc_diffusion_vs_WL,
+    )
     from scipy.integrate import solve_bvp
     from solcore.interpolate import interp1d
     from solcore.light_source import LightSource
 
-    D = np.power(10, np.random.uniform(-5, 0)) # Diffusion coefficient
-    L = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    minority = np.power(10, np.random.uniform(-7, -4))# minority carrier density
-    s = np.power(10, np.random.uniform(0, 3)) # surface recombination velocity
+    D = np.power(10, np.random.uniform(-5, 0))  # Diffusion coefficient
+    L = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    minority = np.power(10, np.random.uniform(-7, -4))  # minority carrier density
+    s = np.power(10, np.random.uniform(0, 3))  # surface recombination velocity
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
     wl = np.linspace(300, 1800, 50) * 1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
     xa = xa_nm * 1e-9
     xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     dist = np.linspace(0, xb, 1000)
     alphas = np.linspace(1e8, 10, len(wl))
 
-    expn = np.exp(- alphas[:, None] * dist[None, :])
+    expn = np.exp(-alphas[:, None] * dist[None, :])
 
     output = alphas[:, None] * expn
     output = output.T
     gen_prof = interp1d(dist, output, axis=0)
 
     zz = np.linspace(xa, xb, 1002)[:-1]
     gg = gen_prof(zz) * phg
 
     expected = np.zeros_like(wl)
 
     for i in range(len(wl)):
-        if np.all(gg[:, i] == 0):  # no reason to solve anything if no generation at this wavelength
+        if np.all(
+            gg[:, i] == 0
+        ):  # no reason to solve anything if no generation at this wavelength
             expected[i] = 0
 
-        A = lambda x: np.interp(x, zz, gg[:, i]) / D + minority / L ** 2
+        def A(x):
+            return np.interp(x, zz, gg[:, i]) / D + minority / L**2
 
         def fun(x, y):
             out1 = y[1]
-            out2 = y[0] / L ** 2 - A(x)
+            out2 = y[0] / L**2 - A(x)
             return np.vstack((out1, out2))
 
         def bc(ya, yb):
-            left = ya[0]
-            right = yb[1] - s / D * (yb[0] - minority)
+            left = ya[0] - minority
+            right = yb[1] + s / D * (yb[0] - minority)
             return np.array([left, right])
 
         guess = minority * np.ones((2, zz.size))
         guess[1] = np.zeros_like(guess[0])
-        solution = solve_bvp(fun, bc, zz, guess)
+        solution = solve_bvp(fun, bc, zz, guess, max_nodes=2 * zz.shape[0])
 
         expected[i] = solution.y[1][0]
 
-    result = get_J_sc_diffusion_vs_WL(xa, xb, gen_prof, D, L, minority, s, wl, phg, side='bottom')
+    result = get_J_sc_diffusion_vs_WL(
+        xa, xb, gen_prof, D, L, minority, s, wl, phg, side="bottom"
+    )
 
     assert result == approx(expected)
 
 
 def test_get_J_sc_diffusion_green_top():
-    from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_diffusion_green
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        get_J_sc_diffusion_green,
+    )
     from solcore.light_source import LightSource
 
-    D = np.power(10, np.random.uniform(-5, 0)) # Diffusion coefficient
-    L = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    minority = np.power(10, np.random.uniform(-7, -4))# minority carrier density
-    s = np.power(10, np.random.uniform(0, 3)) # surface recombination velocity
+    D = np.power(10, np.random.uniform(-5, 0))  # Diffusion coefficient
+    L = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    s = np.power(10, np.random.uniform(0, 3))  # surface recombination velocity
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
     wl = np.linspace(300, 1800, 50) * 1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
     xa = xa_nm * 1e-9
-    xb = np.random.uniform(xa_nm+1, 1100) * 1e-9
+    xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
     beta1 = (xb - xa) / L
-    if beta1 > 1.e2:
-        xb = xa + 99. * L
+    if beta1 > 1.0e2:
+        xb = xa + 99.0 * L
         beta1 = (xb - xa) / L
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     alphas = np.linspace(1e8, 10, len(wl))
 
     # theoreical value from Fonash, Solar cell device physics eq 4.10
     # (the absorption profile has to be offset for xa != 0.)
     beta2 = (xb - xa) * alphas
     beta3 = L * s / D
-    c1 = beta2*beta2/(beta2*beta2 - beta1*beta1)
-    c2 = (beta3*beta1/beta2 + 1.) / (beta3 * np.sinh(beta1) + np.cosh(beta1))
-    expected = (beta3*np.cosh(beta1) + np.sinh(beta1)) / (beta3*np.sinh(beta1) + np.cosh(beta1))
-    expected *= beta1/beta2
-    expected += 1.
+    c1 = beta2 * beta2 / (beta2 * beta2 - beta1 * beta1)
+    c2 = (beta3 * beta1 / beta2 + 1.0) / (beta3 * np.sinh(beta1) + np.cosh(beta1))
+    expected = (beta3 * np.cosh(beta1) + np.sinh(beta1)) / (
+        beta3 * np.sinh(beta1) + np.cosh(beta1)
+    )
+    expected *= beta1 / beta2
+    expected += 1.0
     expected *= np.exp(-beta2)
-    expected = (expected - c2) * c1  * phg / D * np.exp(-alphas * xa)
-    expected -= minority / L * (beta3*np.cosh(beta1) + np.sinh(beta1)) / (beta3*np.sinh(beta1) + np.cosh(beta1))
+    expected = (expected - c2) * c1 * phg / D * np.exp(-alphas * xa)
 
-    result = get_J_sc_diffusion_green(xa, xb, lambda x: alphas * np.exp(-alphas * x),
-                                      D, L, minority, s, phg, side='top')
+    result = get_J_sc_diffusion_green(
+        xa,
+        xb,
+        lambda x: alphas * np.exp(-alphas * x),
+        D,
+        L,
+        s,
+        phg,
+        side="top",
+    )
 
-    assert beta1 < 1.e2
-    assert result == approx(expected, rel=1.e-5)
+    assert beta1 < 1.0e2
+    assert result == approx(expected, rel=1.0e-5)
 
     #  test version for extreme L values
-    Lmax = np.log10((xb - xa) * 1.e-2)
-    L = np.power(10, np.random.uniform(Lmax - 2., Lmax))
+    Lmax = np.log10((xb - xa) * 1.0e-2)
+    L = np.power(10, np.random.uniform(Lmax - 2.0, Lmax))
 
     # theoretical value for Beer-Lambert profile
-    alphas_miL = alphas - 1. / L
-    idx_c = np.abs(alphas_miL) < 1.e-3
+    alphas_miL = alphas - 1.0 / L
+    idx_c = np.abs(alphas_miL) < 1.0e-3
     idx_i = np.logical_not(idx_c)
-    expected = np.zeros_like(alphas)
+
     expected = np.exp(-alphas_miL * xa - xb / L) - np.exp(-alphas * xb)
     expected[idx_i] /= alphas_miL[idx_i]
     expected[idx_c] = np.exp(-alphas[idx_c] * xb)
     expected *= -phg * alphas / D
-    expected -= minority / L
 
-    result = get_J_sc_diffusion_green(xa, xb, lambda x: alphas * np.exp(-alphas * x),
-                                      D, L, minority, s, phg, side='top')
+    result = get_J_sc_diffusion_green(
+        xa,
+        xb,
+        lambda x: alphas * np.exp(-alphas * x),
+        D,
+        L,
+        s,
+        phg,
+        side="top",
+    )
 
-    assert (xb - xa) / L > 1.e2
-    assert result == approx(expected, rel=1.e-5)
+    assert (xb - xa) / L > 1.0e2
+    assert result == approx(expected, rel=1.0e-5)
 
 
 def test_get_J_sc_diffusion_green_bottom():
-    from solcore.analytic_solar_cells.depletion_approximation import get_J_sc_diffusion_green
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        get_J_sc_diffusion_green,
+    )
     from solcore.light_source import LightSource
 
-    D = np.power(10, np.random.uniform(-5, 0)) # Diffusion coefficient
-    L = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    minority = np.power(10, np.random.uniform(-7, -4))# minority carrier density
-    s = np.power(10, np.random.uniform(0, 3)) # surface recombination velocityx
+    D = np.power(10, np.random.uniform(-5, 0))  # Diffusion coefficient
+    L = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    s = np.power(10, np.random.uniform(0, 3))  # surface recombination velocityx
 
     light_source = LightSource(source_type="standard", version="AM1.5g")
-    wl = np.linspace(300, 1800, 50)*1e-9
-    wl_ls, phg = light_source.spectrum(output_units='photon_flux_per_m', x=wl)
+    wl = np.linspace(300, 1800, 50) * 1e-9
+    wl_ls, phg = light_source.spectrum(output_units="photon_flux_per_m", x=wl)
 
     xa_nm = np.random.uniform(1, 1000)
-    xa = xa_nm*1e-9
-    xb = np.random.uniform(xa_nm+1, 1100)*1e-9
+    xa = xa_nm * 1e-9
+    xb = np.random.uniform(xa_nm + 1, 1100) * 1e-9
     beta1 = (xb - xa) / L
-    if beta1 > 1.e2:
-        xb = xa + 99. * L
+    if beta1 > 1.0e2:
+        xb = xa + 99.0 * L
         beta1 = (xb - xa) / L
 
-    ## make a simple Beer-Lambert profile
+    # make a simple Beer-Lambert profile
     alphas = np.linspace(1e8, 10, len(wl))
 
     # theoreical value from Fonash, Solar cell device physics eq 4.15
     beta2 = (xb - xa) * alphas
-    beta3 = -L * s / D
-    c1 = beta2*beta2/(beta2*beta2 - beta1*beta1) * np.exp(-alphas * xa)
-    c2 = (beta3*beta1/beta2 - 1.) / (beta3 * np.sinh(beta1) + np.cosh(beta1))
-    expected = (beta3*np.cosh(beta1) + np.sinh(beta1)) / (beta3*np.sinh(beta1) + np.cosh(beta1))
-    expected *= -beta1/beta2
-    expected += 1.
-    expected = (expected + c2 * np.exp(-beta2)) * c1  * phg / D
-    expected += minority / L * (beta3*np.cosh(beta1) + np.sinh(beta1)) / (beta3*np.sinh(beta1) + np.cosh(beta1))
-
-    result = get_J_sc_diffusion_green(xa, xb, lambda x: alphas * np.exp(-alphas * x),
-                                      D, L, minority, s, phg, side='bottom')
+    beta3 = L * s / D
+    c1 = beta2 * beta2 / (beta2 * beta2 - beta1 * beta1) * np.exp(-alphas * xa)
+    c2 = (beta3 * beta1 / beta2 - 1.0) / (beta3 * np.sinh(beta1) + np.cosh(beta1))
+    expected = (beta3 * np.cosh(beta1) + np.sinh(beta1)) / (
+        beta3 * np.sinh(beta1) + np.cosh(beta1)
+    )
+    expected *= -beta1 / beta2
+    expected += 1.0
+    expected = (expected + c2 * np.exp(-beta2)) * c1 * phg / D
+
+    result = get_J_sc_diffusion_green(
+        xa,
+        xb,
+        lambda x: alphas * np.exp(-alphas * x),
+        D,
+        L,
+        s,
+        phg,
+        side="bottom",
+    )
 
-    assert beta1 < 1.e2
-    assert result == approx(expected, rel=1.e-5)
+    assert beta1 < 1.0e2
+    assert result == approx(expected, rel=1.0e-5)
 
     #  test version for extreme L values
-    Lmax = np.log10((xb - xa) * 1.e-2)
-    L = np.power(10, np.random.uniform(Lmax - 2., Lmax))
+    Lmax = np.log10((xb - xa) * 1.0e-2)
+    L = np.power(10, np.random.uniform(Lmax - 2.0, Lmax))
 
     # theoretical value for Beer-Lambert profile
     beta1 = (xb - xa) / L
     expected = np.exp(-beta1 - alphas * xb) - np.exp(-alphas * xa)
-    expected *= -phg * alphas / D / (alphas + 1. / L)
-    expected += minority / L
+    expected *= -phg * alphas / D / (alphas + 1.0 / L)
 
-    result = get_J_sc_diffusion_green(xa, xb, lambda x: alphas * np.exp(-alphas * x),
-                                      D, L, minority, s, phg, side='bottom')
+    result = get_J_sc_diffusion_green(
+        xa,
+        xb,
+        lambda x: alphas * np.exp(-alphas * x),
+        D,
+        L,
+        s,
+        phg,
+        side="bottom",
+    )
 
-    assert beta1 > 1.e2
-    assert result == approx(expected, rel=1.e-5)
+    assert beta1 > 1.0e2
+    assert result == approx(expected, rel=1.0e-5)
 
 
 def test_identify_layers_exceptions():
     from solcore.analytic_solar_cells.depletion_approximation import identify_layers
     from solcore import material
     from solcore.structure import Layer, Junction
 
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(22, 25))
 
-    Lp = np.power(10, np.random.uniform(-9, -6))# Diffusion length
-    Ln = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
+    Lp = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    Ln = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
 
-    GaAs_n = material("GaAs")(Nd = Nd, hole_diffusion_length=Ln)
-    GaAs_p = material("GaAs")(Na = Na, electron_diffusion_length=Lp)
+    GaAs_n = material("GaAs")(Nd=Nd, hole_diffusion_length=Ln)
+    GaAs_p = material("GaAs")(Na=Na, electron_diffusion_length=Lp)
     GaAs_i = material("GaAs")()
-    Ge_n = material("Ge")(Nd = Nd, hole_diffusion_length=Ln)
+    # Ge_n = material("Ge")(Nd=Nd, hole_diffusion_length=Ln)
 
-    n_width = np.random.uniform(500, 1000)*1e-9
-    p_width = np.random.uniform(3000, 5000)*1e-9
+    n_width = np.random.uniform(500, 1000) * 1e-9
+    p_width = np.random.uniform(3000, 5000) * 1e-9
     i_width = np.random.uniform(300, 500) * 1e-9
 
-    test_junc  = Junction([Layer(n_width, GaAs_n,role="emitter"),
-                           Layer(p_width, GaAs_p, role="neither")])
+    test_junc = Junction(
+      [Layer(n_width, GaAs_n, role="emitter"), Layer(p_width, GaAs_p, role="neither")]
+    )
 
     with raises(RuntimeError):
         identify_layers(test_junc)
 
-    test_junc =  Junction([Layer(n_width, GaAs_n,role="emitter"),
-                           Layer(i_width, GaAs_i, role="intrinsic"),
-                           Layer(p_width, GaAs_p, role="nothing")])
+    test_junc = Junction(
+        [
+            Layer(n_width, GaAs_n, role="emitter"),
+            Layer(i_width, GaAs_i, role="intrinsic"),
+            Layer(p_width, GaAs_p, role="nothing"),
+        ]
+    )
 
     with raises(RuntimeError):
         identify_layers(test_junc)
 
-    test_junc  = Junction([Layer(n_width, Ge_n,role="emitter"),
-                           Layer(p_width, GaAs_p, role="base")])
-
-    with raises(AssertionError):
-        identify_layers(test_junc)
+    # test_junc = Junction(
+    #     [Layer(n_width, Ge_n, role="emitter"), Layer(p_width, GaAs_p, role="base")]
+    # )
+    #
+    # with raises(AssertionError):
+    #     identify_layers(test_junc)
 
 
 def test_process_junction_np():
-    from solcore.analytic_solar_cells.depletion_approximation import identify_layers, identify_parameters
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        identify_layers,
+        identify_parameters,
+    )
     from solcore import material
     from solcore.structure import Layer, Junction
     from solcore.state import State
 
     Na = np.power(10, np.random.uniform(23, 26))
     Nd = np.power(10, np.random.uniform(22, 25))
 
     options = State()
     options.T = np.random.uniform(250, 350)
 
-    Lp = np.power(10, np.random.uniform(-9, -6))# Diffusion length
-    Ln = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
+    Lp = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    Ln = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
 
     GaAs_window = material("GaAs")()
-    GaAs_n = material("GaAs")(Nd = Nd, hole_diffusion_length=Ln)
-    GaAs_p = material("GaAs")(Na = Na, electron_diffusion_length=Lp)
+    GaAs_n = material("GaAs")(Nd=Nd, hole_diffusion_length=Ln)
+    GaAs_p = material("GaAs")(Na=Na, electron_diffusion_length=Lp)
 
-    n_width = np.random.uniform(500, 1000)*1e-9
-    p_width = np.random.uniform(3000, 5000)*1e-9
-    window_width = np.random.uniform(25, 200)*1e-9
-
-    test_junc  = Junction([Layer(window_width, GaAs_window, role="window"),
-                           Layer(n_width, GaAs_n,role="emitter"),
-                           Layer(p_width, GaAs_p, role="base")])
+    n_width = np.random.uniform(500, 1000) * 1e-9
+    p_width = np.random.uniform(3000, 5000) * 1e-9
+    window_width = np.random.uniform(25, 200) * 1e-9
+
+    test_junc = Junction(
+        [
+            Layer(window_width, GaAs_window, role="window"),
+            Layer(n_width, GaAs_n, role="emitter"),
+            Layer(p_width, GaAs_p, role="base"),
+        ]
+    )
 
     id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(test_junc)
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es = identify_parameters(test_junc, options.T, pRegion, nRegion, iRegion)
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es, _ = identify_parameters(
+        test_junc, options.T, pRegion, nRegion, iRegion
+    )
 
     ni_expect = GaAs_n.ni
 
     assert [id_top, id_bottom] == approx([1, 2])
-    assert pn_or_np == 'np'
-    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx([n_width, p_width, 0, 0, 0, Lp, Ln, GaAs_n.hole_mobility * kb * options.T / q,
-                                    GaAs_p.electron_mobility * kb * options.T / q, Nd, Na, ni_expect, GaAs_n.permittivity])
-
-
+    assert pn_or_np == "np"
+    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx(
+        [
+            n_width,
+            p_width,
+            0,
+            0,
+            0,
+            Lp,
+            Ln,
+            GaAs_n.hole_mobility * kb * options.T / q,
+            GaAs_p.electron_mobility * kb * options.T / q,
+            Nd,
+            Na,
+            ni_expect,
+            GaAs_n.permittivity,
+        ]
+    )
 
 
 def test_process_junction_pn():
-    from solcore.analytic_solar_cells.depletion_approximation import identify_layers, identify_parameters
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        identify_layers,
+        identify_parameters,
+    )
     from solcore import material
     from solcore.structure import Layer, Junction
     from solcore.state import State
 
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(23, 26))
 
@@ -686,360 +792,520 @@
 
     Lp = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
     Ln = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
 
     GaAs_n = material("GaAs")(Nd=Nd, hole_diffusion_length=Ln)
     GaAs_p = material("GaAs")(Na=Na, electron_diffusion_length=Lp)
 
-    p_width = np.random.uniform(500, 1000)*1e-9
-    n_width = np.random.uniform(3000, 5000)*1e-9
+    p_width = np.random.uniform(500, 1000) * 1e-9
+    n_width = np.random.uniform(3000, 5000) * 1e-9
 
-    test_junc = Junction([Layer(p_width, GaAs_p, role="emitter"), Layer(n_width, GaAs_n, role="base")])
+    test_junc = Junction(
+        [Layer(p_width, GaAs_p, role="emitter"), Layer(n_width, GaAs_n, role="base")]
+    )
 
     id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(test_junc)
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es = identify_parameters(test_junc, options.T, pRegion, nRegion, iRegion)
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es, _ = identify_parameters(
+        test_junc, options.T, pRegion, nRegion, iRegion
+    )
 
     ni_expect = GaAs_n.ni
 
     assert [id_top, id_bottom] == approx([0, 1])
-    assert pn_or_np == 'pn'
-    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx([n_width, p_width, 0, 0, 0, Lp, Ln, GaAs_n.hole_mobility * kb * options.T / q,
-                                    GaAs_p.electron_mobility * kb * options.T / q, Nd, Na, ni_expect, GaAs_n.permittivity])
+    assert pn_or_np == "pn"
+    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx(
+        [
+            n_width,
+            p_width,
+            0,
+            0,
+            0,
+            Lp,
+            Ln,
+            GaAs_n.hole_mobility * kb * options.T / q,
+            GaAs_p.electron_mobility * kb * options.T / q,
+            Nd,
+            Na,
+            ni_expect,
+            GaAs_n.permittivity,
+        ]
+    )
 
 
 def test_process_junction_nip():
-    from solcore.analytic_solar_cells.depletion_approximation import identify_layers, identify_parameters
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        identify_layers,
+        identify_parameters,
+    )
     from solcore import material
     from solcore.structure import Layer, Junction
     from solcore.state import State
 
     Na = np.power(10, np.random.uniform(23, 26))
     Nd = np.power(10, np.random.uniform(22, 25))
 
     options = State()
     options.T = np.random.uniform(250, 350)
 
-    Lp = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    Ln = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
+    Lp = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    Ln = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
 
-    GaAs_n = material("GaAs")(Nd = Nd, hole_diffusion_length=Ln)
-    GaAs_p = material("GaAs")(Na = Na, electron_diffusion_length=Lp)
+    GaAs_n = material("GaAs")(Nd=Nd, hole_diffusion_length=Ln)
+    GaAs_p = material("GaAs")(Na=Na, electron_diffusion_length=Lp)
     GaAs_i = material("GaAs")()
 
-    n_width = np.random.uniform(500, 1000)*1e-9
-    p_width = np.random.uniform(3000, 5000)*1e-9
-    i_width = np.random.uniform(100, 300)*1e-9
-
-    test_junc  = Junction([Layer(n_width, GaAs_n,role="emitter"),
-                           Layer(i_width, GaAs_i, role="intrinsic"),
-                           Layer(p_width, GaAs_p, role="base")])
+    n_width = np.random.uniform(500, 1000) * 1e-9
+    p_width = np.random.uniform(3000, 5000) * 1e-9
+    i_width = np.random.uniform(100, 300) * 1e-9
+
+    test_junc = Junction(
+        [
+            Layer(n_width, GaAs_n, role="emitter"),
+            Layer(i_width, GaAs_i, role="intrinsic"),
+            Layer(p_width, GaAs_p, role="base"),
+        ]
+    )
 
     id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(test_junc)
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es = identify_parameters(test_junc, options.T, pRegion, nRegion, iRegion)
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es, _ = identify_parameters(
+        test_junc, options.T, pRegion, nRegion, iRegion
+    )
 
     ni_expect = GaAs_n.ni
 
     assert [id_top, id_bottom] == approx([0, 2])
-    assert pn_or_np == 'np'
-    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx([n_width, p_width, i_width, 0, 0, Lp, Ln, GaAs_n.hole_mobility * kb * options.T / q,
-                                    GaAs_p.electron_mobility * kb * options.T / q, Nd, Na, ni_expect, GaAs_n.permittivity])
-
+    assert pn_or_np == "np"
+    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx(
+        [
+            n_width,
+            p_width,
+            i_width,
+            0,
+            0,
+            Lp,
+            Ln,
+            GaAs_n.hole_mobility * kb * options.T / q,
+            GaAs_p.electron_mobility * kb * options.T / q,
+            Nd,
+            Na,
+            ni_expect,
+            GaAs_n.permittivity,
+        ]
+    )
 
 
 def test_process_junction_pin():
-    from solcore.analytic_solar_cells.depletion_approximation import identify_layers, identify_parameters
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        identify_layers,
+        identify_parameters,
+    )
     from solcore import material
     from solcore.structure import Layer, Junction
     from solcore.state import State
 
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(23, 26))
 
     options = State()
     options.T = np.random.uniform(250, 350)
 
     Lp = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
-    Ln = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
+    Ln = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
 
     GaAs_n = material("GaAs")(Nd=Nd, hole_diffusion_length=Ln)
     GaAs_p = material("GaAs")(Na=Na, electron_diffusion_length=Lp)
     GaAs_i = material("GaAs")()
 
     p_width = np.random.uniform(500, 1000)
     n_width = np.random.uniform(3000, 5000)
-    i_width = np.random.uniform(100, 300)*1e-9
+    i_width = np.random.uniform(100, 300) * 1e-9
 
-    test_junc = Junction([Layer(p_width, GaAs_p, role="emitter"),
-                          Layer(i_width, GaAs_i, role="intrinsic"),
-                          Layer(n_width, GaAs_n, role="base")])
+    test_junc = Junction(
+        [
+            Layer(p_width, GaAs_p, role="emitter"),
+            Layer(i_width, GaAs_i, role="intrinsic"),
+            Layer(n_width, GaAs_n, role="base"),
+        ]
+    )
 
     id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(test_junc)
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es = identify_parameters(test_junc, options.T, pRegion, nRegion, iRegion)
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es, _ = identify_parameters(
+        test_junc, options.T, pRegion, nRegion, iRegion
+    )
 
     ni_expect = GaAs_n.ni
 
     assert [id_top, id_bottom] == approx([0, 2])
-    assert pn_or_np == 'pn'
-    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx([n_width, p_width, i_width, 0, 0, Lp, Ln, GaAs_n.hole_mobility * kb * options.T / q,
-                                    GaAs_p.electron_mobility * kb * options.T / q, Nd, Na, ni_expect, GaAs_n.permittivity])
+    assert pn_or_np == "pn"
+    assert [xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx(
+        [
+            n_width,
+            p_width,
+            i_width,
+            0,
+            0,
+            Lp,
+            Ln,
+            GaAs_n.hole_mobility * kb * options.T / q,
+            GaAs_p.electron_mobility * kb * options.T / q,
+            Nd,
+            Na,
+            ni_expect,
+            GaAs_n.permittivity,
+        ]
+    )
 
 
 def test_process_junction_set_in_junction():
-    from solcore.analytic_solar_cells.depletion_approximation import identify_layers, identify_parameters
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        identify_layers,
+        identify_parameters,
+    )
     from solcore import material
     from solcore.structure import Layer, Junction
     from solcore.state import State
 
     options = State()
     options.T = np.random.uniform(250, 350)
 
-    Lp = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
-    Ln = np.power(10, np.random.uniform(-9, -6)) # Diffusion length
+    Lp = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
+    Ln = np.power(10, np.random.uniform(-9, -6))  # Diffusion length
 
     sn = np.power(10, np.random.uniform(0, 3))
     sp = np.power(10, np.random.uniform(0, 3))
 
-    se = np.random.uniform(1, 20)*vacuum_permittivity
+    se = np.random.uniform(1, 20) * vacuum_permittivity
 
     GaAs_n = material("GaAs")()
     GaAs_p = material("GaAs")()
     GaAs_i = material("GaAs")()
 
     p_width = np.random.uniform(500, 1000)
     n_width = np.random.uniform(3000, 5000)
-    i_width = np.random.uniform(100, 300)*1e-9
+    i_width = np.random.uniform(100, 300) * 1e-9
 
     mun = np.power(10, np.random.uniform(-5, 0))
     mup = np.power(10, np.random.uniform(-5, 0))
 
     Vbi = np.random.uniform(0, 3)
 
-    test_junc = Junction([Layer(p_width, GaAs_p, role="emitter"),
-                          Layer(i_width, GaAs_i, role="intrinsic"),
-                          Layer(n_width, GaAs_n, role="base")],
-                         sn = sn, sp = sp, permittivity = se,
-                         ln = Ln, lp= Lp,
-                         mup = mup, mun = mun, Vbi = Vbi)
+    test_junc = Junction(
+        [
+            Layer(p_width, GaAs_p, role="emitter"),
+            Layer(i_width, GaAs_i, role="intrinsic"),
+            Layer(n_width, GaAs_n, role="base"),
+        ],
+        sn=sn,
+        sp=sp,
+        permittivity=se,
+        ln=Ln,
+        lp=Lp,
+        mup=mup,
+        mun=mun,
+        Vbi=Vbi,
+    )
 
     id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(test_junc)
-    xn, xp, xi, sn_c, sp_c, ln, lp, dn, dp, Nd_c, Na_c, ni, es = identify_parameters(test_junc, options.T, pRegion, nRegion, iRegion)
+    xn, xp, xi, sn_c, sp_c, ln, lp, dn, dp, Nd_c, Na_c, ni, es, _ = identify_parameters(
+        test_junc, options.T, pRegion, nRegion, iRegion
+    )
 
     ni_expect = GaAs_n.ni
 
     assert [id_top, id_bottom] == approx([0, 2])
-    assert pn_or_np == 'pn'
-    assert [xn, xp, xi, sn_c, sp_c, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx([n_width, p_width, i_width, sn, sp, Ln, Lp, mun * kb * options.T / q,
-                                    mup * kb * options.T / q, 1, 1, ni_expect, se])
+    assert pn_or_np == "pn"
+    assert [xn, xp, xi, sn_c, sp_c, ln, lp, dn, dp, Nd_c, Na_c, ni, es] == approx(
+        [
+            n_width,
+            p_width,
+            i_width,
+            sn,
+            sp,
+            Ln,
+            Lp,
+            mun * kb * options.T / q,
+            mup * kb * options.T / q,
+            1,
+            1,
+            ni_expect,
+            se,
+        ]
+    )
 
 
 def test_get_depletion_widths():
-    from solcore.analytic_solar_cells.depletion_approximation import get_depletion_widths
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        get_depletion_widths,
+    )
     from solcore.structure import Junction
 
-    xi  = np.power(10, np.random.uniform(-10, -6))
+    xi = np.power(10, np.random.uniform(-10, -6))
 
     Vbi = np.random.uniform(0, 3)
-    es = np.random.uniform(1, 20)*vacuum_permittivity
+    es = np.random.uniform(1, 20) * vacuum_permittivity
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(22, 25))
 
     V = np.linspace(-6, 4, 20)
     V = np.where(V < Vbi - 0.001, V, Vbi - 0.001)
 
     test_junc = Junction()
 
-    wn_e = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Nd / Na)
-    wp_e = (-xi + np.sqrt(xi ** 2 + 2. * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (1 + Na / Nd)
+    wn_e = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Nd / Na
+    )
+    wp_e = (-xi + np.sqrt(xi**2 + 2.0 * es * (Vbi - V) / q * (1 / Na + 1 / Nd))) / (
+        1 + Na / Nd
+    )
 
-    wn_r, wp_r = get_depletion_widths(test_junc, es, Vbi, V, Na, Nd, xi)
+    wn_r, wp_r = get_depletion_widths(test_junc, es, es, Vbi, V, Na, Nd, xi)
 
     assert wn_r == approx(wn_e)
     assert wp_r == approx(wp_e)
 
 
 def test_get_depletion_widths_onesided():
-    from solcore.analytic_solar_cells.depletion_approximation import get_depletion_widths
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        get_depletion_widths,
+    )
     from solcore.structure import Junction
 
-    xi  = np.power(10, np.random.uniform(-10, -6))
+    xi = np.power(10, np.random.uniform(-10, -6))
 
     Vbi = np.random.uniform(0, 3)
-    es = np.random.uniform(1, 20)*vacuum_permittivity
+    es = np.random.uniform(1, 20) * vacuum_permittivity
     Na = np.power(10, np.random.uniform(22, 25))
     Nd = np.power(10, np.random.uniform(22, 25))
 
     V = np.linspace(-6, 4, 20)
     V = np.where(V < Vbi - 0.001, V, Vbi - 0.001)
 
     test_junc = Junction(depletion_approximation="one-sided abrupt")
 
     wn_e = np.sqrt(2 * es * (Vbi - V) / (q * Nd))
     wp_e = np.sqrt(2 * es * (Vbi - V) / (q * Na))
 
-    wn_r, wp_r = get_depletion_widths(test_junc, es, Vbi, V, Na, Nd, xi)
+    wn_r, wp_r = get_depletion_widths(test_junc, es, es, Vbi, V, Na, Nd, xi)
 
     assert wn_r == approx(wn_e)
     assert wp_r == approx(wp_e)
 
 
 def test_get_depletion_widths_set_in_junction():
-    from solcore.analytic_solar_cells.depletion_approximation import get_depletion_widths
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        get_depletion_widths,
+    )
     from solcore.structure import Junction
 
-    wn = np.random.uniform(1,100)
-    wp = np.random.uniform(1,100)
+    wn = np.random.uniform(1, 100)
+    wp = np.random.uniform(1, 100)
     test_junc = Junction(wn=wn, wp=wp)
 
-    wn_r, wp_r = get_depletion_widths(test_junc, 0, 0, 0, 0, 0, 0)
+    wn_r, wp_r = get_depletion_widths(test_junc, 0, 0, 0, 0, 0, 0, 0)
 
     assert wn_r == approx(wn)
     assert wp_r == approx(wp)
 
 
 def test_dark_iv_depletion_pn(pn_junction):
-    from solcore.analytic_solar_cells.depletion_approximation import iv_depletion, get_depletion_widths, get_j_dark, get_Jsrh, identify_layers, identify_parameters
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        iv_depletion,
+        get_depletion_widths,
+        get_j_dark,
+        get_Jsrh,
+        identify_layers,
+        identify_parameters,
+    )
     from scipy.interpolate import interp1d
 
     test_junc, options = pn_junction
     options.light_iv = False
     T = options.T
 
-    id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(test_junc[0])
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es = identify_parameters(test_junc[0], T, pRegion, nRegion, iRegion)
+    id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(
+        test_junc[0]
+    )
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es, _ = identify_parameters(
+        test_junc[0], T, pRegion, nRegion, iRegion
+    )
 
     niSquared = ni**2
 
     kbT = kb * T
 
     Vbi = (kbT / q) * np.log(Nd * Na / niSquared)
 
     test_junc[0].voltage = options.internal_voltages
 
     V = np.where(test_junc[0].voltage < Vbi - 0.001, test_junc[0].voltage, Vbi - 0.001)
 
-    wn, wp = get_depletion_widths(test_junc[0], es, Vbi, V, Na, Nd, xi)
+    wn, wp = get_depletion_widths(test_junc[0], es, es, Vbi, V, Na, Nd, xi)
 
     w = wn + wp + xi
 
     l_top, l_bottom = ln, lp
     x_top, x_bottom = xp, xn
     w_top, w_bottom = wp, wn
     s_top, s_bottom = sp, sn
     d_top, d_bottom = dp, dn
     min_top, min_bot = niSquared / Na, niSquared / Nd
 
     JtopDark = get_j_dark(x_top, w_top, l_top, s_top, d_top, V, min_top, T)
-    JbotDark = get_j_dark(x_bottom, w_bottom, l_bottom, s_bottom, d_bottom, V, min_bot, T)
+    JbotDark = get_j_dark(
+        x_bottom, w_bottom, l_bottom, s_bottom, d_bottom, V, min_bot, T
+    )
 
     JnDark, JpDark = JbotDark, JtopDark
 
-    lifetime_n = ln ** 2 / dn
-    lifetime_p = lp ** 2 / dp  # Jenny p163
+    lifetime_n = ln**2 / dn
+    lifetime_p = lp**2 / dp  # Jenny p163
 
     Jrec = get_Jsrh(ni, V, Vbi, lifetime_p, lifetime_n, w, kbT)
 
     J_sc_top = 0
     J_sc_bot = 0
     J_sc_scr = 0
 
-    current = Jrec + JnDark + JpDark + V / 1e14- J_sc_top - J_sc_bot - J_sc_scr
-    iv = interp1d(test_junc[0].voltage, current, kind='linear', bounds_error=False, assume_sorted=True,
-                           fill_value=(current[0], current[-1]), copy=True)
+    current = Jrec + JnDark + JpDark + V / 1e14 - J_sc_top - J_sc_bot - J_sc_scr
+    iv = interp1d(
+        test_junc[0].voltage,
+        current,
+        kind="linear",
+        bounds_error=False,
+        assume_sorted=True,
+        fill_value=(current[0], current[-1]),
+        copy=True,
+    )
 
     iv_depletion(test_junc[0], options)
 
-    assert test_junc[0].iv(options.internal_voltages) == approx(iv(options.internal_voltages), nan_ok=True)
+    assert test_junc[0].iv(options.internal_voltages) == approx(
+        iv(options.internal_voltages), nan_ok=True
+    )
 
 
 def test_dark_iv_depletion_np(np_junction):
-    from solcore.analytic_solar_cells.depletion_approximation import iv_depletion, get_depletion_widths, get_j_dark, get_Jsrh, identify_layers, identify_parameters
+    from solcore.analytic_solar_cells.depletion_approximation import (
+        iv_depletion,
+        get_depletion_widths,
+        get_j_dark,
+        get_Jsrh,
+        identify_layers,
+        identify_parameters,
+    )
     from scipy.interpolate import interp1d
 
     test_junc, options = np_junction
     options.light_iv = False
     T = options.T
 
     test_junc[0].voltage = options.internal_voltages
 
-    id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(test_junc[0])
-    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es = identify_parameters(test_junc[0], T, pRegion, nRegion, iRegion)
+    id_top, id_bottom, pRegion, nRegion, iRegion, pn_or_np = identify_layers(
+        test_junc[0]
+    )
+    xn, xp, xi, sn, sp, ln, lp, dn, dp, Nd, Na, ni, es, _ = identify_parameters(
+        test_junc[0], T, pRegion, nRegion, iRegion
+    )
 
     niSquared = ni**2
 
     kbT = kb * T
 
     Vbi = (kbT / q) * np.log(Nd * Na / niSquared)
 
     V = np.where(test_junc[0].voltage < Vbi - 0.001, test_junc[0].voltage, Vbi - 0.001)
 
-    wn, wp = get_depletion_widths(test_junc[0], es, Vbi, V, Na, Nd, xi)
+    wn, wp = get_depletion_widths(test_junc[0], es, es, Vbi, V, Na, Nd, xi)
 
     w = wn + wp + xi
 
     l_bottom, l_top = ln, lp
     x_bottom, x_top = xp, xn
     w_bottom, w_top = wp, wn
     s_bottom, s_top = sp, sn
     d_bottom, d_top = dp, dn
     min_bot, min_top = niSquared / Na, niSquared / Nd
 
     JtopDark = get_j_dark(x_top, w_top, l_top, s_top, d_top, V, min_top, T)
-    JbotDark = get_j_dark(x_bottom, w_bottom, l_bottom, s_bottom, d_bottom, V, min_bot, T)
+    JbotDark = get_j_dark(
+        x_bottom, w_bottom, l_bottom, s_bottom, d_bottom, V, min_bot, T
+    )
 
     JpDark, JnDark = JbotDark, JtopDark
 
-    lifetime_n = ln ** 2 / dn
-    lifetime_p = lp ** 2 / dp  # Jenny p163
+    lifetime_n = ln**2 / dn
+    lifetime_p = lp**2 / dp  # Jenny p163
 
     Jrec = get_Jsrh(ni, V, Vbi, lifetime_p, lifetime_n, w, kbT)
 
     J_sc_top = 0
     J_sc_bot = 0
     J_sc_scr = 0
 
-    current = Jrec + JnDark + JpDark + V / 1e14- J_sc_top - J_sc_bot - J_sc_scr
-    iv = interp1d(test_junc[0].voltage, current, kind='linear', bounds_error=False, assume_sorted=True,
-                           fill_value=(current[0], current[-1]), copy=True)
+    current = Jrec + JnDark + JpDark + V / 1e14 - J_sc_top - J_sc_bot - J_sc_scr
+    iv = interp1d(
+        test_junc[0].voltage,
+        current,
+        kind="linear",
+        bounds_error=False,
+        assume_sorted=True,
+        fill_value=(current[0], current[-1]),
+        copy=True,
+    )
 
     iv_depletion(test_junc[0], options)
 
-    assert test_junc[0].iv(options.internal_voltages) == approx(iv(options.internal_voltages), nan_ok=True)
+    assert test_junc[0].iv(options.internal_voltages) == approx(
+        iv(options.internal_voltages), nan_ok=True
+    )
 
 
 def test_qe_depletion_np(np_junction):
-
     from solcore.analytic_solar_cells import qe_depletion
 
     test_junc, options = np_junction
 
     wl = options.wavelength
 
     qe_depletion(test_junc[0], options)
 
     assert np.all(test_junc[0].eqe(wl) < 1)
     assert np.all(test_junc[0].eqe_emitter(wl) < 1)
     assert np.all(test_junc[0].eqe_base(wl) < 1)
     assert np.all(test_junc[0].eqe_scr(wl) < 1)
-    assert np.all(test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
-                  <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3])
-    assert np.all(test_junc[0].eqe_emitter(wl) + test_junc[0].eqe_base(wl) +
-                  test_junc[0].eqe_scr(wl) == approx(test_junc[0].eqe(wl)))
+    assert np.all(
+        test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
+        <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3]
+    )
+    assert np.all(
+        test_junc[0].eqe_emitter(wl)
+        + test_junc[0].eqe_base(wl)
+        + test_junc[0].eqe_scr(wl)
+        == approx(test_junc[0].eqe(wl))
+    )
     assert np.all(test_junc[0].iqe(wl) >= test_junc[0].eqe(wl))
 
-    options['da_mode'] = 'green'
+    options["da_mode"] = "green"
     qe_depletion(test_junc[0], options)
 
     assert np.all(test_junc[0].eqe(wl) < 1)
     assert np.all(test_junc[0].eqe_emitter(wl) < 1)
     assert np.all(test_junc[0].eqe_base(wl) < 1)
     assert np.all(test_junc[0].eqe_scr(wl) < 1)
-    assert np.all(test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
-                  <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3])
-    assert np.all(test_junc[0].eqe_emitter(wl) + test_junc[0].eqe_base(wl) +
-                  test_junc[0].eqe_scr(wl) == approx(test_junc[0].eqe(wl)))
+    assert np.all(
+        test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
+        <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3]
+    )
+    assert np.all(
+        test_junc[0].eqe_emitter(wl)
+        + test_junc[0].eqe_base(wl)
+        + test_junc[0].eqe_scr(wl)
+        == approx(test_junc[0].eqe(wl))
+    )
     assert np.all(test_junc[0].iqe(wl) >= test_junc[0].eqe(wl))
 
 
 def test_qe_depletion_pn(pn_junction):
     from solcore.analytic_solar_cells import qe_depletion
 
     test_junc, options = pn_junction
@@ -1048,99 +1314,194 @@
 
     qe_depletion(test_junc[0], options)
 
     assert np.all(test_junc[0].eqe(wl) < 1)
     assert np.all(test_junc[0].eqe_emitter(wl) < 1)
     assert np.all(test_junc[0].eqe_base(wl) < 1)
     assert np.all(test_junc[0].eqe_scr(wl) < 1)
-    assert np.all(test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
-                  <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3])
-    assert np.all(test_junc[0].eqe_emitter(wl) + test_junc[0].eqe_base(wl) +
-                  test_junc[0].eqe_scr(wl) == approx(test_junc[0].eqe(wl)))
+    assert np.all(
+        test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
+        <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3]
+    )
+    assert np.all(
+        test_junc[0].eqe_emitter(wl)
+        + test_junc[0].eqe_base(wl)
+        + test_junc[0].eqe_scr(wl)
+        == approx(test_junc[0].eqe(wl))
+    )
     assert np.all(test_junc[0].iqe(wl) >= test_junc[0].eqe(wl))
 
-    options['da_mode'] = 'green'
+    options["da_mode"] = "green"
     qe_depletion(test_junc[0], options)
 
     assert np.all(test_junc[0].eqe(wl) < 1)
     assert np.all(test_junc[0].eqe_emitter(wl) < 1)
     assert np.all(test_junc[0].eqe_base(wl) < 1)
     assert np.all(test_junc[0].eqe_scr(wl) < 1)
-    assert np.all(test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
-                  <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3])
-    assert np.all(test_junc[0].eqe_emitter(wl) + test_junc[0].eqe_base(wl) +
-                  test_junc[0].eqe_scr(wl) == approx(test_junc[0].eqe(wl)))
+    assert np.all(
+        test_junc[0].eqe(wl)[test_junc[0].eqe(wl) > 1e-3]
+        <= test_junc.absorbed[test_junc[0].eqe(wl) > 1e-3]
+    )
+    assert np.all(
+        test_junc[0].eqe_emitter(wl)
+        + test_junc[0].eqe_base(wl)
+        + test_junc[0].eqe_scr(wl)
+        == approx(test_junc[0].eqe(wl))
+    )
     assert np.all(test_junc[0].iqe(wl) >= test_junc[0].eqe(wl))
 
-def test_iv_depletion_np(np_junction):
 
+def test_iv_depletion_np(np_junction):
     from solcore.analytic_solar_cells import iv_depletion
 
     test_junc, options = np_junction
     options.light_iv = True
     V = options.internal_voltages
     wl = options.wavelength
 
     iv_depletion(test_junc[0], options)
 
-    wl_sp, ph = options.light_source.spectrum(output_units='photon_flux_per_m', x=wl)
-    Jph = q*np.trapz(test_junc.absorbed*ph, wl)
+    wl_sp, ph = options.light_source.spectrum(output_units="photon_flux_per_m", x=wl)
+    Jph = q * np.trapz(test_junc.absorbed * ph, wl)
 
     approx_Voc = V[np.argmin(abs(test_junc[0].iv(V)))]
 
     quadrant = (V > 0) * (V < approx_Voc)
 
-    power = abs(test_junc[0].iv(V[quadrant])*V[quadrant])[:-1]
+    power = abs(test_junc[0].iv(V[quadrant]) * V[quadrant])[:-1]
 
     assert abs(test_junc[0].iv(0)) <= Jph
-    assert approx_Voc < test_junc[0][1].material.band_gap/q
+    assert approx_Voc < test_junc[0][1].material.band_gap / q
     assert np.all(power < options.light_source.power_density)
 
-    options['da_mode'] = 'green'
+    options["da_mode"] = "green"
     iv_depletion(test_junc[0], options)
 
     approx_Voc = V[np.argmin(abs(test_junc[0].iv(V)))]
 
     quadrant = (V > 0) * (V < approx_Voc)
 
-    power = abs(test_junc[0].iv(V[quadrant])*V[quadrant])[:-1]
+    power = abs(test_junc[0].iv(V[quadrant]) * V[quadrant])[:-1]
 
     assert abs(test_junc[0].iv(0)) <= Jph
-    assert approx_Voc < test_junc[0][1].material.band_gap/q
+    assert approx_Voc < test_junc[0][1].material.band_gap / q
     assert np.all(power < options.light_source.power_density)
 
+
 def test_iv_depletion_pn(pn_junction):
     from solcore.analytic_solar_cells import iv_depletion
 
     test_junc, options = pn_junction
     options.light_iv = True
     V = options.internal_voltages
     wl = options.wavelength
 
     iv_depletion(test_junc[0], options)
 
-    wl_sp, ph = options.light_source.spectrum(output_units='photon_flux_per_m', x=wl)
-    Jph = q*np.trapz(test_junc.absorbed*ph, wl)
+    wl_sp, ph = options.light_source.spectrum(output_units="photon_flux_per_m", x=wl)
+    Jph = q * np.trapz(test_junc.absorbed * ph, wl)
 
     approx_Voc = V[np.argmin(abs(test_junc[0].iv(V)))]
 
     quadrant = (V > 0) * (V < approx_Voc)
 
-    power = abs(test_junc[0].iv(V[quadrant])*V[quadrant])[:-1]
+    power = abs(test_junc[0].iv(V[quadrant]) * V[quadrant])[:-1]
 
     assert abs(test_junc[0].iv(0)) <= Jph
-    assert approx_Voc < test_junc[0][1].material.band_gap/q
+    assert approx_Voc < test_junc[0][1].material.band_gap / q
     assert np.all(power < options.light_source.power_density)
 
-    options['da_mode'] = 'green'
+    options["da_mode"] = "green"
     iv_depletion(test_junc[0], options)
 
     approx_Voc = V[np.argmin(abs(test_junc[0].iv(V)))]
 
     quadrant = (V > 0) * (V < approx_Voc)
 
-    power = abs(test_junc[0].iv(V[quadrant])*V[quadrant])[:-1]
+    power = abs(test_junc[0].iv(V[quadrant]) * V[quadrant])[:-1]
 
     assert abs(test_junc[0].iv(0)) <= Jph
-    assert approx_Voc < test_junc[0][1].material.band_gap/q
+    assert approx_Voc < test_junc[0][1].material.band_gap / q
     assert np.all(power < options.light_source.power_density)
 
+
+def test_depletion_width():
+    from solcore import material
+    from solcore.solar_cell import Junction, Layer
+    from solcore.analytic_solar_cells.depletion_approximation \
+        import get_depletion_widths
+    from solcore.analytic_solar_cells.depletion_approximation \
+        import qe_depletion, iv_depletion
+    from solcore.state import State
+    from solcore.solar_cell_solver import prepare_solar_cell, SolarCell
+    from solcore.optics import solve_beer_lambert
+    from solcore.light_source import LightSource
+
+    Na_top = 1e18*1e6
+    Nd_bottom = 1e18*1e6
+
+    Ln = 1e-6
+    Lp = 1e-6
+
+    InGaP = material("GaInP")
+
+    top_cell_p_material = InGaP(
+        In=0.48,
+        Na=Na_top,
+        electron_diffusion_length=Lp,
+    )
+    top_cell_n_material = InGaP(
+        In=0.48,
+        Nd=Nd_bottom,
+        hole_diffusion_length=Ln,
+    )
+
+    rel_perm = 10 * vacuum_permittivity
+
+    n_width = 30e-9
+    p_width = 30e-9
+
+    test_junc = Junction(
+                [
+                    Layer(n_width, material=top_cell_n_material, role="emitter"),
+                    Layer(p_width, material=top_cell_p_material, role="base"),
+                ],
+                sn=100,
+                sp=100,
+                kind="DA",
+            )
+
+    T = 300
+    Vbi = 2.1
+
+    wn, wp = get_depletion_widths(test_junc, rel_perm, rel_perm, Vbi, 0, Na_top,
+                                  Nd_bottom, 0)
+
+    assert wn > n_width
+    assert wp > p_width
+
+    options = State()
+    wl = np.linspace(290, 700, 150) * 1e-9
+    options.T = T
+    options.wavelength = wl
+    options.position = None
+    options.internal_voltages = np.linspace(-2, 2, 50)
+    options.da_mode = 'green'
+    options.light_iv = True
+
+    light_source = LightSource(source_type="standard", version="AM1.5g")
+
+    options.light_source = light_source
+
+    solar_cell = SolarCell([test_junc])
+
+    prepare_solar_cell(solar_cell, options)
+    solve_beer_lambert(solar_cell, **options)
+
+    iv_depletion(test_junc, options)
+    qe_depletion(test_junc, options)
+
+    max_current = np.trapz(solar_cell.absorbed * light_source.spectrum(
+        output_units="photon_flux_per_m", x=wl)[1], wl) * q
+
+    assert np.all(test_junc.eqe(wl) <= 1)
+    assert np.abs(test_junc.iv(0)) <= max_current
```

### Comparing `solcore-5.9.1/tests/test_dielectric_constant.py` & `solcore-5.9.2/tests/test_dielectric_constant.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_examples.py` & `solcore-5.9.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_light_source.py` & `solcore-5.9.2/tests/test_light_source.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_optics.py` & `solcore-5.9.2/tests/test_optics.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_optimization.py` & `solcore-5.9.2/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_qm.py` & `solcore-5.9.2/tests/test_qm.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_registries.py` & `solcore-5.9.2/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_solar_cell_solver.py` & `solcore-5.9.2/tests/test_solar_cell_solver.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_state.py` & `solcore-5.9.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_structure.py` & `solcore-5.9.2/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/tests/test_tmm_core_vec.py` & `solcore-5.9.2/tests/test_tmm_core_vec.py`

 * *Files identical despite different names*

### Comparing `solcore-5.9.1/PKG-INFO` & `solcore-5.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solcore
-Version: 5.9.1
+Version: 5.9.2
 Summary: Python-based solar cell simulator
 Keywords: photovoltaics modelling physics
 Home-page: https://www.solcore.solar/
 Author-Email: The Quantum Photovoltaics Group <nekins@unsw.edu.au>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -181,15 +181,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Project-URL: Homepage, https://www.solcore.solar/
 Project-URL: Documentation, http://solcore5.readthedocs.io
 Project-URL: Repository, https://github.com/qpv-research-group/solcore5
 Project-URL: Changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Requires-Python: >=3.7
-Requires-Dist: numpy
+Requires-Dist: numpy>=1.21.0
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: tmm
 Requires-Dist: natsort
 Requires-Dist: regex
 Requires-Dist: cycler
 Requires-Dist: pyyaml
```

