# Cricket-Performance-Analysis

This repository contains a Power BI dashboard project focused on analyzing cricket match data, player performance, and team statistics using structured datasets. It provides visual insights into batting, bowling, and match summaries across multiple seasons.

## Project Structure
### Tables
- dim_match_summary.csv
Contains metadata for matches such as match IDs, dates, venues, teams, and outcomes.

- dim_players.csv
Detailed player information including full names, playing roles, and images (for enhanced visual dashboards).

- fact_bating_summary.csv
Batting performance data including runs, balls faced, strike rate, boundaries, and dismissal info.

- fact_bowling_summary.csv
Bowling performance data including overs bowled, runs conceded, wickets taken, and economy rate.

### DAX Measures
To enhance data modeling and simplify visualizations, several DAX measures were used in the dashboard. Here are some examples:
- Total Runs = SUM(bating_summary[runs])

- Total Wickets = SUM(bowling_summary[wickets])

- Batting Average = DIVIDE(SUM(runs), COUNT(dismissals))

- Strike Rate = DIVIDE(SUM(runs) * 100, SUM(balls_faced))

- Economy Rate = DIVIDE(SUM(runs_conceded), SUM(overs_bowled))

## Tools Used
- Power BI Desktop
- Power Query for data transformation
- DAX for calculated measures
- Microsoft Excel/CSV for data preparation

### Dashboard
![image](https://github.com/user-attachments/assets/18da68a3-8954-480c-bbe2-b1c01c73edeb)
