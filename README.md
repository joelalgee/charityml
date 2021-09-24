# CharityML Donor Prediction

Predicting the best donors for CharityML using supervised learning techniques in Python

## Summary

CharityML is a fictitious charity organization located in the heart of Silicon Valley that was established to provide financial support for people eager to learn machine learning. After nearly 32,000 letters were sent to people in the community, CharityML determined that every donation they received came from someone that was making more than $50,000 annually. To expand their potential donor base, CharityML has decided to send letters to residents of California, but to only those most likely to donate to the charity.

In this project, I applied supervised learning techniques to predict which members of the population earned above $50,000 based on census data.

This project had a series of predefined steps to follow, with the analysis for each step needing to be coded. Techniques called upon included feature transformation and scaling, AdaBoost classifier, Logistic Regression, Random Forest classifier, model tuning using a grid search, and extracting feature importances.

The custom packages for evaluation cannot be shared, so the only script available here is finding_donors.html, a static HTML version of the Jupyter Notebook file. The data is included for reference.

## Files

### finding_donors.html

Static HTML version of the step-by-step analysis and discussion.

### census.csv

Modified census dataset consisting of approximately 32,000 data points, with each datapoint having 13 features. This dataset is a modified version of the dataset published in the paper *"Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid",* by Ron Kohavi. You may find this paper [online](https://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf), with the original dataset hosted on [UCI](https://archive.ics.uci.edu/ml/datasets/Census+Income).

## Results

The accuracy score for the model tuned through grid search was 0.88% better that that before tuning, and the F-score was 1.86% better. With 15 million potential letter recipients, an improvement of 1% accuracy could represent the difference between 150,000 letters being sent or not, which has a significant financial impact by reducing either needless cost or missed donation opportunities. An improved F-score suggests better precision, so less letters being sent to people who earn under $50K.

The tuned model scores were a huge improvement on the naive predictor benchmarks (Accuracy score: 0.2478, F-score: 0.2917). This showed that the model provided significant, genuine insight.

## Credits

This project, parts of the code, and the modified data were provided by [Udacity](https://www.udacity.com) as part of their [Intro to Machine Learning with Pytorch nanodegree](https://www.udacity.com/course/intro-to-machine-learning-nanodegree--nd229). Original data were provided by [UCI Center for Machine Learning and Intelligent Systems](https://archive.ics.uci.edu/ml/datasets/Census+Income).
