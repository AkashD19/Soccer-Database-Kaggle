# Soccer-Database-Kaggle
Analysis of the Soccer dataset from Kaggle.

The link to the Database is: https://www.kaggle.com/hugomathien/soccer

The ultimate Soccer database for data analysis and machine learning
What you get:

+25,000 matches
+10,000 players
11 European Countries with their lead championship
Seasons 2008 to 2016
Players and Teams' attributes* sourced from EA Sports' FIFA video game series, including the weekly updates
Team line up with squad formation (X, Y coordinates)
Betting odds from up to 10 providers
Detailed match events (goal types, possession, corner, cross, fouls, cards etc...) for +10,000 matches.

My Analysis includes mostly SQL queries run on SQLITE syntax via Pandas.

1. It looks for correlation between various player attributes like age, stamina, acceleration etc.

2. It looks for change in attributes with age.

3. The crux of this project lies on a stat I created called the Unpredictability Score. The approach was to compute league tables for the Top 5 leagues in Europe namely English Premier League, France Ligue 1, Germany 1 Bundesliga, Italy Serie A and Spanish Liga BBVA for all seasons from 2008/09 - 2015/2016. Then in each year I looked at the scores of the matches played between the Top 5 and the Bottom 5 teams of that year. Whenever a bottom team gets a favorable outcome against a top team I add on to my Unpredictability Score.
Scoring rules are
Bottom as Home Team Win - 1 point

Bottom as Home Team Draw - 0.5 point

Bottom as Away Team Win - 1.25 point

Bottom as Away Team Draw - 0.75 point

The following are the highlights of this Analysis:

a) Contrary to what you may believe Ligue 1 seems most unpredictable i.e. a bottom 5 team gets a favourable outcome against a Top 5 team most often in this league. 

b) La liga had the most unpredictable league and that was 2010-11 but also the most predictable league with lowest unpredictability score in 2014-15 

c) Germany has a general high unpredictableness but it may be due to the reason that I have considered the Top & Bottom 5 even though this league has only 18 teams each season. Having said that,2010-11 was a crazy season in Bundesliga. Dortmund was champion, Bayern Munich came 3rd, Schalke, VfL Wolfsburg, Borussia Mönchengladbach, Eintracht Frankfurt were amongst the lowest ranked teams. Suprisingly Schalke went on to win the DFB Pokal and competed in the Europa League despite being so lowly ranked.

This notebook will be helpful to anyone looking to refresh their SQL skills.
