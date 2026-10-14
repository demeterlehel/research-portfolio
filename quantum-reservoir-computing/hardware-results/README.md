# Quantum Hardware Results

## Overview

This project evaluates a six-qubit, time-encoded quantum reservoir computing architecture on IBM's `ibm_brisbane` quantum processor. The six-qubit reservoir is executed on a physical subset of the processor's qubits, enabling a direct comparison between simulated and hardware-based predictions. IBM Brisbane is a superconducting quantum processor based on the Heron architecture, featuring tunable couplers and a heavy-hexagonal connectivity topology. The experiment examines how finite-shot measurement statistics, gate imperfections, and other hardware effects influence the predictive performance of the reservoir.

## Results

### Hardware Prediction Diagnostics

The figure summarizes the model's predictions on the test set, the relationship between predicted and reference values, and the residual errors.

![Hardware prediction diagnostics](figures/ibm_hardware_prediction_diagnostics.png)

### Simulation vs. Hardware

This figure compares the predictive performance obtained in simulation with that measured on real quantum hardware, illustrating the effects of finite-shot measurements and device noise.

![Simulation vs. hardware](figures/simulation_vs_hardware_comparison.png)

## Quantitative Evaluation

| Execution environment | Test RMSE |
|---|---:|
| Ideal simulation | 0.00450 |
| IBM Quantum hardware | 0.01238 |
