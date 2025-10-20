# Movie Recommendation System

## Description
This project implements a movie recommendation system using the MovieLens dataset. It computes item-based and user-based recommendations using cosine similarity. The system allows you to predict ratings and generate top-N recommendations for users.

## Dataset
The MovieLens dataset contains 25 million movie ratings from users, along with movie titles and genres. It’s widely used for building and testing recommendation systems.

Source: [MovieLens Dataset](https://grouplens.org/datasets/movielens/)

## Key Features
- Load and explore the MovieLens dataset.
- Visualize rating distributions per user and per movie.
- Compute item-based and user-based cosine similarity.
- Predict ratings and evaluate performance (RMSE, MAE).
- Generate top-N movie recommendations for any user.

## Requirements
- Python 3.10+
- pandas
- numpy
- scikit-learn
- matplotlib

## Installation
```bash
pip install pandas numpy scikit-learn matplotlib
```

## Usage
- Load the dataset (ensure paths to `ratings.csv` and `movies.csv` are correct).  
- Run the notebook to compute similarities, evaluate predictions, and generate recommendations.  
- Adjust the number of users/movies sampled to fit your memory constraints.

### Example
```python
# Recommend top 5 movies for a user
recommend_movies(user_id=1, n=5, type='item')
recommend_movies(user_id=1, n=5, type='user')
```

## Findings
- The dataset has over 25 million ratings.
- Most users rate a few movies, most movies have few ratings.
- Top-rated and most popular movies can be identified using the system.
