# Comparing `tmp/comet_toolbox-0.4.3.tar.gz` & `tmp/comet_toolbox-0.4.4.tar.gz`

## Comparing `comet_toolbox-0.4.3.tar` & `comet_toolbox-0.4.4.tar`

### file list

```diff
@@ -1,140 +1,142 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/.gitattributes
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/.vscode/settings.json
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/__init__.py
--rwxr-xr-x   0        0        0     4012 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/data.py
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/data_bids.py
--rwxr-xr-x   0        0        0     3827 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/data_cifti.py
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/graph.py
--rw-r--r--   0        0        0   173989 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/gui.py
--rwxr-xr-x   0        0        0    48745 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/methods.py
--rwxr-xr-x   0        0        0    23073 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/multiverse.py
--rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/simulation.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/simulation.txt
--rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/single_state.txt
--rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/atlas/README.md
--rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
--rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
--rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
--rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/img/content.drawio
--rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/img/content.png
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/img/doi.svg
--rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/img/gui.png
--rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/img/logo.png
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/src/comet/resources/img/pypi.svg
--rw-r--r--   0        0        0   185264 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_analysis.ipynb
--rw-r--r--   0        0        0   452068 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_dfc.ipynb
--rw-r--r--   0        0        0  1314230 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_graph.ipynb
--rw-r--r--   0        0        0   114994 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_multiverse.ipynb
--rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_data/abide_50008.txt
--rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_data/aomic_multi.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_data/simulation.txt
--rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_data/xcpd.tsv
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/example_multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/pipelines.csv
--rw-r--r--   0        0        0    53935 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/specification_curve.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_1.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_10.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_11.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_12.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_13.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_14.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_15.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_16.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_17.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_18.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_19.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_2.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_20.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_21.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_22.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_23.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_24.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_25.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_26.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_27.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_28.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_29.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_3.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_30.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_31.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_32.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_33.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_34.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_35.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_36.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_37.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_38.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_39.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_4.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_40.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_41.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_42.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_43.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_44.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_45.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_46.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_47.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_48.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_49.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_5.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_50.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_51.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_52.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_53.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_54.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_55.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_56.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_57.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_58.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_59.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_6.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_60.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_61.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_62.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_63.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_64.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_65.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_66.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_67.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_68.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_69.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_7.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_70.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_71.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_72.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_73.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_74.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_75.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_76.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_77.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_78.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_79.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_8.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_80.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_81.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_82.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_83.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_84.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_85.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_86.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_87.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_88.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_89.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_9.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_90.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_91.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_92.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_93.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_94.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_95.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/multiverse/results/universe_96.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/tutorials/universes/results/universe_1.pkl
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/LICENSE
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/README.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 comet_toolbox-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/.gitattributes
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/.vscode/settings.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/example_multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/example_multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/__init__.py
+-rwxr-xr-x   0        0        0     4012 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/data.py
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/data_bids.py
+-rwxr-xr-x   0        0        0     3827 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/data_cifti.py
+-rw-r--r--   0        0        0    29362 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/graph.py
+-rw-r--r--   0        0        0   173989 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/gui.py
+-rwxr-xr-x   0        0        0    48876 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/methods.py
+-rwxr-xr-x   0        0        0    23073 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/multiverse.py
+-rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/simulation.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/simulation.txt
+-rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/single_state.txt
+-rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
+-rwxr-xr-x   0        0        0      586 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/atlas/README.md
+-rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
+-rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
+-rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
+-rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/img/content.drawio
+-rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/img/content.png
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/img/doi.svg
+-rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/img/gui.png
+-rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/img/logo.png
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/src/comet/resources/img/pypi.svg
+-rw-r--r--   0        0        0   185264 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_analysis.ipynb
+-rw-r--r--   0        0        0   452068 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_dfc.ipynb
+-rw-r--r--   0        0        0  1314230 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_graph.ipynb
+-rw-r--r--   0        0        0   114994 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_multiverse.ipynb
+-rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_data/abide_50008.txt
+-rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_data/aomic_multi.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_data/simulation.txt
+-rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_data/xcpd.tsv
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/example_multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/pipelines.csv
+-rw-r--r--   0        0        0    53935 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/specification_curve.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_1.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_10.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_11.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_12.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_13.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_14.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_15.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_16.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_17.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_18.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_19.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_2.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_20.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_21.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_22.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_23.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_24.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_25.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_26.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_27.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_28.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_29.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_3.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_30.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_31.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_32.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_33.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_34.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_35.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_36.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_37.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_38.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_39.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_4.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_40.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_41.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_42.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_43.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_44.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_45.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_46.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_47.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_48.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_49.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_5.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_50.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_51.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_52.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_53.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_54.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_55.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_56.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_57.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_58.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_59.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_6.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_60.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_61.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_62.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_63.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_64.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_65.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_66.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_67.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_68.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_69.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_7.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_70.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_71.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_72.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_73.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_74.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_75.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_76.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_77.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_78.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_79.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_8.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_80.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_81.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_82.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_83.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_84.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_85.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_86.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_87.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_88.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_89.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_9.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_90.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_91.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_92.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_93.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_94.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_95.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/multiverse/results/universe_96.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/tutorials/universes/results/universe_1.pkl
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/LICENSE
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/README.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 comet_toolbox-0.4.4/PKG-INFO
```

