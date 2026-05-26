# 🎬 Movie Recommendation System

A **Movie Recommendation Web App** built with Python and Streamlit. The app recommends similar movies using a precomputed cosine similarity matrix and TMDB metadata.

## 📌 Project Overview

This project lets users select a movie title and receive 5 similar movie recommendations.

The recommendation logic is based on:

- Content similarity between movies
- Precomputed feature vectors from TMDB metadata
- Cosine similarity of movie embeddings

---

## 🧠 How It Works

1. Load movie metadata from `movie_dict.pkl`
2. Load precomputed similarity scores from `similarity.pkl`
3. Display a Streamlit select box with movie titles
4. When the user clicks `Recommend`, find the top 5 closest movies
5. Fetch movie posters from TMDB API and show them with titles

---

## 📂 Included Files

- `app.py` - Streamlit app entrypoint
- `movie_dict.pkl` - Serialized movie metadata dictionary
- `similarity.pkl` - Precomputed cosine similarity matrix
- `movies.pkl` - Optional movie DataFrame pickle
- `tmdb_5000_movies.csv` - TMDB movie metadata source
- `tmdb_5000_credits.csv` - TMDB credits metadata source
- `.streamlit/` - Streamlit configuration folder
- `requirements.txt` - Python dependencies
- `MRS.ipynb` - exploratory notebook

---

## 🛠️ Technologies Used

- Python 3
- Streamlit
- Pandas
- NumPy
- Scikit-learn
- Requests

---

## 🚀 Run the App Locally

1. Create and activate your Python environment (example):

```bash
python -m venv venv
source venv/Scripts/activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Start the Streamlit app:

```bash
streamlit run app.py
```

4. Open the app in your browser at the URL shown by Streamlit.

---

## ⚠️ Notes

- The app uses a hardcoded TMDB API key in `app.py` for poster image retrieval.
- If the poster fetch fails, the app may show broken images.
- The recommendation depends on the precomputed `similarity.pkl` file.

---

## 💡 Usage

- Select a movie from the dropdown
- Click `Recommend`
- View the recommended movie titles and posters across 5 columns

---

## 👩‍💻 Author

- **Name:** Fozia
- **GitHub:** https://github.com/Fozia-tech

