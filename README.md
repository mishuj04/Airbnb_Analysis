# 🏠 Airbnb Analysis with Power BI

This project analyzes **Airbnb listings dataset** using Power BI.  
The goal is to uncover insights about pricing, availability, host activity, and neighborhood trends.

---

## 📂 Dataset Overview
The dataset contains the following columns:

- `id`  
- `name`  
- `host_id`  
- `host_name`  
- `neighbourhood_group`  
- `neighbourhood`  
- `latitude`  
- `longitude`  
- `room_type`  
- `price`  
- `minimum_nights`  
- `number_of_reviews`  
- `reviews_per_month`  
- `calculated_host_listings_count`  
- `availability_365`  
- `last_review_year` *(derived)*  
- `last_review_month` *(derived)*  

---

## 🧹 Data Cleaning & Preprocessing
- Removed rows where **`name`** and **`host_name`** were missing.  
- Extracted **month** and **year** from `last_review` → created `last_review_month` and `last_review_year`.  
- Dropped the `last_review` column (10%+ missing values).  
- Replaced missing values in `last_review_month` and `last_review_year` with **mean values**.  

---

## 📝 New Calculations
- **`Total Payment`** column created
- **Power BI Measures created:**
- Average Availability  
- Average Nights  
- Average Price  
- Average Reviews per Month  
- Total Records  

---

## 📊 Dashboard Insights
Key metrics from the Power BI dashboard:

- **Total Records:** 25K  
- **Average Nights:** 8.48  
- **Average Availability:** 111.85 days  
- **Average Price:** $211.90  
- **Average Reviews per Month:** 22.80  

### 🔹 Host-Level Insights
- **Highest Avg Price Host:** Olson (~$10K)  
- **Most Listings:** Sonder (NYC) with 104K+ listings, followed by Blueground (54K).  

### 🔹 Neighborhood Insights
- **Longest Avg Stay:** Spuyten Duyvil (~50+ nights).  
- Other long-stay neighborhoods: Claremont Village, Port Richmond.  

### 🔹 Geographic Distribution
- Listings are heavily concentrated in **New York City & nearby regions**.  

---

## 💡 Business Implications
- Market dominated by large operators like **Sonder** and **Blueground**.  
- **Spuyten Duyvil** attracts long-term stays → potential for extended rental strategies.  
- **Olson’s high prices** indicate premium/luxury rental opportunities.  

---

## ✅ Recommendations
- Help individual hosts compete with large operators by focusing on **unique experiences**.  
- Promote **longer bookings** in short-stay neighborhoods using discounts.  
- Track **Total Payment** metric to find the most profitable areas and room types.  

---

## ⚙️ Tools & Technologies
- **Power BI** – Dashboard & Visualization  
- **Python** – Data Cleaning  

