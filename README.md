# Baseball Data Analysis - SQL Queries and Insights

This project involves analyzing historical baseball data using PySpark. The dataset consists of two tables: `People` (player information) and `Batting` (batting statistics). The analysis focuses on calculating batting averages, identifying home run leaders, and determining team slugging percentages. Below is a summary of the questions addressed and the methods used to derive insights.

## Dataset Overview

- **People Table**: Contains player names, birth details, biographical information, and career milestones.
- **Batting Table**: Contains players' yearly batting statistics, including at-bats, runs, hits, home runs, and more.

## Analysis and Queries

### 1. Batting Average Over .300
- **Objective**: Identify the number of MLB players each year with a batting average over .300, considering only players with more than 50 at-bats.
- **Method**: Calculated the batting average for each player per year and filtered the results to include only players with more than 50 at-bats.

### 2. Home Run Leaders Since 1930
- **Objective**: For each year since 1930, identify the MLB player with the most home runs in each league, including league, team, and batting average.
- **Method**:
  - Filtered data from 1930 onward.
  - For each league and year, identified the player with the most home runs.
  - Considered the player’s team based on their final appearance in the season.
  - Handled ties using the number of RBIs and player ID as tie-breakers.

### 3. Highest Team Slugging Percentages
- **Objective**: Determine the top 10 historical team slugging percentages, including the year and team name.
- **Method**: Calculated slugging percentage for each team by summing total bases (derived from hits, doubles, triples, and home runs) and ranked the top 10 teams.

## Results
The queries for each analysis were executed successfully using PySpark, providing insights into historical player performances and team statistics in Major League Baseball.

## Note
The dataset is in a tidy format provided under Open Data terms. No additional data cleaning was necessary for the scope of this analysis.
