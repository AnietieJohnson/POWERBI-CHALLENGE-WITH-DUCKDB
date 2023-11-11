# <p align="center" > PowerBI Visualization Challenge
![](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/R.png)
## Introduction
It is Day 11 and 12 of the 30 Days DuckDB Challenge! This section explores the realm of data visualization and dashboard creation using Power BI. The primary objective of this task was to create compelling visualizations and an interactive dashboard based on two provided datasets from FIFA. The challenge also included the incorporation of the DuckDB or Mother Duck logo on the dashboard as a symbol of participation in the 30 Days DuckDB Challenge.

## Datasets
The datasets used for this task were pre-cleaned datasets from DuckDBSQL related to FIFA player attributes, ratings, and club information. [Fifa_21_RD1](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/Fifa_21_RD1.csv) and [Fifa_21_RD2](https://github.com/AnietieJohnson/POWERBI-CHALLENGE-WITH-DUCKDB/blob/main/Fifa_21_RD2.csv). 
## Data Import
Utilizing Power BI, the two pre-cleaned datasets were imported and verified for accuracy, mainly using CSV import procedures.
## Data Transformation and Joining

Data cleaning and transformation processes were conducted to ensure data readiness for visualization.
1. Using **Get data Tab**, I chose _text/csv_ and Loaded each file using Data type detection,-: "Based on entire dataset".
2. Loaded the files into PowerQuery Editor for cleaning: 
- Corrected data types for each column
- Renamed column headings for clarity and consistency
- The two datasets were merged using a common column **Name**  using Left join.
## Visualizations

**QUESTION 1: Nationality Distribution**

A bar chart was created to show the distribution of players' nationalities.
I added a slicer that allow users to filter and view number of players from specific countries based on nationality. I further added a drill through that links this bar chart to the table visual in question four, in this way we can see a break down of players in particular country and identify them by their names.

**QUESTION 2: Age vs. Potential**

I Developed a scatter plot to explore the relationship between a player's "Age" and "POT" (potential).
Integrated a trendline to visualize trends between age and potential.

**Question 3: Player Position Analysis**

Generated an interactive pie chart displaying the distribution of player positions.
Enabled interactivity for users to select specific player to view their associated roles. I also filtered the chart to show only top 3 positions

**Question 4: Top Players by Overall Rating**

Created a table listing the top players based on their "OVA" (overall rating) in descending order.
Integrated functionality to allow users to filter and view top-rated players by specific clubs by using a slicer. I also enabled a drill through that allows the table connect to the scatter plot, enabling us to view individual player, their age and POT while taking note of their OVA.

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
