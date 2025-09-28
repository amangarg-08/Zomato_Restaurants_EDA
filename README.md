# 🍴 ZOMATO RESTAURANTS IN INDIA
**(EDA + HYPOTHESIS TESTING)**

---

## 📖 Project Overview
Exploratory Data Analysis (EDA) and Hypothesis Testing on Zomato restaurants dataset to uncover customer preferences, restaurant performance, and market dynamics. The project applies data cleaning, visualization, statistical testing, and feature engineering to generate actionable business insights.

---

## 📊 Dataset
The dataset contains restaurant information from Indian cities, including ratings, cuisines, costs, establishments, and customer engagement.

- **Source**: [Zomato Restaurants in India Dataset on Kaggle](https://www.kaggle.com/datasets/rabhar/zomato-restaurants-in-india)  
- **Size**: ~115 MB  
- **Note**: Due to GitHub file size limits, the full dataset is hosted on Kaggle.  
- **Cleaned Dataset** is included in this repository for quick testing.

---

## 🎯 Objectives
1. Understand the structure of the dataset and clean missing/inconsistent values  
2. Explore univariate, bivariate, and multivariate relationships (ratings, cuisines, costs, establishments)  
3. Identify patterns and trends in restaurant popularity, pricing, and customer engagement  
4. Perform hypothesis testing to statistically validate insights  
5. Engineer new features (e.g., cost per person, popularity score, cuisine flags)  
6. Summarize business insights and provide actionable recommendations  

---

## 🗂 About The Dataset
The dataset contains restaurant data from 99 cities in India including ratings, votes, cuisine types, and other details.

**Key Variables:**  
- `res_id` : Unique id of every restaurant  
- `name` : Name of the restaurant  
- `establishment` : Type of restaurant format  
- `url` : Restaurant URL  
- `address` : Address  
- `city` / `city_id` : City name and id  
- `Locality` / `locality_verbose` : Location details  
- `latitude` / `longitude` : Geo-coordinates  
- `zipcode` : Zipcode  
- `country_id` : Country ID  
- `Cuisines` : Offered cuisines  
- `timings` : Restaurant timings  
- `Average Cost for two` : Cost for two people  
- `price_range` : Price range  
- `currency` : Currency type  
- `highlights` : Key features  
- `aggregate_rating` / `rating_text` : Average rating and text  
- `votes` : Number of ratings  
- `photo_count` : Number of uploaded photos  
- `opentable_support`  
- `delivery` / `takeaway` : -1 (No) / 1 (Yes)  

---

## 📈 EDA Workflow
1. **Data Understanding**  
   - Load the dataset  
   - Explore features, info, and statistics  
   - Summarize dataset  

2. **Data Cleaning & Preparation**  
   - Data type conversions  
   - Remove duplicates  
   - Handle missing values  
   - Outlier detection  
   - Clean categorical columns  
   - Convert cuisines into lists  

3. **Univariate Analysis**  
   - Restaurant Chains and Outlets count  
   - Top Restaurant Chains (by number of outlets)  
   - Number of restaurants (by establishment type / city / cuisine / price range / highlights)  
   - Average cost for two distribution  
   - Ratings distribution  
   - WordCloud of Top Highlights Words  
   - Top restaurant chains (by average rating)  

4. **Bivariate Analysis**  
   - Votes vs photo_count  
   - Average price for two vs aggregate_rating  
   - Votes vs aggregate_rating  

5. **Multivariate Analysis**  
   - Feature correlations  
   - Avg. aggregate_rating, votes, and photos (by establishment & city)  
   - Most expensive restaurants  

6. **Hypothesis Testing**  
   - Independent t-test: Dining vs Quick Bites ratings  
   - Z-test: Average cost comparison (Delhi vs Mumbai)  
   - Chi-Square Test: Price range vs rating  

7. **Key Insights & Observations**  
   - Summarize findings from analysis  

8. **Conclusion & Outcomes**  

---

## 💡 Key Insights & Recommendations

### 1. Restaurant Chains & Outlets
- Chains like Domino’s, KFC, Café Coffee Day dominate multiple cities.  
- ~35% of restaurants are part of a chain.  
- **Insight**: Chains have strong presence but face metro competition.  
- **Recommendation**: Analyze outlet density before expansion.  

### 2. Establishment Type
- Most restaurants are Quick Bites and Casual Dining. Fine Dining is rare.  
- Establishments with alcohol have highest ratings, votes, and photos.  
- **Insight**: Customers prefer affordable dining options.  
- **Recommendation**: Investors should focus on QSRs.  

### 3. Cost Analysis
- Metro cities have different average costs (Mumbai > Delhi).  
- Majority of restaurants are budget-friendly (Rs.250–800).  
- **Recommendation**: City-specific pricing strategy.  

### 4. Cuisine Preferences
- Chinese cuisine ranks high, more than fast food and South Indian.  
- **Recommendation**: Include 2–3 popular cuisines in menus.  

### 5. Ratings & Reviews
- Votes and ratings are positively correlated.  
- **Recommendation**: Encourage reviews & ratings for customer engagement.  

### 6. Photos & Votes
- Restaurants with more photos are more popular.  
- **Recommendation**: Improve online presence with quality images.  

### 7. City-Level Insights
- Delhi NCR, Bangalore, Mumbai dominate outlet count.  
- Gurgaon has highest rated restaurants; Hyderabad has most critics.  
- Smaller cities have fewer but highly rated restaurants.  
- **Recommendation**: Explore Tier-2 cities for growth opportunities.  

---

## 🏆 Final Business Recommendations
- **Expansion**: Focus on Tier-2 cities with fewer outlets but high ratings.  
- **Pricing**: Adjust based on city cost levels.  
- **Marketing**: Encourage votes & reviews.  
- **Digital Strategy**: Upload high-quality food & ambiance images.  
- **Menu**: Include multi-cuisine options.  

---

## 🛠 Tools & Libraries
- Python: Pandas, NumPy, Matplotlib, Seaborn, SciPy  
- Google Colab  
- Visualization: WordCloud, Heatmaps, Barplots, Scatterplots, Boxplots  
