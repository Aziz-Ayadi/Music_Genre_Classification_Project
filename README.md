# Music Genre Classification Project : Project Overview
* Created a machine learning project that tends to classify a user's playlist of songs by genre according to their musical characteristics with a testing accuracy equals to 55.17 %.
* Collected the data to work with from kaggle website (from a competition called `Music Genre Classification 2023|A`) already divided in train and test sets.
* Cleaned data up and engineered features so they will help us in the prediction process like transforming duration in minutes or milliseconds into another feature that holds the same information but only in minutes.
* Optimized Logistic Regression, Decision Tree Classifier, Random Forest Classifier, Support Vector Machines (SVM), K-Neighbors Classifier, Gaussian Naive Bayes, Linear SVC, Gradient Boosting Classifier, Stochastic Gradient Descent Classifier, Perceptron and XgBoost classifiers to get the best training performance and the best estimator.

## Code and resources used
<b>Python Version :</b> 3.9<br>
<b>Packages :</b> Numpy, Pandas, Matplotlib, Seaborn, Scikit-learn, XgBoost<br>
<b>For Web Framework Requirements :</b> `pip install -r requirements.txt`

## Data Collection
Collect data from kaggle website so that training dataset has 14396 songs and test dataset has 3600 songs. With each diamond, we got the folowing :
* Track's ID
* Name of artist or artists who made the track
* Song's name
* The total number of plays the track has had and how recent those plays are
* How suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity
* A perceptual measure of intensity and activity
* The key the track is in
* The overall loudness of a track in decibels (dB)
* The modality (major or minor) of a track, the type of scale from which its melodic content is derived
* The presence of spoken words in a track
* Whether the track is acoustic
* Whether a track contains no vocals
* The presence of an audience in the recording
* A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track
* The overall estimated tempo of a track in beats per minute (BPM)
* Duration of a given track whether in minutes or milliseconds
* A written indicator that shows the number of beats per measure and the type of note that carries the beat in a piece of music
* Track's genre

## Data Cleaning
Clean the data up so that it was usable for our model. I made the following changes and created the following variables:
* Imputing missing values using the appropriate method in both training and test sets for Popularity, key & instrumentalness features
* Encoding categorical features and transforming them to be numerical using a label encoder
* Dropping useless features
* Creating 5-point buckets for popularity feature
* Transforming duration feature into another one that holds the same information but only in minutes
* Standardizing float features using a standard scaler
* Dropping outliers
* Dropping duplicates within Artist and Track Name features

## EDA
I looked at the distributions of the data and the value counts for the various categorical variables to get meaningful insights from our data. Below are the visualizations I made :<br><br>
