# Exploring Qiskit — Trotterization experiments

What this is
------------
Simulations and notebooks exploring Trotterized real-time dynamics of the 2D transverse‑field Ising model, comparing 1st, 2nd and 4th order decompositions against exact diagonalization and toy depolarizing noise models. Intended for researchers and students experimenting with small-scale quantum simulation using Qiskit.

Stack
-----
- **Language(s):** Python (notebooks)
- **Runtime:** CPython 3.8+ (Jupyter)
- **Notable libraries:** qiskit (qiskit-terra), qiskit-aer, numpy, matplotlib

How it's organized
------------------


How it fits together
--------------------
The notebooks construct the TFIM Hamiltonian (SparsePauliOp), build Trotter step circuits for different orders (rx and rzz gates), and compare Trotterized evolution (Statevector or density-matrix simulation with AerSimulator) to exact diagonalization from the Hamiltonian eigen-decomposition. Plotting helpers produce magnetization, correlation, and infidelity figures; the noise model is a simple depolarizing channel on single- and two-qubit gates.

How to run
----------
1. Clone the repository and open a Python virtual environment:
   ```bash
   git clone https://github.com/MeghadeepaA/Exploring_qiskit.git
   cd Exploring_qiskit
   python -m venv .venv
   source .venv/bin/activate      # on macOS / Linux
   .venv\Scripts\activate         # on Windows (PowerShell)

   pip install --upgrade pip
pip install qiskit qiskit-aer numpy matplotlib jupyterlab

