# 3W Dataset

**Disclaimer: this repository is a WIP (work in progress).**

To the best of its authors' knowledge, this is the first realistic and public dataset with rare undesirable real events in oil wells that can be readily used as a benchmark dataset for development of machine learning techniques related to inherent difficulties of actual data.

For more information about the theory behind this dataset, refer to the paper **A Realistic and Public Dataset with Rare Undesirable Real Events in Oil Wells** published in the **Journal of Petroleum Science and Engineering**. Specific challenges (benchmarks) that practitioners and researchers can use together with the 3W dataset are defined and proposed in this paper.

# Preamble

This is the supporting repository for the paper mentioned above.

Authors: Ricardo Emanuel Vaz Vargas, Celso José Munaro, Patrick Marques Ciarelli, André Gonçalves Medeiros, Bruno Guberfain do Amaral, Daniel Centurion Barrionuevo, Jean Carlos Dias de Araújo, Jorge Lins Ribeiro, Lucas Pierezan Magalhães.

When using the 3W dataset, please cite:
```
@article{article,
author = {Vargas, Ricardo E. V. and Munaro, Celso J. and Ciarelli, Patrick M. and Medeiros, André G. and Amaral, Bruno G. and Barrionuevo, Daniel C. and Araújo, Jean C. D. and Ribeiro, Jorge L. and Magalhães, Lucas P.},
year = {2019},
month = {?},
pages = {?},
title = {A Realistic and Public Dataset with Rare Undesirable Real Events in Oil Wells},
volume = {?},
journal = {Journal of Petroleum Science and Engineering},
doi = {?}
}
```

If you have questions or want to contribute with this work, please drop me an email at ricardovvargas at gmail dot com.

# 3W Dataset's Structure

The 3W dataset consists of 1,984 CSV files structured as follows. Due to the limitation of GitHub, this dataset is kept in 7z files splited automatically and saved in the `data` directory. Before using 3W dataset, they must be decompressed. After that, the subdirectory names are the instances' labels. Each file represents one instance. The filename reveals its source. All files are standardized as follow. There are one observation per line and one series per column. Columns are separated by commas and decimals are separated by periods. The first column contains timestamps, the last one reveals the observations' labels, and the other columns are the Multivariate Time Series (MTS) (i.e. the instance itself).

# 3W Dataset's Overview

A 3W Dataset's general presentation with some quantities and statistics is available [here](overview.ipynb).