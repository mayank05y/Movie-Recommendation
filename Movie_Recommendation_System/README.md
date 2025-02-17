Movie Recommendation System
This GitHub repository contains code for building a movie recommendation system using collaborative filtering. The system employs both content-based and collaborative filtering techniques. The code is implemented in Python and utilizes the pandas, numpy, matplotlib, and seaborn libraries for data manipulation, analysis, and visualization.

Here's a breakdown of the code:

1.Data Loading and Exploration:
•	Loads movie ratings data from the 'Movie_Id_Titles' file.
•	Loads movie titles data from the 'Movie_Id_Titles' file.
•	Performs exploratory data analysis, including checking the shape of the data, the number of unique users and items, and displaying sample data.


2.Data Preprocessing:
•	Selects relevant columns from the movie titles data.
•	Merges the ratings data with the processed movie titles data based on the item_id.


3.Exploratory Data Analysis (EDA):
•	Uses matplotlib and seaborn for EDA, including visualizations of movie ratings and viewer counts.
•	Identifies that many movies have been rated by a small number of viewers, leading to a decision to discard movies with low viewer counts.


4.Creating Movie Recommendation:
•	Constructs a user-item matrix with user ratings for each movie.
•	Identifies the most-rated movies based on viewer counts.
•	Selects a movie (e.g., "Star Wars (1977)") to generate recommendations.
•	Computes the correlation between the selected movie and all other movies in the dataset.
•	Filters out movies with low viewer counts.
•	Provides movie recommendations based on correlation.


5.Prediction for a Specific Movie:
•	Defines a function (predict_movies) to predict and recommend movies based on user ratings.
•	Demonstrates the prediction for a specific movie ("Indiana Jones and the Last Crusade (1989)").
•	The code provides a foundation for building a movie recommendation system and can be extended for larger datasets or integrated into a larger project. Users can customize the movie selection for recommendations and further optimize the recommendation algorithm based on specific use cases.