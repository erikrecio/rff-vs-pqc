# rff-vs-pqc 
Code accompanying the paper  
**“Potential and limitations of random Fourier features for dequantizing quantum machine learning”**  
(Quantum 9, 1640, 2025; DOI: 10.22331/q-2025-02-20-1640)

This repository contains experiments comparing **Random Fourier Features (RFF)** and **Parameterized Quantum Circuits (PQC)**.

## Repository layout

```text
RFF_vs_PQC/
├── .ipynb_checkpoints/         # Jupyter autosave checkpoints
├── Data/                       # Input data and intermediate CSV files
├── Plots/                      # Generated plots and figure outputs
├── __pycache__/                # Python bytecode cache
├── .gitignore
├── Timings code.xlsx           # Timing measurements summary
├── circuits.py                 # Circuit definitions / utilities
├── del_coeffs.py               # Delete/clean Fourier coefficients helper
├── edit_csv.py                 # CSV post-processing helper
├── fourier_coefficients_1D.py  # 1D Fourier coefficient computations
├── fourier_coefficients_dD.py  # d-dimensional Fourier coefficient computations
├── main.py                     # Main experiment entry point
├── main2.py                    # Alternate experiment entry point
├── means_std.py                # Aggregate means / standard deviations
├── plot_circuits.py            # Circuit plotting script
├── plot_histograms.py          # Histogram plotting script
├── plot_histograms copy.py     # Variant of histogram plotting
├── plot_histograms copy 2.py   # Variant of histogram plotting
├── tests.ipynb                 # Notebook-based tests / checks
└── tests.py                    # Script-based tests
```

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -U pip
pip install numpy scipy matplotlib pandas jupyter
```

Install any additional dependencies required by imports in the scripts.

## Typical usage

Run main experiments:

```bash
python main.py
python main2.py
```

Compute Fourier coefficients:

```bash
python fourier_coefficients_1D.py
python fourier_coefficients_dD.py
```

Generate plots:

```bash
python plot_circuits.py
python plot_histograms.py
```

Open notebook tests:

```bash
jupyter notebook tests.ipynb
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

## License

Specify license here (e.g., MIT, Apache-2.0).
