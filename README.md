## Description
Today, social media users are overwhelmed by a large number of posts in their news feed. Moreover, most posts are irrelevant.
Ranking news feed posts by relevance has been proposed to help users catch up with the content they may find interesting. <br/>
For this matter, supervised learning models have been commonly used to predict relevance. However, no comparative study was made to determine the most suitable models. <br />

In this work, knowing that the effectiveness of the prediction of relevance depends partly on the chosen model, 
we select, train, and compare seven supervised learning algorithms applied in this case study. <br />

Extensive experimental results on Twitter highlight that choosing the most suitable supervised model is critical to ensure the effectiveness of the ranking process. Furthermore, the comparison results show that ensemble learning models such as Gradient Boosting and Random Forest are the most appropriate to predict the relevance of news feed posts.

## Prediction of a relevance score

To rank the news feed, supervised prediction models have been proposed to predict the relevance of news feed posts. These models analyze labelled training data of tweets a user has read in the past to predict if the user will find a tweet relevant in the future.

<img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/0-%20Prediction%20of%20a%20relevance%20score.png" alt="Prediction of a relevance score" width="500">

## Input features
The input features that may influence the relevance of a given tweet to a given recipient user.

<img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/1-%20Input%20features.png" alt="Input features" width="650">

## Dataset
We randomly selected 46 Twitter users. Then, we collected data over ten months using Twitter Rest API and simulated the news feed of each user. This resulted in 26180 tweets as well as a 35% interaction rate with tweets and an average of 569 tweets as training data instances for each user.

The full dataset is available [here](https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/all_data.csv), here is below a preview of the data and its statistical description.

<img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/0-%20Dataset%20preview.png" alt="Dataset preview" width="900">

<img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/0-%20Statistical%20description%20of%20the%20data.png" alt="Statistical description of the data" width="900">

## Python code
The Python Jupyter Notebook to read and visualize the data and the code is available on [nbviewer](https://nbviewer.org/github/SamBelkacem/Ranking-social-media-news-feed/blob/main/Comparison%20of%20supervised%20models.ipynb).

## Class distribution
The distribution of the tweets in the dataset by relevance (0: not relevant, 1: relevant).

![Class distribution](https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/1-%20Class%20distribution.png)

## Feature distribution
The distribution of values for the different input features. 

![Feature distribution](https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/2-%20Feature%20distribution.png)

## Comparison of supervised models
To predict the relevance of tweets, we trained and compared seven supervised learning algorithms: 

- Gradient Boosting (GB)
- Random Forest (RF)
- Support Vector Machine (SVM)
- Decision Trees (DT)
- Neural networks (ANN)
- Logistic Regression (LR)
- Naive Bayes (NB)

<div style="text-align: center;">
  <img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/4-%20Comparison%20of%20models.png" width="380" hspace="1"/>
  <img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/5-%20Comparison%20of%20models.png" width="380"/>
</div>

<div style="text-align: center;">
  <img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/3-%20Comparison%20of%20models.png" width="380" hspace="1"/>
  <img src="https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/6-%20Comparison%20of%20models.png" width="380"/>
</div>

## Feature importance
We computed feature importance to see, overall, what features are likely to have importance when judging the relevance of tweets by users.

![Feature importance](https://github.com/SamBelkacem/Ranking-social-media-news-feed/blob/main/Images/7-%20Feature%20importance.png)

## Citation
If you want to use any part of this repository, please cite the following thesis.

```
@phdthesis{belkacem:tel-03201363,
  TITLE = {{Machine learning approaches to rank news feed updates on social media}},
  AUTHOR = {Belkacem, Sami},
  URL = {https://theses.hal.science/tel-03201363},
  SCHOOL = {{Universit{\'e} des Sciences et de la Technologie Houari Boumediene Alger}},
  YEAR = {2021},
  MONTH = Apr,
  KEYWORDS = {Social network Analysis SNA ; Machine learning ML ; News Feed ; Relevance prediction ; Analyse des r{\'e}seaux sociaux SNA ; Apprentissage Automatique ; Flux d'information ; Pr{\'e}diction de la pertinence},
  TYPE = {Theses},
  PDF = {https://theses.hal.science/tel-03201363/file/Thesis.pdf},
  HAL_ID = {tel-03201363},
  HAL_VERSION = {v1},
}
```

## Contact
If you have any question or suggestion, please contact me at this email address: s.belkacem@usthb.dz
