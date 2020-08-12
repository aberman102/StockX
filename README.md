# Sneaker Resale Value Predictive Model

Flatiron Module 5 Project Avidan Berman

### Project Overview

Currently one of the few unregulated resale markets left, the Sneaker industry has been quietly booming. Thanks to Michael Jordan in the 1980's, we have seen a massive rise in the popularity of sneakers. This has opened the opportunity to make incredible amounts of money. In this project I take on the challenge of attempting to build a model that can predict the future value of sneakers before they come out.

While exploring our data, these are some questions our team looked to address:

- Does it matter what season a sneaker is released?

- Is there a relationship between the type of shoe that is released and the price it retails at?

- Does Nike Sneakers resale at a higher average price than Adidas Sneakers?

### The Approach

- Scrape data from StockX's API
- Scrape twitter information on each sneaker released
- Engineer novel features to give model deeper insight
- Perform EDA on the dataset and create visualizations using the Seaborn Library
- Build and test multiple prediction models

### Conclusions

- Using an ANOVA Test I determined that there is no statistical difference between Season Released and Average Profit.
- Using an ANOVA Test I determined that there is a statistical difference between Sneaker Category and Retail Price.
- Using a Two Tailed T-Test I determined that there a statisitcal difference between Average Profit for Nike and Adidas Sneakers.

### The Model

I started by creating a training and testing set with a train-test split method. Next, I tested multiple models and used the accuracy and f1 metric's in addition to comparing false positive rates to judge the abilities of our model. The models I tested were Logistic Regression, Decision Tree, Random Forest , Voting Classifier, and an XG-Boost. To solve for class imbalance I generally set the class hyperparameter to 'balanced'. I found that the XG-Boost produced the best results on the test set. The model's accuracy score was 95.29% and an F1 score of 46.51%.

### Recommendations and Future of the Project

- My first recommendation is to ignore the season in which a sneaker comes out, I have found that it isn't a significant factor in future resale values.
- My second recommendation is to understand that different types of sneakers retail at different prices, this lets us know that you should prepare your future investment funds accordingly.
- my third recommendation is to understand that while Nike and Adidas are close competitors, there is a difference in average profits based off of the brand producing the sneaker.

In the future I would like to build on this project to include Neural Network predictons. Additionally I would like to also build a linear model to predict the actual profit of a shoe before it is released in order to prioritize efforts to aquiring specific sneakers.
