✨ What it does:

Given a song title, the app finds lyrically similar songs using:
TF-IDF vectorization of the lyrics (text column)
Cosine similarity between songs
A simple Streamlit UI for interactive search

Place a CSV (e.g. data/spotify_millsongdata.csv) with columns:
artist – artist name
song – song title
link – optional reference link
text – lyrics

.
├── data/
│   └── spotify_millsongdata.csv
├── artifacts/                 # generated files (tfidf, similarity, cleaned df)
├── main.py                    # Streamlit UI
├── preprocess.py              # text cleaning + TF-IDF + similarity build
├── recommend.py               # CLI helper (recommendations in terminal)
├── requirements.txt
└── README.md

# 1) Clone & enter the project
git clone <this-repo-url>
cd <repo-folder>

# 2) Create & activate a virtual environment
python -m venv .venv
# Linux/macOS:
source .venv/bin/activate
# Windows (PowerShell):
# .\.venv\Scripts\Activate.ps1

# 3) Install dependencies
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
# (If you use uv: uv pip install -r requirements.txt)
