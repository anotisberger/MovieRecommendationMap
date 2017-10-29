This repository shows some my analysis of the MovieLens20M dataset. 

I would like to make an app that creates a personalized map of your movie preferences based on a movie recommender system. People enjoy different types of movies, depending on their mood. The classic SVD based movie recommender system does a good job of predicting what rating a user will give to a movie, but does not account for a user wanting to watch different movies at different times. I would like to create an app that identifies the most important movie features for each user, and then creates a 2D map of movies so the user can see the movies grouped by similarity. This application follows naturally from the SVD algorithm. In SVD, movie ratings are broken down into a product of two quantities, user preferences (p) and movie features (q). Each movie has many features - it may be funny, scary, emotional, sci-fi, etc. Each user has a unique preference vector (p) that weighs his or her individual preferences for each of the features described in q. By looking at the features that receive a high value in a given user’s preference vector, it is possible to create a map of movies that have the features they care about. 

I plan on using the MovieLens20M dataset, administered by Grouplens Research. This dataset contains 20 million ratings and 465,000 tag applications applied to 27,000 movies by 138,000 users. It includes tag genome data with 12 million relevance scores across 1,100 tags. 

Data Source:
https://grouplens.org/datasets/movielens/

Plot #1: To verify the premise of my project (that the same user may prefer different movies at different times), I look at how many favorite genres each user has. Most users have 2 or 3 genres that they rate more highly than any other genre. 

Plot #2: I look at the relationship between the percent of movies a user watched in each genre and the average rating he gave to movies in that genre. Not surprisingly, users tend to watch more movies in genres they rate highly. 
