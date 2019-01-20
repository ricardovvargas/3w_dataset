# 3W Dataset

**Disclaimer: this repository is WIP (work in progress).**

This is the first realistic and public dataset with rare undesirable real events in oil wells as far as the authors of this work know. It can be used in development of several kinds of techniques and methods for different tasks associated with undesirable events in oil and gas wells.

For more information about the theory behind this dataset, refer to the paper **A Realistic and Public Dataset with Rare Undesirable Real Events in Oil Wells** published in the **Journal of Petroleum Science and Engineering**.

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

# Dataset Structure

The 3W dataset consists of 1,984 CSV files structured as follows. Due to the limitation of GitHub, this dataset is kept in 7z files splited automatically and saved in the `data` directory. Before using 3W dataset, they must be decompressed. After that, the subdirectory names are the labels of instances. Each file represents one instance. The filename reveals its source. In each file, there are one observation per line and one series per column. Columns are separated by commas and decimals are separated by periods. The first column contains timestamps, the last one reveals labels of observations and the other columns are the Multivariate Time Series (MTS).

# Demonstrations

This repository also contains the following demonstrations about 3W dataset in the folder `demos`:

- [Demonstration 1](demos/demo_1_general_presentation.ipynb): general presentation with some quantities and statistics;
- Demonstration 2: importance of simulated and drawn instances;
- Demonstration 3: example of anomaly detection implementation;
- Demonstration 4: example of early classification implementation.
