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

## Project structure

