# Comparing `tmp/azure-quantum-0.28.263081.tar.gz` & `tmp/azure-quantum-0.28.276173b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-quantum-0.28.263081.tar", last modified: Mon Mar 27 20:53:24 2023, max compression
+gzip compressed data, was "azure-quantum-0.28.276173b1.tar", last modified: Fri Jun  2 01:06:53 2023, max compression
```

## Comparing `azure-quantum-0.28.263081.tar` & `azure-quantum-0.28.276173b1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.714282 azure-quantum-0.28.263081/
--rw-rw-rw-   0        0        0     5568 2023-03-27 20:53:24.714282 azure-quantum-0.28.263081/PKG-INFO
--rw-rw-rw-   0        0        0     5063 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.604899 azure-quantum-0.28.263081/azure/
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.620527 azure-quantum-0.28.263081/azure/quantum/
--rw-rw-rw-   0        0        0      414 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.620527 azure-quantum-0.28.263081/azure/quantum/_authentication/
--rw-rw-rw-   0        0        0      236 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_authentication/__init__.py
--rw-rw-rw-   0        0        0     5047 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_authentication/_chained.py
--rw-rw-rw-   0        0        0    10502 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_authentication/_default.py
--rw-rw-rw-   0        0        0     3570 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.620527 azure-quantum-0.28.263081/azure/quantum/_client/
--rw-rw-rw-   0        0        0      896 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/__init__.py
--rw-rw-rw-   0        0        0     5854 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/_client.py
--rw-rw-rw-   0        0        0     4444 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/_configuration.py
--rw-rw-rw-   0        0        0      694 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/_patch.py
--rw-rw-rw-   0        0        0    80832 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/_serialization.py
--rw-rw-rw-   0        0        0      996 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/_vendor.py
--rw-rw-rw-   0        0        0      501 2023-03-27 20:53:23.000000 azure-quantum-0.28.263081/azure/quantum/_client/_version.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.636146 azure-quantum-0.28.263081/azure/quantum/_client/aio/
--rw-rw-rw-   0        0        0      840 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/aio/__init__.py
--rw-rw-rw-   0        0        0     6010 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/aio/_client.py
--rw-rw-rw-   0        0        0     4487 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/aio/_configuration.py
--rw-rw-rw-   0        0        0      694 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/aio/_patch.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.636146 azure-quantum-0.28.263081/azure/quantum/_client/aio/operations/
--rw-rw-rw-   0        0        0     1154 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/aio/operations/__init__.py
--rw-rw-rw-   0        0        0    54215 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/aio/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/aio/operations/_patch.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.636146 azure-quantum-0.28.263081/azure/quantum/_client/models/
--rw-rw-rw-   0        0        0     2100 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/models/__init__.py
--rw-rw-rw-   0        0        0     2977 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/models/_enums.py
--rw-rw-rw-   0        0        0    41802 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/models/_models.py
--rw-rw-rw-   0        0        0      694 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/models/_patch.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.636146 azure-quantum-0.28.263081/azure/quantum/_client/operations/
--rw-rw-rw-   0        0        0     1154 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/operations/__init__.py
--rw-rw-rw-   0        0        0    75919 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/_client/operations/_patch.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.636146 azure-quantum-0.28.263081/azure/quantum/aio/
--rw-rw-rw-   0        0        0      360 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.651776 azure-quantum-0.28.263081/azure/quantum/aio/_authentication/
--rw-rw-rw-   0        0        0      236 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/_authentication/__init__.py
--rw-rw-rw-   0        0        0     4647 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/_authentication/_chained.py
--rw-rw-rw-   0        0        0    10430 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/_authentication/_default.py
--rw-rw-rw-   0        0        0     3632 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.651776 azure-quantum-0.28.263081/azure/quantum/aio/job/
--rw-rw-rw-   0        0        0       43 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/job/__init__.py
--rw-rw-rw-   0        0        0    11565 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/job/base_job.py
--rw-rw-rw-   0        0        0     3716 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/job/job.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.651776 azure-quantum-0.28.263081/azure/quantum/aio/optimization/
--rw-rw-rw-   0        0        0      484 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/optimization/__init__.py
--rw-rw-rw-   0        0        0      560 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/optimization/online_problem.py
--rw-rw-rw-   0        0        0     3620 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/optimization/problem.py
--rw-rw-rw-   0        0        0    10536 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/optimization/streaming_problem.py
--rw-rw-rw-   0        0        0    12953 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/storage.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.651776 azure-quantum-0.28.263081/azure/quantum/aio/target/
--rw-rw-rw-   0        0        0      831 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/ionq.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.651776 azure-quantum-0.28.263081/azure/quantum/aio/target/microsoft/
--rw-rw-rw-   0        0        0      267 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/microsoft/__init__.py
--rw-rw-rw-   0        0        0     1113 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/microsoft/qio.py
--rw-rw-rw-   0        0        0      416 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/oneqbit.py
--rw-rw-rw-   0        0        0     1413 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/quantinuum.py
--rw-rw-rw-   0        0        0     3336 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/solvers.py
--rw-rw-rw-   0        0        0     2366 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/target.py
--rw-rw-rw-   0        0        0     2449 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/target_factory.py
--rw-rw-rw-   0        0        0      249 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/target/toshiba.py
--rw-rw-rw-   0        0        0    13507 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/aio/workspace.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.667391 azure-quantum-0.28.263081/azure/quantum/argument_types/
--rw-rw-rw-   0        0        0      213 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/argument_types/__init__.py
--rw-rw-rw-   0        0        0      721 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/argument_types/types.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.667391 azure-quantum-0.28.263081/azure/quantum/chemistry/
--rw-rw-rw-   0        0        0      351 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/chemistry/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.667391 azure-quantum-0.28.263081/azure/quantum/cirq/
--rw-rw-rw-   0        0        0      125 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/cirq/__init__.py
--rw-rw-rw-   0        0        0     2773 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/cirq/job.py
--rw-rw-rw-   0        0        0     8039 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/cirq/service.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.667391 azure-quantum-0.28.263081/azure/quantum/cirq/targets/
--rw-rw-rw-   0        0        0      502 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/cirq/targets/__init__.py
--rw-rw-rw-   0        0        0     6804 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/cirq/targets/ionq.py
--rw-rw-rw-   0        0        0     4541 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/cirq/targets/quantinuum.py
--rw-rw-rw-   0        0        0     2076 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/cirq/targets/target.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.667391 azure-quantum-0.28.263081/azure/quantum/job/
--rw-rw-rw-   0        0        0      372 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/job/__init__.py
--rw-rw-rw-   0        0        0    12056 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/job/base_job.py
--rw-rw-rw-   0        0        0     1683 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/job/filtered_job.py
--rw-rw-rw-   0        0        0     4467 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/job/job.py
--rw-rw-rw-   0        0        0    11691 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/job/session.py
--rw-rw-rw-   0        0        0     1219 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/job/workspace_item.py
--rw-rw-rw-   0        0        0     1200 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/job/workspace_item_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.667391 azure-quantum-0.28.263081/azure/quantum/optimization/
--rw-rw-rw-   0        0        0      469 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.683028 azure-quantum-0.28.263081/azure/quantum/optimization/oneqbit/
--rw-rw-rw-   0        0        0      366 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/oneqbit/__init__.py
--rw-rw-rw-   0        0        0      402 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/oneqbit/solvers.py
--rw-rw-rw-   0        0        0      636 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/online_problem.py
--rw-rw-rw-   0        0        0    25096 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/problem.py
--rw-rw-rw-   0        0        0      512 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/solvers.py
--rw-rw-rw-   0        0        0    13733 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/streaming_problem.py
--rw-rw-rw-   0        0        0     9858 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/term.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.683028 azure-quantum-0.28.263081/azure/quantum/optimization/toshiba/
--rw-rw-rw-   0        0        0      302 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/toshiba/__init__.py
--rw-rw-rw-   0        0        0      374 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/optimization/toshiba/solvers.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.683028 azure-quantum-0.28.263081/azure/quantum/qiskit/
--rw-rw-rw-   0        0        0      273 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.683028 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/
--rw-rw-rw-   0        0        0      965 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/__init__.py
--rw-rw-rw-   0        0        0    16340 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/backend.py
--rw-rw-rw-   0        0        0    12920 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/ionq.py
--rw-rw-rw-   0        0        0     3441 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/microsoft.py
--rw-rw-rw-   0        0        0     3884 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/qci.py
--rw-rw-rw-   0        0        0    12897 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/quantinuum.py
--rw-rw-rw-   0        0        0     4081 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/backends/rigetti.py
--rw-rw-rw-   0        0        0    14829 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/job.py
--rw-rw-rw-   0        0        0     9974 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/provider.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.683028 azure-quantum-0.28.263081/azure/quantum/qiskit/results/
--rw-rw-rw-   0        0        0        0 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/results/__init__.py
--rw-rw-rw-   0        0        0      814 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/qiskit/results/resource_estimator.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.683028 azure-quantum-0.28.263081/azure/quantum/serialization/
--rw-rw-rw-   0        0        0       58 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/serialization/__init__.py
--rw-rw-rw-   0        0        0    11227 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/serialization/problem_pb2.py
--rw-rw-rw-   0        0        0    12536 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/storage.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.698681 azure-quantum-0.28.263081/azure/quantum/target/
--rw-rw-rw-   0        0        0      817 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/__init__.py
--rw-rw-rw-   0        0        0     7212 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/ionq.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.698681 azure-quantum-0.28.263081/azure/quantum/target/microsoft/
--rw-rw-rw-   0        0        0      550 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/__init__.py
--rw-rw-rw-   0        0        0     1005 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/job.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.698681 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/
--rw-rw-rw-   0        0        0      402 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/__init__.py
--rw-rw-rw-   0        0        0     3053 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/parallel_tempering.py
--rw-rw-rw-   0        0        0     3147 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/population_annealing.py
--rw-rw-rw-   0        0        0     2564 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/quantum_monte_carlo.py
--rw-rw-rw-   0        0        0     3961 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/simulated_annealing.py
--rw-rw-rw-   0        0        0     3695 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/substochastic_montecarlo.py
--rw-rw-rw-   0        0        0     2393 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/tabu.py
--rw-rw-rw-   0        0        0    11523 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/result.py
--rw-rw-rw-   0        0        0     6600 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/microsoft/target.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.698681 azure-quantum-0.28.263081/azure/quantum/target/oneqbit/
--rw-rw-rw-   0        0        0      210 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/oneqbit/__init__.py
--rw-rw-rw-   0        0        0    13648 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/oneqbit/solvers.py
--rw-rw-rw-   0        0        0     8782 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/params.py
--rw-rw-rw-   0        0        0     7037 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/quantinuum.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.698681 azure-quantum-0.28.263081/azure/quantum/target/rigetti/
--rw-rw-rw-   0        0        0      378 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/rigetti/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/rigetti/result.py
--rw-rw-rw-   0        0        0     6084 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/rigetti/target.py
--rw-rw-rw-   0        0        0    16858 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/solvers.py
--rw-rw-rw-   0        0        0     8929 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/target.py
--rw-rw-rw-   0        0        0     5322 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/target_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.698681 azure-quantum-0.28.263081/azure/quantum/target/toshiba/
--rw-rw-rw-   0        0        0      146 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/toshiba/__init__.py
--rw-rw-rw-   0        0        0     5722 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/target/toshiba/solvers.py
--rw-rw-rw-   0        0        0      241 2023-03-27 20:53:23.000000 azure-quantum-0.28.263081/azure/quantum/version.py
--rw-rw-rw-   0        0        0    19134 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/azure/quantum/workspace.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:53:24.714282 azure-quantum-0.28.263081/azure_quantum.egg-info/
--rw-rw-rw-   0        0        0     5568 2023-03-27 20:53:24.000000 azure-quantum-0.28.263081/azure_quantum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5009 2023-03-27 20:53:24.000000 azure-quantum-0.28.263081/azure_quantum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 20:53:24.000000 azure-quantum-0.28.263081/azure_quantum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      816 2023-03-27 20:53:24.000000 azure-quantum-0.28.263081/azure_quantum.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-27 20:53:24.000000 azure-quantum-0.28.263081/azure_quantum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       46 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/requirements-cirq.txt
--rw-rw-rw-   0        0        0       49 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/requirements-dev.txt
--rw-rw-rw-   0        0        0      130 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/requirements-qiskit.txt
--rw-rw-rw-   0        0        0       19 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/requirements-qsharp.txt
--rw-rw-rw-   0        0        0      275 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/requirements-quil.txt
--rw-rw-rw-   0        0        0      269 2023-03-27 20:53:18.000000 azure-quantum-0.28.263081/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 20:53:24.714282 azure-quantum-0.28.263081/setup.cfg
--rw-rw-rw-   0        0        0     3770 2023-03-27 20:31:34.000000 azure-quantum-0.28.263081/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/
+-rw-rw-rw-   0        0        0     5570 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/PKG-INFO
+-rw-rw-rw-   0        0        0     5063 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.719774 azure-quantum-0.28.276173b1/azure/
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.735368 azure-quantum-0.28.276173b1/azure/quantum/
+-rw-rw-rw-   0        0        0      414 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.735368 azure-quantum-0.28.276173b1/azure/quantum/_authentication/
+-rw-rw-rw-   0        0        0      236 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     5047 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_authentication/_chained.py
+-rw-rw-rw-   0        0        0    10502 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3570 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.735368 azure-quantum-0.28.276173b1/azure/quantum/_client/
+-rw-rw-rw-   0        0        0      896 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/__init__.py
+-rw-rw-rw-   0        0        0     5854 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/_client.py
+-rw-rw-rw-   0        0        0     4444 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/_configuration.py
+-rw-rw-rw-   0        0        0      694 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/_patch.py
+-rw-rw-rw-   0        0        0    80832 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/_serialization.py
+-rw-rw-rw-   0        0        0      996 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/_vendor.py
+-rw-rw-rw-   0        0        0      503 2023-06-02 01:06:52.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.735368 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/
+-rw-rw-rw-   0        0        0      840 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/__init__.py
+-rw-rw-rw-   0        0        0     6010 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/_client.py
+-rw-rw-rw-   0        0        0     4487 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/_configuration.py
+-rw-rw-rw-   0        0        0      694 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/_patch.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.751011 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/operations/
+-rw-rw-rw-   0        0        0     1154 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/operations/__init__.py
+-rw-rw-rw-   0        0        0    54215 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/aio/operations/_patch.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.751011 azure-quantum-0.28.276173b1/azure/quantum/_client/models/
+-rw-rw-rw-   0        0        0     2100 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/models/__init__.py
+-rw-rw-rw-   0        0        0     2977 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/models/_enums.py
+-rw-rw-rw-   0        0        0    41802 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/models/_models.py
+-rw-rw-rw-   0        0        0      694 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/models/_patch.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.751011 azure-quantum-0.28.276173b1/azure/quantum/_client/operations/
+-rw-rw-rw-   0        0        0     1154 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/operations/__init__.py
+-rw-rw-rw-   0        0        0    75919 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/_client/operations/_patch.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.751011 azure-quantum-0.28.276173b1/azure/quantum/aio/
+-rw-rw-rw-   0        0        0      360 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.751011 azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/
+-rw-rw-rw-   0        0        0      236 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     4647 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/_chained.py
+-rw-rw-rw-   0        0        0    10430 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3632 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.751011 azure-quantum-0.28.276173b1/azure/quantum/aio/job/
+-rw-rw-rw-   0        0        0       43 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/job/__init__.py
+-rw-rw-rw-   0        0        0    11565 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/job/base_job.py
+-rw-rw-rw-   0        0        0     3728 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/job/job.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.766607 azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/
+-rw-rw-rw-   0        0        0      484 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/__init__.py
+-rw-rw-rw-   0        0        0      560 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/online_problem.py
+-rw-rw-rw-   0        0        0     3620 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/problem.py
+-rw-rw-rw-   0        0        0    10536 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/streaming_problem.py
+-rw-rw-rw-   0        0        0    12953 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/storage.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.766607 azure-quantum-0.28.276173b1/azure/quantum/aio/target/
+-rw-rw-rw-   0        0        0      831 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/ionq.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.766607 azure-quantum-0.28.276173b1/azure/quantum/aio/target/microsoft/
+-rw-rw-rw-   0        0        0      267 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/microsoft/__init__.py
+-rw-rw-rw-   0        0        0     1113 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/microsoft/qio.py
+-rw-rw-rw-   0        0        0      416 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/oneqbit.py
+-rw-rw-rw-   0        0        0     1413 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/quantinuum.py
+-rw-rw-rw-   0        0        0     3336 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/solvers.py
+-rw-rw-rw-   0        0        0     2366 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/target.py
+-rw-rw-rw-   0        0        0     2449 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/target_factory.py
+-rw-rw-rw-   0        0        0      249 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/target/toshiba.py
+-rw-rw-rw-   0        0        0    13507 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/aio/workspace.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.766607 azure-quantum-0.28.276173b1/azure/quantum/argument_types/
+-rw-rw-rw-   0        0        0      213 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/argument_types/__init__.py
+-rw-rw-rw-   0        0        0      721 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/argument_types/types.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.766607 azure-quantum-0.28.276173b1/azure/quantum/chemistry/
+-rw-rw-rw-   0        0        0      351 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/chemistry/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.766607 azure-quantum-0.28.276173b1/azure/quantum/cirq/
+-rw-rw-rw-   0        0        0      125 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/cirq/__init__.py
+-rw-rw-rw-   0        0        0     2773 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/cirq/job.py
+-rw-rw-rw-   0        0        0     8039 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/cirq/service.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.766607 azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/
+-rw-rw-rw-   0        0        0      502 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/__init__.py
+-rw-rw-rw-   0        0        0     6804 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/ionq.py
+-rw-rw-rw-   0        0        0     4541 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/quantinuum.py
+-rw-rw-rw-   0        0        0     2184 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/target.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.782232 azure-quantum-0.28.276173b1/azure/quantum/job/
+-rw-rw-rw-   0        0        0      372 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/job/__init__.py
+-rw-rw-rw-   0        0        0    12056 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/job/base_job.py
+-rw-rw-rw-   0        0        0     1683 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/job/filtered_job.py
+-rw-rw-rw-   0        0        0     4505 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/job/job.py
+-rw-rw-rw-   0        0        0    11936 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/job/session.py
+-rw-rw-rw-   0        0        0     1198 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/job/workspace_item.py
+-rw-rw-rw-   0        0        0     1200 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/job/workspace_item_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.782232 azure-quantum-0.28.276173b1/azure/quantum/optimization/
+-rw-rw-rw-   0        0        0      469 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.782232 azure-quantum-0.28.276173b1/azure/quantum/optimization/oneqbit/
+-rw-rw-rw-   0        0        0      366 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/oneqbit/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/oneqbit/solvers.py
+-rw-rw-rw-   0        0        0      636 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/online_problem.py
+-rw-rw-rw-   0        0        0    25096 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/problem.py
+-rw-rw-rw-   0        0        0      512 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/solvers.py
+-rw-rw-rw-   0        0        0    13733 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/streaming_problem.py
+-rw-rw-rw-   0        0        0     9858 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/term.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.782232 azure-quantum-0.28.276173b1/azure/quantum/optimization/toshiba/
+-rw-rw-rw-   0        0        0      302 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/toshiba/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/optimization/toshiba/solvers.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.782232 azure-quantum-0.28.276173b1/azure/quantum/qiskit/
+-rw-rw-rw-   0        0        0      273 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.782232 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/
+-rw-rw-rw-   0        0        0      965 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/__init__.py
+-rw-rw-rw-   0        0        0    16467 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/backend.py
+-rw-rw-rw-   0        0        0    12920 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/ionq.py
+-rw-rw-rw-   0        0        0     3441 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/microsoft.py
+-rw-rw-rw-   0        0        0     3884 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/qci.py
+-rw-rw-rw-   0        0        0    13278 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/quantinuum.py
+-rw-rw-rw-   0        0        0     4081 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/rigetti.py
+-rw-rw-rw-   0        0        0    14829 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/job.py
+-rw-rw-rw-   0        0        0     9974 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/provider.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.797876 azure-quantum-0.28.276173b1/azure/quantum/qiskit/results/
+-rw-rw-rw-   0        0        0        0 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/results/__init__.py
+-rw-rw-rw-   0        0        0      814 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/qiskit/results/resource_estimator.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.797876 azure-quantum-0.28.276173b1/azure/quantum/serialization/
+-rw-rw-rw-   0        0        0       58 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/serialization/__init__.py
+-rw-rw-rw-   0        0        0    11227 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/serialization/problem_pb2.py
+-rw-rw-rw-   0        0        0    12536 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/storage.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.797876 azure-quantum-0.28.276173b1/azure/quantum/target/
+-rw-rw-rw-   0        0        0      817 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/__init__.py
+-rw-rw-rw-   0        0        0     7212 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/ionq.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.797876 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/
+-rw-rw-rw-   0        0        0      667 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/__init__.py
+-rw-rw-rw-   0        0        0     1005 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/job.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/
+-rw-rw-rw-   0        0        0      402 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/__init__.py
+-rw-rw-rw-   0        0        0     3053 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/parallel_tempering.py
+-rw-rw-rw-   0        0        0     3145 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/population_annealing.py
+-rw-rw-rw-   0        0        0     2564 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/quantum_monte_carlo.py
+-rw-rw-rw-   0        0        0     3971 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/simulated_annealing.py
+-rw-rw-rw-   0        0        0     3712 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/substochastic_montecarlo.py
+-rw-rw-rw-   0        0        0     2395 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/tabu.py
+-rw-rw-rw-   0        0        0    14916 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/result.py
+-rw-rw-rw-   0        0        0     9169 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/target.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/azure/quantum/target/oneqbit/
+-rw-rw-rw-   0        0        0      210 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/oneqbit/__init__.py
+-rw-rw-rw-   0        0        0    13648 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/oneqbit/solvers.py
+-rw-rw-rw-   0        0        0     8976 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/params.py
+-rw-rw-rw-   0        0        0     7250 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/quantinuum.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/azure/quantum/target/rigetti/
+-rw-rw-rw-   0        0        0      378 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/rigetti/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/rigetti/result.py
+-rw-rw-rw-   0        0        0     5916 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/rigetti/target.py
+-rw-rw-rw-   0        0        0    17063 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/solvers.py
+-rw-rw-rw-   0        0        0     9181 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/target.py
+-rw-rw-rw-   0        0        0     5322 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/target_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/azure/quantum/target/toshiba/
+-rw-rw-rw-   0        0        0      146 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/toshiba/__init__.py
+-rw-rw-rw-   0        0        0     5722 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/target/toshiba/solvers.py
+-rw-rw-rw-   0        0        0      243 2023-06-02 01:06:52.000000 azure-quantum-0.28.276173b1/azure/quantum/version.py
+-rw-rw-rw-   0        0        0    19134 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/azure/quantum/workspace.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/azure_quantum.egg-info/
+-rw-rw-rw-   0        0        0     5570 2023-06-02 01:06:53.000000 azure-quantum-0.28.276173b1/azure_quantum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5009 2023-06-02 01:06:53.000000 azure-quantum-0.28.276173b1/azure_quantum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 01:06:53.000000 azure-quantum-0.28.276173b1/azure_quantum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      866 2023-06-02 01:06:53.000000 azure-quantum-0.28.276173b1/azure_quantum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 01:06:53.000000 azure-quantum-0.28.276173b1/azure_quantum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       46 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/requirements-cirq.txt
+-rw-rw-rw-   0        0        0      296 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/requirements-dev.txt
+-rw-rw-rw-   0        0        0      130 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/requirements-qiskit.txt
+-rw-rw-rw-   0        0        0       19 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/requirements-qsharp.txt
+-rw-rw-rw-   0        0        0      275 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/requirements-quil.txt
+-rw-rw-rw-   0        0        0      269 2023-06-02 01:06:47.000000 azure-quantum-0.28.276173b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 01:06:53.813501 azure-quantum-0.28.276173b1/setup.cfg
+-rw-rw-rw-   0        0        0     3770 2023-06-02 00:44:11.000000 azure-quantum-0.28.276173b1/setup.py
```

### Comparing `azure-quantum-0.28.263081/PKG-INFO` & `azure-quantum-0.28.276173b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 0.28.263081
+Version: 0.28.276173b1
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/qdk-python
 Author: Microsoft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `azure-quantum-0.28.263081/README.md` & `azure-quantum-0.28.276173b1/README.md`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_authentication/_chained.py` & `azure-quantum-0.28.276173b1/azure/quantum/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_authentication/_default.py` & `azure-quantum-0.28.276173b1/azure/quantum/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_authentication/_token.py` & `azure-quantum-0.28.276173b1/azure/quantum/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/_client.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/_configuration.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/_patch.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/_serialization.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/_vendor.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/aio/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/aio/_client.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/aio/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/aio/_configuration.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/aio/_patch.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/aio/operations/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/aio/operations/_operations.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/aio/operations/_patch.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/models/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/models/_enums.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/models/_models.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/models/_patch.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/operations/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/operations/_operations.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/_client/operations/_patch.py` & `azure-quantum-0.28.276173b1/azure/quantum/_client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/_authentication/_chained.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/_authentication/_default.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/_authentication/_token.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/job/base_job.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/job/base_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/job/job.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/job/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 ##
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
+
 import asyncio
 import logging
 import json
