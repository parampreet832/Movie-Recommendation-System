<h2>🎬 Movie Recommendation System</h2>

Production-Grade Content-Based Recommender | NLP • Cosine Similarity • FastAPI

A scalable, production-ready content-based movie recommendation system built using real-world data from TMDB. This project demonstrates end-to-end ML system design, including data ingestion, NLP feature engineering, similarity modeling, API deployment.

<h2>📌 Why This Project Matters</h2>

This project showcases skills evaluated in Data Scientist / ML Engineer interviews:

✅ Translating a business problem into an ML solution

✅ NLP-based feature engineering

✅ Vector similarity & high-dimensional data handling

✅ Clean, modular, testable code

✅ API-first deployment mindset

✅ Tradeoff-aware system design

<h2>🚀 Key Capabilities</h2>
<ul>
<li>Content-based recommendations using textual embeddings</li>

<li>NLP pipeline with tokenization, stemming, stopword removal</li>

<li>Vectorization + Cosine Similarity for fast retrieval</li>

<li>RESTful API using FastAPI</li>

<li>Offline preprocessing + online inference separation</li>

<li>Ready for cloud deployment & scaling</li>
</ul>

<h2>🧠 System Design Overview</h2>

TMDB API<br>
   ↓<br>
Data Ingestion<br>
   ↓<br>
NLP Feature Engineering (NLTK)<br>
   ↓<br>
Vectorization (Bag-of-Words)<br>
   ↓<br>
Cosine Similarity Matrix<br>
   ↓<br>
FastAPI Inference Servicev

<h2>🛠️ Tech Stack</h2>
<table>
<thead><tr>
<td>Layer</td>
<td>Technology</td>
</tr></thead>
<tbody>
<tr><td>Language</td><td>Python</td></tr>
<tr><td>API</td><td>FastAPI</td></tr>
<tr><td>NLP</td><td>NLTK</td></tr>
<tr><td>ML</td><td>Scikit-Learn</td></tr>
<tr><td>Similarity Search</td><td>Cosine Similarity</td></tr>
<tr><td>Data</td><td>Pandas, NumPy</td></tr>
<tr><td>Serving</td><td>Uvicorn</td></tr>
<tr><td>Config</td><td>dotenv</td></tr>
</tbody>
</table>

<h2>📊 Data Source</h2>

Movie metadata fetched using The Movie Database (TMDB) API including:
<ul>
<li>Movie title</li>
<li>Overview</li>
<li>Genres</li>
<li>Tagline</li>
<li>Vote Average</li>
<li>Popularity</li>
</ul>

<h2>Recommendation Strategy</h2>

<h3>Content-Based Filtering</h3>

<h4>Feature Construction</h4>
<ul>
<li>Merge overview, genres, keywords, cast, and crew</li>
<li>Normalize text using NLP preprocessing</li>
</ul>

<h4>Vectorization</h4>

<ul>
<li>Bag-of-Words (CountVectorizer, max_features=5000)</li>
</ul>

<h4>Similarity Metric</h4>

<ul>
<li>Cosine Similarity on sparse vectors</li>
</ul>

<h4>Inference</h4>
<ul>
<li>Top-N most similar movies returned per request</li>
<li>✔️ Chosen for interpretability, simplicity, and low-latency inference</li>
</ul>

<h2>⚙️ Setup Instructions</h2>

<h4>Clone Repository</h4>
  git clone https://github.com/yourusername/movie-recommendation-system.git
  cd movie-recommendation-system

<h4>Create Environment</h4>
  python -m venv venv
  source venv/bin/activate

<h4>Install Dependencies</h4>
  pip install -r requirements.txt

<h4>Configure API Key</h4>
  TMDB_API_KEY=your_api_key_here

<h2>▶️ Run API Server</h2>

uvicorn app.main:app --reload

API will be available at:

https://movie-recommendation-system-6r07.onrender.com

<h6>Swagger UI:</h6>

https://movie-recommendation-system-6r07.onrender.com/docs

<h2>📈 Performance & Scalability Notes</h2>

<ul>
<li>Precomputed similarity matrix → O(1) inference</li>
<li>Stateless FastAPI service → horizontally scalable</li>
<li>Can be upgraded to:
<ul><li>TF-IDF / Word2Vec</li>
<li>ANN search (FAISS)</li>
<li>Hybrid recommender systems</li></ul>
</li>
</ul>

<h2>👩‍💻 Author</h2>

<b>Parampreet Kour</b>
Aspiring Data Scientist
Background: 6+ years PHP Developer → ML Transition

🔗 GitHub: https://github.com/parampreet832

<h2>📜 License</h2>

MIT License

<h2>⭐ Acknowledgements</h2>
<ul>
<li>The Movie Database</li>

<li>FastAPI & Scikit-Learn communities</li>
</ul>
