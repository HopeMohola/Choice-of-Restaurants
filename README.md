# 1. Project Title: The Restaurant Trap
        When Aesthetics Fool The Appetite

# 2. Inspiration:
It was my friend’s birthday. We had planned every detail—outfits, budget, the vibe. We found a fancy-looking restaurant online that matched our aesthetics perfectly. But the food? Bland. Cold. Disappointing. That night, we realized: Looks can deceive. This project is my way of making sure we don’t fall for that again and neither should you.

# 3. Objective: 
To help diners make *smarter*, *data-informed decisions* when choosing restaurants by analyzing the relationship between:
- Restaurant ratings
- Cost for two
- Cuisine
- Service options (table booking, online delivery)
- Location
Using the Zomato Restaurants Dataset, this project aims to uncover whether #*price and appearance correlate with food quality*#, and how to identify #*underrated gems*# or #*overpriced traps*#.

# 4. Tools Used:
- Microsoft Excel : data cleaning and transformation
- Power BI - For data visualization and interactive dashboards

# 5. Investigative Questions:
1. Do higher-priced restaurants always receive better ratings?
2. Which cuisines offer the best value based on price and quality?
3. Are there cities where overpriced restaurants are more common?
4. What is the impact of online ordering or table booking options on customer satisfaction?
5. Which restaurants are hidden gems (low cost, high rating)?
6. Which are overrated traps (high cost, low rating)?

# 6. Data Source:
- Data Source :
- Features used : Restaurant Name, Location, Cuisines, Average Rating, Cost for Two, Online Order, Book Table, Votes

# 7. Data Preparation (Excel):
- Removed duplicates and empty cells
- Normalised cost_for_two values
        - Convert Average Cost for two to numeric (remove commas if any using Find & Replace)
        - Ensure Aggregate rating is numeric (not text)
- Created New features : Value_Score = Rating / Cost, IsOverpriced flag, Cost Category (Low, Medium, High)

# 8. Visuals (Power BI):
- Bar chart: Average Rating by Cost Category
- Heatmap: Cuisine vs. Rating
- Map: Top/Bottom-rated restaurants by city
- Ranking Table: Top 10 Best Value Restaurants
- Filters: Cuisine, Online Order, Booking Option, Cost Range

# 9.  Findings :
Some high-cost restaurants were rated below 3.5, indicating style over substance.
Indian, Mughlai, and North Indian cuisine consistently scored high on value.
Restaurants with online ordering tend to have better ratings.
A list of Top 10 underrated gems was created to guide future choices.

# 10. Conclusion:
This project helped us turn a bad dinner into a smart data story. Next time we go out, we’ll choose food that’s actually worth the hype. Data doesn’t lie, ambiance might.

# 10. Future steps :
- Scrape aesthetic tags or photo metadata to build a visual-style predictor
- Apply sentiment analysis to reviews
- Build a mobile dashboard to rank restaurants nearby by value-for-money




