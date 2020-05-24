Movie Recommendation Engine using Content Based Filtering: Project Overview
----

![Source](https://www.google.com/url?sa=i&url=https%3A%2F%2Fdata.world%2Fpriyankad0993%2Ftop-50-imdb-movies-based-on-ratings&psig=AOvVaw2YhCgzoK6hWLm_OgG0p1C-&ust=1590417860110000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCPC4ta7ezOkCFQAAAAAdAAAAABAD)

<img src ='pictures/movies.png' width = '500' height = '350'>

- Using the IMDB movie dataset taken from Kaggle, the aim of this project was to create a recommendation engine using content based filtering(based on the plot of each movie). 

Code and Resources Used:
Python Version: 3.7 
Packages: pandas, numpy, nltk, countvectorizer,matplotlib, seaborn, and sklearn
Dataset: https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset

Data Exploration
-- 
<img src ='pictures/yearly_movies.png' width = '400' height = '250'>

<img src ='pictures/genres.png' width = '400' height = '250'>

<img src ='pictures/studio.png' width = '400' height = '250'>

Data Cleaning
-- 
After reading and exploring the data, I needed to preprocess and clean it up so that it was usable.
Following Changes:
--
- Fill in missing values
- Extracted the necessary columns : title, director, actors, genre, description 
- Using nltk, I preprocessed the description column
- Used count vectorizer because the presence of the actors and directors are essential especially if he/she has acted directly in relatively more movies

Consine Similarity Matrix
--
- computed the consine similarity matrix
- retrieved the index of the movie that matches the title
- sorted the series of the similarity scores
- index the 10 similar movies

Recommendation
---

<img src ='pictures/recommendatons.png' width = '450' height = '300'>


