Naive Bayes Classification Report on the Iris Dataset

Abstract
This study applies four Naïve Bayes algorithms—Multinomial, Bernoulli, Gaussian, and Complement—on the Iris dataset to evaluate their classification effectiveness. Using Python's Scikit-learn library, we develop models to classify species based on sepal and petal measurements, using a train-test split for performance evaluation. The models' predictive capacities are analyzed through accuracy, precision, recall scores and confusion matrices, highlighting the unique strengths of each algorithm. This analysis aims to provide insight into how varying Naïve Bayes approaches handle continuous feature data, contributing to an understanding of model selection in machine learning classification tasks.
Introduction
Naive Bayes classifiers are a group of probabilistic algorithms based on Bayes' theorem, widely valued for their simplicity and efficiency. This study applies four Naive Bayes classifiers to the classic Iris dataset, a multivariate dataset ideal for classification tasks. The aim is to determine the efficacy of each Naive Bayes variant, showcasing their strengths in processing the Iris dataset's specific features and comparing their predictive accuracy through performance metrics.

Model
This study utilizes Scikit-learn's implementation of Naive Bayes classifiers, applying train-test split validation to separate the dataset into training and testing subsets (70% and 30%, respectively). Each Naive Bayes variant—MultinomialNB, BernoulliNB, GaussianNB, and ComplementNB—is trained on the Iris dataset, with results stored in an organized framework to capture accuracy, precision, recall, and confusion matrix data for comparative analysis.
MultinomialNB: Typically used for categorical data, this variant may be less suited for the continuous features of the Iris dataset, given its focus on word frequency and discrete distributions.
BernoulliNB: Designed for binary/Boolean features, BernoulliNB could perform sub optimally, as the dataset’s continuous attributes may not align well with its assumptions.
GaussianNB: The Gaussian Naive Bayes model is generally effective with continuous data, assuming a normal distribution within each class. Given the Iris dataset's numeric features, GaussianNB is anticipated to yield high classification accuracy.
ComplementNB: A variant suited for imbalanced datasets, ComplementNB was included for completeness and to observe its performance on a balanced dataset like Iris.
Each variant brings a unique approach to classification, showing us how different models with the same goal might adapt or struggle depending on data structure. Through this, we gain insights into model accuracy and into the workings of Naive Bayes models across the spectrum of data types.
 

Method:
In evaluating the performance of each Naive Bayes classifier on the Iris dataset, we utilized several evaluation metrics. These metrics provide insights into each model’s classification power, allowing us to compare their effectiveness in handling continuous data.

Evaluation Metrics:
Each model was evaluated based on the following metrics:
1.	Accuracy: The proportion of correctly classified instances.
2.	Precision: The ratio of correctly predicted positive observations to the total predicted positives.
3.	Recall: The ratio of correctly predicted positive observations to all actual positives.
4.	F1-Score: The weighted average of Precision and Recall.
5.	Confusion Matrix: A table that describes the performance of a model by comparing predicted values with actual values.


Conclusion
The GaussianNB model emerged as the best fit for the Iris dataset, achieving high classification accuracy across all metrics. Its assumption of normally distributed features is well-suited to continuous data, making it optimal in this case. The MultinomialNB model also performed well but is generally more suitable for discrete features. ComplementNB and BernoulliNB had weaker performances, especially BernoulliNB, as it is primarily designed for binary features and doesn’t handle continuous data effectively.
Recommendation
For this dataset, GaussianNB is the recommended model due to its excellent handling of continuous data. MultinomialNB could be an alternative if adjustments are made for discrete data.
