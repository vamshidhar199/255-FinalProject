# 255-FinalProject
## Team 15  Walmart Sales Prediction [ Algorithm Track ]
-  Vamshidhar Reddy Parupally - 016001427
-  Tirupati Venkata Sri Sai Rama Raju Penmatsa - 016037047

## Details
- Dataset : https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting
- Colab notebook for Vamshidhar Reddy's Contribution [also included file in github]: 
  https://colab.research.google.com/drive/1PZpK60do4ptjMqOB4-XqOD75bDw2ygNl?usp=sharing
- Colab notebook for Tirupati Venkata Sri Sai Rama Raju's Contribution :
 https://colab.research.google.com/drive/1fGAk9V3JTfaEljtP4_vEmfswIwGbq0gA?usp=sharing
 
- Video Demo :
  https://drive.google.com/drive/folders/1Y_5N2be5BYA1S2c6qlq-oiWD9VdRFNs7?usp=sharing
## Contributors
### Vamshidhar Reddy Parupally - Contribution

![image](https://user-images.githubusercontent.com/42996478/168497651-b2f48906-a070-49ec-98cd-8f07a011b5e4.png)



<hr>

### Tirupati Venkata Sri Sai Rama Raju Penmatsa - Contribution


![Contributions](https://user-images.githubusercontent.com/48201939/167557235-1b5079c3-b64f-49ca-9242-7808dcbb186a.png)


<hr>

### About Dataset
- This project comprises a thorough data analysis, as well as time series analysis and sales forecasting using multiple models.
- The data was collected between 2010 and 2012, and 45 Walmart locations across the country were examined. 

#### Dataset Description
1) Stores: 
- Store: store numbers rangingfrom 1–45.
- Type: store type ‘A’, ‘B’ or ‘C’.
- Size: no. of products available in the particular store ranging from
34,000 to 210,000

2) Sales: 
- Date: The date of the week.
- WeeklySales: sales during that Week.
- Store: The store number 1–45.
- Dept: One of 1–99.
- IsHoliday: Boolean value representing a holiday week or
not.

3) Features: 
- Temperature: Temperature of the region during that week.
- FuelPrice: Fuel Price in that region during that week.
- MarkDown1:5 : Represents the Type of markdown and what quantity was available during that week.
- CPI: Consumer Price Index during that week.
- Unemployment: The unemployment rate during that week in the region of the store

![image](https://user-images.githubusercontent.com/42996478/168496887-a7a8a5d9-77a6-4fac-af17-ed90dfee7c7b.png)

#### Approach 1 and Approach 2 Pre Processing:
- Merged the 3 different csv files to form the actual dataset to make the training easy.
- Correlation analysis,
- ![image](https://user-images.githubusercontent.com/42996478/168496955-966e4713-5fa9-46a5-8274-440442733ce7.png)

- Null value analysis,
- ![image](https://user-images.githubusercontent.com/42996478/168496958-7e1f8893-d6ff-44d9-9d3e-3cefc5625158.png)

- Outlier analysis,
- ![image](https://user-images.githubusercontent.com/42996478/168496963-692a44a1-e700-4e8a-b22c-b60f2db15978.png)
![image](https://user-images.githubusercontent.com/42996478/168496976-6b5a78b9-be49-4672-940a-e17f949a41ba.png)

- Average weekly sales analysis,
![image](https://user-images.githubusercontent.com/42996478/168497020-4e78c7f6-29e9-406d-b986-83ce17d88fc2.png)
![image](https://user-images.githubusercontent.com/42996478/168496988-61b8519f-a8a1-4dc9-8156-0b26bc544cc3.png)
![image](https://user-images.githubusercontent.com/42996478/168496992-a0aeb85a-793f-4288-b4bd-7c98359f1491.png)

- Label encoding

![image](https://user-images.githubusercontent.com/42996478/168497708-d7fd8eeb-127a-4875-ba3e-d8a807550c44.png)

- Marking the NA values as 0 for “MarkDown” ‘s and dropping “CPI” and “Unemployment”
- Removing Anomalies
![image](https://user-images.githubusercontent.com/42996478/168497101-b1606f73-0dbd-4432-8943-c2dfb9c5df67.png)
![image](https://user-images.githubusercontent.com/42996478/168497105-49b1100e-51e5-4d80-b1c0-88ef20731521.png)
![image](https://user-images.githubusercontent.com/42996478/168497109-a51e0b53-9d8b-4e21-b0c5-4ad7833cbc20.png)








### Algorithms used:
#### LSTM (state of the art)

![image](https://user-images.githubusercontent.com/42996478/168497146-eed6af47-6435-4718-a661-1e4ff52716a1.png)
![image](https://user-images.githubusercontent.com/42996478/168497158-b9ef82fc-1feb-4287-9aff-de9e249062a4.png)
![image](https://user-images.githubusercontent.com/42996478/168497153-08deb486-f933-4ae2-b74d-8b715546a2d1.png)


#### Light GBM (Boosting)

![image](https://user-images.githubusercontent.com/42996478/168497209-5e1bb3e8-0852-4723-a62d-fff831f8bb3a.png)

#### XG Boost (Boosting)

![image](https://user-images.githubusercontent.com/42996478/168497234-8a92ffcf-ed78-496e-901f-4ce0e4f5b892.png)

#### ANN [ 5 Different Configurations ]
#### Random Forest Regressor 

![image](https://user-images.githubusercontent.com/42996478/168497244-bb67dcfc-12d1-41ba-a5b5-1aee0603bebd.png)

#### Decision Tree 
#### ExtraTreeRegressor
#### Application of PCA on the data



### Comparison of the models
## Approach 1
![image](https://user-images.githubusercontent.com/42996478/168497307-19b409e6-f218-401b-8c20-b17143e95e05.png)

## Approach 2
![comparision](https://user-images.githubusercontent.com/48201939/167556324-73233c31-4744-4919-95df-39358dcb53a1.png)


## References
- [1] https://www.kaggle.com/code/bhatnagardaksh/walmart-sales-predictionRandom-Forest
- [2] https://medium.datadriveninvestor.com/walmart-sales-data-analysis-sales-prediction-using-multiple-linear-regression-in-r-programming-adb14afd56fb
- [3] https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting/code
- [4] https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting
- [5] https://www.kaggle.com/code/datamany/random-forest-rnn-walmart-sales-forecastMachine-Learning
- [6] https://machinelearningmastery.com/xgboost-for-regression/
- [7] https://www.analyticsvidhya.com/blog/2021/03/introduction-to-long-short-term-memory-lstm/
- [8] https://www.superdatascience.com/blogs/recurrent-neural-networks-rnn-the-vanishing-gradient-problem
- [9] https://www.analyticsvidhya.com/blog/2017/06/which-algorithm-takes-the-crown-light-gbm-vs-xgboost/
- [10] https://www.geeksforgeeks.org/ml-label-encoding-of-datasets-in-python/
- [11] https://towardsdatascience.com/nlp-101-word2vec-skip-gram-and-cbow-93512ee24314
- [12] https://towardsdatascience.com/time-series-data-analysis-resample-1ff2224edec9
- [13] https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775/
- [14] https://towardsdatascience.com/efficient-time-series-using-pythons-pmdarima-library-f6825407b7f0/
- [15] https://www.analyticsvidhya.com/blog/2018/08/auto-arima-time-series-modeling-python-r/

