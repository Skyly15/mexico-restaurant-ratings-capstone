# Mexico Restaurant Ratings Analysis - Capstone Project

![Dashboard Preview](mexican-restaurant-ratings-dashboard.png)

**Author:** Enoh Umukoro  
**Date:** December 15, 2025  
**Dataset Source:** Restaurant Rating Dataset (Mexico, 2012 consumer survey)

## Project Overview

This capstone project analyzes a restaurant rating dataset from Mexico (collected via a 2012 consumer survey). The dataset includes details on restaurants, cuisines, consumer demographics, preferences, and ratings.  

The objective is to derive **actionable insights** to assist business entrepreneurs and investors in making informed decisions.

The analysis was conducted using **Tableau Public (web authoring)** and directly addresses the four required business questions.

## Data Sources

The dataset comprises five CSV files:

- `restaurants.csv` — Restaurant details (name, city, price, parking, alcohol service, etc.)
- `restaurant_cuisines.csv` — Cuisines offered by each restaurant (one-to-many)
- `ratings.csv` — Consumer ratings (Overall, Food, Service on a 0–2 scale)
- `consumers.csv` — Consumer profile (age, occupation, drink level, etc.)
- `consumer_preferences.csv` — Preferred cuisines per consumer (one-to-many)

Tables were linked in Tableau via **relationships** on `Restaurant_ID` and `Consumer_ID`.

## Dashboard Overview

The interactive dashboard is organized by the four questions, with dedicated visualizations and written insights for each.

### Question 1: What can you learn from the highest rated restaurants? Do consumer preferences have an effect on ratings?

**Visualizations:**
- **Highest Rated Cuisines** — Horizontal bar chart of average overall rating by cuisine
- **Top 10 Highest Rated Restaurants** — Bar chart colored by price level

**Key Insights:**
- Specialty/non-Mexican cuisines dominate the top ratings: **Mediterranean**, **Coffee Shop**, **Family**, **International**, **Japanese**, **Seafood**.
- The top 10 restaurants are predominantly **Medium** or **High** priced.
- **Mexican cuisine** is by far the most preferred by consumers but achieves lower average ratings than rarer/specialty cuisines.
- **Conclusion:** While consumer preferences strongly favor Mexican food, higher ratings are awarded to unique or premium offerings, indicating that quality, ambience, and exclusivity drive top scores.

### Question 2: What are the consumer demographics? Does this indicate a bias in the data sample?

**Visualizations:**
- **Age Distribution** — Custom age groups (18–23, 24–29, etc.)
- **Occupation**
- **Drink Level**

**Key Insights:**
- **Strong sample bias**: Over 80% of reviewers are **students** aged **18–23**.
- Drink levels are primarily **Abstemious**, **Casual Drinker**, or **Social Drinker** — very few heavy drinkers.
- The sample is overwhelmingly young, university-educated, and likely budget-conscious.
- **Yes — significant bias exists**. Ratings likely reflect the tastes of young urban students rather than the broader population, potentially favoring affordable and casual venues.

### Question 3: Are there any demand & supply gaps that you can exploit in the market?

**Visualizations:**
- **Restaurant Supply by Cuisine** — Count of restaurants per cuisine
- **Consumer Demand by Cuisine** — Count of consumer preferences per cuisine

**Key Insights:**
- **Mexican** has high supply (~28 restaurants) and very high demand (~97 preferences) → **saturated market**.
- Notable gaps where **demand significantly exceeds supply**:
  - American
  - Pizzeria
  - Japanese
  - Burgers
  - Italian
  - Coffee Shop / Cafeteria
- These cuisines represent **strong opportunities** for new restaurant ventures.

### Question 4: If you were to invest in a restaurant, which characteristics would you be looking for?

**Visualizations:**
- **Rating by Price**
- **Rating by Parking**
- **Rating by Alcohol Service**

**Key Insights & Recommendations:**
- **Price**: Medium and High priced restaurants receive higher average ratings than Low.
- **Parking**: Valet parking correlates with the highest ratings, followed by dedicated parking ("Yes").
- **Alcohol Service**: Full Bar and Wine & Beer options outperform venues with no alcohol.
- **Investment Recommendations**:
  - Target **Medium to High price** positioning
  - Secure locations with **parking** (ideally Valet)
  - Offer **alcohol service** (Wine & Beer or Full Bar)
  - Prioritize **high-rated cuisines** with demand gaps: Japanese, International, Mediterranean, Seafood, American, Italian, Pizzeria

## Conclusion

The analysis highlights:
- A clear **young student bias** in the rating data
- **Mexican dominance** in both preference and supply, but lower performance in ratings
- **Lucrative gaps** in international and specialty cuisines
- **Premium amenities** (price, parking, alcohol) as key drivers of high ratings

**Investors should focus on underserved cuisines with premium features to capture both demand and high ratings.**

## View the Interactive Dashboard

[Tableau Public Dashboard Link](https://public.tableau.com/views/MexicoRestaurantRatingsCapstoneDashboard/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) 


## Acknowledgments

- Dataset: Restaurant Rating Dataset (Mexico 2012 survey)
- Tool: Tableau Public (web authoring)
- Guidance: DigitaleyDive Bootcamp
