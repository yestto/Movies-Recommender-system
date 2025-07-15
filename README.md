# 🎬 Movie Recommender System (Content-Based)

This project implements a **Content-Based Movie Recommender System** using Python and Jupyter Notebook. It recommends movies similar to a selected title based on text similarity of genres, cast, crew, and other metadata.

---

## 🚀 Features

- ✅ Content-based movie similarity using cosine similarity
- ✅ Metadata processing: genres, keywords, cast, crew
- ✅ Movie poster fetching using TMDB API
- ✅ Simple and clean UI using `streamlit` (optional if frontend is included)

---

## 📁 Project Structure

movie_recommender/
├── movie_recommender.ipynb # Jupyter notebook with full implementation
├── movies.csv # Movie metadata
├── credits.csv # Cast and crew information
├── README.md # This file
├── requirements.txt # Python dependencies
└── .gitignore # Files/folders to ignore

yaml
Copy
Edit

---

## 🛠️ Tech Stack

- **Python**
- `pandas`, `numpy` for data processing
- `scikit-learn` for cosine similarity
- `nltk` for text preprocessing
- `pickle` for saving models
- `requests` for fetching movie posters
- `streamlit` (optional, for deployment/UI)

---

## 🔧 Installation & Setup

1. **Clone the repo**
```bash
git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender
Create virtual environment (optional)

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
(Optional) Run with Streamlit

bash
Copy
Edit
streamlit run app.py
📊 Dataset
The project uses two CSV files:

movies.csv – Contains movie metadata like title, genres, overview, etc.

credits.csv – Contains cast and crew information

These files are merged and processed to form a single dataframe used for recommendations.

🤖 How It Works
Combines important textual features (overview, genres, keywords, cast, crew)

Converts them to a single string and vectorizes it using TF-IDF or CountVectorizer

Calculates cosine similarity between movies

Recommends top N similar movies

📦 Requirements
Contents of requirements.txt (example):

nginx
Copy
Edit
pandas
numpy
scikit-learn
nltk
requests
streamlit
