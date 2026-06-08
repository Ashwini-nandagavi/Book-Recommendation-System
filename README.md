
# 📚Book Recommendation System

A Machine Learning-based Book Recommendation System that provides personalized book recommendations by combining Collaborative Filtering, Popularity-Based Ranking, Author Reputation Analysis, and Location-Aware Recommendations.

---

## 📖 Overview

Finding relevant books among thousands of available options can be challenging for readers. This project solves that problem by building an intelligent recommendation system that suggests books based on user preferences, historical ratings, popularity trends, author reputation, and geographic interests.

The system combines multiple recommendation strategies to improve accuracy and personalization.

---

## 🎯 Objectives

- Build a personalized recommendation engine.
- Analyze user reading behavior and preferences.
- Implement collaborative filtering techniques.
- Improve recommendation quality using hybrid ranking.
- Perform data cleaning, preprocessing, and exploratory data analysis.
- Generate meaningful book suggestions for users.

---

## 📂 Dataset

The project uses the Book-Crossing Dataset consisting of:

### Books Dataset
| Column | Description |
|----------|------------|
| ISBN | Unique Book Identifier |
| Book-Title | Book Name |
| Book-Author | Author Name |
| Year-Of-Publication | Publication Year |
| Publisher | Publisher Name |

### Users Dataset
| Column | Description |
|----------|------------|
| User-ID | User Identifier |
| Location | User Location |
| Age | User Age |

### Ratings Dataset
| Column | Description |
|----------|------------|
| User-ID | User Identifier |
| ISBN | Book Identifier |
| Book-Rating | User Rating |

---

## 🛠 Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn

### Tools
- Jupyter Notebook
- Git
- GitHub

---

## 🔄 Project Workflow

### 1. Data Collection
- Load Books Dataset
- Load Users Dataset
- Load Ratings Dataset

### 2. Data Cleaning
- Handle missing values
- Remove duplicate records
- Fix invalid publication years
- Standardize data formats

### 3. Exploratory Data Analysis (EDA)
- Rating distribution analysis
- Popular books analysis
- User activity analysis
- Author performance analysis
- Geographic user analysis

### 4. Popularity-Based Recommendation
Books are ranked using:

```python
Popularity Score =
Average Rating × Rating Count
```

### 5. Collaborative Filtering

Implemented Item-Based Collaborative Filtering using:

```python
from sklearn.metrics.pairwise import cosine_similarity
```

Steps:

- Create User-Book Matrix
- Fill Missing Values
- Calculate Cosine Similarity
- Generate Similar Book Recommendations

### 6. Author Reputation Analysis

Implemented Bayesian Weighted Rating to rank authors fairly.

Formula:

```python
Weighted Rating =
(v/(v+m))*R + (m/(v+m))*C
```

Where:

- R = Average Rating
- v = Number of Ratings
- m = Minimum Votes Required
- C = Global Average Rating

### 7. Location-Based Recommendation

The system incorporates user location information to recommend books popular within specific regions.

### 8. Hybrid Recommendation Model

Final recommendation score:

```python
Final Score =
0.55 * Similarity Score +
0.25 * Popularity Score +
0.15 * Author Score +
0.05 * Location Score
```

---

## ✨ Features

- Personalized Book Recommendations
- Collaborative Filtering
- Popularity-Based Ranking
- Author Reputation Scoring
- Location-Aware Recommendations
- Data Cleaning & Preprocessing
- Exploratory Data Analysis
- Machine Learning-Based Recommendation Engine

---

## 📊 Exploratory Data Analysis

Performed analysis on:

### User Analysis
- Most Active Users
- Rating Patterns
- User Engagement

### Book Analysis
- Most Popular Books
- Highest Rated Books
- Most Reviewed Books

### Author Analysis
- Top Performing Authors
- Author Popularity

### Location Analysis
- Country-wise User Distribution
- Regional Reading Trends

---

## 📁 Project Structure

```text
Hybrid-Book-Recommendation-System
│
├── Dataset
│   ├── Books.csv
│   ├── Users.csv
│   └── Ratings.csv
│
├── Notebook
│   └── Book_Recommendation_System.ipynb
│
├── Images
│   ├── rating_distribution.png
│   ├── top_books.png
│   └── recommendation_output.png
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Hybrid-Book-Recommendation-System.git
```

Move into the project directory:

```bash
cd Hybrid-Book-Recommendation-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

## ▶️ Usage

Example:

```python
recommend_books(
    book_name="Harry Potter and the Sorcerer's Stone",
    location="India"
)
```

Output:

```text
1. Harry Potter and the Chamber of Secrets
2. Harry Potter and the Prisoner of Azkaban
3. The Hobbit
4. Eragon
5. The Golden Compass
```

---

## 📈 Results

The Hybrid Recommendation System successfully:

- Improved recommendation accuracy.
- Reduced popularity bias.
- Enhanced personalization.
- Combined multiple recommendation techniques.
- Generated meaningful book suggestions.

---

## 💡 Skills Demonstrated

- Machine Learning
- Recommendation Systems
- Data Analysis
- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Collaborative Filtering
- Python Programming
- Statistical Analysis
- Data Visualization

---

## 🔮 Future Enhancements

- Streamlit Web Application
- Deep Learning Recommendation Models
- NLP-Based Book Similarity
- Recommendation API
- Real-Time Recommendation System
- Cloud Deployment
- User Authentication

---

## 👨‍💻 Author

### Ashwini Nandagavi

Aspiring Data Scientist | AI Engineer | Data Analyst

#### Connect With Me

- GitHub: https://github.com/Ashwini-nandagavi
- LinkedIn: https://www.linkedin.com/in/ashwini-nandagavi

---

⭐ If you found this project useful, consider giving it a star on GitHub.
