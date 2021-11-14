# Elections-Analysis

## Project Overview
A Colorado Board of Elections has given you the following tasks to complete the elction audit of a recent local congressional election. To view a general summary of the analysis conducted, a general outline must be constructed (i.e. what steps should I take with this amount of data?). The general outline goes as follows:

1. Calculate the total number of votes cast.
2. Get complete list of candidates who received votes.
3. Calculate the total number of votes each candidate recieved.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

## Resources
-Data Source: election_results.csv
-Software: Python 3.7.6, Visual Studio Code 1.62.0

## Summary
The analysis of the election shows that:
-There were 369,711 votes cast in the election
-The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
-The candidate results were:
  - Charles Casper Stockham received 23.0% of the votes and 85,213 number of votes
  - Diana DeGette received 73.8% of the votes and 272,892 number of the votes 
  - Raymon Anthony Doane received 3.1% of the votes and 11,606 number of the votes
 -The winner of the election was:
  - Diana DeGette who received 73.8% of the vote and 272,892 number of votes
 - The county with the largest voter turnout is Denver who received 82.8% of the votes and 306,055 number of votes

## Challenges of this analysis
The primary challenge of this analysis was formatting the variable in a meticulous manner that produces results. Needless to say that this was my initial challenge and when the coding didn't work and read as a "KeyError", there was an issue in redefining the variable, but then it only read both the precentage and number of votes casted within each county as "0"; ergo having to redefine the variable in line 44. In addition to this, line 73 also proved to be partial to the reason why the county votes only totaled in "0" for both number of votes and percentage per county by not adding an additional condition for "and".

## Election Audit Summary
Despite the challenges faced, the following script can be used for any election so long as the original data is stored as a csv file and the name of the file is changed in line 5 of the script (i.e. the code would read as file_to_load=os.path.join("Resources","file name.csv")). In addition if the file is not csv, the user must change the dependencies in lines 2 to 3. Another note if one chooses to, is to add another segment of coding that displays the number of votes and percentage in a county for each candidate (e.g. Diana DeGette received X% of votes and X number of votes in the county of Denver)
