# FoodHub Data Analysis

This project is aimed at performing an exploratory data analysis (EDA) on the data provided by FoodHub, a food aggregator company. The data contains information about different food orders made by registered customers through their online portal. The goal of this analysis is to gain insights and answers to key questions that can help the company enhance their customer experience and improve their business.

## Context

The number of restaurants in New York is continuously increasing, and many students and busy professionals rely on online food delivery services due to their hectic lifestyles. FoodHub is a company that offers access to multiple restaurants through a single smartphone app. Customers can place direct online orders from their favorite restaurants, and FoodHub assigns a delivery person to pick up the order and deliver it to the customer.

## Objective

As a Data Scientist at FoodHub, my task is to analyze the data provided and find answers to the following key questions:

1. What are the demand patterns for different restaurants?
2. What cuisines are most popular among customers?
3. How much time does it take for restaurants to prepare food on average?
4. How much time does it take for delivery persons to deliver food on average?
5. What is the customer rating distribution and average rating for orders?

## Data Description

The data provided for analysis includes the following columns:

- order_id: Unique ID of the order
- customer_id: ID of the customer who placed the order
- restaurant_name: Name of the restaurant
- cuisine_type: Cuisine ordered by the customer
- cost: Cost of the order
- day_of_the_week: Indicates whether the order is placed on a weekday or weekend (weekday is from Monday to Friday, weekend is Saturday and Sunday)
- rating: Rating given by the customer out of 5
- food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food, calculated as the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation
- delivery_time: Time (in minutes) taken by the delivery person to deliver the food package, calculated as the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information.

## Conclusions:

The dataset consists of 1,898 orders with 9 columns describing the orders. There are no missing values, but a closer inspection of the rating column reveals that there are 736 orders with a "Not given" value, which hides the presence of a missing value. Total revenue generated across all orders is $3,424.35. The main features of interest to understand demand of different restaurants is numbder of orders. To enhance customer expirience we should pay attention to ratings.

### Number of order

The top three cuisine types are American, Japanese, and Italian and accounts for roughly 70% of total orders.American Cuisine is the most popular on weekends with 415 orders and accounting for 30% of total orders.
71% of orders are placed on the weekend. And 29% of orders are placed on weekdays.
The top 5 restaurants accounts for 33% of the orders. And Shake Shack has the most amount of placed orders at 219.
Most orders are between $5 and $15, but there are a few high cost orders that are driving up the mean.

### Ratings

All ratings are 3 or higher. This could mean that customers are having positive experiences with a rating of 3 or above, or it could suggest that customers are not reporting negative experiences when they have them.
There is no apparent good or bad ratings for a specific cuisine type.
The count of ratings appears to be directly proportional to the number of orders placed.
The medium to low-cost orders appears to be the strongest factor in determining a 5-star rating.
The correlation between the cost of an order and the rating is weak.
There appears to be no effect on the order rating based on preparation and delivery time.

## Recommendations:

Encourage customers to leave ratings: To gather more feedback, the business could consider incentivizing customers to rate their orders by offering discounts or rewards, as there are a significant number of orders with missing ratings. Providing discounts or rewards could be seen as a small cost in exchange for valuable customer feedback.
Promote popular cuisines: Promoting cuisines that have already proven to be successful can reduce the investment risk and increase the return on investment.
Prioritize weekends: Similarly, it is important to note that weekends tend to generate more sales. Therefore, it is recommended that the company ensures they have an adequate number of drivers and staff available to meet the increased demand during those periods.
Monitor the correlation between cost and rating: While there appears to be a weak correlation between the cost of an order and the rating, the business should continue to monitor this relationship to ensure that customers feel they are getting value for their money.
