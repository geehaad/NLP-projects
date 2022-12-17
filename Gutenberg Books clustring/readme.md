<h3>Error Analysis</h3>
<h4>Idea:</h4>
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
