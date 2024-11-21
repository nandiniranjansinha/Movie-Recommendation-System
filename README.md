# Movie-Recommendation-System

This repository contains a Movie Recommendation System built using collaborative filtering techniques, matrix factorization, and clustering algorithms. The system utilizes PyTorch for implementing matrix factorization and scikit-learn's KMeans for clustering movies into genres or categories based on user ratings.

## Features
- Dataset: The model works with the MovieLens dataset (ml-latest-small), which includes user ratings for various movies.
- Matrix Factorization: Implements a matrix factorization model using PyTorch to generate latent factors for users and movies.
- Clustering: Clusters movies into groups using KMeans based on their learned embeddings.
- Recommendations: Identifies relationships between movies based on user interaction data.

## Code Overview

* Matrix Factorization Model:
Defined using PyTorch nn.Module.
Contains user and item embeddings initialized with random weights.

* Loader Class:
Custom dataset class that prepares the input tensors for training.
Converts raw movie and user IDs to mapped indices for embedding layers.

* Training:
Trains the matrix factorization model using Adam optimizer over multiple epochs.
Outputs loss values to monitor training progress.

* Clustering:
Uses trained movie embeddings to cluster movies using KMeans.
Outputs top movies in each cluster based on user ratings.
