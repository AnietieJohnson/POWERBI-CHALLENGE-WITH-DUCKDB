# <p align="center" > PowerBI Visualization Challenge
![](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/R.png)
## Introduction
It is Day 11 and 12 of the 30 Days DuckDB Challenge! This section explores the realm of data visualization and dashboard creation using PowerBI. The primary objective of this task is to create compelling visualizations and an interactive dashboard based on two provided datasets from FIFA. The challenge also includes the incorporation of the DuckDB or Mother Duck logo on the dashboard as a symbol of participation in the 30 Days DuckDB Challenge.

## Datasets
The datasets used for this task were pre-cleaned datasets from DuckDBSQL, related to FIFA player attributes, ratings, and club information. [Fifa_21_RD1](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/Fifa_21_RD1.csv) and [Fifa_21_RD2](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/Fifa_21_RD2.csv). 
## Data Import
Utilizing Power BI, the two pre-cleaned datasets were imported and verified for accuracy, mainly using CSV import procedures.
## Data Transformation and Joining

Data cleaning and transformation processes were conducted to ensure data readiness for visualization.
1. Using **Get data Tab**, I chose _text/csv_ and Loaded each file using Data type detection,-: "Based on entire dataset".
2. Loaded the files into PowerQuery Editor for cleaning: 
- Corrected data types for each column
- Renamed column headings for clarity and consistency
- The two datasets were merged ON a common column **"Name"**,  using Left join.
## Visualizations

### Question 1: Nationality Distribution
- **Visualization Created:** A bar chart showcasing the diverse distribution of players' nationalities.
Enhancements: Incorporated a slicer for users to filter and view player counts based on specific countries, offering an interactive way to explore individual nationalities.
- **Drill-Through Integration:** Linked the bar chart to a table visualization in Question 4, facilitating a detailed breakdown of players within a particular country. This allows identification of players by their names, providing a comprehensive view of each nationality's player roster.
### Question 2: Age vs. Potential
- **Visualization Developed:** A scatter plot examining the relationship between a player's "Age" and "POT" (potential).
- **Trendline Inclusion:** Integrated a trendline into the scatter plot to visualize trends and patterns concerning age and potential, aiding in the understanding of any potential correlations or tendencies between these variables.
### Question 3: Player Position Analysis
- **Visualization Generated:** An interactive pie chart illustrating the distribution of player positions. I Enabled slicers for users to select specific players, thereby displaying their associated roles. Additionally, a filter was applied to the chart to focus on the top three positions, enhancing the clarity of the visualization.
### Question 4: Top Players by Overall Rating
- **Visualization Created:** A table displaying the top players based on their "OVA" (overall rating) in descending order.
- **Club-Specific Filtering:** Integrated slicer enabling users to filter and view top-rated players associated with specific clubs 
- **Drill-Through Connection:** Enabled a drill-through feature linking the table to the scatter plot, offering a comprehensive view of individual player details such as their age, potential, and overall rating (OVA).
  
**Interactive Dashboard**
- Consolidated all visualizations from Tasks 1 to 4 into a single Power BI dashboard.
- Incorporated slicers, filters, and drill-through actions to make the dashboard interactive.
![](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/fifa21%20powerbi%20analysis.png)
## Conclusion
The successful completion of the Power BI visualization challenge provided valuable insights into the FIFA player datasets, emphasizing the significance of data visualization in extracting actionable insights from complex datasets. Each visual representing the questions above can be found as a powerbi file [here](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/duckdb%20challenge%20phase%202.pbip)
It can also be viewed as a pdf [here](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/duckdb%20challenge%20phase%202%20pdf.pdf)
## Insights
- **Position Prevalence:** The pie chart representing player positions indicates that the Centre-Back position is notably prevalent. This position is crucial in defensive play, indicating the significance of defensive roles in football strategy.
- **Top Player:** The table displays Lionel Messi as the highest-rated player, highlighting his exceptional skill and performance within the dataset.
- **Top Clubs:** By filtering the club using the slicer, the top 5 clubs based on player ratings (OVA) are identified. This sheds light on the clubs with the highest-rated players, potentially indicating the clubs excelling in player development and performance.
- **POT and Age Correlation:** The scatter plot analysis of Potential (POT) against Age indicates zero correlation between these two variables. This suggests that as players' ages increase, there's no clear and consistent pattern regarding their potential ratings. It indicates that a player's age might not be a determining factor for their potential in the dataset analyzed.
- **Global Talent pool:** The count of players by nationality shows a diverse representation from various countries, emphasizing the widespread global representation within FIFA. This signifies the international nature of the sport and the diverse talent pool involved in football.
  
## REFERENCE
Image Title: Duckdb

Source: Bing Images. 

URL: https://alex-monahan.github.io/2021/08/22/Python_and_SQL_Better_Together.html

Accessed Date: August 23, 2021
