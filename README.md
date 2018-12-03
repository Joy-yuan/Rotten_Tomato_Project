# Rotten_Tomato_Project
<div align="center">
  <img src="https://cals.org/wp-content/uploads/2018/06/movie.jpg"><br><br>
</div>

-----------------
## Group Name: Wonder Women 4.0
## Section: 2

## The Goal of the project: 
#### Analyze the different kinds of movie features & Predict the box_office of future movies based on machine learning models

## What we have been implemented:

#### 1.Scrap data & Data cleaning
The dataset of this project comes from the website “rottentomatoes.com”. We scraped information on top 100 movies from 2000 to 2018, representing popular movies in the past 20 years. Features include (movie) 'name','meter_score','audience_score','rating','genre','cast', 'director','time','studio','runtime', and ‘movie_synopsis’. Our goal is to predict “box_office” based on these features . To quantify  movie,  we created scores for each movie by adding up scores for each cast member and director in the movie, both represented by their corresponding ranking on “imdb.com”.

We also scraped all top reviews from movie critics for each movie from 2014 to 2018.


### 2. Basic Analysis & Visualization 

We analyzed the box office distribution, trend of movie quantities for each genre, rating distribution and director explorations.


### FUN TIME! Know more about your favorite director!
This part allows reader to input the name of his/her favorite director, and a chart indicates the genre and box office preference of this director will be returned.

### 3 Text Mining

For the first part of the text mining, we did the word cloud for all reviews for 500 movies. We use three approaches, including the Hu and Liu’s sentiment analysis lexicon, NRC sentiment data analysis and the Vader analysis to perform the sentiment analysis for those reviews. We work out the rankings of the movies’ reviews and pick up the top four movies for each method. The review word cloud for these four movies are then presented. We conclude that the NRC sentiment data analysis provides a more relatively accurate result for this problem.

In the second, for each of the 500 movies, we conducted text summarization on all reviews. The program generates a short paragraph of summary of reviews for each movie.

In the 'FUN TIME!' section, you will also be able to type in any movie name between 2014 to 2018, and receive the summary of how critics evaluate this movie, given that this movie is in our database.

### 4. Modeling & Prediction

We applied Word Embedding, Lasso, Linear Regression, Random Forest and XGBoost for box office prediction. And finally we choosed XGBoost model for its best performance.

### Fun Time! Let's predict box offices!¶

This part allows reader to input the movie index in our test data set, the predicted box office and real box office will be returned. (The trained XGBoost model could also be used for future box office prediction! But due to the complexity of data preprocessing and Lasso, we decided to use test data to realize this function.)

## Installation instruction:
see requirement.txt for instruction

## Run instruction:
Please go to "Final_Project", then enter "Part II- Analysis+Visualization+Text_mining+Modelling.ipynb". Then, please run all the codes in the file. Please enjoy the fun parts inside. We aslo provide exported html file in the "Final_Project" .

