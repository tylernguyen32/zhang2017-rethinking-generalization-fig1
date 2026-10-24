# Reproducing Figure 1 of "Understanding Deep Learning Requires Rethinking Generalization" (Zhang et al., ICLR 2017)

## Requirements

Python 3.13 and an NVIDIA GPU (tested on an RTX 3080 Ti).

```
python -m pip install torch torchvision --index-url https://download.pytorch.org/whl/cu130
python -m pip install numpy pandas matplotlib ipykernel
```

CIFAR-10 downloads automatically into `data/` on the first run.

## How to run

1. Open `zhang2017_figure1_reproduction.ipynb` in VS Code (Jupyter extension) or JupyterLab and select the Python environment above.
2. Optional smoke test: set `SMOKE_TEST = True`, restart the kernel and click Run All.
3. Full run: set `SMOKE_TEST = False`, `GPU_BUDGET_HOURS = 7.0` and `DETERMINISTIC = False`, restart the kernel and click Run All. The figure is saved to `results_fig1/figures/figure1.png`.
4. If the run stops, click Run All again. Finished runs are skipped and unfinished runs resume.

The ablation (Section 14) runs at the end of the notebook and saves to `results_fig1_ablation_alexnet/`.
