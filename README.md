# FoodHub Data Analysis

🔗 **[View charts and code here](https://github.com/omarqanalyst/EDA_FoodHub/blob/master/FDS_Project_LearnerNotebook_FullCode.ipynb)**

This project explores FoodHub's order data to uncover customer behavior and business insights. FoodHub is a food aggregator that lets customers order from multiple restaurants through one app. The dataset includes nearly 1,900 orders placed via their platform.

## Objective

- As a data scientist at FoodHub, the goal is to answer key business questions:

- Which restaurants and cuisines are in high demand?
- How long does food preparation and delivery take?
- What’s the distribution of customer ratings?
- What factors affect 5-star reviews?

## Insights

### Order Trends
- **Total orders**: 1,898
![image](https://github.com/user-attachments/assets/5635ddea-a3b9-4fc6-8261-add6b08760bc)

 
- **Top cuisines**:
![image](https://github.com/user-attachments/assets/cd5f4ea1-bbc0-4277-8ef1-79df0763adf7)
  (Update 04.08.25: A tree chart would be a better chart)
  - American (most popular on weekends)  
  - Japanese  
  - Italian  
  Together, these three account for ~70% of all orders.
- **Order timing**:
![image](https://github.com/user-attachments/assets/5f256800-764c-425c-b01e-bc331642ded9)

  - 71% of orders happen on weekends  
  - 29% on weekdays
- **Top restaurants**:
![image](https://github.com/user-attachments/assets/e3fb764d-7f47-4c38-aebf-7b1a2ee4a22f)
  - The top 5 restaurants account for 33% of orders  
  - **Shake Shack** leads with 219 orders
- **Order value**:
![image](https://github.com/user-attachments/assets/5845cd95-e24f-4526-9af9-a048c9e0a4f9)
 
  - Most are between $5 and $15  
  - A few high-ticket orders raise the average

### Ratings
- All ratings are 3 or higher
- 736 orders are missing ratings (“Not given”)
- No strong pattern between cuisine and rating

<img width="650" alt="image" src="https://github.com/user-attachments/assets/c2ecbaa7-8df3-4afb-a897-2e9b36c1ad69" />

- Higher ratings are loosely linked to lower-cost orders
- Preparation and delivery time don’t seem to impact ratings

## Recommendations

- **Encourage reviews**: Offer small rewards or discounts to boost customer feedback.
- **Double down on what works**: Promote top cuisines—especially American—on weekends.
- **Staff for the surge**: Ensure more drivers and staff are available on weekends.
- **Track cost vs. satisfaction**: Keep an eye on how perceived value impacts ratings.

## Dataset Overview

The dataset contains the following columns:

- `order_id`: Unique ID of the order  
- `customer_id`: ID of the customer  
- `restaurant_name`: Name of the restaurant  
- `cuisine_type`: Cuisine ordered  
- `cost`: Cost of the order  
- `day_of_the_week`: Weekend or weekday  
- `rating`: Customer rating (1–5 or "Not given")  
- `food_preparation_time`: Time (min) to prepare food  
- `delivery_time`: Time (min) to deliver the order
