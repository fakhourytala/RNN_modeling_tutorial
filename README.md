# RNN Memory Task — Training Code

This repository contains a Jupyter Notebook for training a simple **vanilla Recurrent Neural Network (RNN)** on a toy memory task. The network receives 2‑D inputs (x, y) and learns to produce task‑specific outputs after targets are presented in random order.

> File: `train_rnn.ipynb`

## Features
- Minimal, educational RNN built with **PyTorch**
- Synthetic data generation inside the notebook (no external datasets)
- GPU support if CUDA is available
- Plots of activity and outputs using **matplotlib**

## Getting Started

### 1) Environment
```bash
# Python 3.10+ recommended
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
```

### 2) Install dependencies
```bash
pip install -r requirements.txt
```

### 3) Run the notebook
```bash
# Option A: Jupyter
pip install jupyter
jupyter notebook train_rnn.ipynb

# Option B: JupyterLab (optional)
pip install jupyterlab
jupyter lab train_rnn.ipynb
```

### 4) (Optional) Run as a script
If you prefer running without an interactive UI, you can execute the notebook end‑to‑end with `nbconvert`:

```bash
pip install nbconvert
jupyter nbconvert --to notebook --execute train_rnn.ipynb --output run_output.ipynb
```

This will create `run_output.ipynb` with executed cells, figures, and results.

## Project Structure
```
.
├── train_rnn.ipynb      # Main notebook for data gen, model, training, plots
├── requirements.txt     # Python dependencies
└── README.md            # You are here
```

## Notes & Tips
- **GPU**: The notebook will use CUDA if available (falls back to CPU otherwise).
- **Hyperparameters**: Edit the corresponding cells in the notebook (e.g., learning rate, epochs).
- **Figures**: Plots are generated with matplotlib; you can save them from the notebook.
- **Reproducibility**: Random seeds are set in-code for Python/NumPy/PyTorch where applicable.

## License
Add your preferred license (e.g., MIT) in a `LICENSE` file.

## Citation
If you use this code in academic work, please cite the repository in your methods or acknowledgments.
