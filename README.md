# Spotify Music Recommendation System 🎧

This project presents a Spotify Music Recommendation System that leverages Machine Learning (ML) and Natural Language Processing (NLP) to recommend songs based on a given track. It analyzes song metadata, content features, and user preferences to suggest similar tracks, helping users discover new music that aligns with their taste.

## 🚀 Project Overview

Spotify offers a massive library of tracks, making music discovery both exciting and overwhelming. This system addresses that by providing a personalized recommendation engine that suggests songs similar to a user-selected track. Using cosine similarity and content-based filtering, it matches songs based on musical attributes and metadata.

Technologies used:

* Python
* pandas, NumPy, scikit-learn
* NLTK
* pickle
* Streamlit (for UI)
* Jupyter Notebook / Google Colab (for exploratory analysis and prototyping)
* Visual Studio Code 

🎯 Use Case: When a user selects a song, the system recommends top N similar tracks based on audio features and metadata such as genre, artist, popularity, etc.

---

## 📂 Project Structure

│
├── data/
│   └── spotify\_millsongdata.csv - Raw dataset of songs
│
├── src/
│   ├── cosine\_sim.pkl - Precomputed cosine similarity matrix (excluded from GitHub due to size)
│   ├── song\_data.pkl - Processed data used in the recommendation system
│   ├── recommender.py - Core logic for generating recommendations
│
├── app.py - Streamlit app script
├── requirements.txt - Required Python packages
├── spotify\_recommender.ipynb - EDA and model development
└── README.md - Project documentation

---

## 🔍 Features

* Content-Based Recommendation Engine
* Cosine Similarity-Based Matching
* Text Feature Extraction using NLP
* Interactive UI built with Streamlit
* Searchable song selection
* Top N recommendations with title and artist name

---

## 📈 How It Works

1. Load and preprocess the dataset (cleaning, filtering, feature extraction)
2. Vectorize song features (e.g., genre, lyrics, artist name)
3. Compute cosine similarity between all songs
4. Save model and similarity matrix using pickle
5. Build a UI in Streamlit to select a song and view top similar tracks

---

## 🛠️ Installation & Usage

1. Clone the repository:

   git clone [https://github.com/Shibaditya00/Spotify-Music-Recommendation-System.git](https://github.com/Shibaditya00/Spotify-Music-Recommendation-System.git)

2. Navigate to the project directory:

   cd Spotify-Music-Recommendation-System

3. Create and activate a virtual environment (optional but recommended):

   python -m venv venv
   venv\Scripts\activate      # Windows
   source venv/bin/activate   # macOS/Linux

4. Install dependencies:

   pip install -r requirements.txt

5. Launch the app:

   streamlit run app.py

6. Select a song from the dropdown and explore the recommendations!

---

## 📊 Dataset

<a href="https://github.com/Shibaditya00/Spotify-Music-Recommendation-System/blob/main/src/spotify_millsongdata.csv">Spotify Dataset</a> 

* Source: \[Millsongdata Dataset] — contains metadata and textual information of thousands of songs
* Includes fields such as: song title, artist, genre, lyrics, and more
* Used for training and similarity computation

---

## User Interface

![Screenshot (51)](https://github.com/user-attachments/assets/e51f4941-3e92-42a9-a883-64ffc60954e9)


![Screenshot (52)](https://github.com/user-attachments/assets/829282cf-2bd4-4c38-9bfc-2f9e83ec9265)


![Screenshot (53)](https://github.com/user-attachments/assets/bd0b0ef8-8f7f-45c8-a5c5-b7168cb385c6)

## 📌 Note

Due to GitHub’s file size restrictions, some files like cosine\_sim.pkl (≈700 MB) are not included in the repository. You can:

* Recompute them by running the notebook
* Or use Git LFS to push and track large files

---
