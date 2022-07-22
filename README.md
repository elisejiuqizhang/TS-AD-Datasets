# Public Datasets for Time Series Anomaly Detection

Here I summarized some datasets publicly available for time series anomaly detection.

## 1. Yahoo Time Series Anomaly Detection Benchmark

Request access to this dataset [here](https://webscope.sandbox.yahoo.com/catalog.php?datatype=s&did=70).

Contains 4 folders, A1, A2, A3, A4. 

A1Benchmark is based on the real production traffic to some of the Yahoo! properties. The other 3 benchmarks are based on synthetic time-series. A2 and A3 Benchmarks include outliers, while the A4Benchmark includes change-point anomalies. The bechmarks based on real-data have property and geos removed. Fields in each data file are delimited with (",") characters.

## 2. Numenta Anomaly Benchmark (NAB)

Description of NAB can be found [here](https://numenta.com/machine-intelligence-technology/numenta-anomaly-benchmark/).

Dataset repository is [here](https://github.com/numenta/NAB).

## 3. Secure Water Treatment (SWaT) Dataset

Multivariate time series datasets collected by “iTrust, Centre for Research in Cyber Security, Singapore University of Technology and Design”. See website [here](https://itrust.sutd.edu.sg/itrust-labs_datasets/dataset_info/#swat) to request access to the dataset and check usage requirements.

## 4. Water Distribution (WADI) Dataset

Also collected by “iTrust, Centre for Research in Cyber Security, Singapore University of Technology and Design”. See website [here](https://itrust.sutd.edu.sg/itrust-labs_datasets/dataset_info/#wadi) to request access to the dataset (it can actually be requested at the same time as when requesting for SWaT) and check usage requirements.

## 5. Server Machine Dataset (SMD)

Dataset released [here](https://github.com/NetManAIOps/OmniAnomaly/tree/master/ServerMachineDataset) as a part of the authors' repository of their KDD 2019 paper ["Robust Anomaly Detection for Multivariate Time Series through Stochastic Recurrent Neural Network"](https://dl.acm.org/doi/10.1145/3292500.3330672).

## 6. UCR Time Series Anomaly Archive

Contains over 250 datasets. The link to download the dataset is [here](https://www.cs.ucr.edu/~eamonn/time_series_data_2018/). 

The maintainers of the archive also recommend reading the following papers ["The UEA multivariate time series classification archive, 2018" ](https://arxiv.org/abs/1811.00075) and ["Current Time Series Anomaly Detection Benchmarks are Flawed and are Creating the Illusion of Progress"](https://arxiv.org/abs/2009.13807) before using the dataset.

## 7. Soil Moisture Active Passive (SMAP) Satellite Dataset 

Dataset webpage is [here](https://nsidc.org/data/smap/smap-data.html). Check the dataset description [here](https://smap.jpl.nasa.gov/data/?_ga=2.138417011.1712228197.1658525020-1435945832.1658525020).

* Note that the authors of ["Robust Anomaly Detection for Multivariate Time Series through Stochastic Recurrent Neural Network"](https://dl.acm.org/doi/10.1145/3292500.3330672) have also provided a download link in their [repo](https://github.com/NetManAIOps/OmniAnomaly) - see their "Get data" section:

        You can get the public datasets (SMAP and MSL) using:
        ```shell
        wget https://s3-us-west-2.amazonaws.com/telemanom/data.zip && unzip data.zip && rm data.zip

        cd data && wget https://raw.githubusercontent.com/khundman/telemanom/master/labeled_anomalies.csv
        ```


## 8. Mars Science Laboratory (MSL) Curiosity Rover Datasets

* Note that the authors of ["Robust Anomaly Detection for Multivariate Time Series through Stochastic Recurrent Neural Network"](https://dl.acm.org/doi/10.1145/3292500.3330672) have also provided a download link in their [repo](https://github.com/NetManAIOps/OmniAnomaly) - see their "Get data" section:

        You can get the public datasets (SMAP and MSL) using:
        ```shell
        wget https://s3-us-west-2.amazonaws.com/telemanom/data.zip && unzip data.zip && rm data.zip

        cd data && wget https://raw.githubusercontent.com/khundman/telemanom/master/labeled_anomalies.csv
        ```

