<h2> Overall </h2>
The goal of this project is to classify books by its title, compare the
different models we used; analyze each one and come out the best model
which is most efficient in this problem.

<h2>The dataset:</h2>
1. We scrapped 5 books with different authors and with the same
genre (Philosophy genre):

- The Art of War,

- Beyond Good and Evil,

- The Psychology and Pedagogy of Anger,

- The Republic,

- Meditations

2. Created 200 partitions of each book text, each partition contains
100 words.

3. We come out with a DataFrame contains:

• Partitions columns,

• The title of the book column,

• Author column.

<h2>Preprocess the data:</h2>

• Converted the text to lower case.

• Removed any special characters.

• Used RegexpTokenizer to tokenize the text.

• Created our stop words list and removed from our text.

• Remove single char, and chars with size 2.

<h2>Visualization:</h2>

• Word Cloud

Data visualizations (like charts, graphs, infographics, and more) give a valuable way to
visualize, and statistical important information, but what if your raw data is text-based?
Word cloud generators can help simplify this process.<br>

A word cloud is a collection, or cluster, of words depicted in different sizes. The
bigger and bolder the word appears, the more often it’s mentioned within a given
text and the more important it is.

<h2>Modeling</h2>
- Use Different algorithms and evaluate them:

1. SVM,

2. Decision Tree,

3. k-Nearest Neighbor.

- K-Fold cross validation:

We used K-Fold cross validation with 10 folds and compared the
accuracy of each model, then chose the champion model, and the
transformation and the classification algorithms, and chose it also by
Mean, Bias, variance, standard deviation.

<h3>Choosing Champion Model:</h3>

• In Bag of words we choose SVM according to Accuracy results and Cross -
validation results also calculate mean and variance and choose Algorithm
with high accuracy, mean and low variance of cross-validation results.

• In n-gram we choose Decision Tree Classifier according to Accuracy and
Cross-validation results also calculate mean and variance and choose
Algorithm with high accuracy, mean and low variance of Cross-validation
results.

• In TF-IDF we choose SVM according to Accuracy and Cross-validation results
also calculate mean and variance and choose Algorithm with high accuracy,
mean and low variance of validation results.

• From above results we choose BOW approach with Support Vector Machine
Classifier as Champion model according to results.

• We used K-Fold cross validation with 10 folds and compared the
accuracy of each model, then chose the champion model, and the
transformation and the classification algorithms, and chose it also by
Mean, Bias, variance, standard deviation.

<h2>Error Analysis:</h2>

• We calculated the number of wrong prediction labels by comparing the
predicted output with the actual output of each class.

• And plotted the number of wrong predictions of each class.

<h2>Play with features and decrease accuracy:</h2>

After decided the Champion book, we tried to add some books that
does not belong to the same category of the original book, without
preprocess its text, and also add some special characters to the original
dataset.
