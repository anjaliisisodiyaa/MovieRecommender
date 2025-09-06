
MovieRecommender – ML-Based Movie Recommendation System
## Overview
**MovieRecommender** is a machine learning project that provides personalized movie recommendations based on user-selected movies.  
It uses **content-based filtering** with **cosine similarity** on movie features such as genres, tags, and descriptions.

This project includes:  
- Preprocessed movie dataset  
- Cosine similarity calculation  
- Recommendation engine  
- Saved model/data as .pkl files for easy reuse  
- Interactive user input interface

##  Project Structure

MovieRecommender/
│── notebooks/
│    └── movie_rec.ipynb
│── data/
│    └── movies.csv
│    └── processed_movies.pkl
│── models/
│    └── movie_rec_model.pkl
│── requirements.txt
│── README.md

##  Installation

1. Clone the repository:

git clone https://github.com/anjaliisisodiyaa/MovieRecommender.git
cd MovieRecommender

2. Install dependencies:

pip install -r requirements.txt

##  How to Use

### Using Python Console:

import pandas as pd
from your_module import recommend  # import your recommend function

# Example interactive usage
user_input = input('Enter a movie name: ')
recommended_movies = recommend(user_input)
print('Recommended movies:')
for i, movie in enumerate(recommended_movies, start=1):
    print(f'{i}. {movie}')

### Using saved model and data:

import pickle

# Load model
with open('models/movie_rec_model.pkl', 'rb') as f:
    model = pickle.load(f)

# Load processed data
with open('data/processed_movies.pkl', 'rb') as f:
    df = pickle.load(f)

##  Features

- Content-based movie recommendations  
- Top-N similar movies for any selected movie  
- Interactive user input for recommendations  
- Saves trained model and processed dataset for reuse  

##  Tools & Libraries

- Python 3.x  
- pandas  
- numpy  
- scikit-learn  
- seaborn  
- ast (standard library)  

##  Future Improvements

- Add GUI or web app for interactive recommendations  
- Include collaborative filtering for improved personalization  
- Add movie posters and ratings in recommendations
" > README.md