### Comparing `comet_toolbox-0.4.3/src/comet/data.py` & `comet_toolbox-0.4.4/src/comet/data.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/data_cifti.py` & `comet_toolbox-0.4.4/src/comet/data_cifti.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/graph.py` & `comet_toolbox-0.4.4/src/comet/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -307,21 +307,21 @@
                       include_diagonal: bool = False,
                       include_infinite: bool = False) -> float:
     '''
     Average shortest path length calculated from the distance matrix.
     '''
     is_binary = np.all(np.logical_or(np.isclose(G, 0), np.isclose(G, 1)))
     if is_binary:
-        D = distance_bin(G, inv=False)
+        D = distance_bin(G)
     else:
-        D = distance_wei(G, inv=False)
+        D = distance_wei(G, inv=True)
 
     if np.isinf(D).any():
         import warnings
-        issue = "The graph is not fully connected and infinite path lenghts were set to NaN. Small world estimates might be inaccurate."
+        issue = "The graph is not fully connected and infinite path lenghts were set to NaN"
         warnings.warn(issue)
     if not include_diagonal:
         np.fill_diagonal(D, np.nan)
     if not include_infinite:
         D[np.isinf(D)] = np.nan
 
     Dv = D[~np.isnan(D)]
@@ -664,37 +664,40 @@
     denominator = np.where((degsum <= 2) & (nei != 1), 1.0, degsum - 2 * G)
     M = np.where(denominator != 0, (nei * 2) / denominator, 0.0)
     for i in range(n):
         M[i, i] = 0.0
     return M
 
 @jit(nopython=True)
-def distance_wei(G: np.ndarray, inv: bool = False) -> np.ndarray:
+def distance_wei(G: np.ndarray, inv: bool = True) -> np.ndarray:
     '''(Inverse) distance matrix for weighted networks
 
     Based on the bctpy implelementation by Roan LaPlante: https://github.com/aestrivex/bctpy
     Significantly improved performance due to numba JIT compilation
 
     Parameters
     ----------
     G : PxP np.ndarray
         undireted weighted adjacency/connectivity matrix
 
     inv : bool, optional
-        if True, the element wise inverse of the distance matrux is returned. Default is False
+        if True, the element wise inverse of the distance matrux is returned. Default is True
 
     Returns
     -------
     D : PxP np.ndarray
         (inverse) distance matrix
 
     Notes
     -----
     Algorithm: Modified Dijkstra's algorithm
     '''
+    if inv:
+        G = 1 / G
+
     n = len(G)
     D = np.full((n, n), np.inf)
     np.fill_diagonal(D, 0)
 
     for u in range(n):
         # distance permanence (true is temporary)
         S = np.ones((n,), dtype=np.bool_)
@@ -717,36 +720,28 @@
             if D[u, S].size == 0:  # all nodes reached
                 break
             minD = np.min(D[u, S])
             if np.isinf(minD):  # some nodes cannot be reached
                 break
             V = np.where(D[u, :] == minD)[0]
 
-    np.fill_diagonal(D, 1)
-    if inv:
-        D = 1 / D
-        np.fill_diagonal(D, 0)
-
     return D
 
 @jit(nopython=True)
-def distance_bin(G: np.ndarray, inv: bool = False) -> np.ndarray:
-    '''(Inverse) distance matrix for binary networks
+def distance_bin(G: np.ndarray) -> np.ndarray:
+    '''Distance matrix for binary networks
 
     Based on the bctpy implelementation by Roan LaPlante: https://github.com/aestrivex/bctpy
     Significantly improved performance due to numba JIT compilation
 
     Parameters
     ----------
     G : PxP np.ndarray
         undireted weighted adjacency/connectivity matrix
 
-    inv : bool, optional
-        if True, the element wise inverse of the distance matrux is returned. Default is False
-
     Returns
     -------
     D : PxP np.ndarray
         (inverse) distance matrix
 
     Notes
     -----
