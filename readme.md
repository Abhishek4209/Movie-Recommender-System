# Movie Recommender System using Cosine Similarity and Count Vectorizer

![plate](./example.png)

This Movie Recommender System is built using Python and utilizes cosine similarity along with Count Vectorizer for recommending movies based on their similarity to the user's preferences.

## Overview

The system works by analyzing the textual data associated with each movie, such as the movie title, genre, and synopsis. It then creates a numerical representation of this textual data using Count Vectorizer, which converts text data into numerical vectors. Cosine similarity is then used to measure the similarity between these numerical vectors.

## Features

- **Recommendation Generation**: Given a user's preferences (such as preferred genre or keywords), the system recommends a list of movies that are most similar to the user's input.
- **Flexible Input**: Users can input their preferences through various means, such as selecting a genre or entering keywords.
- **Scalability**: The system can handle a large number of movies efficiently, making it suitable for large movie databases.
- **Easy Integration**: The code is modular and well-documented, making it easy to integrate into existing applications or projects.

## Technologies Used

- **Python**: The primary programming language used for developing the recommender system.
- **Scikit-learn**: Utilized for implementing Count Vectorizer for text vectorization and cosine similarity calculation.
- **Pandas**: Used for data manipulation and handling movie data.
- **nltk**:For performing text to numeric operation. 
- **Flask (optional)**: Can be integrated with a Flask web application for providing a user interface.

## Usage

1. **Install Dependencies**: Make sure you have Python installed on your system along with the necessary libraries mentioned in the `requirements.txt` file.
   
2. **Prepare Data**: Provide the system with movie data in a suitable format. The data should include textual information such as movie title, genre, and synopsis.

3. **Run the System**: Execute the main Python script (`app.py` or similarly named) to run the recommender system.

4. **Input Preferences**: Follow the prompts to input your preferences, such as preferred genre or keywords.

5. **Get Recommendations**: The system will then generate a list of recommended movies based on your preferences.

## Example

```python
# Import necessary modules
from movie_recommender import MovieRecommender

# Create an instance of MovieRecommender
recommender = MovieRecommender()

# Input user preferences
genre = "Action"
keywords = ["superhero", "thrilling", "explosive"]

# Get movie recommendations
recommendations = recommender.get_recommendations(genre, keywords)

# Print recommended movies
print(recommendations)
