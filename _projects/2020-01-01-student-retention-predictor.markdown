---
layout: project_with_colaborator_and_website
title:  "Student Retention Predictor"
date:   2020-01-01 11:54:46
categories:
- project
img: srp.png
thumb: thumb02.jpg
collaborator: https://www.linkedin.com/in/nikhilkapahi/
website: https://feaindia.org/
---
## Student Retention Predictor
------------

### Overview
With this project we intend to predict the likelihood of a student to stick to a selected course and complete it at the time of joining based on the student's background, family's background and also based on some information about the center and faculty. It can also be thought of as a measure for the level of commitment in a student.

We took the data from a school for underprivileged youth in India and we applied Machine Learning principles to achieve this goal.

### Motivation
My friend and collaborator, Nikhil, volunteered in FEA some years ago and had an idea that we apply our recently acquired knowledge in Data Science and Machine Learning to give meaningful inputs to the organization so that they could better focus thier efforts. We set out to answer some questions such as:
* Which features are important
* Does factors like age, gender, family income, family education etc. affect the student's level of commitment
* Which features related to center and faculty could we improve to keep the student interested in the course
* Does the faculty agree with some of the predictions made by the model (just to compare human intuition with it)
* What changes could we make to retain the kind of students who choose to leave the organization

### Challenges we faced with feature engineering
The greatest challenge for us was, and continues to be, the unclean data! We had been practicing our machine learning skills on tailor made clean data and this was the first time we were actually training a model on a real-world dataset.

In addition to a ton of null values, we found that the data is unreliable for many features. For example, the age for some students were as absurd as 120 and -15 years! So, we had to make a lot of assumptions in order to make the dataset somewhat sensible.

Having said that, when we checked the correlations between features we found that they were in resonance with our intuition which led us to conclude that the dataset was not completely unreliable. Once we filled all the null values based on correlations between features we were surprised to see that for most features the data was well distributed. Only some features had a slight positive skew but many had considerable kurtosis before we handled the outliers.

One more pain point that we haven't yet solved is that a few nominal features have too many categories and when we try to encode them or use binning there is considerable information loss and the accuracy is negatively affected.

### Challenges we faced with training the model
We tried a number of different models for this binary classification problem based on regression, neural nets and decision trees, namely Logistic Regression, Deep Neural Nets, CatBoost, LightGBM, XGBoost and Random Forest Classifier. We got the best results with minimum tuning in CatBoost model. We still have some more models in mind to try such as SVM and Gaussian Naive Bayes.

The target feature had 63% of the examples in one category, so the accuracy of our model had to be at least better than that. With CatBoost Classifier we have managed to get 77% test accuracy so far. We have some ideas to make it even better and plan to try them out in the near future such as tuning the hyperparameters using grid search, spending some more time to understand the data & do better feature engineering and finally when we get a good enough score in a few models we could also go for ensemble methods to introduce some bias to reduce overfitting.

### Outcome
Based on the CatBoost model we ranked the features based on their importance, and also inferred a few things based on the correlations between features. We presented our findings to FEA and they were pleased with the results. We discussed some other ideas as well to which Machine Learning could be applied and they were keen on providing us with different data for the same.

We hope to further our knowledge in the field and apply the same to change the world for the better.