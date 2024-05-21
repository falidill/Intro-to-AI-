# Personalized Recommendations for Amazon Prime:

User Documentation

Project Overview

This project aims to enhance viewer engagement and satisfaction on the Amazon Prime platform by providing personalized content suggestions by leveraging machine learning techniques. It develops a recommendation system that analyzes user behavior and preferences to offer tailored movie recommendations.
Data Sources
The project utilizes two datasets obtained from Kaggle:
movies.csv: Contains information about movies, including movie IDs, titles, and genres.
ratings.csv: Consists of user ratings for movies, with columns for user IDs, movie IDs, ratings given, and timestamps.
Tools and Techniques Used
The project employs the following tools and libraries:
•	Python
•	Jupyter Notebook
•	Pandas
•	Scikit-learn
•	Surprise
•	Matplotlib
•	Seaborn

Usage Instructions

To utilize the recommendation system developed in this project, follow the steps outlined below:

Step 1: Data Preparation
Ensure that you have the movies.csv and ratings.csv files available.
Load the datasets into separate pandas DataFrame objects (df1 for movies data and df2 for ratings data) in Python using your preferred environment (e.g., Jupyter Notebook).

Step 2: Data Cleaning
Remove any rows with missing values from both DataFrames (df1 and df2) using the provided code snippets.
Eliminate duplicate rows from both DataFrames to ensure data cleanliness and accuracy.

Step 3: Exploratory Data Analysis (EDA)
Explore the descriptive statistics of the datasets to gain insights into their distributions and characteristics.
Visualize the data, such as the frequency distribution of movie genres, to understand patterns and trends.

Step 4: Model Training
Initialize a reader object specifying the rating scale based on the minimum and maximum ratings in the ratings dataset (df2).
Load the data into a Surprise Dataset object and split it into training and testing sets.
Choose a recommendation model (e.g., Singular Value Decomposition) and train it on the training set.
Generate predictions for the test set using the trained model and evaluate its performance using Root Mean Square Error (RMSE).

Step 5: Generating Recommendations
Define a function (get_user_recommendations) that takes a user ID, recommendation model, and number of recommendations as input parameters.
Within the function, predict ratings for unrated movies by the specified user and select the top recommended movies based on their predicted ratings.
Utilize the function to generate personalized movie recommendations for users.

Example Usage
  
Replace the user_id variable with the ID of the user for whose recommendations are desired. Ensure that the model variable is assigned to the trained recommendation model. Adjust the n_recommendations variable as needed to specify the number of recommendations to return.

Conclusion
The Personalized Recommendations for Amazon Prime project provides a framework for building and deploying a recommendation system to enhance viewer engagement and satisfaction on the Amazon Prime platform. By leveraging machine learning algorithms and user data, personalized content suggestions can significantly improve the platform's performance and user experience.

For further details and implementation, refer to the provided code snippets and instructions in this documentation. 

Happy recommending!

