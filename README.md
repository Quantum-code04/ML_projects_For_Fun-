# 🎬 Movie Recommendation System using k-Nearest Neighbors (kNN)

This project is a simple **movie recommendation system** built using the **k-Nearest Neighbors (kNN)** algorithm. It takes a random movie (via random index) and recommends a set of similar movies based on user ratings.

---

## 📁 Dataset

The project uses the [MovieLens dataset]([https://www.kaggle.com/datasets/grouplens/movielens-latest-small](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?resource=download)) from Kaggle:
- `movies.csv` – contains movie titles and genres.
- `ratings.csv` – contains user ratings for movies.

---

## 🛠️ Technologies Used

- **Python**
- **NumPy**
- **Pandas**
- **scikit-learn** (NearestNeighbors)
- **SciPy** (csr_matrix)

---

## 📌 How It Works

1. Loads `movies.csv` and `ratings.csv`.
2. Creates a **user-movie rating matrix** using pivot.
3. Converts the matrix to a **sparse matrix** using `csr_matrix`.
4. Fits the **kNN model** using cosine similarity.
5. Picks a **random movie index** and finds the most similar movies.
6. Prints the list of recommended movie titles.

---

## 📂 Project Structure

📦knn-movie-recommender/
┣ 📄 movies.csv
┣ 📄 ratings.csv
┣ 📄 knnrecommendation.pynb
┣ 📄 README.md

## 📝 Sample Output

Recommendations for Princess Bride, The (1987):

1: Monty Python and the Holy Grail (1975), with distance of 0.368708074092865:
2: Star Wars: Episode V - The Empire Strikes Back (1980), with distance of 0.39714330434799194:
3: Ferris Bueller's Day Off (1986), with distance of 0.39811694622039795:
4: Raiders of the Lost Ark (Indiana Jones and the Raiders of the Lost Ark) (1981), with distance of 0.4048547148704529:
5: Groundhog Day (1993), with distance of 0.4066782593727112:
