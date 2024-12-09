# Accommodation Insights Dashboard

A comprehensive analysis of accommodation trends, indices, and patterns, developed using **Grafana** with data stored in **InfluxDB**. This project provides actionable insights into room types, cleanliness, business-friendly accommodations, and city-specific trends.

---

## Overview

This project showcases an intelligent dashboard built to analyze accommodation data from major cities like Amsterdam and Athens. The dashboard focuses on key metrics, such as attraction and restaurant indices, cleanliness ratings, and business-friendly features, to deliver data-driven insights for decision-making.

---

## Key Features

1. **Room Type Analysis**
   - Compare average restaurant and attraction indices across room types.
   - Identify trends between weekdays and weekends.

2. **Business-Friendly Accommodations**
   - Analyze city-wise distribution and factors influencing business listings.

3. **Cleanliness Ratings**
   - Understand room-type cleanliness ratings and propose improvements.

4. **Temporal Patterns**
   - Explore how indices such as the restaurant index fluctuate over time.

5. **General Trends**
   - Derive correlations between key metrics like cleanliness and customer satisfaction.

---
### *General Questions Answered*
---

### *For Room Type and Indices*

1. *What is the average restaurant index for each room type?*
   - *Entire Home*: 305  
   - *Private Room*: 313  
   - *Shared Room*: 97.1  

2. *How do room types compare in terms of the average attraction index for different days?*
   - The gauge indicators suggest that:
     - *Weekday (Entire Home)*: 204  
     - *Weekday (Private Room)*: 258  
     - *Weekend (Entire Home)*: 534  
     - *Weekend (Private Room)*: 255  
     - Shared rooms are not visible in the attraction indices.  
   - *Insight*: Weekend attraction index is higher for Entire Home, suggesting more activity and demand.

3. *Why might the shared room have a significantly lower restaurant index compared to private and entire home room types?*
   - Possible reasons:
     - Shared rooms might attract budget travelers who prefer self-catering or cheaper food options.
     - Shared accommodations might be located farther from popular restaurants compared to private or entire homes.

---

### *For Business-Friendly Accommodations*

4. *Why are business-friendly accommodations more prevalent in Amsterdam compared to Athens?*
   - Amsterdam has 219 listings compared to 24 in Athens.  
   - Possible factors:
     - Amsterdam may have a higher demand for business accommodations due to its status as a business hub.
     - Availability of co-working spaces and business amenities might be higher in Amsterdam.

5. *What factors could influence the number of business-friendly accommodations in these cities?*
   - Local business demand, presence of corporate hubs, and conference events.
   - Accessibility of transport and communication infrastructure.
   - City regulations and policies for short-term rentals.

---

### *For Cleanliness Rating*

6. *What are the average cleanliness ratings for different room types?*
   - Based on the bar chart:
     - Entire Home: ~8.2  
     - Private Room: ~8  
     - Shared Room: ~7.8  

7. *How do the average cleanliness ratings vary between Amsterdam and Athens?*
   - Based on the pie chart:
     - Amsterdam and Athens appear to have similar cleanliness ratings, with a 50-50 distribution.
   - *Insight*: Both cities maintain an equivalent level of cleanliness.

8. *What actions could be taken to improve cleanliness ratings for room types with lower scores?*
   - Shared rooms have the lowest cleanliness ratings. Suggestions:
     - Increase cleaning frequency.
     - Provide better cleaning supplies for guests.
     - Introduce stricter quality checks.

---

### *For Trends and Patterns*

9. *What trends can be observed in the restaurant index for different cities over time (e.g., 13:00 to 18:00)?*
   - Amsterdam shows a gradual decline in restaurant index from ~350 at 13:00 to ~300 at 18:00.  
   - Athens starts low and dips further, indicating lesser restaurant activity overall.  
   - *Insight*: Amsterdam has consistently higher restaurant activity compared to Athens, with a steady decline during the afternoon.

10. *How might the time of day impact the restaurant index in Amsterdam and Athens?*
    - Afternoon (13:00–18:00) may reflect a drop in demand as fewer people dine out during these hours.  
    - Athens might have a cultural preference for dining later in the evening, contributing to lower activity earlier.

---

### *General Analysis Questions*

11. *What insights can be drawn from the disparity in attraction indices between weekdays and weekends?*
    - The attraction index is significantly higher on weekends (534 for Entire Home vs. 204 on weekdays).  
    - *Insight*: Tourists and locals likely engage more with attractions during weekends, increasing demand for certain accommodations.

12. *Are there any correlations between restaurant index and cleanliness ratings across room types?*
    - *Observation*: Entire Homes have the highest restaurant index (305) and cleanliness rating (~8.2).  
    - *Insight*: Better-maintained properties may attract more dining activity.

13. *How might these metrics influence customer satisfaction or revenue generation?*
    - Higher cleanliness and attraction indices likely drive customer satisfaction and repeat bookings.  
    - Business-friendly accommodations in Amsterdam could generate more revenue due to higher demand.

---

## Dashboard Visuals and Insights

### 1. Room Type and Indices
- **Average Restaurant Index for Room Types**:
  - *Entire Home*: **305**
  - *Private Room*: **313**
  - *Shared Room*: **97.1**
- **Key Insight**: Shared rooms have significantly lower restaurant indices due to budget-conscious travelers and location factors.

- **Average Attraction Index Comparison**:
  - Weekdays (*Entire Home*): **204**, Weekends: **534**
  - Private Rooms: Lower indices than entire homes on weekends.

---

### 2. Business-Friendly Accommodations
- **City-Wise Listings**:
  - Amsterdam: **219**
  - Athens: **24**
- **Factors Influencing Business Listings**:
  - Amsterdam’s robust business ecosystem.
  - Superior transport and coworking infrastructure.

---

### 3. Cleanliness Ratings
- **Average Ratings**:
  - Entire Home: **8.2**
  - Private Room: **8.0**
  - Shared Room: **7.8**
- **Suggestions**: Improve shared room cleanliness with stricter quality controls and enhanced cleaning procedures.

---

### 4. Temporal Trends
- **Restaurant Index Trends (13:00–18:00)**:
  - Amsterdam shows a gradual decline.
  - Athens remains consistently low, reflecting cultural dining patterns.

---

### 5. General Observations
- Weekends significantly boost attraction indices, with **534** for entire homes.
- Higher cleanliness correlates with higher restaurant activity and customer satisfaction.

---
### Recommendations and Insights
----

### *1. Weekend Demand Drives Higher Attraction Index for Entire Homes*
- The attraction index for *Entire Homes* is significantly higher on weekends (534) compared to weekdays (204).  
  *Insight*: Weekend bookings for Entire Homes are driven by higher tourist activity.  
  *Action*: Focus marketing efforts for Entire Homes on weekends, emphasizing proximity to attractions.

---

### *2. Shared Rooms Struggle with Cleanliness and Restaurant Index*
- Shared rooms have the *lowest cleanliness rating (~7.8)* and a significantly lower restaurant index (97.1 compared to 305 for Entire Homes).  
  *Insight*: Shared accommodations may fail to meet guest expectations for cleanliness and convenience.  
  *Action*: Improve cleaning standards and ensure better food options nearby to attract more customers.

---

### *3. Amsterdam Leads in Business-Friendly Accommodations*
- Amsterdam has 219 business-friendly listings, far surpassing Athens with only 24.  
  *Insight*: Amsterdam's infrastructure and status as a business hub attract more corporate travelers.  
  *Action*: Promote Athens accommodations by highlighting any existing business-friendly features and collaborating with local businesses.

---

### *4. Entire Homes Dominate in Cleanliness Ratings*
- Entire Homes have the *highest cleanliness rating (~8.2)* compared to Private Rooms (~8) and Shared Rooms (~7.8).  
  *Insight*: Entire Homes likely offer better-maintained environments, appealing to more discerning travelers.  
  *Action*: Use cleanliness ratings as a selling point in marketing campaigns for Entire Homes.

---

### *5. Afternoon Restaurant Index Declines Gradually in Amsterdam*
- The restaurant index in Amsterdam declines steadily from *350 at 13:00 to ~300 by 18:00*, while Athens shows consistently low activity.  
  *Insight*: Afternoon hours show reduced dining activity, potentially due to cultural habits or guest preferences.  
  *Action*: Partner with restaurants to offer afternoon discounts or promotions, especially in Amsterdam.

---

### *6. Weekend Attraction Demand Can Influence Pricing*
- The stark difference in attraction indices for weekends versus weekdays (534 vs. 204 for Entire Homes) highlights *weekend tourism demand*.  
  *Insight*: Tourists are more active on weekends, creating an opportunity for dynamic pricing.  
  *Action*: Implement higher weekend pricing for properties near popular attractions.

---