+import time
 
-from azure.quantum.aio.job.base_job import BaseJob, ContentType, DEFAULT_TIMEOUT
+from azure.quantum.aio.job.base_job import BaseJob, DEFAULT_TIMEOUT
 from azure.quantum.job.job import Job as SyncJob
 from azure.quantum.job.filtered_job import FilteredJob
 
 __all__ = ["Job"]
 
 logger = logging.getLogger(__name__)
 
@@ -50,28 +52,27 @@
         :param timeout_secs: Timeout in seconds, defaults to None
         :type timeout_secs: int, optional
         :param print_progress: Print "." to stdout to display progress
         :type print_progress: bool, optional
         :raises TimeoutError: If the total poll time exceeds timeout, raise
         """
         await self.refresh()
-        poll_wait = 0.2
-        total_time = 0.
+        poll_wait = SyncJob._default_poll_wait
+        start_time = time.time()
         while not self.has_completed():
-            if timeout_secs is not None and total_time >= timeout_secs:
+            if timeout_secs is not None and (time.time() - start_time) >= timeout_secs:
                 raise TimeoutError(f"The wait time has exceeded {timeout_secs} seconds.")
- 
+
             logger.debug(
                 f"Waiting for job {self.id},"
                 + f"it is in status '{self.details.status}'"
             )
             if print_progress:
                 print(".", end="", flush=True)
             await asyncio.sleep(poll_wait)
-            total_time += poll_wait
             await self.refresh()
             poll_wait = (
                 max_poll_wait_secs
                 if poll_wait >= max_poll_wait_secs
                 else poll_wait * 1.5
             )
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/optimization/online_problem.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/online_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/optimization/problem.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/optimization/streaming_problem.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/optimization/streaming_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/storage.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/target/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/target/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/target/ionq.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/target/microsoft/qio.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/target/microsoft/qio.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/target/quantinuum.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/target/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/target/solvers.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/target/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/target/target.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/target/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/target/target_factory.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/target/target_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/aio/workspace.py` & `azure-quantum-0.28.276173b1/azure/quantum/aio/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/argument_types/types.py` & `azure-quantum-0.28.276173b1/azure/quantum/argument_types/types.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/cirq/job.py` & `azure-quantum-0.28.276173b1/azure/quantum/cirq/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/cirq/service.py` & `azure-quantum-0.28.276173b1/azure/quantum/cirq/service.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/cirq/targets/ionq.py` & `azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/cirq/targets/quantinuum.py` & `azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/cirq/targets/target.py` & `azure-quantum-0.28.276173b1/azure/quantum/cirq/targets/target.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,7 +64,11 @@
     @abc.abstractmethod
     def _get_azure_workspace(self) -> "Workspace":
         raise NotImplementedError
 
     @abc.abstractmethod
     def _get_azure_target_id(self) -> str:
         raise NotImplementedError
+
+    @abc.abstractmethod
+    def _get_azure_provider_id(self) -> str:
+        raise NotImplementedError
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/job/base_job.py` & `azure-quantum-0.28.276173b1/azure/quantum/job/base_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/job/filtered_job.py` & `azure-quantum-0.28.276173b1/azure/quantum/job/filtered_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/job/job.py` & `azure-quantum-0.28.276173b1/azure/quantum/job/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 ##
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
+
+
 import logging
 import time
 import json
 
 from typing import TYPE_CHECKING
 
 from azure.quantum._client.models import JobDetails
@@ -29,22 +31,24 @@
     :param workspace: Workspace instance to submit job to
     :type workspace: Workspace
     :param job_details: Job details model,
             contains Job ID, name and other details
     :type job_details: JobDetails
     """
 
