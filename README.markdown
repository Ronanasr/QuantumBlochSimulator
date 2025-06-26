# QuantumBlochSimulator: Quantum Gate Simulation on a Single Qubit

## Overview
This project, QuantumBlochSimulator, demonstrates the application of basic quantum gates (Hadamard, Pauli-X, and Rotation) on a single qubit using the QuTiP library in Python. The evolution of the qubit's state is visualized on the Bloch sphere, showcasing fundamental quantum mechanics concepts such as superposition and state rotation. This project is designed as an educational tool for undergraduate physics students exploring quantum computing.

## Prerequisites
- **Python**: Version 3.8 or higher
- **Libraries**:
  - QuTiP (`pip install qutip`)
  - NumPy (`pip install numpy`)
  - Matplotlib (`pip install matplotlib`)

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install the required libraries:
   ```bash
   pip install qutip numpy matplotlib
   ```

## Usage
1. Run the script `qubit_simulation.py`:
   ```bash
   python qubit_simulation.py
   ```
2. The script generates a Bloch sphere plot showing the initial qubit state (|0>) and the states after applying the Hadamard, Pauli-X, and Rotation (π/4) gates. The plot is displayed and saved as `bloch_sphere.png`.

## Project Details
- **Initial State**: The qubit is initialized in the |0> state.
- **Quantum Gates**:
  - **Hadamard Gate**: Creates a superposition state (|0> + |1>)/√2.
  - **Pauli-X Gate**: Flips the qubit state from |0> to |1>.
  - **Rotation Gate**: Rotates the qubit state around the x-axis by π/4, implemented using the formula Rx(θ) = cos(θ/2)I - i*sin(θ/2)σx.
- **Visualization**: The Bloch sphere visualizes the qubit states with distinct colors (blue, red, green, purple) and labels for each state, configured using QuTiP's `point_color` attribute.

## Results
The output is a Bloch sphere plot displaying:
- The initial state (|0>) in blue.
- The state after the Hadamard gate in red.
- The state after the Pauli-X gate in green.
- The state after the rotation gate in purple.

A sample output is saved as `bloch_sphere.png` in the project directory.

## References
- QuTiP Documentation: [http://qutip.org/docs/latest/](http://qutip.org/docs/latest/)
- Nielsen, M. A., & Chuang, I. L. (2010). *Quantum Computation and Quantum Information*.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
