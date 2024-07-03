# Quantum Simulations

This repository contains two quantum simulation projects: Quantum State Tomography and Trapped Ion Simulation. These simulations are designed to explore various aspects of quantum systems and their behavior under different conditions.

## Table of Contents

1. [Quantum State Tomography](#quantum-state-tomography)
   - [Overview](#overview)
   - [Features](#features)
   - [Usage](#usage)
   - [Output Interpretation](#output-interpretation)

2. [Trapped Ion Simulation](#trapped-ion-simulation)
   - [Overview](#overview-1)
   - [Features](#features-1)
   - [Usage](#usage-1)
   - [Output Interpretation](#output-interpretation-1)

3. [Requirements](#requirements)
4. [Installation](#installation)
5. [Contributing](#contributing)
6. [License](#license)

## Quantum State Tomography

### Overview

This simulation demonstrates the process of quantum state tomography, which is a method used to reconstruct an unknown quantum state through multiple measurements. It simulates the creation of random quantum states, performs measurements in different bases, and attempts to reconstruct the original state.

### Features

- Creation of random pure quantum states on the Bloch sphere
- Simulation of measurements in X, Y, and Z bases
- Implementation of quantum state tomography
- Visualization of true and reconstructed states on the Bloch sphere
- Calculation of fidelity between true and reconstructed states

### Usage

To run the Quantum State Tomography simulation:

```Use the Jupyter Notebook titled 'Quantum-State-Tomography'```

You can adjust the following parameters in the script:

- `num_desired_results`: Number of states to generate and reconstruct
- `coherence_time`: Total time available for the simulation
- `manipulation_time`: Time taken for each state manipulation

### Output Interpretation

The simulation produces:

1. A plot showing the true (red) and reconstructed (blue) states on Bloch spheres
2. Console output with:
   - Number of results obtained
   - Total time used
   - Coherence time
   - Fidelity of each reconstructed state

Higher fidelity values (closer to 1.0) indicate better reconstruction of the quantum state.

## Trapped Ion Simulation

### Overview

This simulation explores the behavior of trapped ion quantum systems under various noise conditions. It simulates multiple measurements on a qubit in a noisy environment, analyzing how the number of unique results and the entropy of the system change with increasing noise and number of measurements.

### Features

- Simulation of a noisy quantum environment using depolarizing error
- Multiple measurements on a single qubit with intermediate rotations
- Analysis of unique results and entropy for different noise levels
- Visualization of results through plots

### Usage

To run the Trapped Ion Simulation:

```Use the Jupyter Notebook titled 'Trapped-Ion-Simulations'```

You can adjust the following parameters in the script:

- `num_shots`: Number of times to run each experiment
- `p_depol_range`: Range of depolarizing error probabilities to simulate
- `max_measurements`: Maximum number of measurements to perform in a single circuit

### Output Interpretation

The simulation produces two plots:

1. Unique Results vs Number of Measurements: Shows how the number of unique measurement outcomes changes with the number of measurements for different noise levels.
2. Entropy vs Number of Measurements: Illustrates how the entropy of the measurement results changes with the number of measurements for different noise levels.

Higher noise levels (higher `p_depol` values) generally lead to more unique results and higher entropy, indicating increased randomness in the system.

## Requirements

- Python 3.11
- Seaborn
- Matplotlib
- Qiskit (for Trapped Ion Simulation)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/MajorTimberWolf/Quantum-Simulations.git
   ```

2. Create and activate a conda virtual environment
   ```
   conda env create -f environment.yml
   conda activate quantum-simulations-env
   ```

## Contributing

Contributions to improve the simulations or add new features are welcome. Please feel free to submit pull requests or open issues for discussion.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.