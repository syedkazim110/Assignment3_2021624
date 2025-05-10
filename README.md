# Assignment3_2021624
This repository contains a comparison of **Convolutional Neural Networks (CNN)** and **Recurrent Neural Networks (RNN)** for collaborative filtering on the [MovieLens-1M dataset]https://grouplens.org/datasets/movielens/. The task is to predict user ratings for movies and evaluate performance using **RMSE** and **MAE**.

## 📂 Repository Structure
├── Collaborative_Filtering_CNN_vs_RNN.ipynb # Main notebook
├── README.md # This file


## 📊 Dataset

- **Source:** [MovieLens 1M](https://grouplens.org/datasets/movielens/1m/)
- Contains 1 million ratings from 6,000 users on 4,000 movies.
- Ratings are in the range of **1 to 5**.
- Preprocessing includes label encoding of users and movies.

## 🧠 Models

### 1. CNN-Based Collaborative Filtering
- User and item embeddings concatenated.
- Passed through 1D convolution and dense layers.
- Kernel size adjusted to avoid negative dimensions.

### 2. RNN-Based Collaborative Filtering
- User and item embeddings fed as sequence input.
- Processed using a simple RNN layer followed by dense layers.

## 🧪 Evaluation Metrics

- **Root Mean Squared Error (RMSE)**
- **Mean Absolute Error (MAE)**

| Model | RMSE   | MAE    |
|-------|--------|--------|
| CNN   | 0.8796 | 0.6711 |
| RNN   | 0.8841 | 0.6714 |

> CNN slightly outperformed RNN on both RMSE and MAE.
