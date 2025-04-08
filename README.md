Movie Recommendation System
This is a content-based movie recommendation 
system built using Python and pandas, 
utilizing a movie metadata dataset 
(including genres, keywords, cast, crew, 
and overview). It helps users find similar movies 
based on their preferences.


           
Project Overview

This project combines two datasets:

movies.csv: Contains metadata like budget, genres, overview, release date, etc.
credits.csv: Contains cast and crew details.

The goal is to merge and process this data 
to generate a recommendation system that suggests 
movies similar to the one a user selects.

         Technologies Used:

Python 3
Pandas
NumPy
Seaborn / Matplotlib
Scikit-learn (for vectorization and similarity scoring)
Jupyter Notebook

           Steps Involved:
1. Data Loading and Cleaning
Load movies.csv and credits.csv
Merge on title
Handle missing values and clean columns

2. Feature Selection

Selected features: genres, keywords, overview, 
cast, crew, and title

3. Data Transformation

Convert JSON-style string columns into usable 
Python lists

Extract relevant names from nested structures

4. Tag Creation

Combine all relevant text fields into a single
string ("tags")

Lowercase conversion and whitespace removal

4. Tag Creation

Combine all relevant text fields into a single string ("tags")

Lowercase conversion and whitespace removal

5. Text Vectorization

Use CountVectorizer from scikit-learn to convert 
text into vectors

Apply cosine similarity for distance calculation

6. Recommendation Function

Input a movie title and return top N similar movie 
suggestions based on content

Function Example :

recommend("Avatar")

Output:

1. John Carter  
2. The Avengers  
3. The Dark Knight Rises  
4. Battleship  
5. 300: Rise of an Empire


