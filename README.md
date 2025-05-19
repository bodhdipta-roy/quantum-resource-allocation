# Quantum Resource Allocation through Second-Price Auctions

This repository implements a hybrid classical-quantum approach for quantum resource allocation using second-price (Vickrey) auctions as described in the paper "Quantum Resource Allocation through Second-Price Auctions: A Hybrid Classical-Quantum Approach."

## Paper Reference

[Link to paper will be added upon publication]

## Overview

As quantum computing resources remain scarce and expensive, efficient allocation mechanisms are crucial for their optimal utilization. This project implements a second-price auction system for quantum resource allocation, where:

1. The highest bidder wins the resource
2. The winner pays the second-highest bid price
3. This mechanism encourages truthful bidding

The implementation also includes a quantum job execution component that demonstrates how allocated resources would be used to run quantum circuits, specifically creating entangled qubits.

## Key Features

- **Second-Price Auction Mechanism**: Implements the Vickrey auction for resource allocation
- **Quantum Circuit Execution**: Demonstrates post-allocation usage with a 5-qubit entanglement circuit
- **Simulation and Analysis Tools**: Includes visualization and statistical analysis of auction outcomes
- **Multi-simulation Support**: Runs multiple auction scenarios to evaluate mechanism performance

## Requirements

- Python 3.8 or higher
- NumPy
- Qiskit and Qiskit-Aer
- Matplotlib

## Installation

```bash
# Create and activate a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install numpy qiskit qiskit-aer matplotlib
```

## Usage

Run the main script to execute both a single detailed simulation and multiple simulations for statistical analysis:

```bash
python quantum_auction_algorithm.py
```
## Alternative Usage

You can also use the Jupyter Notebook provided in the `notebooks` directory for an interactive experience:

```bash
jupyter notebook notebooks/quantum_auction_analysis.ipynb
```

The program generates:

1. **Detailed Single Simulation Results**:
   - Resource allocations
   - User bids and payments
   - Quantum circuit execution outcomes

2. **Statistical Analysis**:
   - Average winning bids and payments
   - Visualizations of bid distributions
   - Trend analysis across multiple simulations

## Implementation Details

### Auction Mechanism

The core of the implementation is the `QuantumResourceAuction` class which:
- Determines the highest and second-highest bids for each resource
- Allocates resources to the highest bidders
- Calculates payments based on second-highest bids
- Ensures incentive compatibility (truthful bidding)

### Quantum Circuit

After resource allocation, the system executes a 5-qubit quantum circuit that:
- Applies a Hadamard gate to the first qubit to create superposition
- Uses CNOT gates to entangle this qubit with four other qubits
- Measures all qubits to demonstrate the entanglement effects

## Customization

You can modify these parameters in the code:
- `num_resources`: Number of quantum resources available
- `num_users`: Number of users participating in the auction
- `min_bid` and `max_bid`: Range for random bid generation
- `num_simulations`: Number of auction scenarios to run

## Theoretical Basis

The implementation is based on the Vickrey-Clarke-Groves (VCG) mechanism, which:
- Maximizes social welfare
- Encourages truthful bidding as the dominant strategy
- Efficiently allocates resources to those who value them most

## Future Extensions

- Integration with real quantum hardware providers
- Dynamic pricing based on resource quality and availability
- Multi-resource bundle auctions for complex quantum workflows
- Machine learning integration for predictive bidding

## Citation

If you use this code in your research, please cite the original paper:

```
[Will be added upon publication]
```

## Acknowledgments

- Qiskit team for providing the quantum computing framework

## Authors & Contributors

<a href="https://github.com/bodhdipta-roy">
  <img src="https://avatars.githubusercontent.com/bodhdipta-roy" width="100px;" alt="bodhdipta-roy"/>
</a>

<a href="https://github.com/koushiki-das2003">
  <img src="https://avatars.githubusercontent.com/koushiki-das2003" width="100px;" alt="koushiki-das2003"/>
</a>

<a href="https://github.com/Biswarupayan">
  <img src="https://avatars.githubusercontent.com/Biswarupayan" width="100px;" alt="Biswarupayan"/>
</a>

