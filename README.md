# Netflix_Recommendation_Engine 🎥: Using the data from https://www.kaggle.com/datasets/shivamb/netflix-shows

### This is a group project that I worked on in college. The group was Rachel, Jade, Richard, and me.

- The idea behind this was to recommend similar movies, through collaborative filtering.   
- First, we would combine all the text in certain categories like "Title", "Cast", "Rating", and more.   
- Then, using the combined text, we put it through a tf-idf vectorizer.  
  - This counts the words used in each combined text, and divides by how frequently it appears. This make it so that the weight of the words depends on how frequently it appears.
  - For example, "the" would be a word that appears in basically every movie. Therefore, the word "the" would have a low weight.
- We also used sentence transformers, to compare with the tf-idf vectorizer.
- Then we used cosine similarity to compare the combined text of the movies with other movies, which would give us a number 0-1, where 0 is not similar.
- Finally, we used PCA to clump together similar movies, and we graphed it.
