# Data Analysis Project: Cooking Sessions and User Orders

## Project Overview
This project analyzes data from three datasets to uncover insights into cooking sessions, user behavior, and order trends. The datasets used are:

1. **UserDetails.csv**: Information about users, including demographics and registration details.
2. **CookingSessions.csv**: Records of cooking sessions conducted by users.
3. **OrderDetails.csv**: Details of orders placed by users, linked to cooking sessions.

The primary objectives include:
- Cleaning and merging the datasets.
- Analyzing the relationship between cooking sessions and user orders.
- Identifying popular dishes.
- Exploring demographic factors influencing user behavior.
- Providing actionable business recommendations.

## Data Preparation

### Cleaning Steps
1. Ensured correct data types for date fields (`registration_date`, `session_start`, `session_end`, and `order_date`).
2. Addressed any missing or inconsistent data.
3. Resolved duplicate column names resulting from merges by renaming or selecting appropriate fields.

### Merging Datasets
1. Merged `CookingSessions` and `OrderDetails` on `session_id` using a left join.
2. Combined the resulting dataset with `UserDetails` on `user_id` to create a comprehensive dataset (`full_data`).

## Key Analyses and Visualizations

### 1. Relationship Between Cooking Sessions and User Orders
- Analyzed the number of unique orders per user.
- **Visualization**: Bar chart showing the distribution of unique orders across users.

### 2. Identifying Popular Dishes
- Counted occurrences of dishes in the dataset.
- **Visualization**: Bar chart highlighting the most frequently prepared and ordered dishes.

### 3. Demographic Influence on User Behavior
- Explored how user age correlates with the number of unique orders.
- **Visualization**: Line chart showing the trend of unique orders by age.

## Key Findings
1. Users aged 30-40 tend to place the highest number of unique orders.
2. Spaghetti and Grilled Chicken are among the most popular dishes across sessions and orders.
3. Users who rate their sessions highly are more likely to complete their orders.

## Business Recommendations
1. **Target Demographics**: Focus marketing campaigns on users aged 30-40 to maximize engagement.
2. **Promotions**: Offer discounts or promotions on popular dishes like Spaghetti and Grilled Chicken to increase sales.
3. **Enhance User Experience**: Improve cooking session experiences, as higher session ratings correlate with completed orders.

## Files Included
- `data_analysis_notebook.ipynb`: Jupyter notebook containing the complete analysis and visualizations.
- `UserDetails.csv`: User information dataset.
- `CookingSessions.csv`: Cooking sessions dataset.
- `OrderDetails.csv`: Order details dataset.

## Usage Instructions
1. Ensure all CSV files are in the same directory as the Jupyter notebook.
2. Install the required Python libraries:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Run the notebook to view the analysis and generate visualizations.

## Future Work
- Perform a deeper analysis of session ratings and their impact on order amounts.
- Investigate time-of-day patterns in order placements.
- Explore location-based trends to tailor regional marketing strategies.

## Contact
For questions or suggestions, please contact the project owner at [aditiagrawal199724@gmail.com](mailto:aditiagrawal199724@gmail.com).

