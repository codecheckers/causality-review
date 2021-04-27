# CODECHECK

This directory contains the CODECHECK ([codecheck.org.uk](https://codecheck.org.uk)) for the code underlying the article "Causality indices for bivariate time series data:a comparative review of performance" by Tom Edinburgh, Stephen J. Eglen, and Ari Ercole (see parent directory).

To regenerate the CODECHECK report, run `make codecheck.pdf`. The report generation requires a number of Python packages, you can create a [conda environment](https://docs.conda.io/) from the environment file `environment.yml`. E.g., if you have access to the `conda` package manager, you can run the following sequence of statements:
```console
$ conda env create -f environment.yml
$ conda activate codecheck-env 
$ make codecheck.pdf
```

Note that you will also need a LaTeX distribution (e.g. [TeX Live](https://www.tug.org/texlive/)) that provides `xelatex` and several other packages.
