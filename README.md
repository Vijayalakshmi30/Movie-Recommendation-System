# Movie Recommendation System

## Overview
The Movie Recommendation System is designed to predict user preferences for movies based on historical rating data. The project involves cleaning and preparing data, implementing collaborative filtering techniques, and evaluating model performance using different estimation methods and similarity measures.

## Key Features:
- **Collaborative Filtering**: Implemented both item-based and user-based collaborative filtering techniques.
- **Similarity Measures**: Used Cosine Similarity and Pearson Correlation for measuring similarity.
- **Estimation Methods**: Compared the Standard Estimate method and SVD Estimate method for rating predictions.
- **Performance Evaluation**: Calculated Mean Absolute Error (MAE) to evaluate prediction accuracy.

## Dataset
The system uses the MovieLens dataset, which contains 100,836 ratings across 9,742 movies from 610 users. The dataset includes:
- `movies.csv`: Movie information
- `ratings.csv`: User ratings
- `tags.csv`: User-generated tags
- `links.csv`: External movie information

Data Source: [MovieLens](https://grouplens.org/datasets/movielens/latest/)

## Methodology
### 1. Data Cleaning
- Merged the datasets (`movies.csv`, `ratings.csv`, `links.csv`).
- Filtered out movies with fewer than 100 ratings, reducing the dataset to 138 movies.

### 2. Collaborative Filtering
#### Item-based Collaborative Filtering
- Implemented 8 different combinations:
  1. Standard Estimate Method | Cosine Similarity | Manual function
  2. Standard Estimate Method | Cosine Similarity | Inbuilt function
  3. Standard Estimate Method | Pearson Correlation | Manual function
  4. Standard Estimate Method | Pearson Correlation | Inbuilt function
  5. SVD Estimate Method | Cosine Similarity | Manual function
  6. SVD Estimate Method | Cosine Similarity | Inbuilt function
  7. SVD Estimate Method | Pearson Correlation | Manual function
  8. SVD Estimate Method | Pearson Correlation | Inbuilt function

#### User-based Collaborative Filtering
- Evaluated using similar approaches as Item-based filtering.

### 3. Evaluation
- Compared the Standard Estimate and SVD Estimate methods using MAE.
- Results indicated that the SVD method outperformed the Standard Estimate in computational efficiency.

## Prerequisites
- Python 3.x
- NumPy, Pandas, SciPy for data manipulation
- Scikit-learn for similarity calculations

## Results
- The system provided accurate movie recommendations, with different approaches yielding comparable recommendations.
- SVD Estimate significantly reduced computation time compared to the Standard Estimate method.

## Conclusion
The project showcases how collaborative filtering can be applied to build an efficient recommendation system. Various methods and similarity measures were explored to optimize performance.
