# E-commerce User Behavior Analysis  
*Product Growth Analytics Project using Python (Pandas, Seaborn, Matplotlib)*

---

## Overview  
This project analyzes e-commerce user behavior using real event-level data. The focus is on uncovering user conversion patterns, retention trends, and engagement metrics across the product funnel with the ultimate goal of identifying growth opportunities.

---

## Problem Statement  
> **How do users progress through the e-commerce funnel, and what are the key behavioral and category-based factors driving conversion and retention?**

Understanding funnel performance and cohort behavior helps prioritize high-impact growth levers such as activation, re-engagement, and targeting high-converting product categories.

---

## Background  
The dataset consists of user interactions (`view`, `cart`, `purchase`) with products across categories and brands. Each row represents a single event, capturing timestamp, user ID, product info, and action type.

The aim is to simulate the role of a **Product Growth Analyst** by:
- Quantifying drop-offs across the funnel  
- Analyzing retention by cohort  
- Exploring conversion by category  
- Offering actionable growth recommendations

---

## Key Findings

### 1. **Behavioral Funnel Analysis**
- Users progress from `view` → `cart` → `purchase` 
- Out of **~1.6 million** users who viewed a product:
  - Only **398,308 (24.93%)** added to cart  
  - Only **110,518 (6.92%)** completed a purchase  
  - **~ 75%** of users dropped off before cart, and **~ 70%** of those who reached cart didn’t convert  
- Funnel breakdown:

| Stage     | Users     | Dropoff % | Conversion % | 
|-----------|-----------|-----------|---------------|
| View      | 1,597,754 | 0.0%      | 100.00%       | 
| Cart      | 398,308   | 75.0%     | 24.93%        |
| Purchase  | 110,518   | 72.0%     | 6.92%         |              

---

### 2. **Cohort Retention Analysis**
- Cohorts were based on users' **first purchase date**
- Retention tracked by daily engagement post-acquisition
- Cohort heatmap showed a **steep drop after Day 1**, with few users returning past Day 7  
- Retention averages were calculated to identify long-term engagement patterns

---

### 3. **Category-Level Conversion Analysis**
- View-to-purchase conversion calculated per category
- Several niche or utility-focused categories had surprisingly high conversion rates:

| Category                                | Purchases | Views  | Conversion Rate (%) |
|-----------------------------------------|-----------|--------|----------------------|
| apparel.glove                           | 3,819     | 9,646  | 39.59                |
| stationery.cartrige                     | 2,586     | 10,124 | 25.54                |
| furniture.bathroom.bath                 | 925       | 8,049  | 11.49                |
| appliances.environment.vacuum           | 3,192     | 33,987 | 9.39                 |
| appliances.environment.air_conditioner  | 31        | 336    | 9.23                 |
| accessories.cosmetic_bag                | 110       | 1,549  | 7.10                 |
| appliances.personal.massager            | 35        | 1,335  | 2.62                 |
| appliances.personal.hair_cutter         | 55        | 2,379  | 2.31                 |
| furniture.living_room.cabinet           | 264       | 13,378 | 1.97                 |
| accessories.bag                         | 165       | 9,486  | 1.74                 |

- Gloves and cartridges are likely high-intent or repeat-purchase categories

---

## Insights

- **Funnel Drop-Off**: 
  - Only **6.92% of users** who view products convert to purchase  
  - Cart abandonment is very high — **only 28% of cart users purchase**  
- **Low Retention**: Steep drop-off after Day 1  
- **High-Intent Niches**: Gloves and cartridges had **25–40% conversion**, indicating strong purchase intent  
- **Cohort Trends**: Slightly better retention in earlier cohorts, possibly from stronger acquisition channels

---

## Next Step Recommendations

> To drive growth, I would reccommend the following innitiatives:

1. **Improve Checkout Flow**  
   - Simplify UI and reduce cart-to-purchase friction  
   - Use abandoned cart nudges (email, push) and dynamic discounts  

2. **Increase Early Activation**  
   - Introduce onboarding nudges (e.g., product tips, first-time offers)  
   - Trigger behavioral emails for Day 1 and Day 2 engagement  

3. **Double Down on High-Intent Categories**  
   - Promote categories like gloves and printer cartridges in marketing campaigns  
   - Optimize search/landing experience for high-converting products  

4. **Run Experiments on Retention Drivers**  
   - Test loyalty incentives or membership models on low-retention cohorts  
   - A/B test personalization or pricing in underperforming categories  

---

## Tools & Libraries
- **Python** (Pandas, NumPy, Seaborn, Matplotlib)  
- **Jupyter Notebook**  
- **Exploratory Data Analysis (EDA)**  
- **Cohort & Funnel Analytics**  
- **Growth-Oriented Product Insights**

---

## Target Role Alignment
This project simulates the responsibilities of a **Product Growth Analyst**:
- Funnel tracking and optimization  
- Behavioral segmentation and retention  
- Opportunity sizing across user cohorts and categories  
- Actionable, experiment-driven product recommendations
