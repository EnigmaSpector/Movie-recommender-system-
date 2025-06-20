🎬 Movie Recommender System
A content-based movie recommendation system built using the TMDB (The Movie Database) dataset. It uses cosine similarity on textual features to suggest similar movies based on a selected movie's metadata.

📌 Features
✅ Content-based filtering using movie overviews, genres, keywords, cast, and crew

✅ Preprocessing and feature engineering using NLP techniques

✅ Cosine similarity for finding similar movies

✅ Clean and minimal UI using Streamlit (optional deployment)

✅ Ready for integration into any movie browsing or review platform

📂 Dataset
Source: Kaggle TMDB 5000 Movie Dataset

Files used:

tmdb_5000_movies.csv

tmdb_5000_credits.csv

🛠 Tech Stack
Component	Tool/Library
Language	Python
Data Manipulation	Pandas, NumPy
NLP & Similarity	scikit-learn (TfidfVectorizer, cosine_similarity)
Visualization/UI	Streamlit
Jupyter Notebook	For experimentation

⚙️ How It Works
Data Cleaning: Merges movie and credits dataset, drops nulls, processes genres/keywords/cast/crew.

Feature Engineering:

Extracts top cast, director, and tags.

Combines textual info into a single tags column.

Vectorization:

Uses TfidfVectorizer or CountVectorizer to convert text into vectors.

Similarity Scoring:

Computes pairwise cosine similarity.

Recommendation:

Returns top 5–10 similar movies based on cosine similarity of tags.


📈 Potential Improvements
Incorporate collaborative filtering for better personalization.

Use word embeddings (e.g., BERT) instead of simple vectorizers.

Add user login & feedback loop for dynamic learning.

Deploy using Streamlit Cloud, Heroku, or AWS Lambda.
