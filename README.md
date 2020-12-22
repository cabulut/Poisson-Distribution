# Implementation of Poisson Distibution on Football Leagues 


## Getting Started

Pandas, Requests, BeautifulSoup, Scipy, Matplotlib are essentials


## What is Poisson Distribution and how it is being implemented here?

**Poisson Distribution** is a discrete probability distribution that indicates the probability of a given number of events occurring in a fixed interval of time,space,area,distance and volume. It is useful to estimate the number of events in a large population over a unit of time.


The analysis focuses on football leagues that their table can be find on [SkySport DE](https://sport.sky.de/fussball/tabellen) 


The ultimate goal is to estimate the number of goals happening in a match per League.


The data is scraped from the same link again [SkySport DE](https://sport.sky.de/fussball/tabellen) Web scraping is going to turn league tables into a Pandas dataframe which got preprocessed during the scraping. League name, part of the link (based on German) and number of teams should be added while running the function. Default of the function is English Premier League. You can find an example, other league names and amount of teams below.

**table(league='premier-league-tabelle',teams=20)**

-bundesliga-tabelle: 18
-premier-league-tabelle: 20
-serie-a-tabelle: 20
-ligue-1-tabelle: 20
-la-liga-tabelle": 20
-eredivisie-tabelle: 18
-sueper-lig-tabelle: 21

in function the league argument is ***string*** and teams argument is ***integer***

In order to represent the Poisson Distibution, **Probability Mass Function** has been used. PMF simply maps from each value to its probability and both Poisson Distribution and PMF are associated with discrete random variables. After applying Poisson and PMF, numpy arrays are converted into a single dataframe and plot has been implemented.


## How to read the graph

After implementing above procedures and running all the codes, you are going to end up with a single graph with multiple lines and this graph depicts on **xlabel** that total number of goal might happen in a football match and on **ylabel** it is going to show the possibility of this number of goal happening on league level in single match. For instance, if it shows 0.25 probability for 2 goals and 0.15 probability for 3 goals in La Liga this shows that it is more likely to see 2 goals rather than 3 in La Liga per match. When the number of goals increases, the leagues that more goals happen it is going to be the top line at the end of the **x-coordinated** side of the graph.



###### Contact

[LinkedIn](https://www.linkedin.com/in/caner-bulut-48a0784a/)