# Comparing `tmp/squlearn-0.7.3.tar.gz` & `tmp/squlearn-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squlearn-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "squlearn-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `squlearn-0.7.3.tar` & `squlearn-0.7.4.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0     5514 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2187 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      487 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      532 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/workflows/doc_checks.yml
--rw-r--r--   0        0        0      564 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/workflows/format.yml
--rw-r--r--   0        0        0      679 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1717 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0      630 2024-05-17 08:00:50.936596 squlearn-0.7.3/.github/workflows/tests.yaml
--rw-r--r--   0        0        0     3314 2024-05-17 08:00:50.936596 squlearn-0.7.3/.gitignore
--rw-r--r--   0        0        0     1599 2024-05-17 08:00:50.936596 squlearn-0.7.3/CITATION.cff
--rw-r--r--   0        0        0    11421 2024-05-17 08:00:50.936596 squlearn-0.7.3/LICENSE.txt
--rw-r--r--   0        0        0     3440 2024-05-17 08:00:50.936596 squlearn-0.7.3/README.md
--rw-r--r--   0        0        0      632 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/Makefile
--rw-r--r--   0        0        0      278 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/README.md
--rw-r--r--   0        0        0     4126 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/_static/css/custom.css
--rw-r--r--   0        0        0     2249 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/_static/favicon.png
--rw-r--r--   0        0        0    12664 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/_static/logo.png
--rw-r--r--   0        0        0    44296 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/_static/qnn/qnn.svg
--rw-r--r--   0        0        0    36032 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/_static/schematic.png
--rw-r--r--   0        0        0   121611 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/_static/util/executor.png
--rw-r--r--   0        0        0      161 2024-05-17 08:00:50.936596 squlearn-0.7.3/docs/_templates/class.rst
--rw-r--r--   0        0        0      486 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/_templates/class_with_call.rst
--rw-r--r--   0        0        0      165 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/_templates/function.rst
--rw-r--r--   0        0        0     3568 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/conf.py
--rw-r--r--   0        0        0      146 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/examples/example_kernel_digit_classification.nblink
--rw-r--r--   0        0        0       67 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/examples/example_kernel_grid_search.nblink
--rw-r--r--   0        0        0      142 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/examples/example_qnn_backend_mitigation.nblink
--rw-r--r--   0        0        0      148 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/examples/example_quantum_bayesian_optimization.nblink
--rw-r--r--   0        0        0      223 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/examples/examples_index.rst
--rw-r--r--   0        0        0      524 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/index.rst
--rw-r--r--   0        0        0      940 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/install/install.rst
--rw-r--r--   0        0        0     1018 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/make.bat
--rw-r--r--   0        0        0     5784 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/modules/classes.rst
--rw-r--r--   0        0        0       60 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/qiskit_settings.conf
--rw-r--r--   0        0        0      144 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/requirements.txt
--rw-r--r--   0        0        0      461 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0    10216 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/user_guide/encoding_circuits.rst
--rw-r--r--   0        0        0    13519 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/user_guide/executor.rst
--rw-r--r--   0        0        0    15401 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/user_guide/kernel_methods.rst
--rw-r--r--   0        0        0     6098 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/user_guide/observables.rst
--rw-r--r--   0        0        0    18179 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/user_guide/quantum_neural_networks.rst
--rw-r--r--   0        0        0      165 2024-05-17 08:00:50.940596 squlearn-0.7.3/docs/user_guide/user_guide_index.rst
--rw-r--r--   0        0        0    96711 2024-05-17 08:00:50.940596 squlearn-0.7.3/examples/encoding_circuits/layered_encoding_circuit.ipynb
--rw-r--r--   0        0        0    32387 2024-05-17 08:00:50.940596 squlearn-0.7.3/examples/encoding_circuits/pruning_example.ipynb
--rw-r--r--   0        0        0   552422 2024-05-17 08:00:50.944596 squlearn-0.7.3/examples/encoding_circuits/various_encoding_circuit.ipynb
--rw-r--r--   0        0        0     9791 2024-05-17 08:00:50.944596 squlearn-0.7.3/examples/executor/example_executor_qiskit.ipynb
--rw-r--r--   0        0        0     7553 2024-05-17 08:00:50.944596 squlearn-0.7.3/examples/integration/mlflow.ipynb
--rw-r--r--   0        0        0    40419 2024-05-17 08:00:50.944596 squlearn-0.7.3/examples/kernel/example_fidelity_kernel.ipynb
--rw-r--r--   0        0        0   392223 2024-05-17 08:00:50.944596 squlearn-0.7.3/examples/kernel/example_projected_kernel.ipynb
--rw-r--r--   0        0        0    57347 2024-05-17 08:00:50.944596 squlearn-0.7.3/examples/kernel/example_regularization_mitigation.ipynb
--rw-r--r--   0        0        0   132621 2024-05-17 08:00:50.948596 squlearn-0.7.3/examples/kernel/qgpc_workflow.ipynb
--rw-r--r--   0        0        0    64202 2024-05-17 08:00:50.948596 squlearn-0.7.3/examples/kernel/qgpr_optimization_workflow.ipynb
--rw-r--r--   0        0        0    64741 2024-05-17 08:00:50.948596 squlearn-0.7.3/examples/kernel/qgpr_workflow.ipynb
--rw-r--r--   0        0        0    96580 2024-05-17 08:00:50.948596 squlearn-0.7.3/examples/qnn/classification_example.ipynb
--rw-r--r--   0        0        0    75008 2024-05-17 08:00:50.948596 squlearn-0.7.3/examples/qnn/example_adam.ipynb
--rw-r--r--   0        0        0    76093 2024-05-17 08:00:50.948596 squlearn-0.7.3/examples/qnn/example_minibatch.ipynb
--rw-r--r--   0        0        0   530356 2024-05-17 08:00:50.952597 squlearn-0.7.3/examples/qnn/example_qcnn_encoding_circuit.ipynb
--rw-r--r--   0        0        0   220203 2024-05-17 08:00:50.952597 squlearn-0.7.3/examples/qnn/regression_example.ipynb
--rw-r--r--   0        0        0   194050 2024-05-17 08:00:50.952597 squlearn-0.7.3/examples/qnn/regression_with_variance.ipynb
--rw-r--r--   0        0        0   147762 2024-05-17 08:00:50.956596 squlearn-0.7.3/examples/tutorials/images/encoding_circuit.png
--rw-r--r--   0        0        0    30308 2024-05-17 08:00:50.956596 squlearn-0.7.3/examples/tutorials/images/pipeline.png
--rw-r--r--   0        0        0    97978 2024-05-17 08:00:50.956596 squlearn-0.7.3/examples/tutorials/images/projected_quantum_kernel.png
--rw-r--r--   0        0        0   157564 2024-05-17 08:00:50.956596 squlearn-0.7.3/examples/tutorials/images/quantum_bo.png
--rw-r--r--   0        0        0   503838 2024-05-17 08:00:50.960596 squlearn-0.7.3/examples/tutorials/kernel_digit_classification.ipynb
--rw-r--r--   0        0        0   244971 2024-05-17 08:00:50.960596 squlearn-0.7.3/examples/tutorials/kernel_grid_search.ipynb
--rw-r--r--   0        0        0    90619 2024-05-17 08:00:50.960596 squlearn-0.7.3/examples/tutorials/kernel_regression.ipynb
--rw-r--r--   0        0        0   253985 2024-05-17 08:00:50.960596 squlearn-0.7.3/examples/tutorials/qnn_backend_mitigation.ipynb
--rw-r--r--   0        0        0   745771 2024-05-17 08:00:50.964597 squlearn-0.7.3/examples/tutorials/quantum_bayesian_optimization.ipynb
--rw-r--r--   0        0        0     2165 2024-05-17 08:00:50.964597 squlearn-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      336 2024-05-17 08:00:50.964597 squlearn-0.7.3/src/squlearn/__init__.py
--rw-r--r--   0        0        0     1455 2024-05-17 08:00:50.964597 squlearn-0.7.3/src/squlearn/encoding_circuit/__init__.py
--rw-r--r--   0        0        0        0 2024-05-17 08:00:50.964597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/__init__.py
--rw-r--r--   0        0        0     9625 2024-05-17 08:00:50.964597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py
--rw-r--r--   0        0        0     6454 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py
--rw-r--r--   0        0        0     7139 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py
--rw-r--r--   0        0        0    10302 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py
--rw-r--r--   0        0        0     6419 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py
--rw-r--r--   0        0        0     5685 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py
--rw-r--r--   0        0        0     3808 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py
--rw-r--r--   0        0        0    31845 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py
--rw-r--r--   0        0        0     8823 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py
--rw-r--r--   0        0        0     4555 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py
--rw-r--r--   0        0        0    12664 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/encoding_circuit_base.py
--rw-r--r--   0        0        0    13217 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py
--rw-r--r--   0        0        0   126131 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/layered_encoding_circuit.py
--rw-r--r--   0        0        0    12914 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/pruned_encoding_circuit.py
--rw-r--r--   0        0        0     7106 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py
--rw-r--r--   0        0        0      315 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/__init__.py
--rw-r--r--   0        0        0      161 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/matrix/__init__.py
--rw-r--r--   0        0        0    13571 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/matrix/fidelity_kernel.py
--rw-r--r--   0        0        0    12642 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py
--rw-r--r--   0        0        0    15109 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/matrix/kernel_matrix_base.py
--rw-r--r--   0        0        0     1237 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/matrix/kernel_util.py
--rw-r--r--   0        0        0    28126 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/matrix/projected_quantum_kernel.py
--rw-r--r--   0        0        0     2626 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/matrix/regularization.py
--rw-r--r--   0        0        0      168 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/ml/__init__.py
--rw-r--r--   0        0        0     5636 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/ml/qgpc.py
--rw-r--r--   0        0        0    12897 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/ml/qgpr.py
--rw-r--r--   0        0        0     9115 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/ml/qkrr.py
--rw-r--r--   0        0        0     5972 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/ml/qsvc.py
--rw-r--r--   0        0        0     5940 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/ml/qsvr.py
--rw-r--r--   0        0        0      190 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/optimization/__init__.py
--rw-r--r--   0        0        0      646 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/optimization/kernel_loss_base.py
--rw-r--r--   0        0        0     1323 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/optimization/kernel_optimization_base.py
--rw-r--r--   0        0        0     3675 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/optimization/kernel_optimizer.py
--rw-r--r--   0        0        0     2811 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/optimization/negative_log_likelihood.py
--rw-r--r--   0        0        0     2648 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/kernel/optimization/target_alignment.py
--rw-r--r--   0        0        0      579 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/__init__.py
--rw-r--r--   0        0        0    18957 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_base.py
--rw-r--r--   0        0        0    13837 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_derivatives.py
--rw-r--r--   0        0        0        0 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_implemented/__init__.py
--rw-r--r--   0        0        0     4154 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_implemented/custom_observable.py
--rw-r--r--   0        0        0     6619 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_implemented/ising_hamiltonian.py
--rw-r--r--   0        0        0     3331 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_implemented/single_pauli.py
--rw-r--r--   0        0        0     3449 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_implemented/single_probability.py
--rw-r--r--   0        0        0     4602 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_implemented/summed_paulis.py
--rw-r--r--   0        0        0     4433 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/observables/observable_implemented/summed_probabilities.py
--rw-r--r--   0        0        0      388 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/optimizers/__init__.py
--rw-r--r--   0        0        0     7904 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/optimizers/adam.py
--rw-r--r--   0        0        0     4606 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/optimizers/approximated_gradients.py
--rw-r--r--   0        0        0     2822 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/optimizers/optimizer_base.py
--rw-r--r--   0        0        0     6830 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/optimizers/optimizers_wrapper.py
--rw-r--r--   0        0        0    10576 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/optimizers/sglbo.py
--rw-r--r--   0        0        0      486 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/qnn/__init__.py
--rw-r--r--   0        0        0     8625 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/qnn/barren_plateau_analysis.py
--rw-r--r--   0        0        0    11832 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/qnn/base_qnn.py
--rw-r--r--   0        0        0    28577 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/qnn/loss.py
--rw-r--r--   0        0        0     1650 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn.py
--rw-r--r--   0        0        0     4920 2024-05-17 08:00:50.968597 squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn_base.py
--rw-r--r--   0        0        0    38214 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn_pennylane.py
--rw-r--r--   0        0        0    44856 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn_qiskit.py
--rw-r--r--   0        0        0    10283 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/qnn/qnnc.py
--rw-r--r--   0        0        0     9069 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/qnn/qnnr.py
--rw-r--r--   0        0        0    19738 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/qnn/training.py
--rw-r--r--   0        0        0       92 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/__init__.py
--rw-r--r--   0        0        0     4478 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/data_preprocessing.py
--rw-r--r--   0        0        0    73680 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/executor.py
--rw-r--r--   0        0        0      548 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/optree/__init__.py
--rw-r--r--   0        0        0    32033 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/optree/optree.py
--rw-r--r--   0        0        0    17472 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/optree/optree_derivative.py
--rw-r--r--   0        0        0    69544 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/optree/optree_evaluate.py
--rw-r--r--   0        0        0      166 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/pennylane/__init__.py
--rw-r--r--   0        0        0    26113 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/pennylane/pennylane_circuit.py
--rw-r--r--   0        0        0     1905 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/pennylane/pennylane_gates.py
--rw-r--r--   0        0        0     9208 2024-05-17 08:00:50.972597 squlearn-0.7.3/src/squlearn/util/qfi.py
--rw-r--r--   0        0        0     9207 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/encoding_circuit/test_layered_encoding_circuit.py
--rw-r--r--   0        0        0     6832 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/kernel/ml/test_qgpc.py
--rw-r--r--   0        0        0     7604 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/kernel/ml/test_qgpr.py
--rw-r--r--   0        0        0     6249 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/kernel/ml/test_qkrr.py
--rw-r--r--   0        0        0     6812 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/kernel/ml/test_qsvc.py
--rw-r--r--   0        0        0     6811 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/kernel/ml/test_qsvr.py
--rw-r--r--   0        0        0      857 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/optimizers/test_sglbo.py
--rw-r--r--   0        0        0     4953 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/qnn/test_base_qnn.py
--rw-r--r--   0        0        0     7013 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/qnn/test_qnnc.py
--rw-r--r--   0        0        0     7055 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/qnn/test_qnnr.py
--rw-r--r--   0        0        0     6768 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/qnn/test_training.py
--rw-r--r--   0        0        0     5527 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/util/optree/test_optree_derivative.py
--rw-r--r--   0        0        0     9928 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/util/optree/test_optree_evaluate.py
--rw-r--r--   0        0        0     7337 2024-05-17 08:00:50.972597 squlearn-0.7.3/tests/util/test_executor.py
--rw-r--r--   0        0        0     5664 1970-01-01 00:00:00.000000 squlearn-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     5514 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2187 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      487 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      532 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/workflows/doc_checks.yml
+-rw-r--r--   0        0        0      564 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/workflows/format.yml
+-rw-r--r--   0        0        0      679 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1717 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0      630 2024-06-03 07:52:09.443468 squlearn-0.7.4/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0     3314 2024-06-03 07:52:09.443468 squlearn-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1651 2024-06-03 07:52:09.443468 squlearn-0.7.4/CITATION.cff
+-rw-r--r--   0        0        0    11421 2024-06-03 07:52:09.443468 squlearn-0.7.4/LICENSE.txt
+-rw-r--r--   0        0        0     3440 2024-06-03 07:52:09.443468 squlearn-0.7.4/README.md
+-rw-r--r--   0        0        0      632 2024-06-03 07:52:09.443468 squlearn-0.7.4/docs/Makefile
+-rw-r--r--   0        0        0      278 2024-06-03 07:52:09.443468 squlearn-0.7.4/docs/README.md
+-rw-r--r--   0        0        0     4126 2024-06-03 07:52:09.443468 squlearn-0.7.4/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     2249 2024-06-03 07:52:09.443468 squlearn-0.7.4/docs/_static/favicon.png
+-rw-r--r--   0        0        0    12664 2024-06-03 07:52:09.443468 squlearn-0.7.4/docs/_static/logo.png
+-rw-r--r--   0        0        0    44296 2024-06-03 07:52:09.443468 squlearn-0.7.4/docs/_static/qnn/qnn.svg
+-rw-r--r--   0        0        0    36032 2024-06-03 07:52:09.443468 squlearn-0.7.4/docs/_static/schematic.png
+-rw-r--r--   0        0        0   121611 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/_static/util/executor.png
+-rw-r--r--   0        0        0      161 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/_templates/class.rst
+-rw-r--r--   0        0        0      486 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/_templates/class_with_call.rst
+-rw-r--r--   0        0        0      165 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/_templates/function.rst
+-rw-r--r--   0        0        0     3568 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/conf.py
+-rw-r--r--   0        0        0      146 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/examples/example_kernel_digit_classification.nblink
+-rw-r--r--   0        0        0       67 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/examples/example_kernel_grid_search.nblink
+-rw-r--r--   0        0        0      142 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/examples/example_qnn_backend_mitigation.nblink
+-rw-r--r--   0        0        0      148 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/examples/example_quantum_bayesian_optimization.nblink
+-rw-r--r--   0        0        0      223 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/examples/examples_index.rst
+-rw-r--r--   0        0        0      524 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/index.rst
+-rw-r--r--   0        0        0      940 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/install/install.rst
+-rw-r--r--   0        0        0     1018 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/make.bat
+-rw-r--r--   0        0        0     5784 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/modules/classes.rst
+-rw-r--r--   0        0        0       60 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/qiskit_settings.conf
+-rw-r--r--   0        0        0      144 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/requirements.txt
+-rw-r--r--   0        0        0      461 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0    10216 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/user_guide/encoding_circuits.rst
+-rw-r--r--   0        0        0    13519 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/user_guide/executor.rst
+-rw-r--r--   0        0        0    15401 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/user_guide/kernel_methods.rst
+-rw-r--r--   0        0        0     6098 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/user_guide/observables.rst
+-rw-r--r--   0        0        0    18179 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/user_guide/quantum_neural_networks.rst
+-rw-r--r--   0        0        0      165 2024-06-03 07:52:09.447468 squlearn-0.7.4/docs/user_guide/user_guide_index.rst
+-rw-r--r--   0        0        0    96711 2024-06-03 07:52:09.447468 squlearn-0.7.4/examples/encoding_circuits/layered_encoding_circuit.ipynb
+-rw-r--r--   0        0        0    32387 2024-06-03 07:52:09.447468 squlearn-0.7.4/examples/encoding_circuits/pruning_example.ipynb
+-rw-r--r--   0        0        0   552422 2024-06-03 07:52:09.451468 squlearn-0.7.4/examples/encoding_circuits/various_encoding_circuit.ipynb
+-rw-r--r--   0        0        0     9791 2024-06-03 07:52:09.451468 squlearn-0.7.4/examples/executor/example_executor_qiskit.ipynb
+-rw-r--r--   0        0        0     7553 2024-06-03 07:52:09.451468 squlearn-0.7.4/examples/integration/mlflow.ipynb
+-rw-r--r--   0        0        0    40419 2024-06-03 07:52:09.451468 squlearn-0.7.4/examples/kernel/example_fidelity_kernel.ipynb
+-rw-r--r--   0        0        0   392223 2024-06-03 07:52:09.451468 squlearn-0.7.4/examples/kernel/example_projected_kernel.ipynb
+-rw-r--r--   0        0        0    57347 2024-06-03 07:52:09.455469 squlearn-0.7.4/examples/kernel/example_regularization_mitigation.ipynb
+-rw-r--r--   0        0        0   132621 2024-06-03 07:52:09.455469 squlearn-0.7.4/examples/kernel/qgpc_workflow.ipynb
+-rw-r--r--   0        0        0    64202 2024-06-03 07:52:09.455469 squlearn-0.7.4/examples/kernel/qgpr_optimization_workflow.ipynb
+-rw-r--r--   0        0        0    64741 2024-06-03 07:52:09.455469 squlearn-0.7.4/examples/kernel/qgpr_workflow.ipynb
+-rw-r--r--   0        0        0    96580 2024-06-03 07:52:09.455469 squlearn-0.7.4/examples/qnn/classification_example.ipynb
+-rw-r--r--   0        0        0    75008 2024-06-03 07:52:09.455469 squlearn-0.7.4/examples/qnn/example_adam.ipynb
+-rw-r--r--   0        0        0    76093 2024-06-03 07:52:09.455469 squlearn-0.7.4/examples/qnn/example_minibatch.ipynb
+-rw-r--r--   0        0        0   530356 2024-06-03 07:52:09.459468 squlearn-0.7.4/examples/qnn/example_qcnn_encoding_circuit.ipynb
+-rw-r--r--   0        0        0   220203 2024-06-03 07:52:09.459468 squlearn-0.7.4/examples/qnn/regression_example.ipynb
+-rw-r--r--   0        0        0   194050 2024-06-03 07:52:09.463468 squlearn-0.7.4/examples/qnn/regression_with_variance.ipynb
+-rw-r--r--   0        0        0   147762 2024-06-03 07:52:09.463468 squlearn-0.7.4/examples/tutorials/images/encoding_circuit.png
+-rw-r--r--   0        0        0    30308 2024-06-03 07:52:09.463468 squlearn-0.7.4/examples/tutorials/images/pipeline.png
+-rw-r--r--   0        0        0    97978 2024-06-03 07:52:09.463468 squlearn-0.7.4/examples/tutorials/images/projected_quantum_kernel.png
+-rw-r--r--   0        0        0   157564 2024-06-03 07:52:09.463468 squlearn-0.7.4/examples/tutorials/images/quantum_bo.png
+-rw-r--r--   0        0        0   503838 2024-06-03 07:52:09.467468 squlearn-0.7.4/examples/tutorials/kernel_digit_classification.ipynb
+-rw-r--r--   0        0        0   244971 2024-06-03 07:52:09.467468 squlearn-0.7.4/examples/tutorials/kernel_grid_search.ipynb
+-rw-r--r--   0        0        0    90619 2024-06-03 07:52:09.467468 squlearn-0.7.4/examples/tutorials/kernel_regression.ipynb
+-rw-r--r--   0        0        0   253985 2024-06-03 07:52:09.467468 squlearn-0.7.4/examples/tutorials/qnn_backend_mitigation.ipynb
+-rw-r--r--   0        0        0   745771 2024-06-03 07:52:09.471469 squlearn-0.7.4/examples/tutorials/quantum_bayesian_optimization.ipynb
+-rw-r--r--   0        0        0     2173 2024-06-03 07:52:09.475468 squlearn-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      336 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/__init__.py
+-rw-r--r--   0        0        0     1455 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/__init__.py
+-rw-r--r--   0        0        0     9625 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py
+-rw-r--r--   0        0        0     6454 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py
+-rw-r--r--   0        0        0     7139 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py
+-rw-r--r--   0        0        0    10302 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py
+-rw-r--r--   0        0        0     6419 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py
+-rw-r--r--   0        0        0     5685 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py
+-rw-r--r--   0        0        0     3808 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py
+-rw-r--r--   0        0        0    31845 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py
+-rw-r--r--   0        0        0     8823 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py
+-rw-r--r--   0        0        0     4555 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py
+-rw-r--r--   0        0        0    12664 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/encoding_circuit_base.py
+-rw-r--r--   0        0        0    13217 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py
+-rw-r--r--   0        0        0   126131 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/layered_encoding_circuit.py
+-rw-r--r--   0        0        0    12914 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/pruned_encoding_circuit.py
+-rw-r--r--   0        0        0     7106 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py
+-rw-r--r--   0        0        0      315 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/__init__.py
+-rw-r--r--   0        0        0      161 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/matrix/__init__.py
+-rw-r--r--   0        0        0    13571 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/matrix/fidelity_kernel.py
+-rw-r--r--   0        0        0    12642 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py
+-rw-r--r--   0        0        0    15109 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/matrix/kernel_matrix_base.py
+-rw-r--r--   0        0        0     1237 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/matrix/kernel_util.py
+-rw-r--r--   0        0        0    28126 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/matrix/projected_quantum_kernel.py
+-rw-r--r--   0        0        0     2626 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/matrix/regularization.py
+-rw-r--r--   0        0        0      168 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/ml/__init__.py
+-rw-r--r--   0        0        0     5636 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/ml/qgpc.py
+-rw-r--r--   0        0        0    12897 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/ml/qgpr.py
+-rw-r--r--   0        0        0     9115 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/ml/qkrr.py
+-rw-r--r--   0        0        0     5972 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/ml/qsvc.py
+-rw-r--r--   0        0        0     5940 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/ml/qsvr.py
+-rw-r--r--   0        0        0      190 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/optimization/__init__.py
+-rw-r--r--   0        0        0      646 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/optimization/kernel_loss_base.py
+-rw-r--r--   0        0        0     1323 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/optimization/kernel_optimization_base.py
+-rw-r--r--   0        0        0     3675 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/optimization/kernel_optimizer.py
+-rw-r--r--   0        0        0     2811 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/optimization/negative_log_likelihood.py
+-rw-r--r--   0        0        0     2648 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/kernel/optimization/target_alignment.py
+-rw-r--r--   0        0        0      579 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/__init__.py
+-rw-r--r--   0        0        0    18957 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_base.py
+-rw-r--r--   0        0        0    13837 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_derivatives.py
+-rw-r--r--   0        0        0        0 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_implemented/__init__.py
+-rw-r--r--   0        0        0     4154 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_implemented/custom_observable.py
+-rw-r--r--   0        0        0     6619 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_implemented/ising_hamiltonian.py
+-rw-r--r--   0        0        0     3331 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_implemented/single_pauli.py
+-rw-r--r--   0        0        0     3449 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_implemented/single_probability.py
+-rw-r--r--   0        0        0     4602 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_implemented/summed_paulis.py
+-rw-r--r--   0        0        0     4433 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/observables/observable_implemented/summed_probabilities.py
+-rw-r--r--   0        0        0      388 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/optimizers/__init__.py
+-rw-r--r--   0        0        0     7904 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/optimizers/adam.py
+-rw-r--r--   0        0        0     4606 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/optimizers/approximated_gradients.py
+-rw-r--r--   0        0        0     2822 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/optimizers/optimizer_base.py
+-rw-r--r--   0        0        0     6830 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/optimizers/optimizers_wrapper.py
+-rw-r--r--   0        0        0     7787 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/optimizers/sglbo.py
+-rw-r--r--   0        0        0      486 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/qnn/__init__.py
+-rw-r--r--   0        0        0     8625 2024-06-03 07:52:09.475468 squlearn-0.7.4/src/squlearn/qnn/barren_plateau_analysis.py
+-rw-r--r--   0        0        0    11832 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/base_qnn.py
+-rw-r--r--   0        0        0    28577 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/loss.py
+-rw-r--r--   0        0        0     1650 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn.py
+-rw-r--r--   0        0        0     4920 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn_base.py
+-rw-r--r--   0        0        0    38214 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn_pennylane.py
+-rw-r--r--   0        0        0    44856 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn_qiskit.py
+-rw-r--r--   0        0        0    10283 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/qnnc.py
+-rw-r--r--   0        0        0     9069 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/qnnr.py
+-rw-r--r--   0        0        0    19738 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/qnn/training.py
+-rw-r--r--   0        0        0       92 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/__init__.py
+-rw-r--r--   0        0        0     4478 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/data_preprocessing.py
+-rw-r--r--   0        0        0    73680 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/executor.py
+-rw-r--r--   0        0        0      548 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/optree/__init__.py
+-rw-r--r--   0        0        0    32033 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/optree/optree.py
+-rw-r--r--   0        0        0    17472 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/optree/optree_derivative.py
+-rw-r--r--   0        0        0    69544 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/optree/optree_evaluate.py
+-rw-r--r--   0        0        0      166 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/pennylane/__init__.py
+-rw-r--r--   0        0        0    26113 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/pennylane/pennylane_circuit.py
+-rw-r--r--   0        0        0     1905 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/pennylane/pennylane_gates.py
+-rw-r--r--   0        0        0     9208 2024-06-03 07:52:09.479468 squlearn-0.7.4/src/squlearn/util/qfi.py
+-rw-r--r--   0        0        0     9207 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/encoding_circuit/test_layered_encoding_circuit.py
+-rw-r--r--   0        0        0     6832 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/kernel/ml/test_qgpc.py
+-rw-r--r--   0        0        0     7604 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/kernel/ml/test_qgpr.py
+-rw-r--r--   0        0        0     6249 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/kernel/ml/test_qkrr.py
+-rw-r--r--   0        0        0     6812 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/kernel/ml/test_qsvc.py
+-rw-r--r--   0        0        0     6811 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/kernel/ml/test_qsvr.py
+-rw-r--r--   0        0        0      857 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/optimizers/test_sglbo.py
+-rw-r--r--   0        0        0     4953 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/qnn/test_base_qnn.py
+-rw-r--r--   0        0        0     7013 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/qnn/test_qnnc.py
+-rw-r--r--   0        0        0     7055 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/qnn/test_qnnr.py
+-rw-r--r--   0        0        0     6768 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/qnn/test_training.py
+-rw-r--r--   0        0        0     5527 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/util/optree/test_optree_derivative.py
+-rw-r--r--   0        0        0     9928 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/util/optree/test_optree_evaluate.py
+-rw-r--r--   0        0        0     7337 2024-06-03 07:52:09.479468 squlearn-0.7.4/tests/util/test_executor.py
+-rw-r--r--   0        0        0     5672 1970-01-01 00:00:00.000000 squlearn-0.7.4/PKG-INFO
```

### Comparing `squlearn-0.7.3/.github/CODE_OF_CONDUCT.md` & `squlearn-0.7.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.github/CONTRIBUTING.md` & `squlearn-0.7.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md` & `squlearn-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.github/workflows/doc_checks.yml` & `squlearn-0.7.4/.github/workflows/doc_checks.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.github/workflows/format.yml` & `squlearn-0.7.4/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.github/workflows/publish.yml` & `squlearn-0.7.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.github/workflows/publish_docs.yml` & `squlearn-0.7.4/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.github/workflows/tests.yaml` & `squlearn-0.7.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/.gitignore` & `squlearn-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/CITATION.cff` & `squlearn-0.7.4/CITATION.cff`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,17 @@
       affiliation: Fraunhofer Institute for Manufacturing Engineering and Automation IPA
     - family-names: Rapp
       given-names: Frederic
       orcid: https://orcid.org/0009-0008-6240-8390
       affiliation: Fraunhofer Institute for Manufacturing Engineering and Automation IPA
     - family-names: Hagelüken
       given-names: Manuel
+      orcid: https://orcid.org/0009-0007-9852-3190
       affilliation: Fraunhofer Institute for Manufacturing Engineering and Automation IPA
     - family-names: Roth
       given-names: Marco
       orcid: https://orcid.org/0000-0002-1276-5655
       affiliation: Fraunhofer Institute for Manufacturing Engineering and Automation IPA
   year: 2023
   month: 11
-  doi: 10.48550/arXiv.2311.08990
+  doi: 10.48550/arXiv.2311.08990 
   url: https://arxiv.org/abs/2311.08990
```

