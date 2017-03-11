# Project of Machine Learning and Computational Statistics

#### TOPIC IDEAS

(will be updated upon final decision of the group)

1. Research on how to combine different signals/strategies. As for alpha-seeking strategies, a large number of basic strategies, which are also known as signals, can be combined to construct a portfolio. The benefits are explained by Modern Portfolio Theory. We can figure out an approach to construct the portfolios using machine learning (I am able to provide some signals, with other references).
2. Statistical arbitrage strategy research, which is to find potential trade opportunities in high frequency market data, could be a good application of time-series prediction model. 
3. Market behavior research. Last semester I audited a few classes of Computing in Finance, the professor introduced a research topic of "Market Mimicking", which is to analyze the volatility before/after a market crash.

#### KEY DATES (from the course website)

- Feb 28 (Tues 5pm): Deadline for choosing project groups
- March 6 (Mon 9pm): Email one-sentence project idea(s) to adviser, along with personal intros
- March 8 (Wed 8:35–9:25pm): First meeting with advisers. Each group will give a 5-minute presentation of their project idea to their assigned project adviser, followed by brief discussing with adviser.
- March 23 (Thurs 6pm): Project Proposals Due
- Apr 19th (Wed 8:35–9L25pm): Second meeting with advisers
- May 3rd (Wed 8:35–9:25pm): Third meeting with advisers
- May 9th (Tues 5–7pm): Project Poster Session
- May 12th, 6pm: Final Project Reports Due



#### Project Topic
Multiclass Classification of Rental Listing Quality

#### Data Source
Kaggle, privided by Renthop.
https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries

##### Input:  50MB Json

Numbers: bathrooms, bedrooms, price in USD

Date: created

keys: building_id, listing_id, manager_id

Text: description, display_address, street_address

Categorical features: features

Geographical data: latitude, longitude

Photos: a list of photo links. 

##### Output:

Interest_level: this is the target variable. It has 3 categories: 'high', 'medium', 'low'

#### Project Goals
1. Learn to process multimedia data ranging from numbers, dates, categorical features, text, geographical data, and pictures(tentative).
2. Learn to preprocess geographical data using clustering.
3. Try different classification algorithms like SVM, logistic regresssion, decision tree with AdaBoost, to improve result.
4. Learn to deal with categorical data and interactions among categories.
5. Optional. Learn to use CNN to extract information from pictures. Reference: https://engineeringblog.yelp.com/2016/11/finding-beautiful-yelp-photos-using-deep-learning.html



