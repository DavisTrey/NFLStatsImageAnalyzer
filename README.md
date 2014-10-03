NFLStatsImageAnalyzer
=====================

Analyzes bit-data from NFL probability curves to approximate how much better certain teams played over others. 

To use, screenshot NFL probability curves from live. advancednflstats.com (such as
http://live.advancednflstats.com/weekly.php?gameid2=56230&week=4) and then place them into the ProbabilityImages folder.
Make sure to name them "Team 1 vs. Team 2", where Team 1 is the bottom team on the curve. Then, just run ImageParser.java. 
The program will parse each image's pixels, compute the integral of the curve to estimate the degree to which each team
won the game, and then print the output for each game to console.

Compared to computing with the actual XML data used to compute each graph, this program has approximately .7% error. 
For instance, in the Chiefs vs. Patriots game included in the repo, this program returns .1498, whereas the actual value
is .1486. 