### Comparing `squlearn-0.7.3/LICENSE.txt` & `squlearn-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/README.md` & `squlearn-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/Makefile` & `squlearn-0.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/_static/css/custom.css` & `squlearn-0.7.4/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/_static/favicon.png` & `squlearn-0.7.4/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/_static/logo.png` & `squlearn-0.7.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/_static/qnn/qnn.svg` & `squlearn-0.7.4/docs/_static/qnn/qnn.svg`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/_static/schematic.png` & `squlearn-0.7.4/docs/_static/schematic.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/_static/util/executor.png` & `squlearn-0.7.4/docs/_static/util/executor.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/conf.py` & `squlearn-0.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/index.rst` & `squlearn-0.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/install/install.rst` & `squlearn-0.7.4/docs/install/install.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/make.bat` & `squlearn-0.7.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/modules/classes.rst` & `squlearn-0.7.4/docs/modules/classes.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/user_guide/encoding_circuits.rst` & `squlearn-0.7.4/docs/user_guide/encoding_circuits.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/user_guide/executor.rst` & `squlearn-0.7.4/docs/user_guide/executor.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/user_guide/kernel_methods.rst` & `squlearn-0.7.4/docs/user_guide/kernel_methods.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/user_guide/observables.rst` & `squlearn-0.7.4/docs/user_guide/observables.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/docs/user_guide/quantum_neural_networks.rst` & `squlearn-0.7.4/docs/user_guide/quantum_neural_networks.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/encoding_circuits/layered_encoding_circuit.ipynb` & `squlearn-0.7.4/examples/encoding_circuits/layered_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/encoding_circuits/pruning_example.ipynb` & `squlearn-0.7.4/examples/encoding_circuits/pruning_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/encoding_circuits/various_encoding_circuit.ipynb` & `squlearn-0.7.4/examples/encoding_circuits/various_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/executor/example_executor_qiskit.ipynb` & `squlearn-0.7.4/examples/executor/example_executor_qiskit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/integration/mlflow.ipynb` & `squlearn-0.7.4/examples/integration/mlflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/kernel/example_fidelity_kernel.ipynb` & `squlearn-0.7.4/examples/kernel/example_fidelity_kernel.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/kernel/example_projected_kernel.ipynb` & `squlearn-0.7.4/examples/kernel/example_projected_kernel.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/kernel/example_regularization_mitigation.ipynb` & `squlearn-0.7.4/examples/kernel/example_regularization_mitigation.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/kernel/qgpc_workflow.ipynb` & `squlearn-0.7.4/examples/kernel/qgpc_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/kernel/qgpr_optimization_workflow.ipynb` & `squlearn-0.7.4/examples/kernel/qgpr_optimization_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/kernel/qgpr_workflow.ipynb` & `squlearn-0.7.4/examples/kernel/qgpr_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/qnn/classification_example.ipynb` & `squlearn-0.7.4/examples/qnn/classification_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/qnn/example_adam.ipynb` & `squlearn-0.7.4/examples/qnn/example_adam.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/qnn/example_minibatch.ipynb` & `squlearn-0.7.4/examples/qnn/example_minibatch.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/qnn/example_qcnn_encoding_circuit.ipynb` & `squlearn-0.7.4/examples/qnn/example_qcnn_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/qnn/regression_example.ipynb` & `squlearn-0.7.4/examples/qnn/regression_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/qnn/regression_with_variance.ipynb` & `squlearn-0.7.4/examples/qnn/regression_with_variance.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/images/encoding_circuit.png` & `squlearn-0.7.4/examples/tutorials/images/encoding_circuit.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/images/pipeline.png` & `squlearn-0.7.4/examples/tutorials/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/images/projected_quantum_kernel.png` & `squlearn-0.7.4/examples/tutorials/images/projected_quantum_kernel.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/images/quantum_bo.png` & `squlearn-0.7.4/examples/tutorials/images/quantum_bo.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/kernel_digit_classification.ipynb` & `squlearn-0.7.4/examples/tutorials/kernel_digit_classification.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/kernel_grid_search.ipynb` & `squlearn-0.7.4/examples/tutorials/kernel_grid_search.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/kernel_regression.ipynb` & `squlearn-0.7.4/examples/tutorials/kernel_regression.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/qnn_backend_mitigation.ipynb` & `squlearn-0.7.4/examples/tutorials/qnn_backend_mitigation.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/examples/tutorials/quantum_bayesian_optimization.ipynb` & `squlearn-0.7.4/examples/tutorials/quantum_bayesian_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/pyproject.toml` & `squlearn-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "qiskit-aer>=0.12.0",
     "qiskit-algorithms>=0.3.0",
     "qiskit-ibm-runtime>=0.15.1",
     "qiskit-machine-learning>=0.6.1",
     "pennylane>=0.34.0",
     "scipy>=1.5",
     "scikit-learn>=1.0",
