![Screenshot of Cover Page](https://i.imgur.com/tFUdauh.png)

# Project-1-Python-Foundations

**Contents/Agenda**

* Executive Summary

* Business Problem Overview and Solution Approach

* Data Overview

* EDA - Univariate Analysis

* EDA - Multivariate Analysis

* Appendix

**Executive Summary**

Conclusions from Analysis

* The restaurants fulfilling criteria to get promotional offer are Shake Shack, The Meatball Shop, Blue Ribbon Sushi and Blue Ribbon Fried Chicken. Together with Parm, they are also among top 5 restaurants by orders received and revenue generated.

* There are 1898 orders but only 1200 customer ID, indicating that there are repeated orders by same customer(s), which is confirmed by further checking with the value counts of each customer ID. Therefore, the app can be deemed useful by customer(s). 

* The ID of top 3 most frequent customers to receive 20% discount vouchers given by the company, are 52832, 47440 & 83287, with 13, 10 & 9 as their respective number of orders placed. 

* Net Revenue Generated by the Company Across All Orders is around 6166.3 dollars.

* The revenue generated by the restaurants ranges from 506.47 to 3579.53 dollars. Shake Shack is leading well ahead. It’s revenue generated is more than 2/3 of the restaurant in 2nd position.

* There is slower delivery time on weekdays, as compared to weekends, with a difference of mean by 6mins, despite lesser orders on weekdays.

* Percentage of orders that take more than 60 Minutes to get delivered from time order is placed is 10.54%. The maximum time exceeded is by 8 mins.

* The demand in orders is much higher on weekends, as compared to weekdays. 

* American is the most popular cuisine on weekends. Japanese, Italian and Chinese cuisine show a lot of potential. On the contrary, Korean, Thai, Southern, French, Spanish and Vietnamese are very low in demand. 

* Rating is important as it is positively correlated to cost of the order, which has direct effect on revenue generated by the company. 

* ‘Not given’ accounts for 736 out of 1898 values (around 38.78%) for rating column. It is quite a substantial amount. The inability to include these data together with numerical rating in analysis, can have a significant effect on the conclusions that can be drawn from the dataset. There are also no categories for low rating such as 1 or 2.

* There is much larger number of rating for 5 and also 4, as compared to 3, indicating favourable customer experience.

**Recommendations to Help Improve Business(Cuisine Type and Feedback Ratings)**

* Efficient food preparation and smooth delivery need to be ensured especially for American cuisine on weekend, and also orders for restaurants, Shake Shack, The Meatball Shop, Blue Ribbon Sushi, Blue Ribbon Fried Chicken and Parm.

* Reduce delivery time for weekday to match up with weekend, to boost weekday orders. Reasons for the slower delivery time need to be further investigated, to pinpoint areas for improvement and bridge any gaps.

* Need to procure and analyse more data on rating listed as ‘Not given’ to better understand and manage customer experience, to boost future rating and revenue. Especially when there are no categories for low rating such as 1 or 2, it would be beneficial to analyse the nature of the notes written, whether they are positive eg compliments, negatives eg complaints or just general feedback.

* Explore ways to boost number of numerical ratings, such as inclusion of reward system for numerical rating given eg offering virtual coins, cashback rebate, discount e vouchers, redemption of complimentary side dish/beverage, chance to enter lucky draw, for more precise and realistic picture to be drawn.

* Widen coverage of rewards for frequent customers to further encourage repeat purchases,  eg by inclusion of loyalty rewards like Cashback rebate.

* Promotion of the app to reach wider audience, to increase orders and revenue generated.

* Look into the reasons for frequent customers’ repeated purchase to better understand the strength of the app.

* There can be further analysis of whether the higher cost of the order is due to price of food, or greater quantity ordered.

**Business Problem Overview and Solution Approach**

Context

* The number of restaurants in New York is increasing day by day.
  
* Lots of students and busy professionals rely on those restaurants due to their hectic lifestyles.
  
* Online food delivery service is a great option for them.
  
* It provides them with good food from their favorite restaurants. 

Business

![image](https://i.imgur.com/rJi3v7b.png)

* Offers access to multiple restaurants through a single smartphone app

* Earns money by collecting a fixed margin of the delivery order from the restaurants

![image](https://i.imgur.com/INiD3NS.png)

**Objective**

* Get fair idea about demand of different restaurants which will help in enhancing customer experience. 

* Find answers to key questions shared by Data Science team to help company improve business.

**Solution Approach**

* Gain Data Overview 

* Perform Exploratory Data Analysis, which encompasses Univariate Analysis & Multivariate Analysis, on the data stored by FoodHub, of different orders made by registered customers in their online portal.

* Extract relevant Conclusion, Actionable Insights and Recommendations, majorly focusing on cuisine type, feedback ratings and delivery time.

**Data Information**

The data contains the different data related to a food order. The detailed data dictionary is given below.

* order_id                        : Unique ID of the order

* customer_id                 : ID of the customer who ordered the food

* restaurant_name         : Name of the restaurant

* cuisine_type                 : Cuisine ordered by the customer

* cost_of_the_order        : Cost of the order

* day_of_the_week         : Indicates whether the order is placed on a weekday or weekend 
         (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)

* rating                            : Rating given by the customer out of 5

* food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.

* delivery_time                : Time (in minutes) taken by the delivery person to deliver the food package. This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information.

Note: Values in rating column listed as ‘Not Given’, said to be due to users choosing not to rate the restaurants.

**Data Overview**

* There are 1898 rows and 9 columns.

* The restaurant_name, cuisine_type, day_of_the_week and rating columns are of object type, while the rest of the columns are numerical in nature. The object type columns contain categories in them.

* There are no missing values. All the columns have 1898 observations and there are no null values for each column.

* Once an order is placed, time taken to prepare food:

  Minimum - 20mins,   Average - 27.37mins,   Maximum - 35mins

* 736 orders are not rated, as their ratings are ‘Not given’.

**EDA - Univariate Analysis**

Explore all the variables and provide observations on their distributions.

* Order ID

There are 1898 order ID.

* Customer ID

There are 1200 customer ID. The ID of top 3 most frequent customers are 52832, 47440 & 83287 and their respective number of orders placed are 13, 10 & 9. They will receive the 20% discount vouchers given by the company.

* Restaurant Name

There are 178 restaurant names. The top 5 restaurants in terms of number of orders received are Shake Shack, The Meatball Shop, Blue Ribbon Sushi, Blue Ribbon Fried Chicken and Parm.

![image](https://i.imgur.com/lwX6oo9.png)

![image](https://i.imgur.com/E1YwcAI.png)

![image](https://i.imgur.com/ghhuHG5.png)

![image](https://i.imgur.com/8jO1ytB.png)

![image](https://i.imgur.com/Fbb9acQ.png)

Revenue Generated by Restaurants

* The revenue generated by the restaurants ranges from 506.47 to 3579.53 dollars.

* The top 5 restaurants based on revenue generated coincided with the top 5 restaurants based on orders received.

* Shake Shack is leading well ahead. It’s revenue generated is more than 2/3 of the restaurant in 2nd position. 

Restaurants Fulfilling Criteria to Get Promotional Offer in Advertisement

* The condition to get the offer is that restaurants must have rating count >50 and average rating >4.

* The restaurants fulfilling the criteria to get the promotional offer are Shake Shack, The Meatball Shop, Blue Ribbon Sushi and Blue Ribbon Fried Chicken, as seen in the first 4 rows of the above table. 

Net Revenue Generated by the Company Across All Orders

* The company charges restaurant 25% on orders having cost greater than 20 dollars and 15% on the orders having cost greater than 5 dollars.

* The net revenue is around 6166.3 dollars.

![image](https://i.imgur.com/S4ub6qX.png)













