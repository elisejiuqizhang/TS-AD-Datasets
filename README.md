# Public Datasets for Time Series Anomaly Detection

## Time Series Anomaly Detection Datasets

Here I summarized some datasets publicly available for time series anomaly detection.

### 1. Outlier Detection DataSets (ODDS)

ODDS webpage is [here](http://odds.cs.stonybrook.edu/). Note that the datasets contains not only time series, but also other data types (videos, texts, and graphs).

### 2. Kaggle Credit Card Fraud Detection DataSet (CCFD)

Mainpage is [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). The dataset contains transactions made by credit cards in September 2013 by European cardholders, yet due to privacy and security reasons, what we see is the result of a PCA transformation.

### 3. Yahoo Time Series Anomaly Detection Benchmark

Request access to this dataset [here](https://webscope.sandbox.yahoo.com/catalog.php?datatype=s&did=70).

Contains 4 folders, A1, A2, A3, A4. 

A1Benchmark is based on the real production traffic to some of the Yahoo! properties. The other 3 benchmarks are based on synthetic time-series. A2 and A3 Benchmarks include outliers, while the A4Benchmark includes change-point anomalies. The bechmarks based on real-data have property and geos removed. Fields in each data file are delimited with (",") characters.

### 4. Numenta Anomaly Benchmark (NAB)

Description of NAB can be found [here](https://numenta.com/machine-intelligence-technology/numenta-anomaly-benchmark/).

Dataset repository is [here](https://github.com/numenta/NAB).

### 5. Secure Water Treatment (SWaT) Dataset

Multivariate time series datasets collected by “iTrust, Centre for Research in Cyber Security, Singapore University of Technology and Design”. See website [here](https://itrust.sutd.edu.sg/itrust-labs_datasets/dataset_info/#swat) to request access to the dataset and check usage requirements.

### 6. Water Distribution (WADI) Dataset

Also collected by “iTrust, Centre for Research in Cyber Security, Singapore University of Technology and Design”. See website [here](https://itrust.sutd.edu.sg/itrust-labs_datasets/dataset_info/#wadi) to request access to the dataset (it can actually be requested at the same time as when requesting for SWaT) and check usage requirements.

### 7. Server Machine Dataset (SMD)

Dataset released [here](https://github.com/NetManAIOps/OmniAnomaly/tree/master/ServerMachineDataset) as a part of the authors' repository of their KDD 2019 paper ["Robust Anomaly Detection for Multivariate Time Series through Stochastic Recurrent Neural Network"](https://dl.acm.org/doi/10.1145/3292500.3330672).

### 8. UCR Time Series Anomaly Archive

Contains over 250 datasets. The link to download the dataset is [here](https://www.cs.ucr.edu/~eamonn/time_series_data_2018/). 

The maintainers of the archive also recommend reading the following papers ["The UEA multivariate time series classification archive, 2018" ](https://arxiv.org/abs/1811.00075) and ["Current Time Series Anomaly Detection Benchmarks are Flawed and are Creating the Illusion of Progress"](https://arxiv.org/abs/2009.13807) before using the dataset.

### 9. Soil Moisture Active Passive (SMAP) Satellite Dataset 

Dataset webpage is [here](https://nsidc.org/data/smap/smap-data.html). Check the dataset description [here](https://smap.jpl.nasa.gov/data/?_ga=2.138417011.1712228197.1658525020-1435945832.1658525020).

* The KDD 2018 paper ["Detecting Anomalies in Multivariate Time Series through Stochastic Recurrent Neural Network"](https://arxiv.org/abs/1802.04431) by NASA is the first paper to use this dataset. They provided download link to the dataset in their [repo](https://github.com/khundman/telemanom).

* Note that the authors of ["Robust Anomaly Detection for Multivariate Time Series through Stochastic Recurrent Neural Network"](https://dl.acm.org/doi/10.1145/3292500.3330672) have also used the same versions of SMAP and MSL in their [repo](https://github.com/NetManAIOps/OmniAnomaly)

* The dataset version used by the above two papers can be downloaded using the following commands:

```shell
wget https://s3-us-west-2.amazonaws.com/telemanom/data.zip && unzip data.zip && rm data.zip

cd data && wget https://raw.githubusercontent.com/khundman/telemanom/master/labeled_anomalies.csv
```


### 10. Mars Science Laboratory (MSL) Curiosity Rover Dataset

Dataset webpage is [here](https://pds-atmospheres.nmsu.edu/data_and_services/atmospheres_data/Mars/Mars.html).

* The KDD 2018 paper ["Detecting Anomalies in Multivariate Time Series through Stochastic Recurrent Neural Network"](https://arxiv.org/abs/1802.04431) by NASA is the first paper to use this dataset. They provided download link to the dataset in their [repo](https://github.com/khundman/telemanom).

* Note that the authors of ["Robust Anomaly Detection for Multivariate Time Series through Stochastic Recurrent Neural Network"](https://dl.acm.org/doi/10.1145/3292500.3330672) have also used the same versions of SMAP and MSL in their [repo](https://github.com/NetManAIOps/OmniAnomaly)

* The dataset version used by the above two papers can be downloaded using the following commands:

```shell
wget https://s3-us-west-2.amazonaws.com/telemanom/data.zip && unzip data.zip && rm data.zip

cd data && wget https://raw.githubusercontent.com/khundman/telemanom/master/labeled_anomalies.csv
```

### 11. Skoltech Anomaly Benchmark (SKAB)
Dataset repo is [here](https://github.com/waico/SKAB).

### 12. Artificial Intelligence for IT Operations (AIOps) Challenge Datasets
Datasets maintained by the [Netman Lab](https://netman.aiops.org/) at Tsinghua University, their group's GitHub profile can be found [here](https://github.com/NetManAIOps).

The KPI dataset from their 2018 challenge is [here](https://github.com/NetManAIOps/KPI-Anomaly-Detection), and the 2020 data is [here](https://github.com/NetManAIOps/AIOps-Challenge-2020-Data).

### 13. Pooled Server Metric (PSM) Dataset
This dataset was collected by eBay, and was released [here](https://github.com/eBay/RANSynCoders/tree/main/data) in their repository of an anomaly detection model they proposed named [RANSynCoders](https://github.com/eBay/RANSynCoders).

### 14. PhysioNet Open Access Databases
Check the PhysioNet Data webpage [here](https://physionet.org/about/database/). These datasets are all medicine-related.

One of the datasets [MIT-BIH Supraventricular Arrhythmia Database](https://physionet.org/content/svdb/1.0.0/) was seen used in a VLDB 2022 paper [TranAD: deep transformer networks for anomaly detection in multivariate time series data](https://github.com/imperial-qore/TranAD).


## Time Series Classification Datasets That Could Potentially Be Used for Anomaly Detection

Another common way I see people do is to use time series classification datasets for anomaly detection - you can preprocess the datasets by select one or a few minority classses and label them as anomalies.

### 1. UCI Machine Learning Repository Dataset - Time Series Classification

Look for time series datasets for classification tasks on the UCI repo webpage here [here](https://archive.ics.uci.edu/ml/datasets.php?format=&task=cla&att=&area=&numAtt=&numIns=&type=ts&sort=nameUp&view=table).

### 2. UEA & UCR Time Series Classification Repository
Dataset mainpage is [here](http://www.timeseriesclassification.com/dataset.php).
