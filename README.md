# Spotify Analysis
Personal project to clean, visualize and formulate a KNN model to predict if a song is popular or not. I presented my project at UC Berkeley's Data Science Society Club's project symposium in April of 2022.

# Link to Google Slides:
https://docs.google.com/presentation/d/1Wc1eBcisXemH-hqIt1vjCYLAX44aA1pBN9jV7qCNPI8/edit?usp=sharing

# Link to Deepnote notebook:
https://deepnote.com/workspace/DSS-Rushi-Emma-Justin-Serena-186288fa-eb6b-44a2-8d50-b9093da0e132/project/Spotify-Analysis-03b97c79-68cf-4f10-897d-adffb68056ae/%2Fnotebook.ipynb

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
going through the dataset and deciding what characteristics were going to be useful or not. I decided to drop some characteristics like speechiness, mode, and explicit because their values were 1 or 0, and those values would make it to classify the songs as popular later on. After the data was cleaned I decided to create a heatmap to see what characteristics were related to each other as seen in the image below. Using this heatmap I found that the characteristics of energy, danceability, acousticness, loudness, and liveness would be the best characteristics to choose to perform a K-Nearest-Neighbors analysis to predict if a spotify song was popular or not. After splitting the data into a training and testing set, I calculated the distances between a known popular song and each song in tehe test sets, values for the 5 chosen characteristics noted before. Then comparing the distances to my heuristic each song was split into being popular or not. This was then compared to the songs actual popularity value and I concluded that my algorithm was 86% accurate at determining popularity. 

![image](https://user-images.githubusercontent.com/98563314/169933348-81a943b4-7fbb-4a2f-9401-06a05089270a.png)
