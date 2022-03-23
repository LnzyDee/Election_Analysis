# Election Analysis

## Overview Election Audit
A Colorado Board of Elections employee has given the following tasks to complete the election audit of a recent local congressional election:

1. Calculate the total number of votes cast.
2. Provide the number of votes and percentage of total votes for each county in the precinct.
2. Find the county with the largest voter turnout.
3. Get a complete list of candidates who received votes.
4. Calculate the total number of votes each candidate received.
5. Calculate the percentage of votes each candidate won.
6. Determine the winner of the election based on popular vote.

## Resources
- Data Source: [Election Results CSV](Resources/election_results.csv)
- Software: [Python](https://www.python.org/), 3.7.6, [Visual Studio Code](https://code.visualstudio.com/), 1.65.2

## Election Audit Results
The analysis of the election shows that:
- There were 369,711 votes cast in the election.
- The counties involved in the election were:
  - Jefferson
  - Denver
  - Arapahoe
- The voting results of each county were:
  - Jefferson county reported at 10.5% of the total votes with 38,855 votes.
  - Denver county reported at 82.8% of the total votes with 306,055 votes.
  - Arapahoe county reported at 6.7% of the total votes with 24,801 votes.
- The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were:
  - Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
  - Diane DeGette received 73.8% of the vote and 272,892 number of votes.
  - Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
- The winner of the election was:
  - Diane DeGette who received 73.8% of the vote and 272,892 number of votes.

Results as shown in the terminal and as copied to a text file:

![Terminal Code Results](electiontermresults.png) ![Text Code Results](electiontxtresults.png)

## Election Audit Summary
Provided the proper documents, the script used to procure these results can be re-worked slightly to accommodate getting the results of other elections. By simply changing the file the code works from--in this case it was the "election_results.csv" file, as in photo below--we can use this script for other elections. Making sure the columns listed in the file are the same as those in the election_results.csv file (e.g., Ballot ID, County, Candidate) and in the same order, as shown here:

![Election Results CSV](electionxclss.png)

You may not have to adjust anything but the folder location and file name--as listed in the code as shown below with "Resources", "election_results.csv" and "analysis", "election_results.txt":

![File Location Code](electioncode2.png)

If the column order is different, it's a simple change of a few lines of code; like changing the index number in the "candidate_name = [2]" and "county_name = [1]" variables, as shown here:

![Variable Code](electioncode1.png)

to align with whichever column in the csv file matches the variable needed in order for the code to work on a new set of data. For example, if the two listed above's columns were swapped, the code would instead then read, "candidate_name = [1]" and "county_name = [2]".
