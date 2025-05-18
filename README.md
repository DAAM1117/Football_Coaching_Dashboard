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

## Exploratory Data Analysis
We leverage EDA to answer the following questions: 
- From the players in the current roster, which one represents the biggest sale opportunity in case a sale was necessary?
- What players represent a market opportunity when looking for a young, tall, right footed defender, whose market value doesnt exceed 10.000.000 euros?
- What players are a good alternative for a certain player rumoured to be leaving at the end of the season?

## Results / Recommendations

### First Question
For better visualization of what can be achieved we use the case scenario that we are data analysts working for Liga Deportiva Universitaria de Quito, tailoring our results and presentation for that club.

To get a sense of which players will increase or decrease their market value we can leverage the machine learning predictor that was created. By analyzing all the 25 players that belong to the current roster we can see that Oscar Zambrano is the player who is the most likely to gain market value. He is a young, right-footed midfielder that counts with an overall rating of 69 but that also counts with a 'potential' rating of 82. With solid long passing, short passing, vision, and stamina scores he is an asset for any team that is searching for a strong defensive midfielder that is good at keeping positional control of the midfield while also having the technical abilities to make accurate passes that drive the attack towards the opposition's goal.

With this information in hand we can recommend that it would be an opportunity for LDU to sell this player in the upcoming market. He is a young midfielder with great prospect of growth for the future, whose player profile are sought after by plenty clubs. Taking a deeper look a his data, we can see that he has 1 year left of contract, meaning that LDU has to act fast before his contract runs up. From industry knowledge we know that LDU is a club who is typically pressured to keep itself in the top of the ecuadorian and southamerican competitions, therefore they are typically not known for sustaining and developing young players in the first squad. Besides, taking a look at LDU's roster with our dashboard we can see that the midfield is already filled with plenty of experienced players, which won't leave much chance for Zambrano to gain minutes and experience.      

### Second Question

