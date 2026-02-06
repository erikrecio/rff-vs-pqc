# rff-vs-pqc

Code accompanying the paper  
**“Potential and limitations of random Fourier features for dequantizing quantum machine learning”**  
(Quantum 9, 1640, 2025; DOI: 10.22331/q-2025-02-20-1640)

This repository contains experiments comparing **Random Fourier Features (RFF)** and **Parameterized Quantum Circuits (PQC)**.

## Repository layout

```text
rff-vs-pqc/
├── Data/                 # Input data and intermediate files
├── Plots/                # Generated figure outputs
├── functions/            # Reusable utilities and helper functions
├── scripts/              # Experiment / processing scripts
├── .gitignore
├── README.md
├── main.py               # Main experiment entry point
├── means_std.py          # Aggregate means / standard deviations
└── plot_circuits.py      # Circuit plotting script
```

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -U pip
pip install numpy scipy matplotlib pandas jupyter
```


## Typical usage

Run main experiments:

```bash
python main.py
```

Post-process summary statistics:

```bash
python means_std.py
```

Generate circuit plots:

```bash
python plot_circuits.py
```

## Citation

If you use this code, please cite:

```bibtex
@article{sweke2025rff,
  title   = {Potential and limitations of random Fourier features for dequantizing quantum machine learning},
  author  = {Sweke, Ryan and Recio-Armengol, Erik and Jerbi, Sofiene and Gil-Fuster, Elies and Fuller, Bryce and Eisert, Jens and Meyer, Johannes Jakob},
  journal = {Quantum},
  volume  = {9},
  pages   = {1640},
  year    = {2025},
  doi     = {10.22331/q-2025-02-20-1640}
}
```