-    "scikit-optimize>=0.8",
+    "bayesian-optimization>=1.4.3",
     "tqdm>=4.0",
 ]
 requires-python = ">=3.9"
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/__init__.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/encoding_circuit_base.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/encoding_circuit_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/layered_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/layered_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/pruned_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/pruned_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py` & `squlearn-0.7.4/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/matrix/fidelity_kernel.py` & `squlearn-0.7.4/src/squlearn/kernel/matrix/fidelity_kernel.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py` & `squlearn-0.7.4/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/matrix/kernel_matrix_base.py` & `squlearn-0.7.4/src/squlearn/kernel/matrix/kernel_matrix_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/matrix/kernel_util.py` & `squlearn-0.7.4/src/squlearn/kernel/matrix/kernel_util.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/matrix/projected_quantum_kernel.py` & `squlearn-0.7.4/src/squlearn/kernel/matrix/projected_quantum_kernel.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/matrix/regularization.py` & `squlearn-0.7.4/src/squlearn/kernel/matrix/regularization.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/ml/qgpc.py` & `squlearn-0.7.4/src/squlearn/kernel/ml/qgpc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/ml/qgpr.py` & `squlearn-0.7.4/src/squlearn/kernel/ml/qgpr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/ml/qkrr.py` & `squlearn-0.7.4/src/squlearn/kernel/ml/qkrr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/ml/qsvc.py` & `squlearn-0.7.4/src/squlearn/kernel/ml/qsvc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/ml/qsvr.py` & `squlearn-0.7.4/src/squlearn/kernel/ml/qsvr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/optimization/kernel_loss_base.py` & `squlearn-0.7.4/src/squlearn/kernel/optimization/kernel_loss_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/optimization/kernel_optimization_base.py` & `squlearn-0.7.4/src/squlearn/kernel/optimization/kernel_optimization_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/optimization/kernel_optimizer.py` & `squlearn-0.7.4/src/squlearn/kernel/optimization/kernel_optimizer.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/optimization/negative_log_likelihood.py` & `squlearn-0.7.4/src/squlearn/kernel/optimization/negative_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/kernel/optimization/target_alignment.py` & `squlearn-0.7.4/src/squlearn/kernel/optimization/target_alignment.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/__init__.py` & `squlearn-0.7.4/src/squlearn/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_base.py` & `squlearn-0.7.4/src/squlearn/observables/observable_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_derivatives.py` & `squlearn-0.7.4/src/squlearn/observables/observable_derivatives.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_implemented/custom_observable.py` & `squlearn-0.7.4/src/squlearn/observables/observable_implemented/custom_observable.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_implemented/ising_hamiltonian.py` & `squlearn-0.7.4/src/squlearn/observables/observable_implemented/ising_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_implemented/single_pauli.py` & `squlearn-0.7.4/src/squlearn/observables/observable_implemented/single_pauli.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_implemented/single_probability.py` & `squlearn-0.7.4/src/squlearn/observables/observable_implemented/single_probability.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_implemented/summed_paulis.py` & `squlearn-0.7.4/src/squlearn/observables/observable_implemented/summed_paulis.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/observables/observable_implemented/summed_probabilities.py` & `squlearn-0.7.4/src/squlearn/observables/observable_implemented/summed_probabilities.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/optimizers/adam.py` & `squlearn-0.7.4/src/squlearn/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/optimizers/approximated_gradients.py` & `squlearn-0.7.4/src/squlearn/optimizers/approximated_gradients.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/optimizers/optimizer_base.py` & `squlearn-0.7.4/src/squlearn/optimizers/optimizer_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/optimizers/optimizers_wrapper.py` & `squlearn-0.7.4/src/squlearn/optimizers/optimizers_wrapper.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/optimizers/sglbo.py` & `squlearn-0.7.4/src/squlearn/optimizers/sglbo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import deque
 import numpy as np
