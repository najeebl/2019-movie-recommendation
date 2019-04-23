# Movie Recommendation
Build a recommendation engine which will predict Top 10 recommended movies for a user

# Datasets
- Movie Lens 100K: 
https://grouplens.org/datasets/movielens/100k/
Includes:
* u.data     -- The full u data set, 100000 ratings by 943 users on 1682 items.
              Each user has rated at least 20 movies.  Users and items are
              numbered consecutively from 1.  The data is randomly
              ordered. This is a tab separated list of 
	         user id | item id | rating | timestamp. 
              The time stamps are unix seconds since 1/1/1970 UTC   

* u.info     -- The number of users, items, and ratings in the u data set.

* u.item     -- Information about the items (movies); this is a tab separated
              list of
              movie id | movie title | release date | video release date |
              IMDb URL | unknown | Action | Adventure | Animation |
              Children's | Comedy | Crime | Documentary | Drama | Fantasy |
              Film-Noir | Horror | Musical | Mystery | Romance | Sci-Fi |
              Thriller | War | Western |
              The last 19 fields are the genres, a 1 indicates the movie
              is of that genre, a 0 indicates it is not; movies can be in
              several genres at once.
              The movie ids are the ones used in the u.data data set.

* u.genre    -- A list of the genres.

* u.user     -- Demographic information about the users; this is a tab
              separated list of
              user id | age | gender | occupation | zip code
              The user ids are the ones used in the u.data data set.

* u.occupation -- A list of the occupations.

- Tag database with movie tags?
- IMDB?
- Pass in favorite movies


# Modeling Strategy
- Passing in 3 columns: user, user rating, movie id
- Use Factorization Engine to predict rating for movie
- Use KNN to predict top 10 movies to recommend
- Add more features: demographics, release date.
