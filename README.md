# 🎬 Movie Recommendation System

A hybrid recommendation engine combining collaborative filtering and content-based clustering.

## 🎯 Overview
Built a PyTorch-based movie recommendation system using matrix factorization and K-Means clustering on the MovieLens dataset.

## 📊 Performance
- **RMSE:** 0.89 (±0.89 star prediction accuracy)
- **Dataset:** MovieLens (100,000+ ratings, 610 users, 9,700 movies)
- **Embedding Dimension:** 50
- **Training Epochs:** 20
- **Optimizer:** Adam

## 🏗️ Architecture
```
User/Movie IDs → Embedding Layers → Matrix Factorization → Rating Prediction
                                    ↓
                              Movie Embeddings → K-Means Clustering → Genre Groups
```

## 🔧 Technologies
- **Deep Learning:** PyTorch
- **Clustering:** Scikit-learn (K-Means)
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn

## 📈 Key Features
1. **Collaborative Filtering:** Matrix factorization with learned embeddings
2. **Content Discovery:** K-Means clustering for genre-based grouping
3. **Hybrid Approach:** Combines user preferences with content similarity
4. **Scalable Architecture:** Efficient embedding-based computation


## 📄 License
MIT License
