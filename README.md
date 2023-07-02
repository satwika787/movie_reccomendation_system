# movie_reccomender
A movie recommendation system based on Content filtering using Cosine Similarity to provide personalized movie suggestions.

This project implements a movie recommender system using the _TMBD Movie Dataset_. 
The system recommends movies to users based on their preferences by analyzing movie overviews and genres.

It utilizes the **CountVectorizer** from the **scikit-learn** library for **feature extraction** and **cosine similarity** to calculate the similarity between movies.

## Dataset
The TMBD Movie Dataset is used as the source of movie data for this project. It contains information about movies, including their titles, overviews, and genres. The dataset is loaded using the `pandas` library.
### Setup and Usage
*  Ensure that the TMBD Movie Dataset file is available at the specified path `/content/TMBD Movie Dataset.csv`. If necessary, update the file path in the code.
*  Install the required dependencies, including `pandas` and `scikit-learn`.
*  Run the provided code to load the dataset, perform feature extraction, calculate cosine similarity, and define the recommendation function.
*  To recommend movies, call the `recommend()` function and pass the title of a movie as an argument. The function will output the top 10 recommended movies based on 
   similarity.
#### Results
The recommender system generates movie recommendations by analyzing the similarity between movie overviews and genres. The cosine similarity metric is used to measure the extent of similarity. By modifying the `max_features` parameter of the `CountVectorizer`, you can control the number of features considered during the calculation of similarity.
##### Future Improvements
Here are some improvements that can be considered for enhancing the movie recommender system:
* Incorporating additional features such as actors, directors, or release year to improve recommendation accuracy.


