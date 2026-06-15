# 🎬 Movie Recommender System (Content-Based)

A content-based movie recommender system that suggests movies similar to a user's favourite film by analyzing metadata — such as **genres**, **cast**, and **crew**. It uses **Natural Language Processing (NLP)** and **Machine Learning** to deliver accurate, meaningful recommendations.

---

## 🌐 Live Demo

👉 **Try the Application:** [movierecommender-sys.streamlit.app](https://movierecommender-sys.streamlit.app/)

---

## 🚀 Features

- 🎥 Suggests the **top 5 movies** most similar to your chosen film
- 👥 Considers **cast**, **crew**, **genres**, and **storyline** for accurate recommendations
- 🔢 Uses **NLP and similarity metrics** to measure how closely movies are related
- ⚡ Built with **Streamlit** for a fast and interactive user experience
- 🖱️ Simple interface — just type or select a movie name to get suggestions instantly

---

## 🧠 Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Data Processing | Pandas, NumPy |
| NLP & ML | Scikit-learn, NLTK |
| Algorithms | CountVectorizer, Cosine Similarity |
| Web Framework | Streamlit |
| Development | Jupyter Notebook, VS Code |

---

## 📊 Dataset

| Detail | Info |
|---|---|
| Files Used | `movies.csv`, `credits.csv` |
| Total Records | 4,800+ movies analyzed |

- **movies.csv** — Contains basic movie details (title, genres, overview, etc.)
- **credits.csv** — Contains cast and crew information per movie

---

## 🛠️ How It Works

```
Data Loading
      │
      ▼
Merge movies.csv + credits.csv
      │
      ▼
Feature Extraction
(cast, crew, genres, overview)
      │
      ▼
Text Vectorization
(CountVectorizer)
      │
      ▼
Similarity Calculation
(Cosine Similarity)
      │
      ▼
Top 5 Movie Recommendations
```

### Step-by-Step Breakdown

**1. Data Loading**
Reads and merges `movies.csv` and `credits.csv` on the movie title.

**2. Feature Extraction**
Focuses on key metadata fields — cast, crew (director), genres, and movie overview — to build a rich content profile for each film.

**3. Vectorization**
Converts combined textual information into numerical vectors using `CountVectorizer`, enabling mathematical comparison between movies.

**4. Similarity Calculation**
Applies **Cosine Similarity** on the resulting vectors to rank how closely any two movies relate to each other.

**5. Recommendation**
Users type or select a movie name and instantly receive the **top 5 most similar movies** from the dataset.

---

## 📂 Project Structure

```
MovieRecommenderSystem/
│
├── streamlit_app.py          # Streamlit web application
├── movie-recommender.ipynb   # Jupyter Notebook with model logic
├── requirements.txt          # Python dependencies
│
├── data/
│   ├── movies.csv            # Movie details dataset
│   └── credits.csv           # Cast & crew dataset
```

---

## 📦 Files Included

| File | Description |
|---|---|
| `streamlit_app.py` | Source code for the Streamlit web interface |
| `movie-recommender.ipynb` | Core model logic — EDA, vectorization, similarity |
| `movies.csv` | Basic movie details (title, genres, overview) |
| `credits.csv` | Cast and crew information |
| `requirements.txt` | List of Python dependencies |

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/mitpatelcs/MovieRecommenderSystem.git
cd MovieRecommenderSystem
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv

# On macOS/Linux
source .venv/bin/activate

# On Windows
.venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run streamlit_app.py
```

Open your browser and navigate to: **http://localhost:8501**

---

## 🔮 Future Improvements

- [ ] Add movie posters using TMDB API
- [ ] Support collaborative filtering for personalised recommendations
- [ ] Add user rating-based filtering
- [ ] Expand dataset beyond 4,800 movies
- [ ] Improve NLP preprocessing with lemmatization

---

## ⚠️ Disclaimer

This project is built for educational purposes using a publicly available movie dataset. Recommendations are based purely on metadata similarity and do not reflect any professional or commercial movie suggestion service.

---

## 👨‍💻 Author

**Mit Patel**
