# Comparing `tmp/pycyclops-0.2.8.tar.gz` & `tmp/pycyclops-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycyclops-0.2.8.tar", max compression
+gzip compressed data, was "pycyclops-0.2.9.tar", max compression
```

## Comparing `pycyclops-0.2.8.tar` & `pycyclops-0.2.9.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0    11347 2024-05-15 14:17:57.619942 pycyclops-0.2.8/LICENSE.md
--rw-r--r--   0        0        0     6440 2024-05-15 14:17:57.619942 pycyclops-0.2.8/README.md
--rw-r--r--   0        0        0       23 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/__init__.py
--rw-r--r--   0        0        0      192 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/__init__.py
--rw-r--r--   0        0        0    25741 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/aggregate.py
--rw-r--r--   0        0        0     4344 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/clean.py
--rw-r--r--   0        0        0     3469 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/constants.py
--rw-r--r--   0        0        0       39 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/__init__.py
--rw-r--r--   0        0        0    26086 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/feature.py
--rw-r--r--   0        0        0    26171 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/handle_types.py
--rw-r--r--   0        0        0    17267 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/normalize.py
--rw-r--r--   0        0        0    12116 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/split.py
--rw-r--r--   0        0        0    30240 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/df/vectorized.py
--rw-r--r--   0        0        0     3295 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/diagnoses.py
--rw-r--r--   0        0        0      118 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/features/__init__.py
--rw-r--r--   0        0        0     9640 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/features/medical_image.py
--rw-r--r--   0        0        0    17072 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/impute.py
--rw-r--r--   0        0        0     3228 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/loader.py
--rw-r--r--   0        0        0      638 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/__init__.py
--rw-r--r--   0        0        0       36 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
--rw-r--r--   0        0        0     2110 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
--rw-r--r--   0        0        0      881 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/preprocess.py
--rw-r--r--   0        0        0    35159 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/slicer.py
--rw-r--r--   0        0        0     6471 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/string_ops.py
--rw-r--r--   0        0        0     3027 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/transforms.py
--rw-r--r--   0        0        0    10934 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/utils.py
--rw-r--r--   0        0        0      139 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/__init__.py
--rw-r--r--   0        0        0    12764 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/evaluator.py
--rw-r--r--   0        0        0      159 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/fairness/__init__.py
--rw-r--r--   0        0        0     1104 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/fairness/config.py
--rw-r--r--   0        0        0    37043 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/fairness/evaluator.py
--rw-r--r--   0        0        0     1837 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0    13476 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0    13702 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/auroc.py
--rw-r--r--   0        0        0     4899 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/average_precision.py
--rw-r--r--   0        0        0     2484 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/__init__.py
--rw-r--r--   0        0        0     7774 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/_stat_scores.py
--rw-r--r--   0        0        0     7217 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/accuracy.py
--rw-r--r--   0        0        0    11290 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/auroc.py
--rw-r--r--   0        0        0    11136 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/average_precision.py
--rw-r--r--   0        0        0    12934 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/confusion_matrix.py
--rw-r--r--   0        0        0     1349 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
--rw-r--r--   0        0        0     2066 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
--rw-r--r--   0        0        0     3491 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
--rw-r--r--   0        0        0     1062 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
--rw-r--r--   0        0        0     3916 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
--rw-r--r--   0        0        0    17182 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/f_score.py
--rw-r--r--   0        0        0     2614 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/__init__.py
--rw-r--r--   0        0        0    17136 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
--rw-r--r--   0        0        0    17396 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/accuracy.py
--rw-r--r--   0        0        0    25070 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/auroc.py
--rw-r--r--   0        0        0    26707 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/average_precision.py
--rw-r--r--   0        0        0    27926 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
--rw-r--r--   0        0        0    34008 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/f_score.py
--rw-r--r--   0        0        0     2631 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mae.py
--rw-r--r--   0        0        0     3551 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mape.py
--rw-r--r--   0        0        0    12394 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
--rw-r--r--   0        0        0     4101 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mse.py
--rw-r--r--   0        0        0    16833 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
--rw-r--r--   0        0        0    32246 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
--rw-r--r--   0        0        0    45990 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    25481 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/roc.py
--rw-r--r--   0        0        0     3612 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/smape.py
--rw-r--r--   0        0        0    16929 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/specificity.py
--rw-r--r--   0        0        0     3253 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/wmape.py
--rw-r--r--   0        0        0     1858 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mae.py
--rw-r--r--   0        0        0     2498 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mape.py
--rw-r--r--   0        0        0     6089 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
--rw-r--r--   0        0        0    26623 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric.py
--rw-r--r--   0        0        0    22036 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric_dict.py
--rw-r--r--   0        0        0     3290 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mse.py
--rw-r--r--   0        0        0     7802 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
--rw-r--r--   0        0        0    33336 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall.py
--rw-r--r--   0        0        0    19586 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
--rw-r--r--   0        0        0     9557 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/roc.py
--rw-r--r--   0        0        0     2597 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/smape.py
--rw-r--r--   0        0        0    13798 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/specificity.py
--rw-r--r--   0        0        0      546 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/__init__.py
--rw-r--r--   0        0        0    36009 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/ops.py
--rw-r--r--   0        0        0     9057 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/types.py
--rw-r--r--   0        0        0     4589 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/validation.py
--rw-r--r--   0        0        0     2727 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/wmape.py
--rw-r--r--   0        0        0    26187 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/f_beta.py
--rw-r--r--   0        0        0     1815 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/factory.py
--rw-r--r--   0        0        0     1933 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/__init__.py
--rw-r--r--   0        0        0    16824 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/accuracy.py
--rw-r--r--   0        0        0    22142 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/auroc.py
--rw-r--r--   0        0        0     5544 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/average_precision.py
--rw-r--r--   0        0        0    26687 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/f_beta.py
--rw-r--r--   0        0        0    27455 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall.py
--rw-r--r--   0        0        0    37364 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    21633 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/roc.py
--rw-r--r--   0        0        0    11342 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/sensitivity.py
--rw-r--r--   0        0        0    16029 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/specificity.py
--rw-r--r--   0        0        0    26592 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/stat_scores.py
--rw-r--r--   0        0        0    32052 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/metric.py
--rw-r--r--   0        0        0    26995 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall.py
--rw-r--r--   0        0        0    23073 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall_curve.py
--rw-r--r--   0        0        0    13622 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/roc.py
--rw-r--r--   0        0        0    12350 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/sensitivity.py
--rw-r--r--   0        0        0    14376 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/specificity.py
--rw-r--r--   0        0        0    16991 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/stat_scores.py
--rw-r--r--   0        0        0    10157 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/utils.py
--rw-r--r--   0        0        0     5784 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/utils.py
--rw-r--r--   0        0        0     1658 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/__init__.py
--rw-r--r--   0        0        0     7660 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/catalog.py
--rw-r--r--   0        0        0      727 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/densenet.yaml
--rw-r--r--   0        0        0      647 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/gru.yaml
--rw-r--r--   0        0        0       34 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/logistic_regression.yaml
--rw-r--r--   0        0        0      647 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/lstm.yaml
--rw-r--r--   0        0        0      117 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/mlp_classifier.yaml
--rw-r--r--   0        0        0      577 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/mlp_pt.yaml
--rw-r--r--   0        0        0      512 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/resnet.yaml
--rw-r--r--   0        0        0       53 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/rf_classifier.yaml
--rw-r--r--   0        0        0      590 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/rnn.yaml
--rw-r--r--   0        0        0       91 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/sgd_classifier.yaml
--rw-r--r--   0        0        0      180 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/configs/xgb_classifier.yaml
--rw-r--r--   0        0        0     1791 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/data.py
--rw-r--r--   0        0        0      266 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/__init__.py
--rw-r--r--   0        0        0     2226 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/gru.py
--rw-r--r--   0        0        0     2436 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/lstm.py
--rw-r--r--   0        0        0     3013 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/mlp.py
--rw-r--r--   0        0        0     2214 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/rnn.py
--rw-r--r--   0        0        0     2588 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/plotter.py
--rw-r--r--   0        0        0     7238 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/torch_utils.py
--rw-r--r--   0        0        0     4371 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/utils.py
--rw-r--r--   0        0        0      372 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/__init__.py
--rw-r--r--   0        0        0    10026 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/base.py
--rw-r--r--   0        0        0    49399 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/pt_model.py
--rw-r--r--   0        0        0    39985 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/sk_model.py
--rw-r--r--   0        0        0     9899 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/utils.py
--rw-r--r--   0        0        0      468 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/__init__.py
--rw-r--r--   0        0        0    16172 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/clinical_applicator.py
--rw-r--r--   0        0        0    13248 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/detector.py
--rw-r--r--   0        0        0     2554 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/explainer.py
--rw-r--r--   0        0        0    13859 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/plotter.py
--rw-r--r--   0        0        0     9566 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/reductor.py
--rw-r--r--   0        0        0     9118 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/synthetic_applicator.py
--rw-r--r--   0        0        0    37496 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/tester.py
--rw-r--r--   0        0        0    18561 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/utils.py
--rw-r--r--   0        0        0       81 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/__init__.py
--rw-r--r--   0        0        0      100 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/__init__.py
--rw-r--r--   0        0        0     6005 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/base.py
--rw-r--r--   0        0        0    18872 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/fields.py
--rw-r--r--   0        0        0     3054 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/model_card.py
--rw-r--r--   0        0        0     6166 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/sections.py
--rw-r--r--   0        0        0       37 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/__init__.py
--rw-r--r--   0        0        0     3275 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/base.py
--rw-r--r--   0        0        0    47331 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/classification.py
--rw-r--r--   0        0        0     5463 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/utils.py
--rw-r--r--   0        0        0    39651 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/report.py
--rw-r--r--   0        0        0     1828 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/button.js
--rw-r--r--   0        0        0    15741 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/macros.jinja
--rw-r--r--   0        0        0    14849 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/model_report.jinja
--rw-r--r--   0        0        0    30509 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/plot.js
--rw-r--r--   0        0        0    33209 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/utils.py
--rw-r--r--   0        0        0      143 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/__init__.py
--rw-r--r--   0        0        0     7447 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/base.py
--rw-r--r--   0        0        0    22644 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/classification.py
--rw-r--r--   0        0        0     4211 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/utils.py
--rw-r--r--   0        0        0       23 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/__init__.py
--rw-r--r--   0        0        0     4966 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/common.py
--rw-r--r--   0        0        0    10240 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/file.py
--rw-r--r--   0        0        0     2423 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/index.py
--rw-r--r--   0        0        0     3611 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/log.py
--rw-r--r--   0        0        0     2294 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/optional.py
--rw-r--r--   0        0        0     5571 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/plot.py
--rw-r--r--   0        0        0      874 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/profile.py
--rw-r--r--   0        0        0     6427 2024-05-15 14:17:57.643941 pycyclops-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 pycyclops-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-06-03 12:49:09.934249 pycyclops-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0     6440 2024-06-03 12:49:09.934249 pycyclops-0.2.9/README.md
+-rw-r--r--   0        0        0      409 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/__init__.py
+-rw-r--r--   0        0        0      192 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/__init__.py
+-rw-r--r--   0        0        0    25741 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/aggregate.py
+-rw-r--r--   0        0        0     4344 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/clean.py
+-rw-r--r--   0        0        0     3469 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/constants.py
+-rw-r--r--   0        0        0       39 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/df/__init__.py
+-rw-r--r--   0        0        0    26086 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/df/feature.py
+-rw-r--r--   0        0        0    26167 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/df/handle_types.py
+-rw-r--r--   0        0        0    17267 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/df/normalize.py
+-rw-r--r--   0        0        0    12116 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/df/split.py
+-rw-r--r--   0        0        0    30368 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/df/vectorized.py
+-rw-r--r--   0        0        0     3295 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/diagnoses.py
+-rw-r--r--   0        0        0      118 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/features/__init__.py
+-rw-r--r--   0        0        0     9640 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/features/medical_image.py
+-rw-r--r--   0        0        0    17072 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/impute.py
+-rw-r--r--   0        0        0     3228 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/loader.py
+-rw-r--r--   0        0        0      638 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/packaged_loading_scripts/__init__.py
+-rw-r--r--   0        0        0       36 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
+-rw-r--r--   0        0        0     2110 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
+-rw-r--r--   0        0        0      881 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/preprocess.py
+-rw-r--r--   0        0        0    35496 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/slicer.py
+-rw-r--r--   0        0        0     6471 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/string_ops.py
+-rw-r--r--   0        0        0     3027 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/transforms.py
+-rw-r--r--   0        0        0    10934 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/data/utils.py
+-rw-r--r--   0        0        0      139 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/__init__.py
+-rw-r--r--   0        0        0    12803 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/evaluator.py
+-rw-r--r--   0        0        0      159 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/fairness/__init__.py
+-rw-r--r--   0        0        0     1104 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/fairness/config.py
+-rw-r--r--   0        0        0    37237 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/fairness/evaluator.py
+-rw-r--r--   0        0        0     1837 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0    13476 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0    13702 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/auroc.py
+-rw-r--r--   0        0        0     4899 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/average_precision.py
+-rw-r--r--   0        0        0     2484 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/__init__.py
+-rw-r--r--   0        0        0     7774 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/_stat_scores.py
+-rw-r--r--   0        0        0     7217 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/accuracy.py
+-rw-r--r--   0        0        0    11290 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/auroc.py
+-rw-r--r--   0        0        0    11136 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/average_precision.py
+-rw-r--r--   0        0        0    12934 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/confusion_matrix.py
+-rw-r--r--   0        0        0     1349 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
+-rw-r--r--   0        0        0     2066 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
+-rw-r--r--   0        0        0     3491 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
+-rw-r--r--   0        0        0     1062 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
+-rw-r--r--   0        0        0     3916 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
+-rw-r--r--   0        0        0    17182 2024-06-03 12:49:09.938249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/f_score.py
+-rw-r--r--   0        0        0     2614 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/__init__.py
+-rw-r--r--   0        0        0    17136 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
+-rw-r--r--   0        0        0    17396 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/accuracy.py
+-rw-r--r--   0        0        0    25070 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/auroc.py
+-rw-r--r--   0        0        0    26707 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/average_precision.py
+-rw-r--r--   0        0        0    27926 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
+-rw-r--r--   0        0        0    34008 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/f_score.py
+-rw-r--r--   0        0        0     2631 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/mae.py
+-rw-r--r--   0        0        0     3551 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/mape.py
+-rw-r--r--   0        0        0    12394 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
+-rw-r--r--   0        0        0     4101 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/mse.py
+-rw-r--r--   0        0        0    16833 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
+-rw-r--r--   0        0        0    32246 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
+-rw-r--r--   0        0        0    45990 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    25481 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/roc.py
+-rw-r--r--   0        0        0     3612 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/smape.py
+-rw-r--r--   0        0        0    16929 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/specificity.py
+-rw-r--r--   0        0        0     3253 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/wmape.py
+-rw-r--r--   0        0        0     1858 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/mae.py
+-rw-r--r--   0        0        0     2498 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/mape.py
+-rw-r--r--   0        0        0     6089 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
+-rw-r--r--   0        0        0    26651 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/metric.py
+-rw-r--r--   0        0        0    22025 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/metric_dict.py
+-rw-r--r--   0        0        0     3290 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/mse.py
+-rw-r--r--   0        0        0     7802 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
+-rw-r--r--   0        0        0    33336 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/precision_recall.py
+-rw-r--r--   0        0        0    19586 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
+-rw-r--r--   0        0        0     9557 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/roc.py
+-rw-r--r--   0        0        0     2597 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/smape.py
+-rw-r--r--   0        0        0    13798 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/specificity.py
+-rw-r--r--   0        0        0      546 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/__init__.py
+-rw-r--r--   0        0        0    36009 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/ops.py
+-rw-r--r--   0        0        0     9057 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/types.py
+-rw-r--r--   0        0        0     4589 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/validation.py
+-rw-r--r--   0        0        0     2727 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/wmape.py
+-rw-r--r--   0        0        0    26187 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/f_beta.py
+-rw-r--r--   0        0        0     1815 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/factory.py
+-rw-r--r--   0        0        0     1933 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/__init__.py
+-rw-r--r--   0        0        0    16824 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/accuracy.py
+-rw-r--r--   0        0        0    22142 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/auroc.py
+-rw-r--r--   0        0        0     5544 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/average_precision.py
+-rw-r--r--   0        0        0    26687 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/f_beta.py
+-rw-r--r--   0        0        0    27455 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/precision_recall.py
+-rw-r--r--   0        0        0    37364 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    21633 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/roc.py
+-rw-r--r--   0        0        0    11342 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/sensitivity.py
+-rw-r--r--   0        0        0    16029 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/specificity.py
+-rw-r--r--   0        0        0    26592 2024-06-03 12:49:09.942249 pycyclops-0.2.9/cyclops/evaluate/metrics/functional/stat_scores.py
+-rw-r--r--   0        0        0    32052 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/metric.py
+-rw-r--r--   0        0        0    26995 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/precision_recall.py
+-rw-r--r--   0        0        0    23073 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/precision_recall_curve.py
+-rw-r--r--   0        0        0    13622 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/roc.py
+-rw-r--r--   0        0        0    12350 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/sensitivity.py
+-rw-r--r--   0        0        0    14376 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/specificity.py
+-rw-r--r--   0        0        0    16991 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/stat_scores.py
+-rw-r--r--   0        0        0    10157 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/metrics/utils.py
+-rw-r--r--   0        0        0     5784 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/evaluate/utils.py
+-rw-r--r--   0        0        0     1658 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/__init__.py
+-rw-r--r--   0        0        0     7660 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/catalog.py
+-rw-r--r--   0        0        0      727 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/densenet.yaml
+-rw-r--r--   0        0        0      647 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/gru.yaml
+-rw-r--r--   0        0        0       34 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/logistic_regression.yaml
+-rw-r--r--   0        0        0      647 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/lstm.yaml
+-rw-r--r--   0        0        0      117 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/mlp_classifier.yaml
+-rw-r--r--   0        0        0      577 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/mlp_pt.yaml
+-rw-r--r--   0        0        0      512 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/resnet.yaml
+-rw-r--r--   0        0        0       53 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/rf_classifier.yaml
+-rw-r--r--   0        0        0      590 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/rnn.yaml
+-rw-r--r--   0        0        0       91 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/sgd_classifier.yaml
+-rw-r--r--   0        0        0      180 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/configs/xgb_classifier.yaml
+-rw-r--r--   0        0        0     1791 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/data.py
+-rw-r--r--   0        0        0      266 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/neural_nets/__init__.py
+-rw-r--r--   0        0        0     2226 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/neural_nets/gru.py
+-rw-r--r--   0        0        0     2436 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/neural_nets/lstm.py
+-rw-r--r--   0        0        0     3013 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/neural_nets/mlp.py
+-rw-r--r--   0        0        0     2214 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/neural_nets/rnn.py
+-rw-r--r--   0        0        0     2588 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/plotter.py
+-rw-r--r--   0        0        0     7238 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/torch_utils.py
+-rw-r--r--   0        0        0     4371 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/utils.py
+-rw-r--r--   0        0        0      372 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/wrappers/__init__.py
+-rw-r--r--   0        0        0    10026 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/wrappers/base.py
+-rw-r--r--   0        0        0    49399 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/wrappers/pt_model.py
+-rw-r--r--   0        0        0    39985 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/wrappers/sk_model.py
+-rw-r--r--   0        0        0     9899 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/models/wrappers/utils.py
+-rw-r--r--   0        0        0      468 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/__init__.py
+-rw-r--r--   0        0        0    16172 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/clinical_applicator.py
+-rw-r--r--   0        0        0    13248 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/detector.py
+-rw-r--r--   0        0        0     2554 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/explainer.py
+-rw-r--r--   0        0        0    13859 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/plotter.py
+-rw-r--r--   0        0        0     9566 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/reductor.py
+-rw-r--r--   0        0        0     9118 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/synthetic_applicator.py
+-rw-r--r--   0        0        0    37496 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/tester.py
+-rw-r--r--   0        0        0    18561 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/monitor/utils.py
+-rw-r--r--   0        0        0       81 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/__init__.py
+-rw-r--r--   0        0        0      100 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/model_card/__init__.py
+-rw-r--r--   0        0        0     6005 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/model_card/base.py
+-rw-r--r--   0        0        0    18872 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/model_card/fields.py
+-rw-r--r--   0        0        0     3054 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/model_card/model_card.py
+-rw-r--r--   0        0        0     6166 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/model_card/sections.py
+-rw-r--r--   0        0        0       37 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/plot/__init__.py
+-rw-r--r--   0        0        0     3275 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/plot/base.py
+-rw-r--r--   0        0        0    47331 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/plot/classification.py
+-rw-r--r--   0        0        0     5463 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/plot/utils.py
+-rw-r--r--   0        0        0    39651 2024-06-03 12:49:09.946249 pycyclops-0.2.9/cyclops/report/report.py
+-rw-r--r--   0        0        0     1828 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/report/templates/model_report/button.js
+-rw-r--r--   0        0        0    15741 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/report/templates/model_report/macros.jinja
+-rw-r--r--   0        0        0    14849 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/report/templates/model_report/model_report.jinja
+-rw-r--r--   0        0        0    30509 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/report/templates/model_report/plot.js
+-rw-r--r--   0        0        0    33209 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/report/utils.py
+-rw-r--r--   0        0        0      143 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/tasks/__init__.py
+-rw-r--r--   0        0        0     7447 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/tasks/base.py
+-rw-r--r--   0        0        0    22644 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/tasks/classification.py
+-rw-r--r--   0        0        0     4211 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/tasks/utils.py
+-rw-r--r--   0        0        0       23 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/__init__.py
+-rw-r--r--   0        0        0     4966 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/common.py
+-rw-r--r--   0        0        0    10240 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/file.py
+-rw-r--r--   0        0        0     2423 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/index.py
+-rw-r--r--   0        0        0     3611 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/log.py
+-rw-r--r--   0        0        0     2294 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/optional.py
+-rw-r--r--   0        0        0     5571 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/plot.py
+-rw-r--r--   0        0        0      874 2024-06-03 12:49:09.950249 pycyclops-0.2.9/cyclops/utils/profile.py
+-rw-r--r--   0        0        0     6465 2024-06-03 12:49:09.958249 pycyclops-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     8884 1970-01-01 00:00:00.000000 pycyclops-0.2.9/PKG-INFO
```

### Comparing `pycyclops-0.2.8/LICENSE.md` & `pycyclops-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/README.md` & `pycyclops-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/aggregate.py` & `pycyclops-0.2.9/cyclops/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/clean.py` & `pycyclops-0.2.9/cyclops/data/clean.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/constants.py` & `pycyclops-0.2.9/cyclops/data/constants.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/df/feature.py` & `pycyclops-0.2.9/cyclops/data/df/feature.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/df/handle_types.py` & `pycyclops-0.2.9/cyclops/data/df/handle_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
 
     unique.sort()
 
     map_dict: Dict[Any, int] = {}
     for i, unique_val in enumerate(unique):
         map_dict[unique_val] = i
 
