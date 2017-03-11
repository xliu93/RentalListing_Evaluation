# Project of Machine Learning and Computational Statistics

## TOPIC IDEA

### Introduction
In this project, we will build a predictive model of how popular an apartment rental listing is based on the listing content, in the hope of helping listing website better handle fraud control, identify potential listing quality issues, and allow owners and agents to better understand renters’ needs and preferences.. The apartments involved are located in New York City. Our objective is to give an estimation of the number of inquiries a listing has in the duration that the listing was live on the site, and label it with three categories: high, medium, and low level of interest. 

### PROBLEM OVERVIEW
The dataset is available on [Kaggle][1], provided by RentHop.
[1]: https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries

**Input: 70MB Json**

- Numbers: bathrooms, bedrooms, price in USD
- Date: the date that the listing is created
- keys: building_id, listing_id, manager_id
- Text: description, display_address, street_address
- Categorical features: features
- Geographical data: latitude, longitude
- Photos: zero or more images 

**Outcome**
- Interest_level: The level of interest is defined by the number of inquiries a listing has in the duration that the listing was live on the site, and has 3 categories: 'high', 'medium' and 'low'.

**Loss/Objective function**
- This is a classification problem, and we are intended to use logrithmic multi-class loss.


### PROJECT OBJECTIVE
1. Learn to process multimedia data ranging from numbers, dates, categorical features, text, geographical data, and pictures(if time permits, use CNN with [reference][2]).
2. Learn to preprocess geographical data using clustering.
3. Make thorough application of classification algorithms and compare results.
4. Learn to deal with categorical data and interactions among categories.

### METHOD
1. Currently we don't know what is the best approach, and we will investigate on different classification algorithms including SVM, logistic regresssion, decision tree with AdaBoost.
2. Engineer new features with available data to improve the performance of predictive model.

[2]: https://engineeringblog.yelp.com/2016/11/finding-beautiful-yelp-photos-using-deep-learning.html
<br>

## KEY DATES (from the course website)

- Feb 28 (Tues 5pm): Deadline for choosing project groups
- March 6 (Mon 9pm): Email one-sentence project idea(s) to adviser, along with personal intros
- March 8 (Wed 8:35–9:25pm): First meeting with advisers. Each group will give a 5-minute presentation of their project idea to their assigned project adviser, followed by brief discussing with adviser.
- March 23 (Thurs 6pm): Project Proposals Due
- Apr 19th (Wed 8:35–9L25pm): Second meeting with advisers
- May 3rd (Wed 8:35–9:25pm): Third meeting with advisers
- May 9th (Tues 5–7pm): Project Poster Session
- May 12th, 6pm: Final Project Reports Due
