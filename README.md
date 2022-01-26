# Forest Fires Burned Area Prediction

Predicting the burned area is a **regression** task. In this project, we use the **feature engineering** approaches and **machine learning model** for prediction.  All code and notes are saved in a single ".ipynb" file including  the code for downloading the dataset.

The slides and video of this project presentation  are also provided in this repo. and Bilibili ([机器学习：森林火灾预测 主要的特征工程：被解释变量离散化_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Bi4y1F7fm?spm_id_from=333.999.0.0)), respectively. (plz, allowing my poor English. :)

## Dataset

- The dataset was provided by *UCI Machine Learning resporities* in 2008-02-29.https://archive.ics.uci.edu/ml/datasets/Forest+Fires

- There were 12 input-attributes and 1 output-attribute, including: Weather conditions,Location coordinates, Timestamp, Indexes from Fire Weather Index system and Destroyed area (output)

  <img src="C:\Users\MQL\Pictures\ML\图片7.jpg" alt="图片7" style="zoom:50%;" />

## Methods

Support Vector Regression (SVR) model is suitable for this regression task, while we used data discretization  to predicted attributes turning the continuous numeric variables in different buckets, which increases the granularity by this hashing-like operation, and this approach have lowered the error of prediction. The figure below illustrates two approach by 1) SVR directly, 2) Data Discretization + SVC.

### ![image-20220126203613204](C:\Users\MQL\AppData\Roaming\Typora\typora-user-images\image-20220126203613204.png)

## Metric

We used this two metric to evaluate the model performance.

<img src="C:\Users\MQL\Pictures\ML\图片6.jpg" alt="图片6" style="zoom: 80%;" />

## Results and conclusions

Here, we shown the model with Data Discretization + SVC (The Best Model) and the model with SVR (BASELINE Model). The former model perform well on two both metric. The most important thing is we visualized the predicted result in 3D and found that the predicted result of SVR model has no practical value in reality because all prediction are nearing with zero.

<img src="C:\Users\MQL\Pictures\ML\图片1.jpg" alt="图片1" style="zoom:20%;" />



