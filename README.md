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
- Created New features :
          - Value_Score :  calculates the value score by dividing the aggregate rating by the average cost for two.
          - IsOverpriced flag : flags a restaurant as overpriced if the aggregate rating is less than 3.5 and the average cost for two is more than 1000
          - Cost Category (Low, Medium, High) : categorizes the average cost for two into Low, Medium, or High based on the following thresholds: Low: Less than 500, Medium: 500 to 999, High: 1000 or more
          - Booking + Delivery : formula combines the information on table booking and online delivery to analyze the service. It returns one of the following values:
                        - Both: If both table booking and online delivery are available
                        - Booking: If only table booking is available
                        - Delivery: If only online delivery is available
                        - Not Both: If neither table booking nor online delivery is available

# 8. Visuals (Power BI):
- Table(Overpriced Restaurants) to show worst-rated expensive restaurants (my “Avoid List”)
- Bar Chart(Best Value by Cuisine) to show which cuisines consistently give you value for money?
- Pie Chart(Impact of Booking & Delivery) to show whether or not customers rate delivery-friendly restaurants better?
- Map(City-Wise Insights) to see which cities offer the best dining value.
- Table(Top Ten Restaurants) to see my go to list of restaurants. Low value score, High aggregate rating of greater than 4.2 and votes greater than 1000.
- Filters: Cuisine, Online Order, Booking Option, Cost Range

# 9.  Findings :
Some high-cost restaurants were rated below 3.5, Jakarta City topping the charts with a whooping 100000, indicating style over substance. Then the other cities that followed were New Delhi.
Chinese, Mughlai, and North Indian cuisine consistently scored high on value in the high and medium cost category, in the low cost category North Indian, Fast Food and Chinese scored high.
None of the restaurants offer both table booking and delivery. There seems to be more restaurants that have no table booking(8.36k) and no online delivery(7.07K). Restaurants with online ordering tend to have better ratings but they also appear to have the highest worst ratings.
I developed an interactive map that allows users to select a city, cuisine type, budget category(low, medium, high). The map also provides options to filter restaurants based on table booking, and online delivery availabilty, catering to bothdine-in and takeaway preferences. Upon selection, the map displays a list of recommended restaurants in the chosen city, along with their addressesand ratings. This feature provides users with a comprehensiveoverview of dining options, allowing them to make informed decisions about where they want to eat.
A list of Top 10 underrated gems was created to guide future choices. It revealed 3 which are 
        Restaurant Name	Aggregate rating	Sum of Average Cost for two	Sum of Votes	Value Score
        Bukhara - ITC Maurya	4.4	6500	2826	0.0006769231
        Talaga Sampireun	4.9	600000	5514	0.0000245000
        Toodz House	4.6	165000	1476	0.0000278788
        
# 10. Conclusion:
This project helped us turn a bad dinner into a smart data story. Next time we go out, we’ll choose food that’s actually worth the hype. Data doesn’t lie, ambiance might.

# 10. Future steps :
- Scrape aesthetic tags or photo metadata to build a visual-style predictor
- Apply sentiment analysis to reviews

# 11. Challenges experienced:
The currencies were different. So I might have a higher amount but it could be low in value.




