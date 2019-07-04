# Description of the HVG machinery in _scran_

This directory contains some files describing the HVG detection machinery in _scran_.
In `theory/`:

- `description.tex` focuses on the theoretical basis behind `trendVar` and `decomposeVar`.
- `comparison.tex` considers the differences between the possible HVG detection methods in _scran_.

In `real/`:

- `fitTrendVar_test.Rmd` tests the behaviour of the `fitTrendVar()` on a range of scenarios.

In `simulations/`:

- `power` contains simulation scripts to compare the performance of `decomposeVar` with `technicalCV2` and `improvedCV2` for detecting HVGs.
Each simulation script describes a different type of variability, though this is not particularly important for gene-wise testing.
- `alpha` assesses the type I error rate for the tests in `decomposeVar`, `technicalCV2` and `improvedCV2`.
- `filter` examines the motivation for the default filter threshold in `trendVar`.
