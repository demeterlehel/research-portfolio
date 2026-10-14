# Quantum Reservoir Computing for Nonlinear and Chaotic Time Series

This project investigates **time-encoded quantum reservoir computing (QRC)** for predicting nonlinear and chaotic dynamical systems. It explores the use of input-dependent quantum evolution times as an alternative to conventional gate-based input encoding, with the aim of constructing a quantum reservoir whose dynamics can be exploited for time-series prediction.

The project combines numerical simulations, experiments on real quantum hardware, and a thesis documenting the underlying approach and its results. The quantum reservoir uses fixed parameters, while a classical linear readout is trained to map the extracted quantum features to the target dynamics.

## Project Structure

### 1. Simulations

The simulation component investigates the predictive capabilities of the time-encoded reservoir on nonlinear and chaotic benchmark systems, including the Lorenz-63 attractor and the Mackey–Glass delay equation.

The experiments examine one-step-ahead prediction, multi-step forecasting, autonomous closed-loop prediction, and the influence of reservoir configuration and input encoding.

See [`simulations/`](simulations/) for the simulation notebook, figures, and documentation.

### 2. Quantum Hardware

This component evaluates a six-qubit time-encoded quantum reservoir on IBM's `ibm_brisbane` quantum processor, part of the IBM Heron r1 processor family. The processor has 133 physical qubits and uses superconducting qubits with a heavy-hexagonal connectivity topology.

The hardware results are compared with simulation to investigate the effects of finite-shot measurement statistics, gate imperfections, and other device-dependent noise sources on prediction accuracy.

The evaluation yields a test RMSE of approximately **0.01238** on real hardware, compared with **0.00450** in simulation.

See [`hardware/`](hardware/) for the saved diagnostic figures and the simulation-versus-hardware comparison.

### 3. Thesis

This directory contains the Hungarian bachelor's thesis associated with the project and an English translation of its abstract. The thesis provides a more detailed account of the theoretical background, methodology, implementation, and results.

See [`thesis/`](thesis/) for the thesis PDF and the English abstract.

## Methodological Overview

The reservoir's quantum dynamics are driven by an input-dependent evolution time. The quantum circuit itself is not trained; instead, classical information is extracted from quantum measurements and used to fit a linear readout.

The overall workflow consists of:

1. Generating or selecting a nonlinear dynamical time series.
2. Encoding the input into the evolution time of a fixed quantum reservoir.
3. Extracting quantum measurement features.
4. Training a classical linear readout.
5. Evaluating prediction accuracy in simulation and, where available, on physical quantum hardware.

## Research Focus

The project addresses three closely related questions:

- Can time-encoded quantum dynamics provide useful representations for nonlinear time-series prediction?
- How does predictive performance change when the reservoir is evaluated on physical quantum hardware rather than in simulation?
- What limitations arise when a quantum reservoir is used for autonomous forecasting of chaotic dynamics?

Together, the simulations, hardware experiments, and thesis provide complementary perspectives on the potential and practical limitations of time-encoded quantum reservoir computing.

## Reproducibility

The simulation and hardware directories contain the available figures and documentation for their respective experiments. The hardware results are presented as saved outputs; reproducing the physical-device experiments may require access to IBM Quantum services and a compatible backend.
