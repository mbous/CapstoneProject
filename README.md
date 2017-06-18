# Capstone Football Project

###18 June 2017
###Mohamed Boussaid

## Introduction / background
Last year I have been betting on the soccer market. I was excited to make a decent additional income form value betting on live soccer matches, after hearing from others that it would be doable to gain from the bookmakers. In the beginning I was betting on the live goal market (team goals and total goals) by using Unibet as bookmaker. During the live match I based my decisions on live indicators, which were offered by Bet365, and on past team performance, offered by Flashscore. The live indicators where for example dangerous attacks, shots on goals and ball possession. Past performance was checked by looking at the scoring power of the last 10 matches in combination with the league ladder stats (i.e. team goals so far). I placed only a bet if certain condition were met. First, bets were only placed just after half time or after one hour of playing. And I only placed a bet when no goal occurred by the team which overweighs its opponent according to overall (live) stats. Furthermore, I applied some rules of thumb in the decision making process, like when a team has three times as much dangerous attacks compared to its opponent after completion of half time. When I was betting, I thought it would be nice if you could build a simple model which would estimate the probability of a goal occurrence (i.e. team goal over 0.5) based on self-chosen indicators. Ideally, it would be nice to experiment whether there exits some value (i.e. whether bookmaker odds are greater model odd) by betting on team goals.

## Research problem 
Ideally:
Predict the odds of team goal occurrence in second half based on half time match statistics. Compare this prediction with the half time odds of the bookmaker.

Alternative:
Predict the number of team goals in second half based on half time match statistics. Compare this prediction with the realized number of goals in second half.

I plan to use the following data for my project. 
Data: 
Source: www.football.data.co.uk
League: Premier League 2016/17 
Indicators:
*	HS = Home Team Shots
* AS = Away Team Shots
*	HST = Home Team Shots on Target
*	AST = Away Team Shots on Target
*	HC = Home Team Corners
*	AC = Away Team Corners
* FTHG = Full Time Home Team Goals
*	FTAG = Full Time Away Team Goals
*	FTR = Full Time Result (H=Home Win, D=Draw, A=Away Win)
*	HTHG = Half Time Home Team Goals
*	HTAG = Half Time Away Team Goals
*	HTR = Half Time Result (H=Home Win, D=Draw, A=Away Win)

##Issues
*	Obtaining half-time odds bookmaker.
* Indicator dangerous attacks are unfortunately not available in the source data

My plan is to compute derive some descriptive statistics and scatterplots of the above mentioned variables before I come up with a model specification (for example a regression model).

