# Movie-Watch-Pattern-Clustering_202401100300171
# Movie Watch Pattern Clustering

This project focuses on clustering users based on their movie watching patterns, using features such as watching time, genre preferences, and rating behavior. The objective is to identify user segments that can help improve recommendation systems and marketing strategies for streaming platforms.

## Dataset
The dataset contains the following columns:
- `watch_time_hour`: Hour of the day (0-23) when the user typically watches movies.
- `genre_preference`: The user's favorite genre (e.g., action, comedy, thriller).
- `avg_rating_given`: The average rating (numeric) the user gives to movies.

## Project Structure
- `movie_watch.csv`: Input dataset.
- `clustering_analysis.ipynb` or code block: Contains data preprocessing, clustering, and visualization steps.
- `Movie Watch Pattern Clustering Report`: Contains methodology and findings.

## Methodology
1. **Preprocessing**
   - Encode categorical feature (`genre_preference`) using one-hot encoding.
   - Scale numerical features (`watch_time_hour`, `avg_rating_given`) using `StandardScaler`.

2. **Clustering**
   - Use K-Means clustering to group users.
   - Determine the optimal number of clusters using the Elbow Method.

3. **Evaluation**
   - Silhouette Score
   - Davies-Bouldin Index

4. **Visualization**
   - Use PCA for 2D representation of high-dimensional clusters.

## Requirements
- Python 3.x
- pandas
- scikit-learn
- matplotlib
- seaborn

Install the dependencies using:
```bash
pip install pandas scikit-learn matplotlib seaborn
```

## Usage
1. Load the dataset.
2. Run the clustering pipeline.
3. Visualize clusters and evaluate metrics.

## References
- Scikit-learn Documentation: https://scikit-learn.org/stable/
- Seaborn Documentation: https://seaborn.pydata.org/
- "Data Clustering: 50 Years Beyond K-Means" by Anil K. Jain

## License
This project is open-source and free to use for educational and research purposes.

