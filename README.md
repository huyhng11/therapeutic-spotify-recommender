## 🎵 Therapeutic Spotify Recommender – Mood-Aware Music for Mental Wellness

This project explores a personalized music recommendation system designed to support users’ emotional well-being. By analyzing Spotify listening behavior and track audio features, we generate playlists that gently guide users from their current mood (e.g., sad or angry) to a more positive state (e.g., happy or calm).

> 🧘 A Spotify-powered tool for **on-demand music therapy**—combining data science and mental health support.

### 🔍 Key Features

- 🎧 **Therapeutic Playlist Generator**  
  Recommend 10-song playlists based on a user's dominant mood, with adjustable blend ratios (e.g., 70/30 Sad→Happy).

- 📈 **Emotional Clustering with ML**  
  Clusters songs using K-Means based on audio features like **valence**, **energy**, and **acousticness**.

- 🧠 **Mood Transition Model**  
  Uses **K-Nearest Neighbors (KNN)** to recommend tracks aligned with both current and target emotional states.

- ✅ **Validated by Real Users**  
  - 70% reported a mood improvement  
  - 100% playlist completion rate  
  - High user satisfaction with personalized “persona cards” and blend sliders

### 📊 Techniques & Tools

- Machine Learning: `KMeans`, `GMM`, `Fuzzy C-Means`, `Decision Tree`, `KNN`  
- Data Analysis: Pandas, Matplotlib, Seaborn  
- Data Sources:  
  - [Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)  
  - [User Spotify streaming history](https://github.com/Elabs-llc/CodeAlpha_Music_Recomendation_System/tree/main/data)


### 🧪 Results & Findings

- 📌 **K-Means** outperformed other clustering models with:
  - Silhouette Score: `0.4015`
  - Davies-Bouldin Index: `0.8389`

- 📌 **Fuzzy C-Means** showed comparable performance:
  - Silhouette Score: `0.3992`
  - Davies-Bouldin Index: `0.8631`

- 📌 **GMM** underperformed:
  - Silhouette Score: `0.1102`
  - Davies-Bouldin Index: `2.0537`

- 📌 **User Feedback:**
  - 70% of test users experienced **positive mood shifts**
  - 100% of users completed the recommended playlists
  - 4 out of 5 participants found the system “emotionally relevant”
  - Persona cards and blend sliders were the most appreciated features

- 🎯 Final model: **K-Means + KNN**, selected for clarity, accuracy, and therapeutic alignment

### 📁 File Description

| File/Folder         | Description |
|---------------------|-------------|
| `notebooks/`        | Jupyter Notebooks for preprocessing, modeling, and evaluation |
| `data/`             | CSVs of Spotify tracks and user streaming history |
| `final_report.pdf`  | Full technical report detailing methodology and findings |
| `README.md`         | Project overview and instructions |
| `output/`           | Generated playlists and visualizations |

### 🔮 Future Improvements

- Integrate behavioral tracking (clicks, skips, time-on-track)
- Collaborate with certified music therapists for model refinement
- Run longitudinal A/B tests for emotional impact validation