-from skopt import gp_minimize
-from scipy.optimize import minimize
+from bayes_opt import BayesianOptimization, UtilityFunction
 
 from .approximated_gradients import FiniteDiffGradient
 from .optimizer_base import OptimizerBase, SGDMixin, default_callback, OptimizerResult
 
 
 class SGLBO(OptimizerBase, SGDMixin):
     """sQUlearn's implementation of the SGLBO optimizer
@@ -15,21 +14,17 @@
     * **tol** (float): Tolerance for the termination of the optimization (default: 1e-6)
     * **maxiter** (int): Maximum number of iterations per fit run (default: 100)
     * **maxiter_total** (int): Maximum number of iterations in total (default: maxiter)
     * **eps** (float): Step size for finite differences (default: 0.01)
     * **num_average** (int): Number of gradients to average (default: 1)
     * **bo_n_calls** (int): Number of iterations for the Bayesian Optimization (default: 20)
     * **bo_bounds** (List): Lower and upper bound for the search space for the Bayesian Optimization for each dimension. Each bound should be provided as a tupel (default: (0.0, 0.3))
-    * **bo_bounds_fac** (float): Factor to adapt the bounds based on the gradient information (default: None)
     * **bo_n_initial_points** (int): Number of initial points for the Bayesian Optimization (default: 10)
-    * **bo_x0_points** (list of lists): Initial input points (default: None)
-    * **bo_aqc_optimizer** (str): Method to minimize the acquisition function. "sampling" or "lbfgs" (default: "lbfgs")
-    * **bo_acq_func** (str): Acquisition function for the Bayesian Optimization (default: "EI"). Valid values are: "LCB", "EI", "PI", "gp_hedge"
-    * **bo_noise** (float): Noise for noisy observations (default: "gaussian")
-    * **min_surrogate** (bool): If True, the surrogate model is minimized to find the optimal step size (default: False)
+    * **bo_acq_func** (str): Acquisition function for the Bayesian Optimization (default: "ei"). Valid values are: "ucb", "ei", "poi"
+    * **bo_xi** (float): Exploration-exploitation trade-off parameter for the Bayesian Optimization (default: 0.01)
     * **log_file** (str): File to log the optimization (default: None)
 
     Args:
         options (dict): Options for the SGLBO optimizer
 
     """
 
