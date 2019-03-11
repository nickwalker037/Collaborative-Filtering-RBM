# Collaborative-Filtering-RBM
Movie recommendation system built using a Restricted Boltzman Machine based Collaborative Filtering Model 

This notebook consists of an algorithm that recommends movies for a user to watch by finding similar users based on movie ratings. The model makes use of the movielens dataset published by [grouplens](https://grouplens.org/datasets/movielens/). The dataset contains movies, users, and user ratings. 

The output of the RBM model recommends movies similar to the visual below, where a higher output indicates a higher probability that the user will like the movie based on their previous ratings and similar ratings of other people. 

<img src="http://i1380.photobucket.com/albums/ah175/nickwalker037/films_zpshc4dkk4a.png~original"  width="300"> 

Mean Absolute Error is used to measure error and the the model achieves a relatively low error rate of 0.0523 after 15 iterations. 
- Although the error values returned are very low, suggesting a well performing model, the initial weights and biases of the model were initialized with zeros causing the error rate to start at a relatively low value -- i.e. there are 3706 movies in the dataset and users typically only watch below 50 total movies so if the model suggested they do not watch any movies the error value would still be low


This model was constructed as part of the IBM Deep Learning certification via edX
