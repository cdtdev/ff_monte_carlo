# ff_monte_carlo
Fantasy Football Python Monte Carlo Simulator

A simple Python script which simulates a specified number of random fatnasy football seasons to produce each team's playoff probability.

Python is required to run the script and there are no variables. To set you league's information, change the following areas of the script:

#number of random season's to simulate
simulations = 1000000 
#weeks in the regular season
league_weeks = 13 
#number of teams to playoffs
teams_to_play_off = 4 


#team_names:: list of team names. list order is used to 
#index home_teams and away_teams

#home_teams, away_teams: list of remaining matchups in the regular season.
#Indexes are based on order from team_names

#current_wins: Integer value represents each team's win count.
#The decimal is used to further order teams based on points for eg 644.8 points would be 0.006448.
#Order needs to be the same as team_names

team_names = ['Kingsland Tough Bruddas','Schroedingers Cats','The Killer Brees','Deez Nuts 4 Prez','Oakeridge Overlords','College Hillbilly','Norwood Knuckles','West City Possums','Crazy Monkeys','Mount Thunderbolts','Southeast Bulls','Te Puke Thunder']
home_teams = [3,4,6,8,9,10,1,2,5,7,11,12,3,4,6,8,9,10,3,4,6,8,9,10,1,2,5,7,11,12]
away_teams = [5,12,1,11,2,7,8,10,9,6,4,3,11,1,2,7,12,5,1,7,5,2,11,12,9,4,8,3,10,6]
current_wins = [3.007153,6.008344,5.007673,2.006870,3.006512,4.007109,6.007020,4.007222,3.007082,4.007003,4.007539,4.007405]

###ONLY CONFIGURE THE VALUES ABOVE

The following output is provided
Team Name, Playoff Probability, First Position Probability, Second Position Proability, ...., Last Playoff position proability

Sample out is shown below:

Kingsland Tough Bruddas	6.16	0.08	0.68	1.75	3.65
Schroedingers Cats	94.53	52.17	25.91	10.32	6.13
The Killer Brees	74.4	11.83	23.78	23.35	15.45
Deez Nuts 4 Prez	0.12	0.0	0.0	0.0	0.12
Oakeridge Overlords	3.27	0.01	0.28	1.26	1.71
College Hillbilly	22.52	1.86	4.41	7.51	8.74
Norwood Knuckles	80.47	27.27	24.53	17.73	10.94
West City Possums	27.23	2.12	5.13	8.53	11.45
Crazy Monkeys	4.53	0.06	0.55	1.45	2.46
Mount Thunderbolts	17.76	1.11	2.79	6.07	7.79
Southeast Bulls	37.32	1.82	6.43	12.04	17.04
Te Puke Thunder	31.68	1.65	5.52	9.99	14.52

Average # of wins for playoff spot
1	9.28
2	8.43
3	7.84
4	7.34

Histrogram of wins required for final playoff spot
1	0.0	0.0
2	0.0	0.0
3	0.0	0.0
4	0.0	0.0
5	0.0	0.0
6	0.637	8.218
7	64.819	85.062
8	34.33	6.72
9	0.214	0.001
10	0.0	0.0
11	0.0	0.0
12	0.0	0.0
13	0.0	0.0
1,000,000 Simulations ran in 0:01:11.413177

