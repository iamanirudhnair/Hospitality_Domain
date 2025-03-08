# Hospitality Domain Project Using Power BI

## Project Overview

This project demonstrates the use of Power BI in the hospitality domain to analyze and visualize data, providing insights to improve business decisions. The project integrates various hospitality datasets, such as hotel booking data, customer preferences, revenue, occupancy rates, and more. Through Power BI, we can present actionable insights for management to drive better operational efficiency, customer service, and profitability.

The main objective is to build dynamic reports and dashboards that are visually appealing and easy to interpret for decision-makers in the hospitality industry.

![image_alt](https://github.com/iamanirudhnair/Hospitality_Domain/blob/main/Hospitality_Dashboard.png?raw=true)

## What I Learned

Throughout this project, I gained several valuable insights and learned the following:

1. **Data Import and Transformation**: 
   - I learned how to import data from various sources (Excel, CSV, SQL databases, etc.) into Power BI.
   - Using Power Query, I transformed and cleaned the data by filtering out unnecessary columns, handling missing data, and ensuring the dataset is ready for analysis.

2. **Data Modeling**:
   - Creating relationships between tables using the Power BI model view.
   - Learned about one-to-many relationships, calculated columns, and measures to represent data more effectively.

3. **Visualization Techniques**:
   - I used multiple types of visualizations, such as bar charts, pie charts, maps, and line graphs, to represent trends and KPIs.
   - Implemented slicers and filters to allow users to interact with the data, exploring specific hotel performance based on various criteria (e.g., location, customer demographics, booking date).

4. **DAX (Data Analysis Expressions)**:
   - I wrote several DAX formulas to create custom measures, such as calculating total revenue, occupancy rates, and average customer ratings.
   - This technique enhanced the interactivity of my report by allowing dynamic aggregation based on user selections.

5. **Dashboard Creation**:
   - I designed a comprehensive dashboard that provides a snapshot of key metrics such as occupancy rates, revenue trends, customer demographics, and more.
   - Emphasis was placed on creating an intuitive design with meaningful visual hierarchies, so that even users without technical expertise can understand the insights quickly.

## Techniques Used & Why Chosen

1. **Power Query for Data Transformation**:
   - **Why**: Power Query was essential for cleaning and preparing data for analysis. I used it to filter out irrelevant data, handle missing values, and normalize column formats.
   - **Benefit**: Streamlined data preprocessing, ensuring the data is accurate and in a usable form for analysis.

2. **DAX for Calculated Measures**:
   - **Why**: DAX expressions are extremely powerful for aggregating and summarizing data in custom ways. I created measures like "Revenue per Available Room (RevPAR)", "Occupancy Rate", and "Average Customer Rating" using DAX.
   - **Benefit**: Enables dynamic, real-time calculations that adjust based on user input, providing customized insights in the dashboard.

3. **Slicers and Filters**:
   - **Why**: Slicers allow for easy data filtering, which makes the report interactive. Users can segment the data by customer demographics, hotel locations, or specific date ranges.
   - **Benefit**: Enhances user experience, allowing stakeholders to drill down into the data that is most relevant to their needs.

4. **Maps for Geospatial Analysis**:
   - **Why**: In a hospitality context, location is a key factor in understanding performance. By using maps, I could plot hotel locations and provide insights based on geographical data.
   - **Benefit**: Geospatial analysis helps to uncover regional trends and opportunities for targeted marketing or operational adjustments.

## Errors Encountered and Solutions

### 1. **Error: Circular Dependency in DAX Measures**
   - **Description**: While creating custom DAX measures for revenue and occupancy rate, I encountered an error related to circular dependency.
   - **Solution**: To resolve this, I reviewed my data model and made sure that there were no relationships creating a circular reference between tables. By adjusting my table relationships and ensuring they were directional (one-to-many), I resolved the issue.

### 2. **Error: Data Type Mismatch in Power Query**
   - **Description**: When importing data from CSV, I faced issues with mismatched data types, especially when the columns contained both text and numeric values.
   - **Solution**: I used Power Query’s "Transform" feature to explicitly change the data types of each column to match the expected formats (e.g., converting text columns to numbers where appropriate).

### 3. **Error: Incorrect Aggregation of Revenue in DAX**
   - **Description**: My revenue measure was aggregating incorrectly, as I wasn't accounting for each booking's specific date range (some bookings spanned multiple nights).
   - **Solution**: I created a more complex DAX formula that accounted for the "nights stayed" per booking to ensure the revenue was calculated correctly. I used a `SUMX` function along with proper date filtering to ensure the data was accurately aggregated.

### 4. **Error: Slow Dashboard Performance**
   - **Description**: The performance of my dashboard slowed down significantly when there were too many slicers and filters applied, especially on large datasets.
   - **Solution**: I optimized the model by reducing the number of slicers, avoiding complex relationships between tables, and ensuring that calculated columns and measures were as efficient as possible. Additionally, I set up incremental data refresh to limit the volume of data being processed.

## Conclusion

This Power BI project has significantly enhanced my skills in data visualization, data modeling, and creating interactive dashboards tailored for the hospitality industry. The techniques I used helped in delivering valuable insights that could influence business decisions in a hotel or resort environment. By applying the knowledge from this project, I feel confident in using Power BI for complex datasets and creating dashboards that deliver key metrics in an easily understandable way.
