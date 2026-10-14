# Quantum Hardware Results

## Overview

This directory contains results from evaluating a time-encoded quantum reservoir computing model on real IBM Quantum hardware. The experiment investigates whether the predictive performance demonstrated in simulation can be retained when the reservoir is executed on a physical quantum processor.

## Results

### Hardware Prediction Diagnostics

The figure summarizes the model's predictions on the test set, the relationship between predicted and reference values, and the residual errors.

![Hardware prediction diagnostics](figures/hardware_prediction_diagnostics.png)

### Simulation vs. Hardware

This figure compares the predictive performance obtained in simulation with that measured on real quantum hardware, illustrating the effects of finite-shot measurements and device noise.

![Simulation vs. hardware](figures/simulation_vs_hardware.png)

## Quantitative Evaluation

| Execution environment | Test RMSE |
|---|---:|
| Ideal simulation | 0.00450 |
| IBM Quantum hardware | 0.01238 |

The hardware implementation achieves a test RMSE of approximately **0.01238**, compared with **0.00450** in simulation. The hardware error is approximately 2.75 times larger, reflecting the additional challenges associated with physical quantum execution and measurement.

## Key Findings

- **Predictive performance:** The model retains predictive capability when executed on real quantum hardware.
- **Hardware effects:** The higher test error indicates a measurable performance gap between simulation and hardware execution.
- **Practical relevance:** The results provide a benchmark for assessing the feasibility of time-encoded quantum reservoir computing under realistic hardware constraints.
