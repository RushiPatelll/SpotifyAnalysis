# Spotify Analysis
Personal project to clean, visualize and formulate a KNN model to predict if a song is popular or not.

# The Dataset
The dataset can be found here: https://www.kaggle.com/datasets/ektanegi/spotifydata-19212020
This dataset inclues songs from 1921-2020. There are over 160,000 songs and each song is attributed with different chracteristics, which are:
- acousticness
- danceability
- energy
- duration
- instrumentalness
- valence
- popularity
- tempo
- liveness
- loudness
- speechiness
- year
- mode
- explicit
- key
- artists
- name

# Goals
My goal for this project was to go through the data science lifecycle on this dataset by first
going through the dataset and deciding what characteristics were going to be useful or not. I decided to drop some characteristics like speechiness, mode, and explicit because their values were 1 or 0, and those values would make it to classify the songs as popular later on. After the data was cleaned I decided to create a heatmap to see what characteristics were related to each other as seen in the image below. Using this heatmap I found that the characteristics of energy, danceability, acousticness, loudness, and liveness would be the best characteristics to choose to perform a K-Nearest-Neighbors analysis to predicts if a spotify song was popular or not.

![image](https://user-images.githubusercontent.com/98563314/169933348-81a943b4-7fbb-4a2f-9401-06a05089270a.png)
