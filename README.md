# The Reviewer
## Project Overview
One of the most important challenges for football clubs currently is planning for future seasons regarding the composition of their squad. Buying and selling players represents a critical decision as clubs' budgets are limited and players' values can be quite high. For this reason, we have decided to leverage the power of BI and Machine Learning to develop a tool that would present football coaches with KPIs and important metrics that will allow the coach to easily decide on what players represent a potential purchasing or selling opportunity. 
Our football dashboard consists of 3 main components:
- Homepage: Central navigation hub that allows navigation to the other views.
- Team Overview: Platform that provides a general overview of the coach's club roster.
- Scouting Platform: A platform that presents the coach with players that meet a desired set of conditions.

In order to add value with our dashboard, it was decided that we would leverage machine learning algorithms to predict players' future market value. In this way, we are not only looking at descriptive analytics but we are also harnessing predictive analytics to support our findings and claims. On the other hand, the scouting platform utilizes similarity-based algorithms to provide recommendations of players with similar profiles. The code for the algorithms can be found here in Github while the Tableau dashboard can be  visualized [here](https://public.tableau.com/app/profile/daniel.andrade5878/viz/TheReviewer/Homepage) (Please donwload the file for optimum visualization and to avoid problems with extensions)
   
  
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

### Which player represent a market opportunity?
For better visualization of what can be achieved we use the case scenario that we are data analysts working for Liga Deportiva Universitaria de Quito, tailoring our results and presentation for that club.

To get a sense of which players will increase or decrease their market value we can leverage the machine learning predictor that was created. By analyzing all the 25 players that belong to the current roster we can see that Oscar Zambrano stands as the most favorable market opportunity. He is a young, right-footed midfielder that counts with an overall rating of 69 but that also counts with a 'potential' rating of 82. With solid long passing, short passing, vision, and stamina scores he is an asset for any team that is searching for a strong defensive midfielder that is good at keeping positional control of the midfield while also having the technical abilities to make accurate passes that drive the attack towards the opposition's goal.

With this information in hand we can recommend that it would be an opportunity for LDU to sell this player in the upcoming market. He is a young midfielder with great prospect of growth for the future, whose player profile are sought after by plenty clubs. Taking a deeper look a his data, we can see that he has 1 year left of contract, meaning that LDU has to act fast before his contract runs up. From industry knowledge we know that LDU is a club who is typically pressured to keep itself in the top of the ecuadorian and southamerican competitions, therefore they are typically not known for sustaining and developing young players in the first squad. Besides, taking a look at LDU's roster with our dashboard we can see that the midfield is already filled with plenty of experienced players, which won't leave much chance for Zambrano to gain minutes and experience.      

### Looking for a player under certain conditions

It is very common for coaches to request to their teams for player alternatives that meet certain conditions. In this occasion we will fullfill that request for a young, right footed defender. Since the team is on a budget the coach has also asked that the player's value does not exceed 10.000.000 euros. Using the dashboard's filters to narrow our selection gave us a shortlist of 6 candidates that all meet the specified criterias.From here on, we conduct a deeper analysis of each player's potential, release clause value and fluctuation in market value to determine the best choice.  By using the created dashboard we can come up with a selection of 3 players:
    
1. D. Coppola
<img width="1901" height="1023" alt="image" src="https://github.com/user-attachments/assets/cf32f208-f970-4102-82da-8e2c77d2be13" />

2. Z. Debast
<img width="1900" height="1021" alt="image" src="https://github.com/user-attachments/assets/a0c9b08e-fde2-4042-8f7a-e7362b341443" />

3. A. Nagalo
<img width="1900" height="1023" alt="image" src="https://github.com/user-attachments/assets/0dbae217-6d0e-44ce-9722-ccab4e84150f" />


When comparing the dashboard results for all 3 players we can observe that A. Nagalo is the best overall choice, as he is not only the player with the highest 'potential' rating, he is also the one with the lowest salary, which makes it easier to negotiate wages with him. According to our prediction algorithm he is also the one with the highest predicted market value. All indicators point that he is not only a sound decision for squad building but also a good investment opportunity financially speaking.

### Finding a replacement for a certain player

Rumour has it that L. Alzugaray will be signing for a brazilian team at the end of the season. We can leverage the recommendation algorithm we developed and integrated into the dashboard to evaluate his top 3 best replacements options.

<img width="1898" height="1025" alt="image" src="https://github.com/user-attachments/assets/7d824b63-277f-4d62-8323-91c638ec99ae" />

By conducting a similar analysis to the ones in previous sections we can give the recommendation to the club's coaches that the best replacement for Alzugaray would be Francisco Conciençao as he is the youngest player out of the selection (which alligns with the develop young talents mentality at the club). Not only is his 'potential' rating higher than the other candidates, making him a financially sound decision, but our recommendation algorithm ensures that he has a similar playing style and set of skills that characterize the creative players like Alzugaray. Yet another benefit to Francisco is his relatively low release clause and salary, the other players are more experienced and settled, making their signing a much more costly operation. In case the club was looking for a much more secure signing with a higher guarantee of instant impact, R. Garro is good option as his vision, long pass, positioning and ball control ratings reflect the profile of that solid midfielder that provides stability in attacking and defending scenarios.  



