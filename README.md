# 3W Dataset

To the best of its authors' knowledge, this is the first realistic and public dataset with rare undesirable real events in oil wells that can be readily used as a benchmark dataset for development of machine learning techniques related to inherent difficulties of actual data.

For more information about the theory behind this dataset, refer to the paper **A realistic and public dataset with rare undesirable real events in oil wells** published in the **Journal of Petroleum Science and Engineering** (link [here](https://doi.org/10.1016/j.petrol.2019.106223)). Specific challenges (benchmarks) that practitioners and researchers can use together with the 3W dataset are defined and proposed in this paper.

# Preamble

This is the supporting repository for the paper mentioned above. If you use the 3W dataset or the proposed benchmarks, please cite the paper and the 3W dataset:
```
@article{VARGAS2019106223,
title = "A realistic and public dataset with rare undesirable real events in oil wells",
journal = "Journal of Petroleum Science and Engineering",
volume = "181",
pages = "106223",
year = "2019",
issn = "0920-4105",
doi = "https://doi.org/10.1016/j.petrol.2019.106223",
url = "http://www.sciencedirect.com/science/article/pii/S0920410519306357",
author = "Ricardo Emanuel Vaz Vargas and Celso José Munaro and Patrick Marques Ciarelli and André Gonçalves Medeiros and Bruno Guberfain do Amaral and Daniel Centurion Barrionuevo and Jean Carlos Dias de Araújo and Jorge Lins Ribeiro and Lucas Pierezan Magalhães",
keywords = "Fault detection and diagnosis, Oil well monitoring, Abnormal event management, Multivariate time series classification",
abstract = "Detection of undesirable events in oil and gas wells can help prevent production losses, environmental accidents, and human casualties and reduce maintenance costs. The scarcity of measurements in such processes is a drawback due to the low reliability of instrumentation in such hostile environments. Another issue is the absence of adequately structured data related to events that should be detected. To contribute to providing a priori knowledge about undesirable events for diagnostic algorithms in offshore naturally flowing wells, this work presents an original and valuable dataset with instances of eight types of undesirable events characterized by eight process variables. Many hours of expert work were required to validate historical instances and to produce simulated and hand-drawn instances that can be useful to distinguish normal and abnormal actual events under different operating conditions. The choices made during this dataset's preparation are described and justified, and specific benchmarks that practitioners and researchers can use together with the published dataset are defined. This work has resulted in two relevant contributions. A challenging public dataset that can be used as a benchmark for the development of (i) machine learning techniques related to inherent difficulties of actual data, and (ii) methods for specific tasks associated with detecting and diagnosing undesirable events in offshore naturally flowing oil and gas wells. The other contribution is the proposal of the defined benchmarks."
}
```
```
Vargas, Ricardo; Munaro, Celso; Ciarelli, Patrick; Medeiros, André; Amaral, Bruno; Barrionuevo, Daniel; Araújo, Jean; Ribeiro, Jorge; Magalhães, Lucas (2019), “Data for: A Realistic and Public Dataset with Rare Undesirable Real Events in Oil Wells”, Mendeley Data, v1. http://dx.doi.org/10.17632/r7774rwc7v.1 
```

If you have questions or want to contribute with this work, please drop me an email at ricardovvargas at gmail dot com.

# 3W Dataset's Structure

The 3W dataset consists of 1,984 CSV files structured as follows. Due to the limitation of GitHub, this dataset is kept in 7z files splited automatically and saved in the `data` directory. Before using 3W dataset, they must be decompressed. After that, the subdirectory names are the instances' labels. Each file represents one instance. The filename reveals its source. All files are standardized as follow. There are one observation per line and one series per column. Columns are separated by commas and decimals are separated by periods. The first column contains timestamps, the last one reveals the observations' labels, and the other columns are the Multivariate Time Series (MTS) (i.e. the instance itself).

# 3W Dataset's Overview

A 3W Dataset's general presentation with some quantities and statistics is available [here](overview.ipynb).

# Experiments for Proposed Benchmarks

The results of the following experiments can be used as baselines. 

- Bechmark 1: Impact of Using Simulated and Hand-Drawn Instances (code and results [here](demo_1_benchmark_impact_of_using_simulated_and_hand-drawn_instances.ipynb)).
- Bechmark 2: Anomaly Detection (code and results [here](demo_2_benchmark_anomaly_detection.ipynb)).

# Citations

If you know any other work that cites the 3W dataset, I will be grateful if you let me know by email (ricardovvargas at gmail dot com).

1) R.E.V. Vargas, C. Munaro, P. Ciarelli. A methodology for generating datasets for development of anomaly detectors in oil wells based on Artificial Intelligence techniques. I Congresso Brasileiro em Engenharia de Sistemas em Processos. 2019. https://www.ufrgs.br/psebr/wp-content/uploads/2019/04/Abstract_A019_Vargas.pdf

2) R.E.V. Vargas. Base de dados e benchmarks para prognóstico de anomalias em sistemas de elevação de petróleo. Universidade
Federal do Espírito Santo. Doctoral thesis. 2019.