@@ -764,99 +759,96 @@
         L = (nPATH != 0) * (D == 0)
 
     for i in range(D.shape[0]):
         for j in range(D.shape[1]):
             if not D[i, j]:
                 D[i, j] = np.inf
 
-    np.fill_diagonal(D, 1)
-    if inv:
-        D = 1 / D
-        np.fill_diagonal(D, 0)
+    np.fill_diagonal(D, 0)
 
     return D
 
 # BCT wrapper functions with type hinting (GUI needs to know the parameter types)
 def backbone_wu(CIJ: np.ndarray,
                 avgdeg: int = 0,
                 verbose: bool = False) -> tuple[np.ndarray, np.ndarray]:
     res = bct.backbone_wu(CIJ, avgdeg, verbose)
-    res_dict = {"Connection matrix of the minimum spanning tree of CIJ": res[0],
-                "Connection matrix of the minimum spanning tree plus strongest connections up to some average degree <avgdeg>": res[1]}
-    return res_dict
+    label = ["Connection matrix of the minimum spanning tree of CIJ", \
+             "Connection matrix of the minimum spanning tree plus strongest connections up to some average degree <avgdeg>"]
+    return res, label
 
 def betweenness(G: np.ndarray,
                 weighted: bool = True) -> np.ndarray:
     res = bct.betweenness_wei(G) if weighted else bct.betweenness_bin(G)
-    res_dict = {"Nodal betweenness centrality (weighted)": res} if weighted else {"Nodal betweenness centrality (binary)": res}
-    return res_dict
+    label = "Nodal betweenness centrality (weighted)" if weighted else "Nodal betweenness centrality (binary)"
+    return res, label
 
 def clustering_coef(G: np.ndarray,
                        weighted: bool = True) -> np.ndarray:
     res = bct.clustering_coef_wu(G) if weighted else bct.clustering_coef_bu(G)
-    res_dict = {"Nodal clustering coefficient (weighted)": res} if weighted else {"Nodal clustering coefficient (binary)": res}
-    return res_dict
+    label = "Nodal clustering coefficient (weighted)" if weighted else "Nodal clustering coefficient (binary)"
+    return res, label
 
 def degrees_und(CIJ: np.ndarray) -> np.ndarray:
     res = bct.degrees_und(CIJ)
-    res_dict = {"Nodal degree": res}
-    return res_dict
+    label = "Nodal degree"
+    return res, label
 
 def density_und(CIJ: np.ndarray) -> tuple[float, int, int]:
     res = bct.density_und(CIJ)
-    res_dict = {"Density": res[0], "Number of vertices": res[1], "Number of edges": res[2]}
-    return res_dict
+    label = ["Density", "Number of vertices", "Number of edges"]
+    return res, label
 
 def eigenvector_centrality_und(CIJ: np.ndarray) -> np.ndarray:
     res = bct.eigenvector_centrality_und(CIJ)
-    res_dict = {"Nodal eigenvector centrality": res}
-    return res_dict
+    label = "Nodal eigenvector centrality"
+    return res, label
 
 def gateway_coef_sign(CIJ: np.ndarray,
                       ci: Literal["louvain"] = "louvain",
                       centrality_type: Literal["degree", "betweenness"] = "degree", ) \
                                         -> tuple[np.ndarray, np.ndarray]:
     ci, _ = bct.community_louvain(CIJ)
     res = bct.gateway_coef_sign(CIJ, ci, centrality_type)
-    res_dict = {"Gateway coefficient for positive weights": res[0], \
-                "Gateway coefficient for negative weights": res[1]}
-    return res_dict
+    label = ["Gateway coefficient for positive weights", \
+             "Gateway coefficient for negative weights"]
+    return res, label
 
 def pagerank_centrality(A: np.ndarray,
                         d: float = 0.85,
                         falff: Literal["byesian prior"] = "byesian prior") -> np.ndarray:
     res = bct.pagerank_centrality(A, d, None)
-    res_dict = {"Nodal pageranking vectors": res}
-    return res_dict
+    label = "Nodal pageranking vectors"
+    return res, label
 
 def participation_coef(CIJ: np.ndarray,
                        ci: Literal["louvain"] = "louvain",
                        sparse: bool = False,
                        degree: Literal["undirected"] = "undirected") -> np.ndarray:
     ci, _ = bct.community_louvain(CIJ)
     res = bct.participation_coef_sparse(CIJ, ci, degree) if sparse else bct.participation_coef(CIJ, ci, degree)
