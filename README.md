# **Movie Recommendation System**

This project implements a User-Based Collaborative Filtering Movie Recommendation System using the MovieLens dataset. It analyzes user preferences and recommends movies similar users have liked.

## **Features**

* User-based collaborative filtering using cosine similarity

* Interactive recommendation generation

* Heatmap visualization of user similarity

* Built using pandas, scikit-learn, matplotlib, and seaborn

## **Dataset**

Make sure you have the following files in your project directory:

* movies.csv — contains movie IDs, titles, and genres

* ratings.csv — contains user ratings for different movies

You can download the dataset from MovieLens Latest Small Dataset.

## **How It Works**

1.Data Loading: Reads and merges movies.csv and ratings.csv.

2.User-Movie Matrix: Creates a pivot table of users and their rated movies.

3.Cosine Similarity: Computes similarity between users based on their rating vectors.

4.Recommendation: Suggests movies that similar users have liked but the target user hasn't seen yet.

**Sample Output**

Example usage to recommend movies for a user:

user_id = 6

recommendations = recommend_movies(user_id)

Output:

Generating recommendations for User 6...

Recommended movies:

  Toy Story (1995) (score: 132.77)
  
  Star Wars: Episode IV - A New Hope (1977) (score: 118.19)
  
  Mission: Impossible (1996) (score: 110.96)
  
  Matrix, The (1999) (score: 102.83)
  
  Star Wars: Episode V - The Empire Strikes Back (1980) (score: 93.75)
## **Visualization**

A heatmap of the user similarity matrix is plotted using the first 10 users

## **Requirements**

Install the dependencies using pip:

pip install pandas scikit-learn matplotlib seaborn

## Future Improvements


* Add item-based filtering and hybrid recommendation

* Integrate Flask for a web UI

* Allow dynamic input for users