-    series = series.replace(map_dict)
+    series = series.map(map_dict)
 
     inv_map = {v: k for k, v in map_dict.items()}
     meta = {FEATURE_MAPPING_ATTR: inv_map}
 
     return series, meta
```

### Comparing `pycyclops-0.2.8/cyclops/data/df/normalize.py` & `pycyclops-0.2.9/cyclops/data/df/normalize.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/df/split.py` & `pycyclops-0.2.9/cyclops/data/df/split.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/df/vectorized.py` & `pycyclops-0.2.9/cyclops/data/df/vectorized.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import copy
 import logging
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
+import pandas as pd
 
 from cyclops.data.df.normalize import VectorizedNormalizer
 from cyclops.data.df.split import split_idx
 from cyclops.data.impute import np_fill_null_num
 from cyclops.utils.common import list_swap
 from cyclops.utils.file import save_array
 from cyclops.utils.index import take_indices_over_axis
@@ -187,15 +188,19 @@
         if len(axis_names) != data.ndim:
             raise ValueError(
                 "Number of array axes and the number of axis names do not match.",
             )
         if not all(isinstance(name, str) for name in axis_names):
             raise ValueError("Axis names must be strings.")
         for i, index in enumerate(indexes):
-            if not isinstance(index, list) and not isinstance(index, np.ndarray):
+            if (
+                not isinstance(index, list)
+                and not pd.api.types.is_string_dtype(index)
+                and not isinstance(index, np.ndarray)
+            ):
                 raise ValueError("Indexes must be a list of list or numpy.ndarray.")
 
             index_ = np.array(index)
             if len(index_) != data.shape[i]:
                 raise ValueError(
                     (
                         f"Axis {i} index has {len(index_)} elements, "
```

### Comparing `pycyclops-0.2.8/cyclops/data/diagnoses.py` & `pycyclops-0.2.9/cyclops/data/diagnoses.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/features/medical_image.py` & `pycyclops-0.2.9/cyclops/data/features/medical_image.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/impute.py` & `pycyclops-0.2.9/cyclops/data/impute.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/loader.py` & `pycyclops-0.2.9/cyclops/data/loader.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/__init__.py` & `pycyclops-0.2.9/cyclops/data/packaged_loading_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py` & `pycyclops-0.2.9/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/preprocess.py` & `pycyclops-0.2.9/cyclops/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/slicer.py` & `pycyclops-0.2.9/cyclops/data/slicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functions and classes for creating subsets of Hugging Face datasets."""
 
 import copy
 import datetime
 import itertools
+import json
 from dataclasses import dataclass, field
 from functools import partial
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
@@ -244,14 +245,27 @@
         else:
             raise ValueError(
                 "Expected `intersections` to be a list of tuples or an integer. "
                 f"Got {self.intersections} instead.",
             )
         self.spec_list.extend(intersect_list)
 
+        # remove duplicates
+        seen = set()
+        result = []
+
+        for spec in self.spec_list:
+            spec_str = json.dumps(spec, sort_keys=True)
+            if spec_str not in seen:
+                seen.add(spec_str)
+                result.append(spec)
+
+        seen.clear()
+        self.spec_list = result
+
     def _parse_and_register_slice_specs(
         self,
         slice_spec: Dict[str, Dict[str, Any]],
     ) -> None:
         """Construct and register a slice functions from slice specifications."""
         if not isinstance(slice_spec, dict):
             raise TypeError(
```

### Comparing `pycyclops-0.2.8/cyclops/data/string_ops.py` & `pycyclops-0.2.9/cyclops/data/string_ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/transforms.py` & `pycyclops-0.2.9/cyclops/data/transforms.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/data/utils.py` & `pycyclops-0.2.9/cyclops/data/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/evaluator.py` & `pycyclops-0.2.9/cyclops/evaluate/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,17 @@
 
         fairness_config.dataset = dataset
         fairness_config.target_columns = target_columns
         fairness_config.prediction_columns = prediction_columns
         fairness_config.batch_size = batch_size
         fairness_config.remove_columns = ignore_columns
 
-        fairness_results = evaluate_fairness(**asdict(fairness_config))
+        fairness_results = evaluate_fairness(
+            **asdict(fairness_config), array_lib=array_lib
+        )
         results["fairness"] = fairness_results
 
     return results
 
 
 def _load_data(
     dataset: Union[str, Dataset, DatasetDict],
@@ -300,15 +302,15 @@
                             array_lib=array_lib,
                         )
 
                         # update the metric state
                         metrics.update(targets, predictions)
 
                     metric_output = metrics.compute()
-                    metrics.reset()
+                metrics.reset()
 
                 model_name: str = "model_for_%s" % prediction_column
                 results.setdefault(model_name, {})
                 results[model_name][slice_name] = metric_output
 
         set_decode(dataset, True)  # restore decoding features
```

### Comparing `pycyclops-0.2.8/cyclops/evaluate/fairness/config.py` & `pycyclops-0.2.9/cyclops/evaluate/fairness/config.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/fairness/evaluator.py` & `pycyclops-0.2.9/cyclops/evaluate/fairness/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,14 +724,17 @@
         The prediction column.
     threshold : Union[float, List[float]], optional, default=None
         The threshold to use for the metrics.
     batch_size : int
         The batch size to use for the computation.
     metric_name : Optional[str]
         The name of the metric to compute.
+    array_lib : {"torch", "numpy, "cupy"}, default="numpy"
+        The array library to use for the metric computation. The metric results
+        will be returned in the format of `array_lib`.
 
     Returns
     -------
     Dict[str, Any]
         The computed metrics.
 
     """
```

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/__init__.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/accuracy.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/auroc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/average_precision.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/__init__.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/_stat_scores.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/accuracy.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/auroc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/average_precision.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/confusion_matrix.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/base.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/f_score.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/f_score.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/__init__.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/accuracy.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/auroc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/average_precision.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/f_score.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/f_score.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mae.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/mae.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mape.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mse.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/roc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/smape.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/specificity.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/wmape.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/functional/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mae.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/mae.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mape.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,14 +427,15 @@
                 )
             else:
                 raise TypeError(
                     f"Expected the value of state `{state_name}` to be an array API "
                     "object or a list of array API objects. But got "
                     f"`{type(default_value)} instead.",
                 )
+        self._defaults = {}
 
         self._update_count = 0
         self._computed = None
         self._cache = None
         self._is_synced = False
 
     def clone(self) -> "Metric":
```

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric_dict.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/metric_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
                 return clone(obj)
             return deepcopy(obj)
 
         if self._groups_created and not self._state_is_copy:
             for metric_names in self._metric_groups.values():
                 base_metric = self.data[metric_names[0]]
                 for metric_name in metric_names[1:]:
-                    for state in self.data[metric_name]._defaults:
+                    for state in base_metric._defaults:
                         base_metric_state = getattr(base_metric, state)
                         setattr(
                             self.data[metric_name],
                             state,
                             deepcopy_state(base_metric_state)
                             if copy_state
                             else base_metric_state,
```

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mse.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/negative_predictive_value.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall_curve.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/roc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/smape.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/specificity.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/__init__.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/ops.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/types.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/validation.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/utils/validation.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/wmape.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/experimental/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/f_beta.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/factory.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/__init__.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/accuracy.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/auroc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/average_precision.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/f_beta.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall_curve.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/roc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/sensitivity.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/specificity.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/stat_scores.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/functional/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/metric.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall_curve.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/roc.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/sensitivity.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/specificity.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/stat_scores.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/metrics/utils.py` & `pycyclops-0.2.9/cyclops/evaluate/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/evaluate/utils.py` & `pycyclops-0.2.9/cyclops/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/__init__.py` & `pycyclops-0.2.9/cyclops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/catalog.py` & `pycyclops-0.2.9/cyclops/models/catalog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -182,20 +182,20 @@
 
     Raises
     ------
     TypeError
         If model is not a pyTorch or sklearn model.
 
     """
+    if is_sklearn_model(model):
+        return SKModel(model, **kwargs)
     if is_pytorch_model(model):
         from cyclops.models.wrappers import PTModel
 
         return PTModel(model, **kwargs)
-    if is_sklearn_model(model):
-        return SKModel(model, **kwargs)
     raise TypeError("``model`` must be a PyTorch or sklearn model")
 
 
 def create_model(
     model_name: str,
     wrap: bool = True,
     **config_overrides,
```

### Comparing `pycyclops-0.2.8/cyclops/models/configs/densenet.yaml` & `pycyclops-0.2.9/cyclops/models/configs/densenet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/configs/gru.yaml` & `pycyclops-0.2.9/cyclops/models/configs/gru.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/configs/lstm.yaml` & `pycyclops-0.2.9/cyclops/models/configs/lstm.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/configs/mlp_pt.yaml` & `pycyclops-0.2.9/cyclops/models/configs/mlp_pt.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/configs/resnet.yaml` & `pycyclops-0.2.9/cyclops/models/configs/resnet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/configs/rnn.yaml` & `pycyclops-0.2.9/cyclops/models/configs/rnn.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/data.py` & `pycyclops-0.2.9/cyclops/models/data.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/neural_nets/gru.py` & `pycyclops-0.2.9/cyclops/models/neural_nets/gru.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/neural_nets/lstm.py` & `pycyclops-0.2.9/cyclops/models/neural_nets/lstm.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/neural_nets/mlp.py` & `pycyclops-0.2.9/cyclops/models/neural_nets/mlp.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/neural_nets/rnn.py` & `pycyclops-0.2.9/cyclops/models/neural_nets/rnn.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/plotter.py` & `pycyclops-0.2.9/cyclops/models/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/torch_utils.py` & `pycyclops-0.2.9/cyclops/models/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/utils.py` & `pycyclops-0.2.9/cyclops/models/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/wrappers/base.py` & `pycyclops-0.2.9/cyclops/models/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/wrappers/pt_model.py` & `pycyclops-0.2.9/cyclops/models/wrappers/pt_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/wrappers/sk_model.py` & `pycyclops-0.2.9/cyclops/models/wrappers/sk_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/models/wrappers/utils.py` & `pycyclops-0.2.9/cyclops/models/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/clinical_applicator.py` & `pycyclops-0.2.9/cyclops/monitor/clinical_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/detector.py` & `pycyclops-0.2.9/cyclops/monitor/detector.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/explainer.py` & `pycyclops-0.2.9/cyclops/monitor/explainer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/plotter.py` & `pycyclops-0.2.9/cyclops/monitor/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/reductor.py` & `pycyclops-0.2.9/cyclops/monitor/reductor.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/synthetic_applicator.py` & `pycyclops-0.2.9/cyclops/monitor/synthetic_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/tester.py` & `pycyclops-0.2.9/cyclops/monitor/tester.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/monitor/utils.py` & `pycyclops-0.2.9/cyclops/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/model_card/base.py` & `pycyclops-0.2.9/cyclops/report/model_card/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/model_card/fields.py` & `pycyclops-0.2.9/cyclops/report/model_card/fields.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/model_card/model_card.py` & `pycyclops-0.2.9/cyclops/report/model_card/model_card.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/model_card/sections.py` & `pycyclops-0.2.9/cyclops/report/model_card/sections.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/plot/base.py` & `pycyclops-0.2.9/cyclops/report/plot/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/plot/classification.py` & `pycyclops-0.2.9/cyclops/report/plot/classification.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/plot/utils.py` & `pycyclops-0.2.9/cyclops/report/plot/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/report.py` & `pycyclops-0.2.9/cyclops/report/report.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/templates/model_report/button.js` & `pycyclops-0.2.9/cyclops/report/templates/model_report/button.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/templates/model_report/macros.jinja` & `pycyclops-0.2.9/cyclops/report/templates/model_report/macros.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/templates/model_report/model_report.jinja` & `pycyclops-0.2.9/cyclops/report/templates/model_report/model_report.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/templates/model_report/plot.js` & `pycyclops-0.2.9/cyclops/report/templates/model_report/plot.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/report/utils.py` & `pycyclops-0.2.9/cyclops/report/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/tasks/base.py` & `pycyclops-0.2.9/cyclops/tasks/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/tasks/classification.py` & `pycyclops-0.2.9/cyclops/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/tasks/utils.py` & `pycyclops-0.2.9/cyclops/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/utils/common.py` & `pycyclops-0.2.9/cyclops/utils/common.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/utils/file.py` & `pycyclops-0.2.9/cyclops/utils/file.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/utils/index.py` & `pycyclops-0.2.9/cyclops/utils/index.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/utils/log.py` & `pycyclops-0.2.9/cyclops/utils/log.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/utils/optional.py` & `pycyclops-0.2.9/cyclops/utils/optional.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/utils/plot.py` & `pycyclops-0.2.9/cyclops/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/cyclops/utils/profile.py` & `pycyclops-0.2.9/cyclops/utils/profile.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.8/pyproject.toml` & `pycyclops-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pycyclops"
-version = "0.2.8"
+version = "0.2.9"
 description = "Framework for healthcare ML implementation"
 authors = ["Vector AI Engineering <cyclops@vectorinstitute.ai>"]
 license = "Apache-2.0"
 repository = "https://github.com/VectorInstitute/cyclops"
 documentation = "https://vectorinstitute.github.io/cyclops/"
 packages = [
     { include = "cyclops" },
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
-pandas = "^2.0"
+pandas = {version = "^2.1", extras = ["performance"]}
 numpy = "^1.24.0"
 scikit-learn = "^1.4.0"
 scipy = "^1.11.0"
 matplotlib = "^3.8.3"
 datasets = "^2.15.0"
 psutil = "^5.9.4"
 pyarrow = "^14.0.0"
```

### Comparing `pycyclops-0.2.8/PKG-INFO` & `pycyclops-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycyclops
-Version: 0.2.8
+Version: 0.2.9
 Summary: Framework for healthcare ML implementation
 Home-page: https://github.com/VectorInstitute/cyclops
 License: Apache-2.0
 Author: Vector AI Engineering
 Author-email: cyclops@vectorinstitute.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,15 +27,15 @@
 Requires-Dist: datasets (>=2.15.0,<3.0.0)
 Requires-Dist: hydra-core (>=1.2.0,<2.0.0)
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: llvmlite (>=0.40.0,<0.41.0) ; extra == "alibi" or extra == "alibi-detect" or extra == "all"
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: monai[itk] (>=1.3.0,<2.0.0) ; extra == "monai" or extra == "all"
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: pandas[performance] (>=2.1,<3.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: plotly (>=5.7.0,<6.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pyarrow (>=14.0.0,<15.0.0)
 Requires-Dist: pybtex (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.0,<2.0.0)
```