-    res_dict = {"Nodal participation coefficient (sparse)": res} if sparse else {"Nodal participation coefficient": res}
-    return res_dict
+    label = "Nodal participation coefficient (sparse)" if sparse else "Nodal participation coefficient"
+    return res, label
 
 def participation_coef_sign(CIJ: np.ndarray,
                             ci: Literal["louvain"] = "louvain",) -> tuple[np.ndarray, np.ndarray]:
     ci, _ = bct.community_louvain(CIJ)
     res = bct.participation_coef_sign(CIJ, ci)
-    res_dict = {"Nodal participation coefficient from positive weights": res[0], "Nodal participation coefficient from negative weights": res[1]}
-    return res_dict
+    label = ["Nodal participation coefficient from positive weights", "Nodal participation coefficient from negative weights"]
+    return res, label
 
 """
 def rich_club(CIJ: np.ndarray,
                  weighted: bool=True,
                  klevel: int = None) -> np.ndarray:
     res = bct.rich_club_wu(CIJ, klevel) if weighted else bct.rich_club_bu(CIJ, klevel)
     print("rich club", type(res))
     print(res)
-    res_dict = {"Rich club coefficient vectors (weighted)": res} if weighted else {"Rich club coefficient vectors (binary)": res}
-    return res_dict"""
+    label = "Rich club coefficient vectors (weighted)" if weighted else "Rich club coefficient vectors (binary)"
+    return res, label"""
 
 """
 def transitivity(CIJ: np.ndarray,
                  weighted: bool=True) -> float:
     res = bct.transitivity_wu(CIJ) if weighted else bct.transitivity_bu(CIJ)
-    res_dict = {"Global transitivity (weighted)": res} if weighted else {"Global transitivity (binary)": res}
-    return res_dict"""
+    label = "Global transitivity (weighted)" if weighted else "Global transitivity (binary)"
+    return res, label"""
```

### Comparing `comet_toolbox-0.4.3/src/comet/gui.py` & `comet_toolbox-0.4.4/src/comet/gui.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/methods.py` & `comet_toolbox-0.4.4/src/comet/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from scipy.spatial import distance
 from scipy.signal import windows, hilbert
 from scipy.linalg import eigh, solve, inv
 from scipy.optimize import minimize
 from sklearn.metrics import mutual_info_score
 from statsmodels.stats.weightstats import DescrStatsW
 from pycwt import cwt, Morlet
-from pydfc.dfc_methods import *
+from pydfc.dfc_methods import BaseDFCMethod, SLIDING_WINDOW, SLIDING_WINDOW_CLUSTR, \
+                              TIME_FREQ, CAP, HMM_DISC, HMM_CONT, WINDOWLESS
 from pydfc import time_series
 from typing import Literal
 
 from joblib import Parallel, delayed
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["OMP_NUM_THREADS"] = "1"
```

### Comparing `comet_toolbox-0.4.3/src/comet/multiverse.py` & `comet_toolbox-0.4.4/src/comet/multiverse.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/simulation.pkl` & `comet_toolbox-0.4.4/src/comet/resources/simulation.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/simulation.txt` & `comet_toolbox-0.4.4/src/comet/resources/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/single_state.txt` & `comet_toolbox-0.4.4/src/comet/resources/single_state.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii` & `comet_toolbox-0.4.4/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/atlas/README.md` & `comet_toolbox-0.4.4/src/comet/resources/atlas/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Atlas summary
 
 ## Available parcellations
