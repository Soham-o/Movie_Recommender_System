🎬 Movie Recommendation System
This project is a content-based movie recommendation system built using Python and Streamlit. Given a movie title, it suggests similar movies using a combination of movie metadata and cosine similarity, along with movie posters fetched via the TMDb API.

 Features
🧠 Content-based filtering using movie overviews and metadata

🎥 Poster images retrieved dynamically using the TMDb API

⚡ Fast and interactive web interface built with Streamlit

📦 Precomputed similarity matrix for quick recommendations

🚀 How it Works
Loads a dataset of 5000+ movies (tmdb_5000_movies.csv and tmdb_5000_credits.csv)
Preprocesses the data and computes a similarity score between each movie
When a user selects a movie, the system recommends 5 most similar movies based on cosine similarity
Uses TMDb API to fetch posters of the recommended movies

🛠 Tech Stack
Python
Pandas, Scikit-learn
Streamlit
TMDb API
Pickle (for loading preprocessed data)

📂 Project Structure
bash
Copy
Edit
├── movies_rs.py                  # Main Streamlit app
├── movies.pkl                    # Movie metadata (preprocessed)
├── similarity.pkl                # Similarity matrix
├── tmdb_5000_movies.csv          # Original movies dataset
├── tmdb_5000_credits.csv         # Original credits dataset
├── movies_recommendation_system.ipynb  # Jupyter Notebook (EDA & preprocessing)
📦 Setup Instructions
Clone the repository

Install required packages:
pip install -r requirements.txt

Run the app:
streamlit run movies_rs.py

🗝️ API Key
Make sure to replace the TMDb API key in the fetch_poster() function with your own key from themoviedb.org.
