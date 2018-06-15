# Sentiment-Analysis

<hr>

In the following code we built a SVM classifier for IMDB Movies reviews.

<hr>

* <b>Data-Sets</b><br>
We used a data set that contains 49950 IMDB reviews taged as positive and negative<br>
The training set is consisted of 70% of the reviews, while the test set is consisted of 30% of them.<br>
<hr>
* <b>Analyzing & Pre-Processing The Data</b><br>
We tried to find and grade the most significant set of tokens that will contribute more information for the reviews Sentiment's.
Afterward we chose the TF-IDF for gradeing and normalize the tokens to vectors.
On the TF-IDF we chose to use the Ngram model to get information from the previews world, set it up to (1,5), and using stopword to clean up the noisy world and custom made function to tokenized the reviews by using WordNetLemmatizer to gain one appearance for words that have same meaning in different declensions.
The SVM classifier how's get the output of the TF-IDF using A linear kernel and the C chose to be 15.
<hr>

* <b>Performance</b><br>
We saw that when we try to "clean" the pos and neg train individually the acc wes bad 77%, then we use the TF-IDF to give a unuiq score to each token according to its appearance in a nagetive or a positive sentiment respectivly each document.

We could do so since TF-IDF is a numerical statistic that is intended to reflect how important a word is to a document in a our text, we than got a satisfying accuracy percentage wich stands on 88%.
<hr>