+    _default_poll_wait = 0.2
+
     def __init__(self, workspace: "Workspace", job_details: JobDetails, **kwargs):
         self.results = None
         super().__init__(
             workspace=workspace,
             details=job_details,
             **kwargs
         )
-    
+
     def submit(self):
         """Submit a job to Azure Quantum."""
         _log.debug(f"Submitting job with ID {self.id}")
         job = self.workspace.submit_job(self)
         self.details = job.details
 
     def refresh(self):
@@ -73,28 +77,27 @@
         :param timeout_secs: Timeout in seconds, defaults to None
         :type timeout_secs: int, optional
         :param print_progress: Print "." to stdout to display progress
         :type print_progress: bool, optional
         :raises TimeoutError: If the total poll time exceeds timeout, raise
         """
         self.refresh()
-        poll_wait = 0.2
-        total_time = 0.
+        poll_wait = Job._default_poll_wait
+        start_time = time.time()
         while not self.has_completed():
-            if timeout_secs is not None and total_time >= timeout_secs:
+            if timeout_secs is not None and (time.time() - start_time) >= timeout_secs:
                 raise TimeoutError(f"The wait time has exceeded {timeout_secs} seconds.")
- 
+
             logger.debug(
                 f"Waiting for job {self.id},"
                 + f"it is in status '{self.details.status}'"
             )
             if print_progress:
                 print(".", end="", flush=True)
             time.sleep(poll_wait)
-            total_time += poll_wait
             self.refresh()
             poll_wait = (
                 max_poll_wait_secs
                 if poll_wait >= max_poll_wait_secs
                 else poll_wait * 1.5
             )
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/job/session.py` & `azure-quantum-0.28.276173b1/azure/quantum/job/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,18 @@
             raise ValueError("If `session_details` is not passed, you should at least pass the `target`.")
 
         if details is None:
             import uuid
             import re
             id = id if id is not None else str(uuid.uuid1())
             name = name if name is not None else f"session-{id}"
-            provider_id = provider_id if provider_id is not None else re.match(r"(\w+)\.", target_name).group(1)
+            if provider_id is None:
+                match = re.match(r"(\w+)\.", target_name)
+                if match is not None:
+                    provider_id = match.group(1)
             details = SessionDetails(id=id,
                                      name=name,
                                      provider_id=provider_id,
                                      target=target_name,
                                      job_failure_policy=job_failure_policy,
                                      **kwargs)
 
@@ -234,14 +237,18 @@
     def _get_azure_workspace(self) -> "Workspace":
         raise NotImplementedError
 
     @abstractmethod
     def _get_azure_target_id(self) -> str:
         raise NotImplementedError
 
+    @abstractmethod
+    def _get_azure_provider_id(self) -> str:
+        raise NotImplementedError
+
     def open_session(
         self,
         details: Optional[SessionDetails] = None,
         id: Optional[str] = None,
         name: Optional[str] = None,
         job_failure_policy: Union[str, SessionJobFailurePolicy, None] = None,
         **kwargs
@@ -287,10 +294,11 @@
 
         session = Session(details=details,
                           id=id,
                           name=name,
                           job_failure_policy=job_failure_policy,
                           workspace=self._get_azure_workspace(),
                           target=self._get_azure_target_id(),
+                          provider_id=self._get_azure_provider_id(),
                           **kwargs)
         self.latest_session = session
         return session.open()
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/job/workspace_item.py` & `azure-quantum-0.28.276173b1/azure/quantum/job/workspace_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 from azure.quantum._client.models import ItemDetails, ItemType, SessionDetails, JobDetails
 
 if TYPE_CHECKING:
     from azure.quantum.workspace import Workspace
 
 __all__ = ["WorkspaceItem"]
 
+
 class WorkspaceItem(abc.ABC):
     """
 
     :param workspace: Workspace instance to submit job to
     :type workspace: Workspace
     :param item_details: Item details model,
             contains item ID, name and other details
     :type item_details: ItemDetails
     """
 
     def __init__(self, workspace: "Workspace", details: ItemDetails, **kwargs):
         self._workspace = workspace
         self._details = details
-        self._id = details.id
         self._item_type = details.item_type
 
     @property
     def workspace(self) -> "Workspace":
         return self._workspace
 
     @property
     def details(self) -> Union[SessionDetails, JobDetails]:
         return self._details
 
     @property
     def id(self) -> str:
-        return self._id
+        return self._details.id
 
     @property
     def item_type(self) -> ItemType:
         return self._item_type
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/job/workspace_item_factory.py` & `azure-quantum-0.28.276173b1/azure/quantum/job/workspace_item_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/optimization/online_problem.py` & `azure-quantum-0.28.276173b1/azure/quantum/optimization/online_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/optimization/problem.py` & `azure-quantum-0.28.276173b1/azure/quantum/optimization/problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/optimization/solvers.py` & `azure-quantum-0.28.276173b1/azure/quantum/optimization/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/optimization/streaming_problem.py` & `azure-quantum-0.28.276173b1/azure/quantum/optimization/streaming_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/optimization/term.py` & `azure-quantum-0.28.276173b1/azure/quantum/optimization/term.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/backends/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/backends/backend.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,18 @@
 To install run: pip install azure-quantum[qiskit]"
     )
 
 
 class AzureBackendBase(Backend, SessionHost):
     @abstractmethod
     def __init__(
-        self, configuration: BackendConfiguration, provider: Provider = None, **fields
+        self,
+        configuration: BackendConfiguration,
+        provider: Provider = None,
+        **fields
     ):
         super().__init__(configuration, provider, **fields)
 
     @classmethod
     @abstractmethod
     def _default_options(cls) -> Options:
         pass
@@ -197,14 +200,17 @@
 
     def _get_azure_workspace(self) -> "Workspace":
         return self.provider().get_workspace()
 
     def _get_azure_target_id(self) -> str:
         return self.name()
 
+    def _get_azure_provider_id(self) -> str:
+        return self._azure_config()["provider_id"]
+
 
 class AzureQirBackend(AzureBackendBase):
     @abstractmethod
     def __init__(
         self, configuration: BackendConfiguration, provider: Provider = None, **fields
     ):
         super().__init__(configuration, provider, **fields)
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/backends/ionq.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/backends/microsoft.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/microsoft.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/backends/qci.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/qci.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/backends/quantinuum.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/quantinuum.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 ##
 
 from typing import Dict
 from azure.quantum.version import __version__
+import warnings
 
 from .backend import AzureBackend, AzureQirBackend
 from abc import abstractmethod
 from qiskit import QuantumCircuit
 from qiskit.providers.models import BackendConfiguration
 from qiskit.providers import Options
 from qiskit.providers import Provider
@@ -31,15 +32,14 @@
     "y",
     "z",
     "rx",
     "ry",
     "rz",
     "h",
     "cx",
-    "ccx",
     "cz",
     "s",
     "sdg",
     "t",
     "tdg",
     "v",
     "vdg",
@@ -48,14 +48,25 @@
     "reset",
 ]
 
 QUANTINUUM_PROVIDER_ID = "quantinuum"
 QUANTINUUM_PROVIDER_NAME = "Quantinuum"
 
 
+def _get_n_qubits(name):
+    name = name.lower()
+    if ".h1-" in name or "hqs-lt" in name:
+        return 20
+    if ".h2-" in name:
+        return 32
+    warnings.warn(
+        UserWarning(f"Number of qubits not known for target {name}. Defaulting to 20."))
+    return 20
+
+
 class QuantinuumQirBackendBase(AzureQirBackend):
     @abstractmethod
     def __init__(
         self, configuration: BackendConfiguration, provider: Provider = None, **fields
     ):
         super().__init__(configuration, provider, **fields)
 
@@ -69,23 +80,23 @@
             {
                 "provider_id": QUANTINUUM_PROVIDER_ID,
             }
         )
         return config
 
     def _get_n_qubits(self, name):
-        name = name.lower()
-        return 20 if "h1-1" in name or "s1" in name else 12
+        return _get_n_qubits(name)
 
 
 class QuantinuumSyntaxCheckerQirBackend(QuantinuumQirBackendBase):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.hqs-lt-s1-apival", "quantinuum.sim.h1-1sc",
         "quantinuum.hqs-lt-s2-apival", "quantinuum.sim.h1-2sc",
+        "quantinuum.sim.h2-1sc",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
         default_config = BackendConfiguration.from_dict(
@@ -115,14 +126,15 @@
 
 
 class QuantinuumEmulatorQirBackend(QuantinuumQirBackendBase):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.hqs-lt-s1-sim", "quantinuum.sim.h1-1e",
         "quantinuum.hqs-lt-s2-sim", "quantinuum.sim.h1-2e",
+        "quantinuum.sim.h2-1e",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
         default_config = BackendConfiguration.from_dict(
@@ -152,14 +164,15 @@
 
 
 class QuantinuumQPUQirBackend(QuantinuumQirBackendBase):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.hqs-lt-s1", "quantinuum.qpu.h1-1",
         "quantinuum.hqs-lt-s2", "quantinuum.qpu.h1-2",
+        "quantinuum.qpu.h2-1",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
         default_config = BackendConfiguration.from_dict(
@@ -235,23 +248,23 @@
 
         input_data = circuit.qasm()
         workspace = self.provider().get_workspace()
         target = workspace.get_targets(self.name())
         return target.estimate_cost(input_data, num_shots=shots)
 
     def _get_n_qubits(self, name):
-        name = name.lower()
-        return 20 if "h1-1" in name or "s1" in name else 12
+        return _get_n_qubits(name)
 
 
 class QuantinuumSyntaxCheckerBackend(QuantinuumBackend):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.hqs-lt-s1-apival", "quantinuum.sim.h1-1sc",
         "quantinuum.hqs-lt-s2-apival", "quantinuum.sim.h1-2sc",
+        "quantinuum.sim.h2-1sc",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
         default_config = BackendConfiguration.from_dict(
@@ -281,14 +294,15 @@
 
 
 class QuantinuumEmulatorBackend(QuantinuumBackend):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.hqs-lt-s1-sim", "quantinuum.sim.h1-1e",
         "quantinuum.hqs-lt-s2-sim", "quantinuum.sim.h1-2e",
+        "quantinuum.sim.h2-1e",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
         default_config = BackendConfiguration.from_dict(
@@ -318,14 +332,15 @@
 
 
 class QuantinuumQPUBackend(QuantinuumBackend):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.hqs-lt-s1", "quantinuum.qpu.h1-1",
         "quantinuum.hqs-lt-s2", "quantinuum.qpu.h1-2",
+        "quantinuum.qpu.h2-1",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
         default_config = BackendConfiguration.from_dict(
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/backends/rigetti.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/backends/rigetti.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/job.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/provider.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/qiskit/results/resource_estimator.py` & `azure-quantum-0.28.276173b1/azure/quantum/qiskit/results/resource_estimator.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/serialization/problem_pb2.py` & `azure-quantum-0.28.276173b1/azure/quantum/serialization/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/storage.py` & `azure-quantum-0.28.276173b1/azure/quantum/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/__init__.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/ionq.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/job.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/parallel_tempering.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/parallel_tempering.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/population_annealing.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/population_annealing.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
             an increasing evolution (0 < initial < final).
         :param timeout:
             specifies maximum number of seconds to run the core solver
             loop. initialization time does not respect this value, so the
             solver may run longer than the value specified. Setting this value
             will trigger the parameter free population annealing solver.
         """
