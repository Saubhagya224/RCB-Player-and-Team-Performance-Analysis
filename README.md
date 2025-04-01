# IPL Analysis – Optimizing RCB’s Player Auction Strategy (2017 Mega Auction)

This analysis examines Royal Challengers Bangalore's IPL performance, identifying top players and optimizing team composition. By analyzing player stats and team performance across seasons, we provide data-driven insights for strategic selection in future IPL seasons.

# Project Objective

Royal Challengers Bangalore (RCB) has been a consistently competitive team in the IPL but has struggled to secure a
championship title. The management aims to leverage data to identify top-performing players and improve team composition ahead of the mega player auction for IPL 2017.

- Identify top-performing and consistent players.
- Analyze value-for-money investments in the auction.
- Develop data-driven strategies for building a strong, well-balanced team.
- Provide insights on team performance trends, venue impacts, and auction strategies.

# Data Sources and Database Schema

## Primary Data Tables Used
   
This analysis was based on historical IPL data, extracted from multiple SQL tables:

### Ball-by-Ball Data (ball_by_ball)

- Every delivery played, including batsmen, bowler, runs, extras, and wickets.
- Helps track player consistency across seasons.

### Match Data (match)

- Includes match results, win margins, venues, and toss outcomes.
- Useful for venue-based strategies and toss impact analysis.

### Player Performance Data (player_match)

- Contains players’ runs, wickets, and roles (batsman, bowler, all-rounder).
- Helps in ranking players for auction strategy.

### Player Information Table (player)

- Includes age, batting/bowling style, and team associations.
- Helps in selecting experienced vs. young talent.

### Season Data (season)

- Provides information on season-wise team performance.
- Helps analyze year-on-year improvement.

### Venue Data (venue)

- Contains information on stadiums and cities.
- Helps in understanding home vs. away performance trends.

# Key Questions and Analysis Performed

To help RCB make better decisions, here covered both objective and strategic questions using SQL queries.

## Performance Analysis of RCB Over the Years

- Used the match table to count RCB's wins.
- Used ball_by_ball and extra_runs to include both regular and extra runs.
- Compared total runs scored and wickets taken across seasons.
  
## Identifying Top-Performing Players

- Used player_match to calculate strike rate (Runs/Balls Faced × 100).
- Used player_match to compute average runs per dismissal.
- Computed wickets per match for all bowlers using ball_by_ball.
- Identified all-rounders by filtering players with:
  1. Above-average batting (higher than league average)
  2. Above-average bowling (wickets taken higher than average)
     
## Venue and Toss Impact Analysis

- Compared toss winners vs. match winners in different venues.
- Created a venue-wise win/loss table to identify strong & weak stadiums.
- Compared wicket-taking ability across different bowling styles.
  
## Auction Strategy – Selecting the Best Players

- Ranked players based on multi-season performance consistency.
- Mapped player performances across venues.
- Identified top-performing all-rounders for versatility.
- Evaluated Runs per Cost and Wickets per Cost to avoid overpaying.
  
## Business & Viewership Insights

- Analyzed run trends in high-scoring games to improve RCB’s strategy.
- Compared RCB's performance at home vs. away to suggest strategies.
- Correlated high-scoring matches and close finishes with audience engagement.

# SQL Queries and Implementation

## Used SQL queries to extract insights, such as:

 - Finding RCB’s Win Record in 2013
 -  Finding Top 10 Players by Strike Rate
 -  Identifying All-Rounders
 -  Impact of Toss on Match Results
 -  Correcting Data Issues (Delhi Capitals vs. Delhi Daredevils)

# Visualizations and Business Recommendations

## To present insights effectively, used graphs and charts, such as:

 📊 Bar Charts → Top batsmen by strike rate, top bowlers by wickets.
 
 📈 Line Graphs → RCB’s year-on-year performance trends, toss decisions.
 
 📍 Area Graphs → Highest number of sixes in the field.

# Final Auction Strategy Recommendations for RCB

## Invest in Consistent Performers

- Target batsmen with a high strike rate & low dismissal rate.
- Avoid players with extreme fluctuations in performance.
  
## Pick Versatile Players (All-Rounders)

- Select players who contribute both runs & wickets.
- Maximize flexibility in squad selection.

## Optimize Auction Spending
- Use data-driven insights to avoid overpaying for underperformers.
- Identify undervalued players with high impact.

## Leverage Home Advantage

- Choose bowlers effective in high-scoring venues.
- Select batters suited for fast pitches.

## Improve Toss & Match Strategies

- Use historical trends to decide batting vs. bowling first.
- Optimize game plans based on opposition strengths/weaknesses.

# How to Use This Project

- Run the SQL queries to replicate the analysis.
- Use findings to explore RCB's performance trends, player stats, and team insights.

# Tools Used

- SQL (MySQL) – Querying and data retrieval.
- Excel – Advanced analysis and visualization.
- PowerPoint – Presentation of key insights and recommendations.

# Conclusion

RCB has been competitive but inconsistent, struggling in critical phases like Powerplay and Death overs. Kohli and De Villiers have been key performers, while venue-based strategies impact win rates. To improve, RCB should focus on all-rounders, consistent players, and better toss decisions for strategic advantage.
