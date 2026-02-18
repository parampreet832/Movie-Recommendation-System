🎬 Movie Recommendation System

Production-Grade Content-Based Recommender | NLP • Cosine Similarity • FastAPI

A scalable, production-ready content-based movie recommendation system built using real-world data from TMDB. This project demonstrates end-to-end ML system design, including data ingestion, NLP feature engineering, similarity modeling, API deployment.

-----------------------------------------------------------------------------

📌 Why This Project Matters

This project showcases skills evaluated in Data Scientist / ML Engineer interviews:

✅ Translating a business problem into an ML solution

✅ NLP-based feature engineering

✅ Vector similarity & high-dimensional data handling

✅ Clean, modular, testable code

✅ API-first deployment mindset

✅ Tradeoff-aware system design

-----------------------------------------------------------------------------

🚀 Key Capabilities

Content-based recommendations using textual embeddings

NLP pipeline with tokenization, stemming, stopword removal

Vectorization + Cosine Similarity for fast retrieval

RESTful API using FastAPI

Offline preprocessing + online inference separation

Ready for cloud deployment & scaling

-----------------------------------------------------------------------------

🧠 System Design Overview

TMDB API
   ↓
Data Ingestion
   ↓
NLP Feature Engineering (NLTK)
   ↓
Vectorization (Bag-of-Words)
   ↓
Cosine Similarity Matrix
   ↓
FastAPI Inference Service

-----------------------------------------------------------------------------

🛠️ Tech Stack

Layer	              Technology
Language            Python
API	                FastAPI
NLP	                NLTK
ML	                Scikit-Learn
Similarity Search	  Cosine Similarity
Data	              Pandas, NumPy
Serving	            Uvicorn
Config	            dotenv

-----------------------------------------------------------------------------

📊 Data Source

Movie metadata fetched using The Movie Database (TMDB) API

Includes:

Movie title

Overview

Genres

Tagline

Vote Average

Popularity

-----------------------------------------------------------------------------

Recommendation Strategy

Content-Based Filtering (Explainable ML)

Feature Construction

  . Merge overview, genres, keywords, cast, and crew

  . Normalize text using NLP preprocessing

Vectorization

  . Bag-of-Words (CountVectorizer, max_features=5000)

Similarity Metric

  . Cosine Similarity on sparse vectors

Inference

  . Top-N most similar movies returned per request

  . ✔️ Chosen for interpretability, simplicity, and low-latency inference

-----------------------------------------------------------------------------

⚙️ Setup Instructions

Clone Repository
  git clone https://github.com/yourusername/movie-recommendation-system.git
  cd movie-recommendation-system

Create Environment
  python -m venv venv
  source venv/bin/activate

Install Dependencies
  pip install -r requirements.txt

Configure API Key
  TMDB_API_KEY=your_api_key_here

-----------------------------------------------------------------------------

▶️ Run API Server

uvicorn app.main:app --reload

API will be available at:

https://movie-recommendation-system-6r07.onrender.com


Swagger UI:

https://movie-recommendation-system-6r07.onrender.com/docs

-----------------------------------------------------------------------------

📈 Performance & Scalability Notes

Precomputed similarity matrix → O(1) inference

Stateless FastAPI service → horizontally scalable

Can be upgraded to:

TF-IDF / Word2Vec

ANN search (FAISS)

Hybrid recommender systems

-----------------------------------------------------------------------------

👩‍💻 Author

Parampreet Kour
Aspiring Data Scientist | ML Engineer
Background: 6+ years Software Engineering → ML Transition

🔗 GitHub: https://github.com/parampreet832

-----------------------------------------------------------------------------


📜 License

MIT License

-----------------------------------------------------------------------------

⭐ Acknowledgements

The Movie Database

FastAPI & Scikit-Learn communities
