# LiFi Comparative Analysis: LiFi 1.0 (LED) vs LiFi 2.0 (VCSEL)

Simulation-based comparative study of two Light Fidelity (LiFi) technologies for indoor optical wireless communication: conventional LED-based LiFi (LiFi 1.0) and VCSEL-based LiFi using narrow, steerable Gaussian beams (LiFi 2.0). Developed as part of a Bachelor's thesis (TFG).

## What's here

Two independent, self-contained Jupyter notebooks:

- **[`single_cell_analysis_v5.ipynb`](single_cell_analysis_v5.ipynb)** — compares the LED and VCSEL channel models under a single access point. First at equal transmit power, to isolate the channel model itself, then under each technology's own realistic power constraint (illuminance for the LED, eye safety for the VCSEL), and finally looks at what tiling multiple VCSEL beams within one cell can and can't fix.
- **[`multi_cell_analysis_v2.ipynb`](multi_cell_analysis_v2.ipynb)** — extends the comparison to a multi-access-point deployment: coverage across a range of services, equal-infrastructure and cross-equivalence comparisons, scalability/densification, and inter-cell cooperation.

The two notebooks share the same scenario, channel models, and key parameters (beam waist, eye-safe power, coverage threshold, beam count), so results carry over directly from one to the other. Every non-trivial parameter is grounded in a cited standard or reference paper — see each notebook's own References / Traceability sections for the exact source and equation.

## Repository structure

```
.
├── single_cell_analysis_v5.ipynb   # single-cell comparison
├── multi_cell_analysis_v2.ipynb    # multi-cell / network-level comparison
└── sources/                        # cited reference papers (PDF)
```

## Running the notebooks

Requires Python 3 with `numpy`, `matplotlib`, and `pandas`. Each notebook is fully self-contained — every parameter and helper function is defined inline — so it's enough to open it in Jupyter (or VS Code / JupyterLab) and run all cells top to bottom.

## References

Both notebooks cite the papers and standards behind every modelling choice (channel models, eye-safety limits, capacity bound, etc.) in their own References / Traceability sections, matched against the PDFs in [`sources/`](sources/).
