Project description and motivation

Hallo and welcome to the Seattle Airbnb project. This project is part of the "Data Scientist nanodegree" by Udacity.
The purpose of the project is to analyze a real world dataset and communicate findings in an understandable manner. 
The dataset that was chosen is the Seattle Airbnb homes that contain data from Airbnb listings in the Seattle area.
The main goal of the project is to answer the three following questions:

1) What are the characteristics of a home that influence its price most and what is the importance of each charcteristic?
2) What is the average price of a home based on the amount of people it can accommodate?
3) What are the Top10 neighborhoods in regards with the mean price a home can have?

Libraries required to run the code

•	Numpy
•	Pandas
•	Matplotlib
•	Seaborn
•	Sklearn

Files included

•	README document
•	airbnb.ipynb:  Jupyter notebook where the code used to produce the results is written.
•	listings.csv:  CSV file that contains Airbnb home data for Seattle – provided by Udacity.

Summary of results

In this short analysis of the dataset, a ML linear regression model has been built to predict home prices based on other features a potential home can have. Due to the very large amount of independent variables,  I used the ‘ExtraTreesClassifier’ to select the most important features when it comes to predicting the price. Then, I insert those features in a linear regression model and derive the coefficients. This analysis showed that that what affects the price most, is the number of people that a listing can accommodate.  This has a strong positive correlation with the price. Similar trend was observed also with the “review_scores_location” feature, meaning that the location of the listing plays a key role to the price of the listing.

It is also notable, that the “review_scores_value”  has a negative correlation with price. Although at first this can sound strange, it reveals that people tend to give high scores in listings that have a low price. These are the most important features that influence the price. 
The analysis also illustrates the price level a home can reach based on the approximate amount of people it can accommodate.  Starting from 0-4 persons, the average price is a little bit above 100$ and it can go up to 200$ and 375$ for accommodating 4-8 and 8-16 persons respectively.
Finally, the Top10 of the high price rated neighborhoods of Seattle  is illustrated. These include Fairmount Park with an average price of 375$ followed by Industrial District and Portage Bay with approximately 240$. The other neighborhoods show quite little difference in average home price.
That was a very short analysis of Seattle based Airbnb listings. To gain better knowledge and make safer conclusions its essential to dive deeper into the data and build more sophisticated models that would show a higher evaluation metric.

Acknowledgment

I would hereby like to thank the Udacity team not only for providing the data necessary to finalize this project, but also for all the support and lessons in the past and in the future.
