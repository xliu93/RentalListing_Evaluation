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
2. Make thorough application of classification algorithms and compare results.
3. Learn to deal with categorical data and interactions among categories.

### METHOD
1. Breaking down the three levels of interest 'high', 'medium', and 'low', we can think of the three levels representing whether the building is under-valued, properly-valued, or over-valued by the owner, with the information provided. Thus, to achieve high accuracy, we need to model the expected value of a certain listing. This may include factors on room, location, service, appliances, attractiveness of description, good photos, market price of alternatives, etc. 
2. Currently we don't know what is the best approach, and we will investigate on different classification algorithms including but not limited to SVM, logistic regresssion, decision tree with AdaBoost.
3. Since we don't have an existing feature to indicate convenience of life around the building, we have to create either a score or category of it.  Possibly we can preprocess geographical data using clustering methods under the assumption that close locations will have similar community services. 
4. Number of bedrooms is somewhat a rigid demand when finding a rental, and it has few possible values, say 0(studio), 1, 2, 3, and 4+. We can regard it as categorical data under certain conditions. This also happends to our location clusters. We should decide whether to use different models for different categories or to use same model across categories.
5. The 'feature' column in dataset is somewhat repetitive to 'description' but in a structured way. We will try to find the contribution of additional information given by the text description as well as the interaction between the two features. 
6. More feature engineering will go on as we proceed with the project.

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
