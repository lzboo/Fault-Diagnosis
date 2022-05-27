# Fault-Diagnosis
Fault Diagnosis Method

## Dataset:
  We used the bearing dataset provided by CWRU and selected some of the data for our experiments.
  * Data source：[CWRU](https://engineering.case.edu/bearingdatacenter/home)
  * Data: The CWRU dataset is rich, providing sampling data at different motor speeds (4) and at different test positions (3).Fault Diagnosis can be divided into different classification problems:
    * 2 classes = ("normal", "fault")
    * 4 classes = ("normal", "ball", "inner", "outer")
    * 10 classes = ("normal",
                   "ball_18",
                   "ball_36",
                   "ball_54",
                   "inner_18",
                   "inner_36",
                   "inner_54",
                   "outer_18",
                   "outer_36",
                   "outer_54")
   * For the different methods, we constructed two datasets: data1(ML) and data2(ML)
    
## Method:
  We used two approaches for fault diagnosis: 
  1. **Traditional machine learning approach**：
     * Feature Extract: Construct **4 frequency domain features** + **8 time domain features**
     * Model:KNN / SVM / XGBoost
  2. **Data-driven deep learning approach**：
     * Sampling Timing Data Reconstruction(Two ways):
       1) Converting signals to 2-D images [Paper](https://ieeexplore.ieee.org/abstract/document/8114247)
       2) Wavelet transform of time-series data to generate spectrograms（To be completed）
     * Model:CNN

