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


## Running the App
Start the Streamlit application:
```bash
cd src
streamlit run main.py
```
The app will open in your browser at http://localhost:8501