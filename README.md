## What it does

Type a song title and get lyrically similar songs.  
Under the hood:
- **TF-IDF** vectorization of song lyrics (`text`)
- **Cosine similarity** across songs
- Simple **Streamlit** UI for search & display

---

## Dataset

Place a CSV (e.g., `data/spotify_millsongdata.csv`) with columns:

- `artist` – artist name  
- `song` – song title  
- `link` – optional reference link  
- `text` – lyrics

> Tip: For very large CSVs, sample rows during preprocessing (e.g., 10k) to speed things up.

---


---

## Quick start

### 1) Clone & enter the project
```bash
git clone <YOUR-REPO-URL>
cd <YOUR-REPO-FOLDER>
python -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
# using uv? -> uv pip install -r requirements.txt
streamlit run main.py

