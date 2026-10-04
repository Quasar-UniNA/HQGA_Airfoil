# HQGA for Airfoil Shape Optimization

This repository contains the source code used to perform the experiments presented in the paper:

**Airfoil Shape Optimization using the Hybrid Quantum Genetic Algorithm on Noisy Intermediate-Scale Quantum Computers**

The code integrates the Hybrid Quantum Genetic Algorithm (HQGA) with **XFOIL** for airfoil shape optimization.

The experiment must be executed from the directory containing:

```text
HQGA_Airfoil_Script.py
run_xfoil.sh
NACA0012.dat (optional)
rae2822.dat (optional)
```

The files `eval_obj.in` and `eval_obj.out` are generated automatically during execution and do not need to be provided beforehand.

## Airfoil Selection

The airfoil can be selected using the `AIRFOIL` variable in the Python script:

```python
AIRFOIL = "NACA2412"
```

The available configurations are:

```python
AIRFOIL = "NACA2412"
AIRFOIL = "NACA0012"
AIRFOIL = "RAE2822"
```

For NACA 0012 and RAE 2822, the corresponding baseline geometry files (`NACA0012.dat` and `rae2822.dat`) must be present in the working directory.

## Output

The experiment generates the results in both `.pkl` and `.csv` formats.

