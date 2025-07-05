# Movie Rating Prediction with Python

This project predicts the IMDb rating of a movie based on features like genre, year, duration, and votes using machine learning models in Python.

Project Objective:

To build a regression model that can estimate the IMDb rating of Indian movies using historical movie data.  
This helps in understanding which factors (like genres, popularity, release year) influence user or critic ratings.

Technologies Used:

- Python
- Pandas
- NumPy
- Scikit-learn (RandomForestRegressor)
- Jupyter Notebook

Dataset:

- Dataset: IMDb Movies India.csv
- Source: IMDb (Indian Movies)
- Features:
  - Name, Year, Duration, Genre, Rating, Votes, Director, Actor 1/2/3

Steps Performed:

1. Data Cleaning
   - Removed missing values from key columns.
   - Converted duration to minutes.
   - Cleaned and converted vote counts to integers.
   - Split multiple genres into lists for one-hot encoding.

2. Feature Engineering
   - Extracted top 15 genres and applied one-hot encoding.
   - Used only relevant numeric and categorical features.

3. Model Building
   - Used RandomForestRegressor to predict ratings.
   - Split data into training and validation sets (80/20).

4. Evaluation
   - Used MAE (Mean Absolute Error) and RMSE (Root Mean Squared Error) as performance metrics.

Example Output:
MAE : 0.82 rating points
RMSE : 1.07 rating points


The model predicts IMDb ratings with an average error of less than 1 star.

How to Run:

1. Clone the repository  
   `git clone https://github.com/swatijoshi765/movie-rating-prediction.git`

2. Install required libraries  
   `pip install pandas numpy scikit-learn`

3. Run the notebook  
   Open `movie rating.ipynb` in Jupyter or VS Code and run all cells.

Future Improvements:

- Add Director and Actor features using encoding or embeddings.
- Try advanced models (XGBoost, LightGBM).
- Tune hyperparameters for better accuracy.
- Add a Streamlit or Flask web app frontend.

Learnings:

- Data cleaning is crucial  
- Feature selection and engineering improve model performance  
- Random forests work well for regression problems with categorical data

Author:

Swati Joshi  
Data Science Student and Aspiring Data Analyst



