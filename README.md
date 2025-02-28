# T20-World-Cup-2024-Match-Analysis

This repository contains a detailed analysis of the T20 World Cup 2024 match between India and the United States of America. The project uses ball-by-ball innings data to derive key statistics, visualize performance metrics, and provide insights into the match dynamics. Built with Python, Pandas, and Plotly, this analysis includes batter and bowler statistics, run progressions, partnership contributions, and more.

## Overview

This project provides an analysis of T20 World Cup 2024 matches using Python and data visualization techniques. The analysis includes team performance, player statistics, match outcomes, and other key insights derived from match data.
The analysis focuses on the India vs. USA match from the T20 World Cup 2024. Using a ball-by-ball dataset, the project computes and visualizes:

1.Total runs and wickets for each team.

2.Batter-specific statistics (runs, balls faced, strike rate, boundaries).

3.Bowler-specific statistics (wickets, runs conceded, economy rate, dot balls).

4.Run progression, wicket timelines, and partnership contributions.

5.Key moments in the innings (e.g., wickets falling, significant scoring).

6.Run rate comparisons between the teams.

7.The dataset (india-usa_innings_data.csv) contains 236 rows and 21 columns, capturing detailed ball-by-ball information.

## Features

**Match Data Analysis**: Insights into team performances, run rates, wickets, and player contributions.

**Visualization**: Graphs and charts for better understanding of match trends.

**Comparative Analysis**: Comparison of team performances across different matches.

**Predictive Insights**: Basic predictions on match outcomes using regression-based analysis.

**Data Cleaning**: Handles missing values and ensures data consistency.

**Statistical Analysis**: Computes key metrics like strike rates, economy rates, and total extras.

**Visualizations**:
  
   1.Run progression over overs for both teams.
  
   2.Wicket timelines.
  
   3.Batter run distribution.
  
   4.Bowler performance (economy rate vs. wickets).
  
   5.Partnership contributions (stacked bar charts).
  
   6.Key moments in the innings with annotations.
  
   7.Run rate comparisons (average and per over).

**Interactive Charts**: Uses Plotly for dynamic and visually appealing graphs.

## Technologies Used

1.Python

2.Pandas (for data manipulation)

3.Matplotlib & Seaborn (for visualization)

4.Scikit-learn (for predictive analysis)

5.Jupyter Notebook (for running the analysis)

## Usage

1.Load the dataset (t20_wc_2024_matches.csv) into the Jupyter Notebook.

2.Run the analysis scripts to generate insights.

3.Visualize the trends and key statistics.

## Dataset

The dataset I am using provides a comprehensive record of the innings, including player performance, team statistics, and specific events like dismissals and reviews.

<img width="1019" alt="Screenshot 2025-02-28 at 3 57 37 PM" src="https://github.com/user-attachments/assets/58b85ada-c4f6-4b2d-bc88-c139db2d9d3c" />

<img width="781" alt="Screenshot 2025-02-28 at 3 58 00 PM" src="https://github.com/user-attachments/assets/9bc7b962-c6de-4322-82fc-1678f82d9d14" />

The missing values and data types:

<img width="361" alt="Screenshot 2025-02-28 at 3 58 23 PM" src="https://github.com/user-attachments/assets/c4864b9b-a40e-455f-ac6b-cdfe493871dc" />

<img width="361" alt="Screenshot 2025-02-28 at 3 58 36 PM" src="https://github.com/user-attachments/assets/64c32df8-91e8-431f-94da-ed9647098a9b" />

The data has null values in various columns. But in such datasets, even null values have a meaning, so we will leave them as it is and move forward.

## After Gruoping Data

I have grouped the data that we needed to analyze this properly. We can look at all the grouped insights one by one.

1. **total_runs**:

<img width="361" alt="Screenshot 2025-02-28 at 3 58 58 PM" src="https://github.com/user-attachments/assets/bcd7d5b3-6907-44c8-81ae-e268d18754a1" />

2. **total_wickets**:

<img width="361" alt="Screenshot 2025-02-28 at 3 59 18 PM" src="https://github.com/user-attachments/assets/3ea02051-c51a-4791-8e95-8882cb4ca9a2" />

3. **total_extras**:

<img width="633" alt="Screenshot 2025-02-28 at 3 59 34 PM" src="https://github.com/user-attachments/assets/10004c57-02eb-49db-a602-b7903b8c92f6" />

## Plot 1:

Lets have a look at the progression of the run over overs:

<img width="975" alt="Screenshot 2025-02-28 at 4 00 00 PM" src="https://github.com/user-attachments/assets/95cc837f-c52c-4a64-a1e1-aca067a5f2dd" />

The graph shows the progression of cumulative run over the overs for both India and the USA in their T20 World Cup match. Initially, both teams had a steady run rate, with India slightly ahead in early overs. As the innings progressed, USA gained momentum and took the lead briefly around the middle overs. However, India accelerated their scoring in the later overs, surpassing the USAand maintaining the lead until the end. The key takeways is India's strong finish, which enabled them to secure the win by consistently increasing their run rate in the final overs.

## Plot 2

Let's have look at the wickets timeline:

<img width="975" alt="Screenshot 2025-02-28 at 4 00 14 PM" src="https://github.com/user-attachments/assets/9ffd2e2f-3439-4d53-a1f2-2e87397058d0" />

The wicket timeline graph illustrates the distribution of wickets taken over the overs for both India and the USA. The USA lost wickets more frequently, especially in the early overs, with two wickets falling in the first over, followed by consistent wicket losses throughout their innings. In contrast, India experienced their wicket losses more evenly spread across their innings, with a couple of early wickets but maintaining longer parternership in the middle overs. The frequent loss of wickets by the USA disrupted their momentum, while India's ability to avoid clusters of wickets falling in succesion helped them maintain a steady scoring rate and ultimately secure the win.

## Plot 3

Let's have a look at the run distribution by batter:

<img width="975" alt="Screenshot 2025-02-28 at 4 00 28 PM" src="https://github.com/user-attachments/assets/8aeec37f-eec1-4872-a271-65018d072752" />

Notably, S.A. Yadav emerged as the higest scorer with a significant contribution, followed by NR Kumar and S. Dube. These three players were pivotal in their team's innings, providing the bulk of the runs.

## Plot 4

Let's have a look at the bowling performance:

<img width="975" alt="Screenshot 2025-02-28 at 4 00 49 PM" src="https://github.com/user-attachments/assets/25eb6165-e9af-47ed-b16d-b0c23ab58bac" />

The bowling performance graph compares the economy rate and wickets taken by various bowlers in the match between India and the USA. Arshdeep Singh stands out the most effective bowler, taking the higest number of wickets (4) with a commendable economy rate. Other notable performance include SN Netravalkar, both taking 2 wickets each with modrate economy rates. Bowler like S Dube, having a higher economy rate, contrbuted less in terms of wickets