@@ -40,23 +35,19 @@
             options = {}
 
         self.tol = options.get("tol", 1e-6)
         self.maxiter = options.get("maxiter", 100)
         self.maxiter_total = options.get("maxiter_total", self.maxiter)
         self.eps = options.get("eps", 0.01)
         self.bo_n_calls = options.get("bo_n_calls", 20)
-        self.bo_bounds = options.get("bo_bounds", [(0.0, 0.3)])
-        self.bo_aqc_func = options.get("bo_aqc_func", "EI")
-        self.bo_aqc_optimizer = options.get("bo_aqc_optimizer", "lbfgs")
+        self.bo_bounds = options.get("bo_bounds", (0.0, 0.3))
+        self.bo_aqc_func = options.get("bo_aqc_func", "ei")
+        self.bo_xi = options.get("bo_xi", 0.01)
         self.bo_n_initial_points = options.get("bo_n_initial_points", 10)
-        self.bo_x0_points = options.get("bo_x0_points")
-        self.bo_noise = options.get("bo_noise", "gaussian")
-        self.bo_bounds_fac = options.get("bo_bounds_fac", None)
         self.log_file = options.get("log_file", None)
-        self.min_surrogate = options.get("min_surrogate", False)
         self.num_average = options.get("num_average", 1)
 
         self.callback = callback
         self.options = options
         self.x = None
         self.func = None
         self.gradient_deque = deque(maxlen=self.num_average)
