# Building a Spam Filter with Naive Bayes

## Introduction
Nowadays, communication channels are constantly attacked by fraudulent mechanisms, which tend to "steal" time and money from people and organizations. Spamming activity is one of them and wastes people's time, while also "eats up" a lot of network bandwidth. Data Science could not be absent from this battle front and, fortunately, it is capable to offer valuable solutions.

## Scope
This project aims to build a **Spam Filter** using Python, which classifies new messages as `spam` or `ham`, by utilizing the Mutlinomial Naive Bayes Theorem. Its accuracy aims for a ratio of above 90%, or else, we expect that more than 90% of the new messages will be classified correctly.

## Scenario

The Data Corp board decided to boost the youth market sales, by introducing a new mobile app, under the 'Communication' category. In order to beat its rivals, a potential competitive advantage was scrutinised - **anti-spamming**. So, the Data Science department I belong to, was charged to come in contact with the engineering team and provide them with an algorithm, that takes as input the user's sms and automatically filters out the spam ones. This algorithm would be implemented to the new app and should score an accuracy ratio of at least 90% (the standard one achieved by the competitors).

## Data Sets

To train the algorithm, we are going to use a dataset of 5.572 SMS messages that are already classified by humans. The dataset was put together by Tiago A. Almeida and José María Gómez Hidalgo and it can be downloaded from the The [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection). The data collection process is described in more details on this [page](http://www.dt.fee.unicamp.br/~tiago/smsspamcollection/#composition), where you can also find some of the papers authored by Tiago A. Almeida and José María Gómez Hidalgo.

## Roadmap

1. We briefly explore the full data set, consisting of 5.572 SMS messages, which is distributed among `spam` and `ham` content by approximately 87% and 13%, respectively.

2. We randomise it, so as to retain the original spam/ham proportions and then divide it into two sub-sets, opting for a 80% — 20% split-up:

- `training_set`: used to “train” the computer how to classify messages
- `test_set`: used to finally test how good the spam filter is (accuracy)

3. We Pre-Process them by using a series of free Python libraries (including Pandas, NLTK and Re) and Extract the necessary Features, so as to feed the model with meaningful data and train it effectively.

4. Finally, we evaluate the model by measuring its classification accuracy as the percentage of succesfully labeled SMS.

## Conclusion

We managed to manipulate hundreds of SMS texts, preprocessed them effectively and encoded them into numeric vectors. As a result, we managed to train our model and provide the firm with an algorithm of 97% accuracy, fair above the initial target of 90%.

## Additional Analysis
There is quite a number of additional analyses to be performed, expanding this one. You are welcome to extend and shape yours in any direction you may prefer. For instance:

* You may try to run the algorithm, by exluding one or more of the aforementioned techinques (stemming, lemmatization etc) and figure out whether the final accuracy is positively affected.

* Analyze the 27 messages that were classified incorrectly and try to figure out why the algorithm classified them incorrectly.

[*It stands as an independent analysis in an effort to enhance my ability to communicate results, reason about data statistically and stay motivated to continuously implement newly aquired skills & capabilities, so as to enrich my portfolio of data science-oriented projects*]