+
  1. Glasser MMP + subcortical (<https://balsa.wustl.edu/file/87B9N>)
  2. Schaefer 2018 (200 parcels, 17 networks, <https://github.com/ThomasYeoLab/CBIG/tree/master/stable_projects/brain_parcellation/Schaefer2018_LocalGlobal/Parcellations/HCP/fslr32k/cifti>)
  3. Schaefer 2018 + subcortical (200 cortical + 54 subcortical, 17 networks, <https://github.com/yetianmed/subcortex/tree/master/Group-Parcellation/3T/Cortex-Subcortex>)
 
 ## Available methods
- - np.mean: Average over all vertices/voxels within the parcel
+
+Currently only np.mean is available to average over all vertices/voxels within the parcel
```

### Comparing `comet_toolbox-0.4.3/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii` & `comet_toolbox-0.4.4/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii` & `comet_toolbox-0.4.4/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat` & `comet_toolbox-0.4.4/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/img/content.drawio` & `comet_toolbox-0.4.4/src/comet/resources/img/content.drawio`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/img/content.png` & `comet_toolbox-0.4.4/src/comet/resources/img/content.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/img/doi.svg` & `comet_toolbox-0.4.4/src/comet/resources/img/doi.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/img/gui.png` & `comet_toolbox-0.4.4/src/comet/resources/img/gui.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/img/logo.png` & `comet_toolbox-0.4.4/src/comet/resources/img/logo.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/src/comet/resources/img/pypi.svg` & `comet_toolbox-0.4.4/src/comet/resources/img/pypi.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_analysis.ipynb` & `comet_toolbox-0.4.4/tutorials/example_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_dfc.ipynb` & `comet_toolbox-0.4.4/tutorials/example_dfc.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_graph.ipynb` & `comet_toolbox-0.4.4/tutorials/example_graph.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_multiverse.ipynb` & `comet_toolbox-0.4.4/tutorials/example_multiverse.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_data/abide_50008.txt` & `comet_toolbox-0.4.4/tutorials/example_data/abide_50008.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_data/aomic_multi.pkl` & `comet_toolbox-0.4.4/tutorials/example_data/aomic_multi.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_data/simulation.txt` & `comet_toolbox-0.4.4/tutorials/example_data/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_data/xcpd.tsv` & `comet_toolbox-0.4.4/tutorials/example_data/xcpd.tsv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/example_multiverse/results/multiverse_summary.csv` & `comet_toolbox-0.4.4/tutorials/example_multiverse/results/multiverse_summary.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/multiverse/results/forking_paths.pkl` & `comet_toolbox-0.4.4/tutorials/multiverse/results/forking_paths.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/multiverse/results/multiverse_summary.csv` & `comet_toolbox-0.4.4/tutorials/multiverse/results/multiverse_summary.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/multiverse/results/pipelines.csv` & `comet_toolbox-0.4.4/tutorials/multiverse/results/pipelines.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/tutorials/multiverse/results/specification_curve.png` & `comet_toolbox-0.4.4/tutorials/multiverse/results/specification_curve.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/.gitignore` & `comet_toolbox-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/LICENSE` & `comet_toolbox-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.4.3/README.md` & `comet_toolbox-0.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## Comet - A dynamic functional connectivity toolbox for multiverse analysis
 
 [![DOI](src/comet/resources/img/doi.svg)](https://doi.org/10.1101/2024.01.21.576546) [![PyPI](src/comet/resources/img/pypi.svg)](https://pypi.org/project/comet-toolbox/)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e766745c5c04d4786ea28f7135c193e)](https://app.codacy.com/gh/mibur1/dfc-multiverse/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 ### Important notes
 
 * This package is at an early stage of development, with frequent changes being made. If you intend to use this package at this stage, I kindly ask that you contact me via the email address in the [pyproject.toml](https://github.com/mibur1/dfc-multiverse/blob/main/pyproject.toml) file.
 * Many features are not yet tested, so there will be bugs (the question is just how many). A comprehensive testing suite and documentation will be added in the near future
 
 ### Current Features
```

### Comparing `comet_toolbox-0.4.3/pyproject.toml` & `comet_toolbox-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comet-toolbox"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   {name="Micha Burkhardt", email="micha.burkhardt@uol.de"},
 ]
 description = "Dynamic functional connectivity toolbox for multiverse analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `comet_toolbox-0.4.3/PKG-INFO` & `comet_toolbox-0.4.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: comet-toolbox
-Version: 0.4.3
+Version: 0.4.4
 Summary: Dynamic functional connectivity toolbox for multiverse analysis
 Project-URL: Homepage, https://github.com/mibur1/dfc-multiverse
 Project-URL: Issues, https://github.com/mibur1/dfc-multiverse/issues
 Author-email: Micha Burkhardt <micha.burkhardt@uol.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,15 @@
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: tqdm>=4.66.1
 Description-Content-Type: text/markdown
 
 ## Comet - A dynamic functional connectivity toolbox for multiverse analysis
 
 [![DOI](src/comet/resources/img/doi.svg)](https://doi.org/10.1101/2024.01.21.576546) [![PyPI](src/comet/resources/img/pypi.svg)](https://pypi.org/project/comet-toolbox/)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e766745c5c04d4786ea28f7135c193e)](https://app.codacy.com/gh/mibur1/dfc-multiverse/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
 ### Important notes
 
 * This package is at an early stage of development, with frequent changes being made. If you intend to use this package at this stage, I kindly ask that you contact me via the email address in the [pyproject.toml](https://github.com/mibur1/dfc-multiverse/blob/main/pyproject.toml) file.
 * Many features are not yet tested, so there will be bugs (the question is just how many). A comprehensive testing suite and documentation will be added in the near future
 
 ### Current Features
```

