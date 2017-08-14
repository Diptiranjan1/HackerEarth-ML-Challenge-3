# Machine Learning Challenge 3 – HackerEarth

This is a code that we used to get 59 Rank in HackerEarth. It’s a bit lousy due to last minute (literally) top to down changes. But its worth it. And will update with a better version soon.

* [LeadersBoard](https://www.hackerearth.com/challenge/competitive/machine-learning-challenge-3/leaderboard/) - Here is the Ranking

## Details

You are given three files to download: train.csv, test.csv and sample_submission.csv Variables in this data set are anonymized due to privacy. 
The training data is given for 10 days ( 10 Jan 2017 to 20 Jan 2017). The test data is given for next 3 days. 

### Prerequisites



```
Python; Packages – Pandas,Catboost,LightGBM
```


## For details about what has been done check the file Approach.txt


```

PREPROCESSING
1)Initially by making a table between browserid and devid we find that browserid having devid with none value have a single type of device. So we replace it with respective devices.

2)we find leaks in data like siteid = 'IE' and 'Internet Explorer'. We bring these under one category.

3)Fill the none/null values as given in the sample code.


MODEL TRAINING
1) We have 3 models -> CATBOOST 1, LIGHTGBM, CATBOOST 2
2) Data Distribution between these 3 -> CATBOSST 1 -> 4000000
					LIGHTGBM   -> 4000000
					CATBOOST 2 -> 2000000

3) We have made Catboost 1 the strongest followed by lightgbm then catboost 2.
4) Results from each are added according to this equation -
	Probability = (CatBoost1*.41 + Lightgbm*.59)*.41 + Catboost2*.59 

 
```



## Links - 

* [Competition Page](https://www.hackerearth.com/problem/machine-learning/predict-ad-clicks/) - Check here for more detailed description of parameters.
* [Dataset](https://he-s3.s3.amazonaws.com/media/hackathon/machine-learning-challenge-3/predict-ad-clicks/205e1808-6-dataset.zip) – Download the dataset as I havent provided it.



## Team Members
* **Omar Usman Oppal** (https://www.linkedin.com/in/omarusmanuppal/)
* **Karanveer Singh** (https://www.facebook.com/karanveer.singh1)
* **Diptiranjan Harichandan** (https://www.linkedin.com/in/dharichandan/)



# HackerEarth-ML-Challenge-3
# HackerEarth-ML-Challenge-3
