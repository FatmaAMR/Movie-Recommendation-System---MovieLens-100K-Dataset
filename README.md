# MovieLens 100K Recommender System

## Project Overview
This project implements a **Movie Recommender System** and demonstrates multiple collaborative filtering techniques and matrix factorization to recommend movies to users based on their preferences.

The system provides:
- **User-Based Collaborative Filtering (User-CF)** – Finds similar users and recommends what they liked.  
- **Item-Based Collaborative Filtering (Item-CF)** – Finds similar items and recommends based on rated movies.  
- **Matrix Factorization (SVD)** – Learns hidden factors from ratings to generate better predictions.  

Evaluation is done using **Precision@K**, and an **interactive Gradio interface** is built for easy exploration.

---

## Tools & Libraries
- **Python 3**  
- **Pandas** – data manipulation  
- **NumPy** – numerical operations  
- **Scikit-learn** – similarity measures, SVD  
- **Gradio** – interactive web interface  
- **Kaggle Notebook** – development environment  

---

## Dataset
- **Source**: [MovieLens 100K Dataset]([https://grouplens.org/datasets/movielens/100k/](https://www.kaggle.com/datasets/prajitdatta/movielens-100k-dataset))  
- Contains **100,000 ratings** from **943 users** on **1,682 movies**.  
- Files used:
  - `u.data` – user ratings  
  - `u.item` – movie metadata (titles, genres)  

---

## Workflow
1. Load and preprocess the dataset.  
2. Build a **user-item rating matrix**.  
3. Implement:
   - User-CF (cosine similarity between users)  
   - Item-CF (cosine similarity between movies)  
   - SVD (matrix factorization with latent features)  
4. Evaluate using **Precision@K**.  
5. Build a **Gradio Interface** for interactive recommendations.  

---

## Evaluation
Example Precision@10 results (values may vary due to random split):  
- User-CF: `0.21`  
- Item-CF: `0.24`  
- SVD: `0.29`  

---

## 🖥️ Interface
An interactive interface was built using **Gradio**.  
Users can select a **User ID**, choose a **Recommendation Method**, and view the **Top-N recommended movies**.

![5909223852645403118](https://github.com/user-attachments/assets/31320494-fbee-4106-9df8-fc1a9ff7f4c9)

