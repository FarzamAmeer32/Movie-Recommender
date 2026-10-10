
# 🎬 AI Movie Recommendation System

**Discover your next favorite movie with AI.**

An end-to-end movie recommendation web application built using **Python, NLP, and Content-Based Filtering**. It recommends movies based on their similarities and integrates the TMDB API to display movie posters, ratings, and details through a Netflix-inspired interface.

---

## ✨ Features

* 🎯 **Smart Recommendations** — Find movies similar to your selected title.

* 🧠 **NLP-Based Similarity** — Analyze movie metadata to identify related films.

* 📐 **Cosine Similarity** — Rank movies based on their feature-vector similarity.

* 🎞️ **TMDB Integration** — Retrieve movie posters, ratings, and additional details.

* ⚡ **Precomputed Similarity** — Generate recommendations without recalculating the entire similarity matrix for every request.

* 🌐 **Interactive Web App** — Explore recommendations through a responsive, Netflix-inspired interface.

## 🖥️ Preview

*Add a screenshot of your application here to showcase the user interface and movie recommendations.*

---

## ⚙️ How It Works

1. **Data Processing** — Clean movie metadata and combine relevant features, including genres, keywords, cast, crew, and overview.

2. **Text Vectorization** — Convert combined textual features into numerical vectors using CountVectorizer.

3. **Similarity Calculation** — Calculate cosine similarity between movie vectors.

4. **Recommendation** — Retrieve the most similar movies for the selected title.

5. **Movie Enrichment** — Use the TMDB API to retrieve posters, ratings, and movie details.

6. **Display Results** — Present recommendations through the Flask-powered web application.

---

## 🏗️ Architecture

**User → Frontend (HTML, CSS, JavaScript) → Flask Backend**

The Flask backend connects to two components:

* **Recommendation Engine:** Uses the precomputed similarity matrix to identify similar movies.

* **TMDB API:** Retrieves movie posters, ratings, and additional information.

The backend combines the recommendations and movie details before displaying the results on the frontend.

---

## 🛠️ Tech Stack

| Category         | Technologies          |
| ---------------- | --------------------- |
| Language         | Python                |
| Data Processing  | Pandas, NumPy         |
| Machine Learning | Scikit-learn          |
| NLP              | CountVectorizer       |
| Similarity       | Cosine Similarity     |
| Backend          | Flask, REST API       |
| Frontend         | HTML, CSS, JavaScript |
| Movie Data       | TMDB API              |
| Serialization    | Pickle                |

---

## 📁 Project Structure

* **app.py** — Flask application and backend logic.

* **movie_recommender.ipynb** — Data preprocessing and recommendation model development.

* **movies.pkl** — Serialized movie dataset.

* **similarity.pkl** — Precomputed movie similarity matrix.

* **requirements.txt** — Project dependencies.

* **templates/index.html** — Frontend HTML template.

* **static/style.css** — Styling and layout.

* **static/script.js** — Frontend interactions.

---

## 🚀 Getting Started

### Prerequisites

* Python 3.9+

* A TMDB API key

### 1. Clone the Repository

Clone the project from GitHub and navigate to the project directory.

Repository: [Movie-Recommender](https://github.com/FarzamAmeer32/Movie-Recommender)

### 2. Install Dependencies

Install the required Python packages listed in `requirements.txt`.

### 3. Configure the TMDB API

Set your TMDB API key in the application configuration. Keep credentials private and never commit API keys to GitHub.

### 4. Run the Application

Start the Flask application and open [**http://127.0.0.1:5000**](http://127.0.0.1:5000) in your browser.

---

## 🔮 Future Enhancements

* Hybrid recommendations using content-based and collaborative filtering.

* Personalized recommendations based on user preferences.

* User accounts, watchlists, and rating history.

* Cloud deployment and production-ready configuration.

---

## 👨‍💻 Author

**Muhammad Farzam Ameer**

[GitHub Profile](https://github.com/FarzamAmeer32) · [Project Repository](https://github.com/FarzamAmeer32/Movie-Recommender)

---

*Built with Python, Machine Learning, and a love for movies 🎬*