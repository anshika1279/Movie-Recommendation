# 🎬 Movie Recommender

A Streamlit-based movie recommendation system that uses TF-IDF vectorization and cosine similarity to suggest movies similar to your selection.

## Features

- 🎯 **Intelligent Recommendations** - Uses TF-IDF and cosine similarity on movie genres, keywords, and overviews
- 🎨 **Beautiful UI** - Built with Streamlit for an intuitive user experience
- 📺 **Movie Details** - Displays plots and posters fetched from OMDB API
- 📊 **Large Dataset** - Works with thousands of movies from the movies.csv dataset

## Tech Stack

- **Python 3.x**
- **Streamlit** - Web framework
- **Scikit-learn** - Machine learning (TF-IDF, cosine similarity)
- **Pandas** - Data manipulation
- **NLTK** - Natural language processing
- **Requests** - HTTP library for OMDB API


## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender
```

2. Install dependencies:
``` bash
pip install -r requirements.txt
```
3. Setup
Before running the app for the first time, you need to preprocess the dataset:
```bash
cd src
python preprocess.py
```
This will:
- Load and clean the movies dataset
- Apply TF-IDF vectorization
- Calculate cosine similarity matrix
- Save processed data to pickle files for quick loading

4. Running the App
Start the Streamlit application:
```bash
cd src
streamlit run main.py
```
5. Configuration
Edit config.json to add your OMDB API key:
```bash
{
  "OMDB_API_KEY": "your_api_key_here"
}
```

## How It Works
1. Preprocessing - The preprocess.py script cleans and combines movie features (genres, keywords, overview)
2. Vectorization - TF-IDF converts text to numerical features
3. Similarity - Cosine similarity compares the selected movie with all others
4. Recommendations - Returns the top 5 most similar movies with posters and plots