3) Yan Li, Tingjian Ge, Cindy Chen. Data Stream Event Prediction Based on Timing Knowledge and State Transitions. PVLDB, 13(10): 1779-1792. 2020. http://www.vldb.org/pvldb/vol13/p1779-li.pdf

4) Tao Lu, Wen Xia, Xiangyu Zou, Qianbin Xia. Adaptively Compressing IoT Data on the Resource-constrained Edge. 3rd {USENIX} Workshop on Hot Topics in Edge Computing (HotEdge 20). 2020. https://www.usenix.org/system/files/hotedge20_paper_lu.pdf

5) Matheus A. Marins, Bettina D. Barros, Ismael H. Santos, Daniel C. Barrionuevo, Ricardo E.V. Vargas, Thiago de M. Prego, Amaro A. de Lima, Marcello L.R. de Campos, Eduardo A.B. da Silva, Sergio L. Netto. Fault detection and classification in oil wells and production/service lines using random forest. Journal of Petroleum Science and Engineering. 2020. https://doi.org/10.1016/j.petrol.2020.107879.

6) W. Fernandes Junior, R.E.V. Vargas, K.S. Komati, K.A. de Souza Gazolli. Detecção de anomalias em poços produtores de petróleo usando aprendizado de máquina. XXIII Congresso Brasileiro de Automática. 2020. 

7) R. Scoralick, B. Barbosa, R.E.V. Vargas, I. Humberto. Detecção de falhas com Stacked Autoencoders e técnicas de reconhecimento de padrões em poços de petróleo operados por gas lift. XXIII Congresso Brasileiro de Automática. 2020. 

8) Jiangguo Liu, Jianli Gu, Huishu Li, Kenneth H. Carlson. Machine learning and transport simulations for groundwater anomaly detection,
Journal of Computational and Applied Mathematics. 2020. https://doi.org/10.1016/j.cam.2020.112982.

9) Eduardo S.P. Sobrinho, Felipe L. Oliveira, Jorel L.R. Anjos, Clemente Gonçalves, Marcus V.D. Ferreira, Lucas G.O. Lopes, William W.M. Lira, João P.N. Araújo, Thiago B. Silva, Lucas P. Gouveia. Uma ferramenta para detectar anomalias de produção utilizando aprendizagem profunda e árvore de decisão. Rio Oil & Gas Expo and Conference 2020. 2020. https://icongresso.ibp.itarget.com.br/arquivos/trabalhos_completos/ibp/3/final.IBP0938_20_27112020_085551.pdf.

10) I.M.N. Oliveira. Técnicas de inferência e previsão de dados como suporte à análise de integridade de revestimentos. Universidade Federal de Alagoas. Master's degree dissertation. 2020.

11) Luiz Müller, Marcelo Ramos Martins. Proposition of Reliability-based Methodology for Well Integrity Management During Operational Phase. 30th European Safety and Reliability Conference and 15th Probabilistic Safety Assessment and Management Conference. 2020. https://doi.org/10.3850%2F978-981-14-8593-0_3682-cd.

12) R.S.F. Nascimento. Detecção de anomalias em poços de produção de petróleo offshore com a utilização de autoencoders e técnicas de reconhecimento de padrões. Universidade Federal de Lavras. Master's degree dissertation. 2021.

13) Taimur Hafeez, Lina Xu, Gavin Mcardle. Edge Intelligence for Data Handling and Predictive Maintenance in IIOT. IEEE Access. 2021. https://ieeexplore.ieee.org/document/9387301.

14) Aurea Soriano-Vargas, Rafael Werneck, Renato Moura, Pedro Mendes Júnior, Raphael Prates, Manuel Castro, Maiara Gonçalves, Manzur Hossain, Marcelo Zampieri, Alexandre Ferreira, Alessandra Davólio, Bernd Hamann, Denis José Schiozer, Anderson Rocha. A visual analytics approach to anomaly detection in hydrocarbon reservoir time series data. Journal of Petroleum Science and Engineering. 2021. https://doi.org/10.1016/j.petrol.2021.108988.

15) Yan Li, Tingjian Ge. Imminence Monitoring of Critical Events: A Representation Learning Approach. International Conference on Management of Data. 2021. https://doi.org/10.1145/3448016.3452804.
