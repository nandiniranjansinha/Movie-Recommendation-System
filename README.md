# 🎬 Movie Recommendation System
### Colab Link: https://colab.research.google.com/drive/1rx6Dg0Tq1p-9Mi1MCAG4nt-hW-dvXjzt?usp=sharing

A hybrid recommendation engine combining collaborative filtering and content-based clustering.

## 🎯 Overview
Built a PyTorch-based movie recommendation system using matrix factorization and K-Means clustering on the MovieLens dataset.


## 🏗️ Architecture
```
User/Movie IDs → Embedding Layers → Matrix Factorization → Rating Prediction
                                    ↓
                              Movie Embeddings → K-Means Clustering → Genre Groups
```

## 📊 Performance Metrics

| Metric | Value | Interpretation |
|--------|-------|----------------|
| **RMSE** | 0.55 | Prediction error of ±0.55 stars |
| **MAE** | 0.40 | Average error of ±0.40 stars |
| **R² Score** | 0.72 | Explains 72% of rating variance |
| **Loss Reduction** | 97% | Highly effective training |

### Model Details
- **Dataset:** MovieLens (100,000+ ratings)
- **Users:** 610
- **Movies:** 9,724
- **Test Samples:** 20,168
- **Embedding Dimensions:** 8
- **Training Epochs:** 128
- **Optimizer:** Adam (lr=1e-3)

## 📈 Training Results

![Training Loss](training_loss.png)

**Key Findings:**
- Model converged smoothly from loss 11.06 → 0.33
- No overfitting observed
- Consistent improvement across all epochs
- Strong generalization to test set

## 🎯 Sample Predictions

| Actual Rating | Predicted | Error |
|--------------|-----------|-------|
| 4.5 | 4.47 | -0.03 |
| 4.0 | 3.88 | -0.12 |
| 3.5 | 3.84 | +0.34 |
| 3.0 | 3.20 | +0.20 |

**Average prediction accuracy: ±0.39 stars**

## 🏆 Model Strengths

1. **High Accuracy:** R² of 0.72 indicates strong predictive power
2. **Low Error:** MAE of 0.40 means predictions are highly reliable
3. **Efficient Training:** Achieved convergence in 128 epochs (~3 minutes on GPU)
4. **Scalable:** Handles 100K+ ratings efficiently
5. **Generalizable:** Strong performance on unseen test data


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
