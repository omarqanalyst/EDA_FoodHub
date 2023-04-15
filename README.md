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
