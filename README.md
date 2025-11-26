# Movie_Recommendation_Project_DE

# Movie Recommendation System

This project is a simple movie recommendation system built using PySpark. The goal is to recommend movies to users based on patterns in their past ratings and similarities between movies.

The system uses two main machine learning models:

1. **ALS (Alternating Least Squares)** – This helps predict how much a user might like a movie they haven’t rated yet.
2. **Word2Vec** – This helps understand how similar movies are to each other based on user behavior.

Together, these two models help provide smarter, more accurate recommendations.

## What This Project Does

* Loads a large movie dataset.
* Trains an ALS model using user ratings.
* Builds a Word2Vec model to capture movie-to-movie relationships.
* Combines both models to recommend movies.
* Evaluates recommendation quality using NDCG.

## Project Flow (in simple words)

1. **Prepare the data:** Read ratings and movie info from parquet files.
2. **Train ALS model:** This learns how users behave — which movies they like or dislike.
3. **Train Word2Vec model:** This looks at groups of movies watched/rated together and learns which movies "go together".
4. **Generate recommendations:** For each user, the system gives a list of movies they are most likely to enjoy.
5. **Evaluate the results:** Uses NDCG@K to check how good the recommendations are.

## Future Enhancements

* **Popularity & Trend Recommender:** Suggest movies that are currently trending.
* **Hybrid Model:** Combine ALS, Word2Vec, and popularity signals to get better recommendations.
* **Improve Evaluation:** Tune hyperparameters like rank, iterations, regularization.
* **Include Movie Metadata:** Use genres, descriptions, and tags to improve accuracy.

## How to Run

Just open the notebook and run cells step‑by‑step on google-colab. Make sure the dataset paths match your local environment.


