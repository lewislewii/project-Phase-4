Recommendation System
Author: group 3

<img width="1387" alt="345150956-5b78dcc5-c8f7-4e63-82b1-22af0f76a7e1" src="https://github.com/lewislewii/project-Phase-4/assets/151353099/44d32f8f-6a2c-455b-b000-6333ca680802">Movies 

Overview
RMX consultancy created a user based and item based collaborative filtering methods on movie lens dataset to create a movie recommendation system for Showmax to:

Accurately recommend top 5 movies
Provide insights and recommendations to Showmax
Create a accurate movie recommendation system using user ratings and viewing history
Business Problem
Showmax is a subscription-based video-on-demand service that aims to provide users with a wide variety of TV shows, movies, and original content for streaming over the internet. Its business revolves around offering entertainment content to subscribers, focusing on convenience, choice, and quality of viewing experience to attract and retain customers in a competitive digital streaming market.

Showmax aims to enhance user engagement and satisfaction by improving its movie recommendation system. The goal is to provide personalized recommendations to users based on their viewing history and preferences, ultimately increasing user retention and content consumption on the platform.

Showmax has tasked RMX Consultancy to enhance its competitive edge against competitors such as Netflix by implementing a personalized movie recommendation system. The goal is to recommend the top 5 movies to users based on their ratings and viewing history, leveraging collaborative filtering techniques to deliver a superior viewing experience.

Data
This dataset (ml-latest-small) describes 5-star rating and free-text tagging activity from MovieLens, a movie recommendation service.
The dataset contains 100,836 ratings and 3,683 tag applications across 9,742 movies. These data were created by 610 users between March 29, 1996 and September 24, 2018. This dataset was generated on September 26, 2018.
Users were selected at random for inclusion. All selected users had rated at least 20 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.
The data are contained in the files links.csv, movies.csv, ratings.csv and tags.csv
ratings.csv:
Contains user ratings for movies.
Format: userId,movieId,rating,timestamp.
Ratings are on a 5-star scale with half-star increments.
Timestamps are in seconds since January 1, 1970 (UTC).
tags.csv:
Contains user-generated tags for movies.
Format: userId,movieId,tag,timestamp.
Tags are single words or short phrases.
Timestamps are in seconds since January 1, 1970 (UTC).
movies.csv:
Contains movie information.
Format: movieId,title,genres.
Titles include release years in parentheses.
Genres are pipe-separated from a predefined set of categories.
links.csv:
Contains identifiers to link to other movie databases.
Format: movieId,imdbId,tmdbId.
movieId corresponds to MovieLens, imdbId to IMDb, and tmdbId to The Movie Databases
Results
Movie Genres Count: Drama was the most common genre with a count of 40,000+ while Film noir being the least common with a count of less than 1,000

image
Ratings Distribution: Majority of the movies had a rating of between 3.5 and 4.0

image
Tags Frequency: For tags used, Netflix, queue, funny, quirky, atmospheric, surreal and superhero are the most common tags used by the users

image
Average Rating per User: Most users gave the movies ratings of between 3.5 and 4.0

image
Average Rating per Movie Year of release: Movies produced after 1980 seems to have generally lower ratings compared to movies produced before 1980

image
Average Rating Across Genres Over the Years: Drama, comedy and musical received higher average ratings in early to mid-20th century. Animation and Fantasy have become popular in recent years. Genres like Documentary, Film-Noir have maintained consistently high ratings over time.

image
Conclusions
The KNNBaseline model successfully recommended top 5 movies for users, considering both predicted ratings and similar movie suggestions.
The item-based collaborative filtering model, while useful, demonstrated lower accuracy compared to the KNNBaseline model done on the user based collaborative filtering.
Integrating it with other methods or using hybrid approaches could enhance the recommendation system’s performance on Showmax.
The tuned KNNBaseline model is more effective in predicting user preferences compared to the initial model.
Improved predictive accuracy translates to more relevant and personalized movie recommendations for users.
Use the KNNBaseline model's recommendations to personalize user experience on Showmax. This can help in engaging users by suggesting movies they are likely to enjoy based on their past ratings.
The KNNBaseline model provided accurate recommendations with higher predicted ratings and lower RMSE, suggesting it may be more effective in recommending top movies compared to KNNwith Mean and SVD
Recommendations
Implement Hybrid Approach: The team is recommended to combine both collaborative filtering and content-based filtering to leverage the strengths of each method to improve the accuracy.
Data Enrichment: Consider using the links.csv dataset to connect to external datasets such as IMDb or TMDb to enrich the movie metadata with more detailed information that can improve the recommendation systems
*Obtain reviews for movies that do not have a sufficient amount of reviews to be deemed reliable to the dataset or consider removing from model
Deal with popularity bias: Increase the representation of less popular movies or undersample the most popular movies
Incorporate more movie features: Recommending movies based other features such as genres, tags might improve the accuracy
Monitor and Retrain: Regularly tune and evaluate the recommendation models with new data to ensure they adapt to changing user preferences and movie trends. This will help maintain the accuracy and relevance of recommendations.
Links to project resources
Presentation - https://github.com/ruth-karimi/Movies-Recommendation-System/blob/main/Movie%20Recommendation%20System.pdf
Code -
Data -
README - https://github.com/ruth-karimi/Movies-Recommendation-System/edit/main/README.md
Repository Structure
image
