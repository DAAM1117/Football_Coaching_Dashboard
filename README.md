# The Reviewer
## Project Overview
One of the most important challenges for football clubs currently is planning for future seasons regarding the composition of their squad. Buying and selling players represents a critical decision as clubs' budgets are limited and players' values can be quite high. For this reason, we have decided to leverage the power of BI and Machine Learning to develop a tool that would present football coaches with KPIs and important metrics that will allow the coach to easily decide on what players represent a potential purchasing or selling opportunity. 
Our football dashboard consists of 3 main components:
- Homepage: Central navigation hub that allows navigation to the other views.
- Team Overview: Platform that provides a general overview of the coach's club roster.
- Scouting Platform: A platform that presents the coach with players that meet a desired set of conditions.

In order to add value with our dashboard, it was decided that we would leverage machine learning algorithms to predict players' future market value. In this way, we are not only looking at descriptive analytics but we are also harnessing predictive analytics to support our findings and claims. On the other hand, the scouting platform utilizes similarity-based algorithms to provide recommendations of players with similar profiles. The code for the algorithms can be found here in Github while the Tableau dashboard can be  visualized [here](https://public.tableau.com/app/profile/daniel.andrade5878/viz/FootballDashboard_17425254712750/Homepage?publish=yes) (Please donwload the file for optimum visualization and to avoid problems with extensions)
   
  
## Data Sources
Research of the literature showed that multiple studies use EAFC's database as a trustable source for player's statistics. Therefore, we are going to use the famous videogame's database found on [Kaggle](https://www.kaggle.com/datasets/stefanoleone992/ea-sports-fc-24-complete-player-dataset?select=male_players.csv).(Important note: For the sake of practice, some changes to the file were also made in Excel)  

## Tools
- Excel: Data Cleaning and Transforming
- Python : EDA, Data Cleaning and Modeling
- Tableau: Data Visualization

## Data Cleaning and Preparation
1. Fixing variable type
2. Handling duplicates
3. Handling missing values
4. Feature reduction
5. Handling outliers
6. Feature Scaling and Encoding
