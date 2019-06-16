In order to run the model, please follow the steps as detailed below:

Step 1: Download the 2 (.pkl) scikit-learn models from my google drive and save it to your local disk:

Model 1: 15 most recent day kNN model (Link: https://drive.google.com/open?id=1-4d8Ij5wWFmbZS59TSHweOfQv5ra4q1d)
Model 2: kNN model with 1-day lagged demand as an extra engineered feature
(Link: https://drive.google.com/open?id=1Qwiy4uyXps0Z-PC49ouZgUdXmBoFlAvH)

Step 2: 
Upload the downloaded scikit-learn models to the 'My Drive' directory of your Google drive (drive/My Drive/)

Step 3:
Upload your test data set onto the 'My Drive' directory of your Google drive as testing.csv (drive/My Drive/testing.csv)

Note: 
Make sure that your test data set has the exactly same data structures as the training data provided in order for the algorithm to       run smoothly yet accurately.

The test data set should have the following structures. 

<class 'pandas.core.frame.DataFrame'>
RangeIndex: 150000 entries, 0 to 149999
Data columns (total 4 columns):
geohash6     150000 non-null object
day          150000 non-null int64
timestamp    150000 non-null object
demand       150000 non-null float64
dtypes: float64(1), int64(1), object(2)
memory usage: 4.6+ MB
None


  geohash6  day timestamp    demand
0   qp09d6   32      6:30  0.335199
1   qp02zg   25       1:0  0.042383
2   qp08gm   40      4:30  0.016331
3   qp0974   59      5:45  0.097868
4   qp0973   37      3:45  0.001806
5   qp09sb   24       0:0  0.105745
6   qp09uv   30       3:0  0.304235
7   qp09gx   60     23:30  0.121063
8   qp0d0b   35      8:45  0.000623
9   qp02zj   17     13:30  0.069005

Please include demand column (response variable) in your test data as well, instead of having just the predictors, because they are needed for the algorithm and model to run. 

Step 4:
Go to https://github.com/JasonLimJS/Grab-AI-for-SEA/blob/master/Final%20Algorithm%20to%20Test%20with%20Test%20Data%20Set.ipynb
Open Google Colaboratory then run the code step by step according to the instructions given.

RMSE and predicted values (pandas DataFrame format) would be produced at the end of the session once the code has been completely run.

Step 5:
For further enquiry, please do not hesitate to contact me at jason94lim@gmail.com or +60179898240.

Appendix:
All the thought processes and detailed steps involved in building this model could be found in Jupyter notebook entitled Model_Development_Doc.ipynb (https://github.com/JasonLimJS/Grab-AI-for-SEA/blob/master/Model_Development_Doc.ipynb)

