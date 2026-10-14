# Research Portfolio

This repository presents selected research projects at the intersection of statistical physics, nonlinear dynamics, quantum computing, and philosophy of science. It brings together computational research, experiments in quantum reservoir computing, and philosophical work on the foundations of scientific explanation.

## Projects

### 1. Quantum Reservoir Computing

**Time-Encoded Quantum Reservoir Computing for Nonlinear and Chaotic Time Series**

This project investigates time-encoded quantum reservoir computing (QRC) as an approach to nonlinear time-series prediction. It combines numerical simulations of chaotic dynamical systems with experiments on real quantum hardware, examining the predictive capabilities and practical limitations of fixed quantum reservoirs with trained classical readouts.

The project includes simulation results for the Lorenz-63 attractor and the Mackey–Glass delay equation, a six-qubit implementation evaluated on IBM's `ibm_brisbane` quantum processor, and the associated thesis.

See [`quantum-reservoir-computing/`](quantum-reservoir-computing/).

### 2. Philosophy of Science

**Causal Antifundamentalism and the Base Rate Fallacy**

This project examines John D. Norton's account of causation as folk science, focusing on the negative argument for causal antifundamentalism. It reconstructs the argument as a form of pessimistic induction and argues that, so reconstructed, it commits the base rate fallacy. The analysis combines formal argument reconstruction with probabilistic reasoning and concludes by examining Norton's notion of folk science in relation to the pessimistic meta-induction.

The directory contains the original Hungarian paper and an English translation of its abstract.

See [`philosophy-of-science/`](philosophy-of-science/).

## Research Interests

- Statistical physics and complex systems
- Nonlinear dynamics and chaotic time series
- Quantum reservoir computing and quantum machine learning
- Computational modelling and data-driven approaches to physical systems
- Philosophy of science, scientific explanation, and causation

## Repository Structure

```text
research-portfolio/
├── README.md
├── quantum-reservoir-computing/
│   ├── README.md
│   ├── simulations/
│   ├── hardware/
│   └── thesis/
└── philosophy-of-science/
    ├── abstract_en.md
    └── paper_hu.pdf
