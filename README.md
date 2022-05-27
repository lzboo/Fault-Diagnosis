# Fault-Diagnosis
Fault Diagnosis Method

## Dataset:
  We used the bearing dataset provided by CWRU and selected some of the data for our experiments.
  * Data source：[CWRU](https://engineering.case.edu/bearingdatacenter/home)
  * data_1:Ten csv files (normal + 9 types of faults), each file contains the data obtained from different positions of the motor (BA/DE/FE) sampled at 12kHZ frequency
  * data_2:Ten csv files (normal + 9 types of faults)

## Method:
  We used two approaches for fault diagnosis: 
  1. **Traditional machine learning approach**：
     * Feature Extract: Construct **4 frequency domain features** + **8 time domain features**
     * Model:KNN / SVM / XGBoost
  2. **Data-driven deep learning approach**：
     * Sampling Timing Data Reconstruction(Two ways):
       1)Converting signals to 2-D images [Paper](https://ieeexplore.ieee.org/abstract/document/8114247)
       2)Wavelet transform of time-series data to generate spectrograms（To be completed）
     * Model:CNN

