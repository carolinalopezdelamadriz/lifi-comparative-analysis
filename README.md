# LiFi Comparative Analysis: LiFi 1.0 (LED) vs LiFi 2.0 (VCSEL)

Simulation-based comparative study of two Light Fidelity (LiFi) technologies for indoor optical wireless communication: conventional LED-based LiFi (LiFi 1.0) and VCSEL-based LiFi using narrow, steerable Gaussian beams (LiFi 2.0). Developed as part of a Bachelor's thesis (TFG).

## What's here

Two independent, self-contained Jupyter notebooks:

- **[`single_cell_analysis.ipynb`](single_cell_analysis.ipynb)** — compares the LED and VCSEL channel models under a single access point. First at equal transmit power, to isolate the channel model itself, then under each technology's own realistic power constraint (illuminance for the LED, eye safety for the VCSEL), and finally looks at what tiling multiple VCSEL beams within one cell can and can't fix.
- **[`multi_cell_analysis.ipynb`](multi_cell_analysis.ipynb)** — extends the comparison to a multi-access-point deployment: coverage across a range of services, equal-infrastructure and cross-equivalence comparisons, scalability/densification, and inter-cell cooperation.

The two notebooks share the same scenario, channel models, and key parameters (beam waist, eye-safe power, coverage threshold, beam count), so results carry over directly from one to the other. Every non-trivial parameter is grounded in a cited standard or reference paper — see each notebook's own References / Traceability sections, and [`references.md`](references.md), for the exact source and equation.

## Repository structure

```
.
├── single_cell_analysis.ipynb   # single-cell comparison
├── single_cell_analysis.html    # pre-rendered export, viewable without Jupyter
├── multi_cell_analysis.ipynb    # multi-cell / network-level comparison
├── multi_cell_analysis.html     # pre-rendered export, viewable without Jupyter
└── references.md                # full citations for every paper/standard used
```

## Running the notebooks

Requires Python 3 with `numpy`, `matplotlib`, and `pandas`. Each notebook is fully self-contained — every parameter and helper function is defined inline — so it's enough to open it in Jupyter (or VS Code / JupyterLab) and run all cells top to bottom. If you just want to read the results without running anything, open the `.html` export instead.

## References

Both notebooks cite the papers and standards behind every modelling choice (channel models, eye-safety limits, capacity bound, etc.) in their own References / Traceability sections. The full citation list, with links (DOI or arXiv), is in [`references.md`](references.md) — the papers themselves aren't included in this repo, since most are under IEEE copyright.

## License

MIT — see [LICENSE](LICENSE).
