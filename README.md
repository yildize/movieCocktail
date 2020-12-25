# Movie Combiner 
* Movie Combiner suggests you new movies based on the selected combination of movies.
* Not sure which movie to watch? Want to watch something similar to movies you've watched before?
* Search and select movies you've already watch, mix them as you wish and get the closest movies to the combination.
* Here is the link of the app: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/yildize/movieCombiner/master?urlpath=voila%2Frender%2FmovieCombiner.ipynb)

## How it Works?
* For example you can search for the movies **the Matrix (1999)** and **Titanic (1997)**,combine them as you wish and find the top ten closest movies to this combination.

## Distance?
* Any distance value less than 0.5 represents a significant similarity between the combination and the suggested movie. It is basically the L2 distance between vectors.

## Under the Hood
* Movie combiner uses movie embeddings obtained by a collaborative filtering model trained on 25m movie ratings.
* By using the embedding vectors of selected movies, a new combined embedding vector is generated. After that, it is all about finding the closest L2 distances to the generated new embedding vector.

## Tips
* This project is done for educational purposes only, there might be some bugs on the GUI.
* Search bar only allows searches of three or more characters. So if you are looking for a movie '21' you should search as '21 (' or if you're looking for the movie 'V' then you should search as 'V ('
