# CA05 - kNN Based Movie Recommender Engine

## Author
- **Name:** Jerry Nicholson Hsu
- **Course:** BSAN 6070 - Machine Learning
- **Institution:** Loyola Marymount University
- **Semester:** Spring 2026

## Overview
This project builds a Movie Recommender System using the k-Nearest Neighbors (kNN) algorithm. Given a query movie, the system identifies the 5 most similar movies based on genre features and IMDB ratings.

## Business Question
> Given a movies dataset, what are the 5 most similar movies to a query movie?

## Dataset
- **Source:** UCI IMDB Dataset (via GitHub)
- **File:** `movies_recommendation_data.csv`
- **Size:** 30 movies
- **Features:** IMDB Rating, Biography, Drama, Thriller, Comedy, Crime, Mystery
- **URL:** https://raw.githubusercontent.com/ArinB/MSBA-CA-Data/main/CA05/movies_recommendation_data.csv

## Algorithm
- **Model:** k-Nearest Neighbors (kNN)
- **Library:** scikit-learn `NearestNeighbors`
- **Distance Metric:** Euclidean
- **k value:** 5

## Results
Top 5 movies most similar to **"The Post"** (IMDB: 7.2, Biography, Drama):

| Rank | Movie | Distance |
|------|-------|----------|
| 1 | Queen of Katwe | 0.2000 |
| 2 | The Wind Rises | 0.6000 |
| 3 | 12 Years a Slave | 0.9000 |
| 4 | Hacksaw Ridge | 1.0000 |
| 5 | A Beautiful Mind | 1.0000 |

## Files
- `CA05_kNN_Recommender_Jerry_Hsu.ipynb` - Main Jupyter Notebook
- `movies_recommendation_data.csv` - Dataset (backup copy)
- `README.md` - This file

## How to Run
1. Clone this repository
2. Navigate to the `CA05 - kNN Recommender` folder
3. Open the notebook: `jupyter notebook CA05_kNN_Recommender_Jerry_Hsu.ipynb`
4. Run all cells
> **Note:** If the GitHub URL is not working, replace the url line in Step 2 with: `df = pd.read_csv("movies_recommendation_data.csv")` and make sure the CSV file is in the same folder as the notebook.

## Key Takeaways
- kNN recommends movies by measuring feature similarity using Euclidean distance
- The model only captures similarity based on available features (genres + IMDB rating)
- Factors like directors, actors, and themes are not captured in this dataset
- Real-world systems like Netflix and Amazon use this same core logic at massive scale
