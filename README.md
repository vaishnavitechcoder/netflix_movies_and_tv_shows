# netflix_movies_and_tv_shows

An Unsupervised ML Capstone Project Problem Statement: This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine. We need to do:

Exploratory Data Analysis.
Understanding what type of content is available in different countries.
Is Netflix increasingly focusing on TV rather than movies in recent years?
Clustering similar content by matching text-based features.

![image](https://github.com/vaishnavitechcoder/netflix_movies_and_tv_shows/assets/133495294/cafb87ab-a4d4-41bb-9b98-3091238eb2a8)

WHAT I DID?

The first step I did after importing the dataset is knowing the basic information about the dataset. After that, I planned the Data Wrangling part and Data preprocessing steps. First I converted a date feature that is by default loaded as the object to pandas datetime object so that I can use that feature easily for future purposes as datetime object gives many predefined methods to specifically work with date. Next, I didn't handle the missing values in the dataset, because the missing data appeared in some features with less in numbers so we can use that for EDA which doesn't make any difference. Next thing is I going to use the text-based feature that is "Description" for training machine learning model. These are the reason behind of not handling the missing values. The next step is text preprocessing, before making this feature into a meaningful multi-dimensional vector, I need to do some preprocessing steps which are changing to lowercase, then removing punctual, stopping words and extra white spaces, etc.

Finally, I used the TfidVector to change the text data into numerical, I chose 400 as the maximum features so each review observation will be converted into 400 length features.

Then after converting this vector, the next step is building clustering machine learning models. I tried three different models, the first one is K-means, then I tried Hierarchical Clustering, and finally DBSCAN algorithm.

