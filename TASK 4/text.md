Here’s the text for a GitHub repository based on your movie recommendation system:

---

# Movie Recommendation System 🎥

This project is a content-based movie recommendation system that suggests similar movies based on user preferences. The dataset consists of Hindi movies categorized by genres such as Action, Horror Thriller, Motivation, and Science-fiction action.

---

## Features ✨

- Utilizes cosine similarity and the k-Nearest Neighbors (k-NN) algorithm for recommendations.  
- Recommends movies based on the highest-rated movie a user has previously rated.  
- Supports different genres including Action, Horror Thriller, Motivation, and Science-fiction action.

---

## Dataset 📊

### Ratings Data
The ratings dataset includes information about user ratings for movies.

```python
ratings_data = {
    "userId": [1, 2, 1, 3, 4, 2, 5, 3, 6, 4],
    "movieId": [101, 101, 102, 103, 102, 103, 104, 105, 101, 105],
    "rating": [4.5, 3.0, 4.0, 5.0, 4.5, 4.8, 5.0, 3.5, 4.2, 4.0],
}
```

### Movies Data
The movies dataset includes movie IDs and their titles with genres:

```python
movies_data = {
    "movieId": [101, 102, 103, 104, 105],
    "title": [
        "Pushpa: The Rule-Part2 (Action)",
        "Singham Again (Action)",
        "Kalki 2898 AD (Science-fiction action film)",
        "Bhool Bhulaiya 3 (Horror Thriller)",
        "Srikanth (Motivation)",
    ],
}
```

---

## Methodology 🧠

1. Sparse Matrix Creation:  
   Converts the `ratings` dataset into a sparse matrix format, where rows represent movies and columns represent users.

2. Cosine Similarity with k-NN:  
   Leverages `scikit-learn`'s NearestNeighbors to find movies that are similar based on user ratings.

3. Recommendation Logic:  
   - Identifies the movie with the highest rating by the user.  
   - Finds the top `k` similar movies using k-NN.  
   - Excludes the movie already watched by the user.

---

## Example Usage 🛠️

### Input
User ID: `1`  
Top `3` recommendations.

### Output
```plaintext
Since you watched Pushpa: The Rule-Part2 (Action), you might also like:
Singham Again (Action)
Kalki 2898 AD (Science-fiction action film)
Bhool Bhulaiya 3 (Horror Thriller)
```

---

## Code Structure 📁

- `create_matrix`: Converts the data into a sparse matrix.  
- `find_similar_movies`: Finds movies similar to a given movie using k-NN.  
- `recommend_movies_for_user`: Provides personalized recommendations based on user ratings.

---

## Installation 🛠️

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
   cd movie-recommendation-system
   ```

2. Install required dependencies:
   ```bash
   pip install pandas numpy scikit-learn scipy
   ```

3. Run the script:
   ```bash
   python movie_recommendation.py
   ```

---

## Requirements 📋

- Python 3.8+  
- Libraries: `pandas`, `numpy`, `scikit-learn`, `scipy`

---

## Contributing 🤝

Contributions are welcome! Please feel free to submit a pull request or create an issue.

---

## License 📜

This project is licensed under the MIT License.

---

## Acknowledgements 🙏

- Scikit-learn for its robust machine learning algorithms.  
- Inspiration from Hindi cinema and its wide array of genres.

---

Feel free to customize this text further for your GitHub repository!
