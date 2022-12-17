<h1>Overview:</h1>
The goal of this project is to produce clusters from our books, compare the
different models we used; analyze each one and come out the best model
which is most efficient in this problem.

<h2>The dataset:</h2>
1. We imported 5 books with different authors and different genres
from Gutenberg.
- Austen-emma
- Bible-kjv
- Chesterton-brown
- Shakespeare-caesar
- Blake-poems

2. Created 200 partitions of each book text, each partition contains
150 words.
3. We come out with a DataFrame contains:
• Partitions columns
• The label of the book column

<h2>Preprocess the data:</h2>

• Converted the text to lower case.

• Removed any special characters.

• Used RegexpTokenizer to tokenize the text.

• Created our stop words list and removed from our text.

• Remove single char, and chars with size 2.

• Label Encoder.

<h2>Text Transformations:</h2>
• BOW<br>
• TF-IDF<br>
• LDA<br>
• Word-Embedding.<br>
We used PCA to reduce the number of features of every one of the
four vectorizers to plot them in 2d.<br>

<h2>Error Analysis</h2>
<h3>Idea:</h3>
- In the error analysis process, we looked at each cluster in our
chosen (champion) model, and visualize how they cluster the
books, and how much data they managed to cluster, and tried to
find the most frequent words (10 words) in each cluster.<br>

- We compared the most frequent words in each cluster and find the
most similar ones.<br>

- We found that the clusters separate the docs well, and in the most
occurred words, there is no big conflict between the clusters.<br>

- So, we searched for the paragraphs that the model failed to cluster
right and print the most occurred words.<br>

- We want to reduce the similarity between each cluster, the more
the cluster are far from each other, the more the model is good.<br>

- The words that appear in many clusters are the ones that confuse
our model, and that led to increase the error in it.

<h2>Model:</h2>
• then used K-means with Kappa, , homogeneity_score, v_measure_score and silhoutte algorithms to choose best K 

•  We used the error analysis technique with our champion model:<br>

Kmeans with TFIDF.<br>

•  We made a data frame contains each word with its TF IDF values
and what the number of the cluster it was belong to.<br>

•  We get the most occurred words in each cluster (0:4)