@@ -64,17 +55,15 @@
         if self.log_file is not None:
             f = open(self.log_file, "w")
             header = (
                 f"maxiter_total: {self.maxiter_total}\n"
                 f"bo_n_calls: {self.bo_n_calls}\n"
                 f"bo_bounds: {self.bo_bounds}\n"
                 f"bo_aqc_func: {self.bo_aqc_func}\n"
-                f"bo_aqc_optimizer: {self.bo_aqc_optimizer}\n"
                 f"bo_n_initial_points: {self.bo_n_initial_points}\n"
-                f"bo_x0_points: {self.bo_x0_points}\n"
             )
             output = " %9s  %13s  %13s  %13s \n" % ("Iteration", "f(x)", "Gradient", "Step")
             f.write(header)
             f.write(output)
             f.close()
 
     def minimize(
@@ -112,24 +101,14 @@
 
         while self.iteration < maxiter:
             # calculate the gradient
             fval = fun(self.x)
             self.gradient_deque.append(grad(self.x))
             gradient = np.average(self.gradient_deque, axis=0)
 
-            # adapt bounds and x0 based on the gradient
-            if (
-                self.bo_bounds is not None
-                and self.bo_x0_points is not None
-                and self.bo_bounds_fac is not None
-            ):
-                self.bo_bounds, self.bo_x0_points = self.__adapt_bounds(
-                    self.bo_bounds, self.bo_x0_points, gradient
-                )
-
             x_updated = self.step(x=self.x, grad=gradient)
 
             # check termination
             if np.linalg.norm(self.x - x_updated) < self.tol:
                 break
 
             if self.log_file is not None:
@@ -174,81 +153,43 @@
         # cost function to optimize the step size in one dimension
         def step_size_cost(x):
             updated_point = start_point.copy()
             updated_point = updated_point - x * gradient
 
             return func(updated_point)
 
-        # bayesian optimization to estimate the step size in one dimension
-        res = gp_minimize(
-            step_size_cost,
-            self.bo_bounds,
-            n_calls=self.bo_n_calls,
-            acq_func=self.bo_aqc_func,
-            acq_optimizer=self.bo_aqc_optimizer,
-            x0=self.bo_x0_points,
-            n_jobs=-1,
+        # Convert the minimization problem into a maximization problem
+        def neg_step_size_cost(x):
+            return -step_size_cost(x)
+
+        # Define the bounds for Bayesian Optimization
+        pbounds = {"x": self.bo_bounds}
+
+        acquisition_function = UtilityFunction(kind=self.bo_aqc_func, xi=self.bo_xi)
+
+        # Initialize Bayesian Optimization
+        bo = BayesianOptimization(
+            f=neg_step_size_cost,
+            pbounds=pbounds,
+            verbose=0,
             random_state=0,
-            noise=self.bo_noise,
-            n_initial_points=self.bo_n_initial_points,
+            allow_duplicate_points=True,
         )
 
-        # minimize the surrogate model to find the optimal step size
-        if self.min_surrogate:
-
-            def func_surrogate(x):
-                reg = res.models[-1]
-                x = res.space.transform(x.reshape(1, -1))
-                return reg.predict(x.reshape(1, -1))[0]
+        # Perform the optimization
+        bo.maximize(
+            init_points=self.bo_n_initial_points,
+            n_iter=self.bo_n_calls,
+            acquisition_function=acquisition_function,
+        )
 
-            res_surr = minimize(
-                func_surrogate, x0=res.x[0], method="Nelder-Mead", tol=1e-6, bounds=self.bo_bounds
-            )
-            x_val = res_surr.x
-        else:
-            x_val = res.x
+        x_val = bo.max["params"]["x"]
 
         return x_val
 
-    def __adapt_bounds(
-        self, current_bounds: list, current_x0: list, gradient: np.ndarray
-    ) -> tuple:
-        """
-        Function to adapt the bounds and initial points for gp_minimize based on the gradient information.
-
-        Args:
-            current_bounds (List): Current bounds for the search space.
-            current_x0 (List): Current initial points.
-            gradient (np.ndarray): Gradient of the objective function.
-
-        Returns:
-            Tuple: Updated bounds for the search space and initial points.
-        """
-
-        # Compute the magnitude of the gradient
-        grad_magnitude = np.linalg.norm(gradient)
-
-        # Update the bounds based on the gradient magnitude
-        updated_bounds = []
-        for bound in current_bounds:
-            lower = max(bound[0] - self.bo_bounds_fac * grad_magnitude, 0.0)
-            upper = bound[1] + self.bo_bounds_fac * grad_magnitude
-            updated_bounds.append((lower, upper))
-
-        # Update the initial points based on the updated bounds and maintaining distribution
-        updated_x0 = []
-
-        # Distribute the x0 points evenly within the updated bounds
-        for i in range(len(current_x0)):
-            t = i / len(current_x0)  # t goes from 0 to 1
-            updated_x0_point = [lower + t * (upper - lower) for (lower, upper) in updated_bounds]
-            updated_x0.append(updated_x0_point)
-
-        return updated_bounds, updated_x0
-
     def _log(self, fval, gradient, dx):
         """Function for creating a log entry of the optimization."""
         if self.log_file is not None:
             f = open(self.log_file, "a")
             if fval is not None:
                 output = " %9d  %13.7f  %13.7f  %13.7f  \n" % (
                     self.iteration,
```

### Comparing `squlearn-0.7.3/src/squlearn/qnn/barren_plateau_analysis.py` & `squlearn-0.7.4/src/squlearn/qnn/barren_plateau_analysis.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/base_qnn.py` & `squlearn-0.7.4/src/squlearn/qnn/base_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/loss.py` & `squlearn-0.7.4/src/squlearn/qnn/loss.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn.py` & `squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn_base.py` & `squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn_pennylane.py` & `squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn_pennylane.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/lowlevel_qnn_qiskit.py` & `squlearn-0.7.4/src/squlearn/qnn/lowlevel_qnn_qiskit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/qnnc.py` & `squlearn-0.7.4/src/squlearn/qnn/qnnc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/qnnr.py` & `squlearn-0.7.4/src/squlearn/qnn/qnnr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/qnn/training.py` & `squlearn-0.7.4/src/squlearn/qnn/training.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/data_preprocessing.py` & `squlearn-0.7.4/src/squlearn/util/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/executor.py` & `squlearn-0.7.4/src/squlearn/util/executor.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/optree/__init__.py` & `squlearn-0.7.4/src/squlearn/util/optree/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/optree/optree.py` & `squlearn-0.7.4/src/squlearn/util/optree/optree.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/optree/optree_derivative.py` & `squlearn-0.7.4/src/squlearn/util/optree/optree_derivative.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/optree/optree_evaluate.py` & `squlearn-0.7.4/src/squlearn/util/optree/optree_evaluate.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/pennylane/pennylane_circuit.py` & `squlearn-0.7.4/src/squlearn/util/pennylane/pennylane_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/pennylane/pennylane_gates.py` & `squlearn-0.7.4/src/squlearn/util/pennylane/pennylane_gates.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/src/squlearn/util/qfi.py` & `squlearn-0.7.4/src/squlearn/util/qfi.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/encoding_circuit/test_layered_encoding_circuit.py` & `squlearn-0.7.4/tests/encoding_circuit/test_layered_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/kernel/ml/test_qgpc.py` & `squlearn-0.7.4/tests/kernel/ml/test_qgpc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/kernel/ml/test_qgpr.py` & `squlearn-0.7.4/tests/kernel/ml/test_qgpr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/kernel/ml/test_qkrr.py` & `squlearn-0.7.4/tests/kernel/ml/test_qkrr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/kernel/ml/test_qsvc.py` & `squlearn-0.7.4/tests/kernel/ml/test_qsvc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/kernel/ml/test_qsvr.py` & `squlearn-0.7.4/tests/kernel/ml/test_qsvr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/optimizers/test_sglbo.py` & `squlearn-0.7.4/tests/optimizers/test_sglbo.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/qnn/test_base_qnn.py` & `squlearn-0.7.4/tests/qnn/test_base_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/qnn/test_qnnc.py` & `squlearn-0.7.4/tests/qnn/test_qnnc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/qnn/test_qnnr.py` & `squlearn-0.7.4/tests/qnn/test_qnnr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/qnn/test_training.py` & `squlearn-0.7.4/tests/qnn/test_training.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/util/optree/test_optree_derivative.py` & `squlearn-0.7.4/tests/util/optree/test_optree_derivative.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/util/optree/test_optree_evaluate.py` & `squlearn-0.7.4/tests/util/optree/test_optree_evaluate.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/tests/util/test_executor.py` & `squlearn-0.7.4/tests/util/test_executor.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.3/PKG-INFO` & `squlearn-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squlearn
-Version: 0.7.3
+Version: 0.7.4
 Summary: A library for quantum machine learning following the scikit-learnstandard.
 Keywords: quantum,machine learning,qml
 Author-email: David Kreplin <david.kreplin@ipa.fraunhofer.de>, Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>, Jan Schnabel <jan.schnabel@ipa.fraunhofer.de>, Frederic Rapp <frederic.rapp@ipa.fraunhofer.de>, Manuel Hagelüken <manuel.hagelueken@ipa.fraunhofer.de>, Marco Roth <marco.roth@ipa.fraunhofer.de>
 Maintainer-email: David Kreplin <david.kreplin@ipa.fraunhofer.de>, Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Requires-Dist: qiskit-aer>=0.12.0
 Requires-Dist: qiskit-algorithms>=0.3.0
 Requires-Dist: qiskit-ibm-runtime>=0.15.1
 Requires-Dist: qiskit-machine-learning>=0.6.1
 Requires-Dist: pennylane>=0.34.0
 Requires-Dist: scipy>=1.5
 Requires-Dist: scikit-learn>=1.0
-Requires-Dist: scikit-optimize>=0.8
+Requires-Dist: bayesian-optimization>=1.4.3
 Requires-Dist: tqdm>=4.0
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: myst-parser ; extra == "dev"
 Requires-Dist: nbmake ; extra == "dev"
 Requires-Dist: nbsphinx ; extra == "dev"
 Requires-Dist: nbsphinx_link ; extra == "dev"
```

