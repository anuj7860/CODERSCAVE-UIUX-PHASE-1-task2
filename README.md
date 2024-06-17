# CODERSCAVE-UIUX-PHASE-1-task2 (GOLDEN TASK)
Creating a Zomato sales dashboard involves multiple steps, including data preparation, data analysis, and visualization. Here's a step-by-step approach to creating a report based on the given dataset and tables:

# Step 1: Data Preparation

#1.1 Understanding the Tables
- **Food Table**: Contains information about food items.
  - `food_id`: Unique identifier for each food item.
  - `item_id`: Identifier for the item category.
  - `veg_or_non_veg`: Indicates whether the food item is vegetarian or non-vegetarian.
 
  - ![image](https://github.com/anuj7860/CODERSCAVE-UIUX-PHASE-1-task2/assets/138881508/4898ee99-12b8-4b15-a418-35efe848ed5d)


- **Menu Table**: Contains information about the menu items offered by different restaurants.
  - `menu_id`: Unique identifier for each menu item.
  - `r_id`: Identifier for the restaurant.
  - `f_id`: Foreign key referring to `food_id` in the Food Table.
  - `price`: Price of the menu item.
  - `cuisine`: Type of cuisine (e.g., Italian, Chinese).
  - `veg_or_non_veg`: Indicates whether the menu item is vegetarian or non-vegetarian.
 
  - ![Screenshot 2024-06-17 191810](https://github.com/anuj7860/CODERSCAVE-UIUX-PHASE-1-task2/assets/138881508/8a3ed2a6-279c-45e0-8ecb-0db80f866341)


- **Order Table**: Contains information about customer orders.
  - `order_id`: Unique identifier for each order.
  - `price`: Total price of the order.
  - `currency`: Currency used for the transaction.
  - `city`: City where the order was placed.
  - `type`: Type of order (e.g., delivery, dine-in).
  - `year`: Year when the order was placed.
 
  - ![Screenshot 2024-06-17 191818](https://github.com/anuj7860/CODERSCAVE-UIUX-PHASE-1-task2/assets/138881508/9bd4841a-760c-43be-9318-d2232edde60e)


- **Rating Table**: Contains ratings for food items.
  - `food_id`: Foreign key referring to `food_id` in the Food Table.
  - `rating`: Rating of the food item.
 
  - ![Screenshot 2024-06-17 191826](https://github.com/anuj7860/CODERSCAVE-UIUX-PHASE-1-task2/assets/138881508/8e3f407f-5ef9-4fe2-a0e4-5a70ccd5f837)


#### 1.2 Data Cleaning and Transformation
- **Normalization**: Ensure consistent formatting of data, such as currency and price.
- **Handling Missing Values**: Address any missing values in the dataset by either filling them or removing the corresponding rows.
- **Data Integration**: Merge tables to create a unified dataset for analysis.
  - Join `Menu Table` with `Food Table` on `food_id` to include food details in the menu.
  - Join `Order Table` with the integrated Menu and Food tables on `f_id` and `menu_id` to incorporate order details.

# Step 2: Data Analysis

# 2.1 Key Metrics to Analyze
- **Total Sales**: Calculate the total sales amount.
- **Average Order Value**: Calculate the average value of an order.
- **Top Cities by Sales**: Identify cities with the highest sales.
- **Cuisine Popularity**: Determine the most popular cuisines.
- **Veg vs. Non-Veg Sales**: Compare sales of vegetarian and non-vegetarian items.
- **Yearly Sales Trends**: Analyze sales trends over different years.
- **Food Ratings**: Analyze average ratings for food items.

# Step 3: Visualization

# 3.1 Tools for Visualization
- Use tools like Tableau, Power BI, or Excel for creating visualizations.

# 3.2 Creating Dashboards
- **Total Sales Dashboard**:
  - Bar chart showing total sales by city.
  - Line chart showing yearly sales trends.
  
- **Cuisine Dashboard**:
  - Pie chart showing the distribution of sales by cuisine type.
  - Bar chart comparing average ratings for different cuisines.

- **Veg vs. Non-Veg Dashboard**:
  - Bar chart showing total sales for vegetarian and non-vegetarian items.
  - Pie chart showing the proportion of veg and non-veg items sold.

- **Order Analysis Dashboard**:
  - Heat map showing sales by city and year.
  - Scatter plot showing order value distribution.

# 3.3 Interactive Elements
- Add filters for year, city, cuisine, and veg/non-veg categories to allow dynamic exploration of the data.

#Step 4: Reporting

# 4.1 Summary of Findings
- **Sales Overview**: Total sales amount and average order value.
- **Top Cities**: Cities with the highest sales.
- **Popular Cuisines**: Most popular cuisines based on sales.
- **Veg vs. Non-Veg**: Comparison of sales and popularity.
- **Trends**: Key trends over the years.

# 4.2 Insights and Recommendations
- **Marketing Focus**: Target marketing efforts on top-performing cities and popular cuisines.
- **Menu Optimization**: Promote high-rated food items and consider introducing more popular cuisines.
- **Strategic Decisions**: Use sales trends to plan for future growth and expansion.

#4.3 Visualization Integration
- Embed visualizations into the report to support findings with clear and interactive charts and graphs.

# Managing Relationships in between Tbles

![Screenshot 2024-06-17 191933](https://github.com/anuj7860/CODERSCAVE-UIUX-PHASE-1-task2/assets/138881508/f8eaa5fc-9241-4010-86da-a6729b6d0b49)

# working of the Dashboard
https://drive.google.com/file/d/18VVkxMJF8Pkb44HbXCeIgpCdoCbjH8qd/view?usp=sharing
