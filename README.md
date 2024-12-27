# Movie Recommender System

This is a Movie Recommender System built with **Streamlit** and **Machine Learning**. It recommends movies based on the user's selected movie, using a content-based filtering approach, and retrieves posters for each recommended movie through an API.

## Features

- Select a movie from a list of popular movies.
- Get movie recommendations based on a content-based filtering model.
- Display the posters of the recommended movies.
- Deployed on Render for easy access.

## Demo

##### Access the deployed app on Render: https://movie-recommender-ml-t170.onrender.com

## Technologies Used

- **Streamlit**: For building the web interface.
- **Pandas**: For handling movie data.
- **Pickle**: For loading the pre-trained machine learning model and movie data.
- **Requests**: To fetch movie posters from an external API.
- **Render**: For deployment.

## Installation

### Prerequisites

Before running the application locally, make sure you have the following installed:

- Python 3.7+
- Pip (Python package manager)

### Step-by-Step Guide

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Parth-Bisht-227/movie-recommender-ml.git
   
2. Go to the project directory:
   ```bash
   cd movie-recommender-ml
   
3. Create and activate a virtual environment (optional but recommended):

   For Windows:
  ```bash
  python -m venv .venv
  .venv\Scripts\activate
  ```
   For Mac/Linux:
  ```bash
  python3 -m venv .venv
  source .venv/bin/activate
```
4. Install Required Dependencies:
```bash
pip install -r requirements.txt
```
5. Run the StreamLit app
```bash
streamlit run app.py
```
## Files in this Repository
- app.py: Main Streamlit application file.
- movie_dict.pkl: Serialized movie data used by the recommendation system.
- similarity.pkl: Precomputed similarity matrix used for making movie recommendations.
- requirements.txt: Python dependencies required to run the application.

## How It Works
- User Selection: The user selects a movie from a dropdown menu.
- Recommendation Generation: Based on the selected movie, a recommendation system using a content-based filtering approach calculates the similarity between the selected movie and others in the dataset.
- Fetch Movie Posters: The app fetches movie posters from The Movie Database API (TMDb) for each recommended movie.
- Display Results: The app displays the top 5 recommended movies along with their posters.


## Acknowledgments
- The Movie Database (TMDb) API for providing movie data and posters.
- Streamlit for an easy-to-use web framework.
- Pandas for data handling.
- Nitish Sir @campusX -youtube for the helpful tutorial! ✨