-
         if timeout is not None:
             name = "microsoft.populationannealing-parameterfree.cpu"
 
         super().__init__(
             workspace=workspace,
             provider_id="Microsoft",
             name=name,
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/quantum_monte_carlo.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/quantum_monte_carlo.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from azure.quantum.target.solvers import Solver
 from azure.quantum.workspace import Workspace
 
 logger = logging.getLogger(__name__)
 
 class QuantumMonteCarlo(Solver):
+
     target_names = [
         "microsoft.qmc.cpu"
     ]
     def __init__(
         self,
         workspace: Workspace,
         name: str = "microsoft.qmc.cpu",
@@ -48,15 +49,14 @@
         :param transverse_field_end:
             ending strength of the external field
         :param beta_start:
             Low starting temp i.e. beta start
         :param restarts:
             Number of simulation runs
         """
-
         super().__init__(
             workspace=workspace,
             provider_id="Microsoft",
             name=name,
             input_data_format="microsoft.qio.v2",
             output_data_format="microsoft.qio-results.v2",
             **kwargs
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/simulated_annealing.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/simulated_annealing.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             solver may run longer than the value specified.
         :param seed:
             specifies a random seed value.
         :platform:
             specifies hardware platform
             HardwarePlatform.CPU.
         """
+        
         param_free = (
             beta_start is None
             and beta_stop is None
             and sweeps is None
             and restarts is None
         )
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/substochastic_montecarlo.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/substochastic_montecarlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 ##
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
+import warnings
 import logging
 
 from typing import Optional
 
 from azure.quantum.target.solvers import RangeSchedule, Solver
 from azure.quantum.workspace import Workspace
 from azure.quantum.job.base_job import ContentType
 
 logger = logging.getLogger(__name__)
 
 class SubstochasticMonteCarlo(Solver):
+
     target_names = (
         "microsoft.substochasticmontecarlo.cpu",
         "microsoft.substochasticmontecarlo-parameterfree.cpu",
     )
     def __init__(
         self,
         workspace: Workspace,
@@ -57,15 +59,14 @@
             Number of steps to attempt for each walker. Must be positive.
         :param timeout:
             Specifies maximum number of seconds to run the core solver
             loop. Initialization time does not respect this value, so the
             solver may run longer than the value specified. Setting this value
             will trigger the parameter free substochastic monte carlo solver.
         """
-
         if timeout is not None:
             name = "microsoft.substochasticmontecarlo-parameterfree.cpu"
         super().__init__(
             workspace=workspace,
             provider_id="Microsoft",
             name=name,
             input_data_format="microsoft.qio.v2",
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/qio/tabu.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/qio/tabu.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from azure.quantum.target.solvers import Solver
 from azure.quantum.workspace import Workspace
 
 logger = logging.getLogger(__name__)
 
 class Tabu(Solver):
+
     target_names = (
         "microsoft.tabu.cpu",
         "microsoft.tabu-parameterfree.cpu"
     )
     def __init__(
         self,
         workspace: Workspace,
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/microsoft/target.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/microsoft/target.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 ##
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
 import re
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, Type
+from typing import Any, Dict, Optional, Type, Union
 from ...job import Job
 from ...job.base_job import ContentType
 from ...workspace import Workspace
 from ..params import InputParams, InputParamsItem, AutoValidatingParams, \
     validating_field
 from ..target import Target
 from . import MicrosoftEstimatorJob
 
 
+class QubitParams:
+    GATE_US_E3 = "qubit_gate_us_e3"
+    GATE_US_E4 = "qubit_gate_us_e4"
+    GATE_NS_E3 = "qubit_gate_ns_e3"
+    GATE_NS_E4 = "qubit_gate_ns_e4"
+    MAJ_NS_E4 = "qubit_maj_ns_e4"
+    MAJ_NS_E6 = "qubit_maj_ns_e6"
+
+
+class QECScheme:
+    SURFACE_CODE = "surface_code"
+    FLOQUET_CODE = "floquet_code"
+
+
+def _check_error_rate(name, value):
+    if value <= 0.0 or value >= 1.0:
+        raise ValueError(f"{name} must be between 0 and 1")
+
+
 @dataclass
 class MicrosoftEstimatorQubitParams(AutoValidatingParams):
     @staticmethod
     def check_instruction_set(name, value):
         if value not in ["gate-based", "gate_based", "GateBased", "gateBased",
                          "Majorana", "majorana"]:
             raise ValueError(f"{name} must be GateBased or Majorana")
-        
+
     @staticmethod
     def check_time(name, value):
         pat = r"^(\+?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?)\s*(s|ms|μs|µs|us|ns)$"
         if re.match(pat, value) is None:
             raise ValueError(f"{name} is not a valid time string; use a "
                              "suffix s, ms, us, or ns")
-
-    @staticmethod
-    def check_error_rate(name, value):
-        if value <= 0.0 or value >= 1.0:
-            raise ValueError(f"{name} must be between 0 and 1")
-
     name: Optional[str] = None
     instruction_set: Optional[str] = validating_field(check_instruction_set)
     one_qubit_measurement_time: Optional[str] = validating_field(check_time)
     two_qubit_joint_measurement_time: Optional[str] = \
         validating_field(check_time)
     one_qubit_gate_time: Optional[str] = validating_field(check_time)
     two_qubit_gate_time: Optional[str] = validating_field(check_time)
     t_gate_time: Optional[str] = validating_field(check_time)
     one_qubit_measurement_error_rate: Optional[float] = \
-        validating_field(check_error_rate)
+        validating_field(_check_error_rate)
     two_qubit_joint_measurement_error_rate: Optional[float] = \
-        validating_field(check_error_rate)
+        validating_field(_check_error_rate)
     one_qubit_gate_error_rate: Optional[float] = \
-        validating_field(check_error_rate)
+        validating_field(_check_error_rate)
     two_qubit_gate_error_rate: Optional[float] = \
-        validating_field(check_error_rate)
-    t_gate_error_rate: Optional[float] = validating_field(check_error_rate)
+        validating_field(_check_error_rate)
+    t_gate_error_rate: Optional[float] = validating_field(_check_error_rate)
 
-    _default_models = ["qubit_gate_us_e3", "qubit_gate_us_e4",
-                       "qubit_gate_ns_e3", "qubit_gate_ns_e4",
-                       "qubit_maj_ns_e4", "qubit_maj_ns_e6"]
+    _default_models = [QubitParams.GATE_US_E3, QubitParams.GATE_US_E4,
+                       QubitParams.GATE_NS_E3, QubitParams.GATE_NS_E4,
+                       QubitParams.MAJ_NS_E4, QubitParams.MAJ_NS_E6]
     _gate_based = ["gate-based", "gate_based", "GateBased", "gateBased"]
     _maj_based = ["Majorana", "majorana"]
 
     def post_validation(self, result):
         # check whether all fields have been specified in case a custom qubit
         # model is specified
         custom = result != {} and \
@@ -81,54 +94,86 @@
             raise LookupError("one_qubit_measurement_error_rate must be set")
 
         # this only needs to be checked for gate based qubits
         if self.instruction_set in self._gate_based:
             if self.one_qubit_gate_time is None:
                 raise LookupError("one_qubit_gate_time must be set")
 
+
 @dataclass
 class MicrosoftEstimatorQecScheme(AutoValidatingParams):
     name: Optional[str] = None
-    error_correction_threshold: Optional[float] = None
+    error_correction_threshold: Optional[float] = \
+        validating_field(_check_error_rate)
     crossing_prefactor: Optional[float] = None
     logical_cycle_time: Optional[str] = None
     physical_qubits_per_logical_qubit: Optional[str] = None
 
 
+@dataclass
+class ErrorBudgetPartition(AutoValidatingParams):
+    logical: float = 0.001 / 3
+    t_states: float = 0.001 / 3
+    rotations: float = 0.001 / 3
+
+
+@dataclass
+class MicrosoftEstimatorConstraints(AutoValidatingParams):
+    @staticmethod
+    def at_least_one(name, value):
+        if value < 1:
+            raise ValueError(f"{name} must be at least 1")
+
+    logical_depth_factor: Optional[float] = validating_field(at_least_one)
+    max_t_factories: Optional[int] = validating_field(at_least_one)
+
+
 class MicrosoftEstimatorInputParamsItem(InputParamsItem):
     """
     Input params for microsoft.estimator target
 
     :ivar error_budget Total error budget for execution of the algorithm
     """
 
     def __init__(self):
         super().__init__()
 
         self.qubit_params: MicrosoftEstimatorQubitParams = \
             MicrosoftEstimatorQubitParams()
         self.qec_scheme: MicrosoftEstimatorQecScheme = \
             MicrosoftEstimatorQecScheme()
-        self.error_budget: Optional[float] = None
+        self.constraints: MicrosoftEstimatorConstraints = \
+            MicrosoftEstimatorConstraints()
+        self.error_budget: Optional[Union[float, ErrorBudgetPartition]] = None
 
     def as_dict(self, validate=True) -> Dict[str, Any]:
         result = super().as_dict(validate)
 
         qubit_params = self.qubit_params.as_dict(validate)
         if len(qubit_params) != 0:
             result["qubitParams"] = qubit_params
 
         qec_scheme = self.qec_scheme.as_dict(validate)
         if len(qec_scheme) != 0:
             result["qecScheme"] = qec_scheme
 
+        constraints = self.constraints.as_dict(validate)
+        if len(constraints) != 0:
+            result["constraints"] = constraints
+
         if self.error_budget is not None:
-            if validate and (self.error_budget <= 0 or self.error_budget >= 1):
-                raise ValueError("error_budget must be value between 0 and 1")
-            result["errorBudget"] = self.error_budget
+            if isinstance(self.error_budget, float) or \
+                    isinstance(self.error_budget, int):
+                if validate and \
+                        (self.error_budget <= 0 or self.error_budget >= 1):
+                    message = "error_budget must be value between 0 and 1"
+                    raise ValueError(message)
+                result["errorBudget"] = self.error_budget
+            elif isinstance(self.error_budget, ErrorBudgetPartition):
+                result["errorBudget"] = self.error_budget.as_dict(validate)
 
         return result
 
 
 class MicrosoftEstimatorParams(InputParams, MicrosoftEstimatorInputParamsItem):
     def __init__(self, num_items: Optional[int] = None):
         InputParams.__init__(
@@ -164,13 +209,35 @@
             input_data_format="qir.v1",
             output_data_format="microsoft.resource-estimates.v1",
             provider_id="microsoft-qc",
             content_type=ContentType.json,
             **kwargs
         )
 
+    def submit(self,
+               input_data: Any,
+               name: str = "azure-quantum-job",
+               input_params: Union[Dict[str, Any], InputParams, None] = None,
+               **kwargs) -> Job:
+        try:
+            from qiskit import QuantumCircuit, transpile
+            from qiskit_qir import to_qir_module
+            from qiskit_qir.visitor import SUPPORTED_INSTRUCTIONS
+            if isinstance(input_data, QuantumCircuit):
+                input_data = transpile(input_data,
+                                       basis_gates=SUPPORTED_INSTRUCTIONS,
+                                       optimization_level=0)
+                (module, _) = to_qir_module(input_data, record_output=False)
+                input_data = module.bitcode
+        finally:
+            return super().submit(input_data, name, input_params, **kwargs)
+
     @classmethod
     def _get_job_class(cls) -> Type[Job]:
         return MicrosoftEstimatorJob
 
+    def _qir_output_data_format(self) -> str:
+        """"Fallback output data format in case of QIR job submission."""
+        return "microsoft.resource-estimates.v1"
+
     def make_params(self, num_items: Optional[int] = None):
         return MicrosoftEstimatorParams(num_items=num_items)
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/oneqbit/solvers.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/oneqbit/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/params.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,19 @@
         result = {}
 
         for name, field in self.__dataclass_fields__.items():
             field_value = self.__getattribute__(name)
             if field_value is not None:
                 # validate field?
                 if validate and "validate" in field.metadata:
-                    field.metadata["validate"].__func__(name, field_value)
+                    func = field.metadata["validate"]
+                    # check for indirect call (like in @staticmethod)
+                    if hasattr(func, "__func__"):
+                        func = func.__func__
+                    func(name, field_value)
 
                 # translate field name to camel case
                 s = sub(r"(_|-)+", " ", name).title().replace(" ", "")
                 attribute = ''.join([s[0].lower(), s[1:]])
                 result[attribute] = field_value
 
         if validate:
@@ -132,14 +136,15 @@
         A function that is called after all individual fields have been
         validated, but before the result is returned.
 
         Here result is the current dictionary.
         """
         pass
 
+
 def validating_field(validation_func, default=None):
     """
     A helper method to declare field for an AutoValidatingParams data class.
     """
     return field(default=default, metadata={"validate": validation_func})
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/quantinuum.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/quantinuum.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         # Note: Target names on the same line are equivalent.
         "quantinuum.hqs-lt-s1",        "quantinuum.qpu.h1-1",
         "quantinuum.hqs-lt-s1-apival", "quantinuum.sim.h1-1sc",
         "quantinuum.hqs-lt-s1-sim",    "quantinuum.sim.h1-1e",
         "quantinuum.hqs-lt-s2",        "quantinuum.qpu.h1-2",
         "quantinuum.hqs-lt-s2-apival", "quantinuum.sim.h1-2sc",
         "quantinuum.hqs-lt-s2-sim",    "quantinuum.sim.h1-2e"
+        "quantinuum.qpu.h2-1",
+        "quantinuum.sim.h2-1sc",
+        "quantinuum.sim.h2-1e",
     )
 
     def __init__(
         self,
         workspace: Workspace,
         name: str = "quantinuum.sim.h1-1sc",
         input_data_format: str = "honeywell.openqasm.v1",
@@ -141,20 +144,24 @@
                         if node.op.name in ["measure", "reset"]:
                             N_m += 1
                         elif node.op.num_qubits == 1:
                             N_1q += 1
                         else:
                             N_2q += 1
 
-        if "-sim" in self.name or "sim.h1-1e" in self.name or "sim.h1-2e" in self.name:
+        import re
+        is_emulator_regex = re.compile("^.*(-sim|-[0-9]*e)$")
+        is_syntax_checker_regex = re.compile("^.*(-apival|-[0-9]*sc)$")
+
+        if is_emulator_regex.match(self.name):
             currency_code = "EHQC"
         else:
             currency_code = "HQC"
 
-        if "apival" in self.name or "sc" in self.name:
+        if is_syntax_checker_regex.match(self.name):
             HQC = 0.0
         else:
             HQC = 5 + num_shots * (N_1q + 10 * N_2q + 5 * N_m) / 5000
 
         return CostEstimate(
             events=[
                 UsageEvent(
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/rigetti/result.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/rigetti/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/rigetti/target.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/rigetti/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,36 +25,32 @@
 
     See https://qcs.rigetti.com/qpus for details on a QPU target.
     """
 
     QVM = "rigetti.sim.qvm"
     """A simulator target for Quil. See https://github.com/quil-lang/qvm for more info."""
 
-    ASPEN_M_2 = "rigetti.qpu.aspen-m-2"
     ASPEN_M_3 = "rigetti.qpu.aspen-m-3"
 
     def simulators() -> List[str]:
         """Returns a list of simulator targets"""
         return [
             RigettiTarget.QVM.value,
         ]
 
     def qpus() -> List[str]:
         """Returns a list of QPU targets"""
         return [
-            RigettiTarget.ASPEN_M_2.value,
             RigettiTarget.ASPEN_M_3.value,
         ]
 
     def num_qubits(target_name) -> int:
         """Returns the number of qubits supported by the given target"""
         if target_name == RigettiTarget.QVM.value:
             return 20
-        elif target_name == RigettiTarget.ASPEN_M_2.value:
-            return 80
         elif target_name == RigettiTarget.ASPEN_M_3.value:
             return 80
         else:
             raise ValueError(f"Unknown target {target_name}")
 
 
 @dataclass
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/solvers.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ##
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
+import warnings
 import logging
 
 from typing import TYPE_CHECKING, Union, Any, Optional
 from enum import Enum
 from azure.quantum.job.base_job import ContentType
 from azure.quantum import Workspace, Job
 from azure.quantum.job.base_job import DEFAULT_TIMEOUT
@@ -112,15 +113,16 @@
         Azure Quantum Workspace.
 
         :param problem:
             The Problem to solve. It can be an instance of a Problem,
             or the URL of an Azure Storage Blob where the serialized version
             of a Problem has been uploaded.
         """
-        
+        if (self.provider_id == "Microsoft"):
+            warnings.warn('Please note that Microsoft QIO solvers will be deprecated and no longer available in Azure Quantum after June 30th 2023.')
         from azure.quantum.optimization import Problem
         if isinstance(problem, Problem):
             self.check_valid_problem(problem)
             return super().submit(
                 input_data=problem,
                 name=problem.name,
                 input_params=self.params,
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/target.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 f"Cannot refresh the Target status: \
 target '{self.name}' of provider '{self.provider_id}' not found."
             )
 
     @property
     def current_availability(self):
         return self._current_availability
-    
+
     @property
     def average_queue_time(self):
         return self._average_queue_time
 
     @staticmethod
     def _encode_input_data(data: Any) -> bytes:
         """Encode input data to bytes.
@@ -137,14 +137,18 @@
             return data
         else:
             stream = io.BytesIO()
             if isinstance(data, dict):
                 data = json.dumps(data)
             stream.write(data.encode())
             return stream.getvalue()
+        
+    def _qir_output_data_format(self) -> str:
+        """"Fallback output data format in case of QIR job submission."""
+        return "microsoft.quantum-results.v1"
 
     def submit(
         self,
         input_data: Any,
         name: str = "azure-quantum-job",
         input_params: Union[Dict[str, Any], InputParams, None] = None,
         **kwargs
@@ -172,15 +176,15 @@
         output_data_format = None
         content_type = None
 
         # If the input_data is `QirRepresentable`
         # we need to convert it to QIR bitcode and set the necessary parameters for a QIR job.
         if input_data and isinstance(input_data, QirRepresentable):
             input_data_format = kwargs.pop("input_data_format", "qir.v1")
-            output_data_format = kwargs.pop("output_data_format", "microsoft.quantum-results.v1")
+            output_data_format = kwargs.pop("output_data_format", self._qir_output_data_format())
             content_type = kwargs.pop("content_type", "qir.v1")
 
             def _get_entrypoint(input_data):
                 # TODO: this method should be part of QirRepresentable protocol
                 # and will later move to the QSharpCallable class in the qsharp package
                 import re
                 method_name = re.search(r"(?:^|\.)([^.]*)$", input_data._name).group(1)
@@ -224,20 +228,23 @@
 
     def supports_protobuf(self):
         """
         Return whether or not the Solver class supports protobuf serialization.
         This should be overridden by Solver subclasses which do support protobuf.
         """
         return False
-    
+
     def estimate_cost(
         self,
         input_data: Any,
         input_params: Union[Dict[str, Any], None] = None
     ):
         return NotImplementedError("Price estimation is not implemented yet for this target.")
 
     def _get_azure_workspace(self) -> "Workspace":
         return self.workspace
 
     def _get_azure_target_id(self) -> str:
         return self.name
+
+    def _get_azure_provider_id(self) -> str:
+        return self.provider_id
```

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/target_factory.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/target_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/target/toshiba/solvers.py` & `azure-quantum-0.28.276173b1/azure/quantum/target/toshiba/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure/quantum/workspace.py` & `azure-quantum-0.28.276173b1/azure/quantum/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure_quantum.egg-info/PKG-INFO` & `azure-quantum-0.28.276173b1/azure_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 0.28.263081
+Version: 0.28.276173b1
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/qdk-python
 Author: Microsoft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `azure-quantum-0.28.263081/azure_quantum.egg-info/SOURCES.txt` & `azure-quantum-0.28.276173b1/azure_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.263081/azure_quantum.egg-info/requires.txt` & `azure-quantum-0.28.276173b1/azure_quantum.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,37 +9,41 @@
 protobuf<4.0,>=3.14.0
 Markdown>=3.4.1
 python-markdown-math>=0.8
 
 [all]
 cirq-core<2.0,>=1.1.0
 cirq-ionq<2.0,>=1.1.0
-azure-devtools<2.0,>=1.2.0
+urllib3==1.26.14
+vcrpy==4.2.1
+azure-devtools==1.2.0
 asyncmock<1.0,>=0.4.0
 qiskit-ionq<1.0,>=0.3.3
 qiskit-terra<1.0,>=0.19.1
 qiskit-qir<0.4,>=0.3.1
 Markdown<4.0,>=3.4.1
 python-markdown-math<1.0,>=0.8.0
-qsharp>=0.27.258160
+qsharp>=0.28.263081
 pyquil>=3.3.2
 
 [cirq]
 cirq-core<2.0,>=1.1.0
 cirq-ionq<2.0,>=1.1.0
 
 [dev]
-azure-devtools<2.0,>=1.2.0
+urllib3==1.26.14
+vcrpy==4.2.1
+azure-devtools==1.2.0
 asyncmock<1.0,>=0.4.0
 
 [qiskit]
 qiskit-ionq<1.0,>=0.3.3
 qiskit-terra<1.0,>=0.19.1
 qiskit-qir<0.4,>=0.3.1
 Markdown<4.0,>=3.4.1
 python-markdown-math<1.0,>=0.8.0
 
 [qsharp]
-qsharp>=0.27.258160
+qsharp>=0.28.263081
 
 [quil]
 pyquil>=3.3.2
```

### Comparing `azure-quantum-0.28.263081/setup.py` & `azure-quantum-0.28.276173b1/setup.py`

 * *Files identical despite different names*

