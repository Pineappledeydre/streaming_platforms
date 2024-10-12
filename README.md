To incorporate the **Movie Recommendation System** into your README, here’s a version with the new section added:

---

# 🎬 Streaming Giants: A Comparative Analysis of Netflix, Disney+, and Amazon Prime

This project provides a comparative analysis of three major streaming platforms: **Netflix**, **Disney+**, and **Amazon Prime**. It dives deep into the content available on each platform, exploring aspects like movie/TV show durations, release years, genres, ratings, and the geographical distribution of content. Additionally, the project includes a **Movie Recommendation System** that suggests similar titles based on various content attributes.

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Datasets](#datasets)
- [Installation](#installation)
- [Features](#features)
- [Analysis Highlights](#analysis-highlights)
- [Movie Recommendation System](#movie-recommendation-system)
- [Technologies Used](#technologies-used)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## 📌 Project Overview

This project was created to compare the content offerings of **Netflix**, **Disney+**, and **Amazon Prime**, analyzing key points such as:
- **Content Type Distribution**: Movies vs TV Shows.
- **Duration**: How long movies typically are on each platform.
- **Genres**: How platforms categorize their content.
- **Country-Specific Insights**: Countries producing the most content.
- **Ratings**: Family-friendly vs adult-targeted content.
- **Trends over Time**: Analyzing content additions and release year trends.
- **Movie Recommendations**: Suggesting similar movies based on various attributes (e.g., genre, director, cast).

## 📊 Datasets

The project uses publicly available datasets from **Kaggle**, including:
1. [**Netflix Movies and TV Shows Dataset**](https://www.kaggle.com/datasets/shivamb/netflix-shows): Metadata on movies and TV shows available on Netflix.
2. [**Disney+ Movies and TV Shows Dataset**](https://www.kaggle.com/datasets/ruchi798/disney-plus-shows): Metadata on movies and TV shows available on Disney+.
3. [**Amazon Prime Movies and TV Shows Dataset**](https://www.kaggle.com/datasets/shivamb/amazon-prime-movies-and-tv-shows): Metadata on Amazon Prime content.

Each dataset includes features such as:
- Title, Director, Cast
- Country of Origin
- Release Year
- Rating (e.g., TV-MA, PG)
- Duration (movies in minutes, TV shows by season count)
- Listed Genres

## 💻 Installation

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/streaming-giants-analysis.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd streaming-giants-analysis
   ```

3. **Create a virtual environment** (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate  # For MacOS/Linux
   .\env\Scripts\activate  # For Windows
   ```

4. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the Jupyter Notebook** (or your preferred IDE):
   ```bash
   jupyter notebook streaming_platforms.ipynb
   ```

## ✨ Features

- **Data Preprocessing**:
  - Handling missing values.
  - Parsing columns like "duration" and converting to numeric values.
  - Feature engineering.
  
- **Exploratory Data Analysis**:
  - Platform-wise content distribution (Movies vs TV Shows).
  - Ratings analysis to assess audience targeting.
  - Genre correlation analysis.
  - Cross-country analyss.


## 📈 Analysis Highlights

- **Content Type Distribution**: Most content across all platforms is movie-based, with Amazon Prime offering the most, followed by Netflix, and then Disney+.
  
- **Duration**: Average movie duration across all platforms is approximately 92 minutes. TV shows on Netflix tend to have more seasons on average than those on other platforms.
  
- **Ratings**: Disney+ focuses heavily on family-friendly content, while Netflix and Amazon Prime offer a wider variety of mature content.

- **Geographical Insights**: Countries like the United States, India, and the UK dominate in terms of content production, with the U.S. being a major source for all three platforms.

## 🔍 Movie Recommendation System

The **Movie Recommendation System** suggests similar titles based on shared characteristics such as genres, cast, director, and description. This recommendation system employs several techniques:
  
- **Feature Encoding**: One-hot encoding for categorical features like 'type', 'genres', 'country', 'director', and 'cast'.
- **TF-IDF Vectorization**: For movie descriptions to capture content-based similarities.
- **Clustering**: K-Means clustering to group similar movies for recommendation.
- **Graph-based Approach**: Using a graph where nodes represent movies, genres, and people (cast/director) for multi-dimensional recommendations.

## 🛠 Technologies Used

- **Programming Languages**: Python
- **Data Libraries**:
  - Pandas (for data manipulation)
  - Numpy (for numerical operations)
  - Matplotlib, Seaborn, Plotly (for data visualization)
  - Scikit-learn (for preprocessing, vectorization, and clustering)
  - NetworkX (for graph-based recommendation system)

## 📊 Visualizations

The project includes various visualizations that help convey key insights:
- **Content Distribution**: Bar charts and heatmaps comparing content type (movies vs TV shows) across platforms.
- **Ratings Analysis**: Pie charts and bar plots showing the distribution of audience ratings.
- **Genre Correlation Heatmaps**: Highlighting relationships between genres for both movies and TV shows.
- **Country-Specific Analysis**: Bar charts illustrating which countries produce the most content.
- **Movie Recommendation Subgraphs**: Visualizing the connections between recommended movies, genres, cast, and directors.

## 🧐 Conclusion

This project reveals:
- The content strategies of Netflix, Disney+, and Amazon Prime are quite distinct.
- Netflix and Amazon Prime target a broader demographic with more mature content, while Disney+ remains family-friendly.
- The **Movie Recommendation System** enhances user experience by providing suggestions based on movie attributes, leveraging advanced encoding and graph-based relationships.
