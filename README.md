# Election_Analysis

## Election-Audit Overview
After working on writing a Python program to determine election results by candidate, I was asked to provide meaningful data regarding voter turnout by county.  The data I was asked to find through coding were: to determine how many votes were cast by county, to find what percentage of total turnout belonged to each county, and to declare which county had the highest turnout.

## Election-Audit Results

Based on the data returned by my Python program, here is what I found:

  -   The first item I needed to determine was the total votes cast in the election.  In order to do this, I first defined the variable equal to zero.

<img width="298" alt="Total_Votes_Equals_Zero" src="https://user-images.githubusercontent.com/99457275/159079972-606cf5ba-a2f4-43d1-8f43-d0df8a473131.png">

While reading the CSV file line by line with a for loop, I incremented the total vote count by one for each line.  This counter variable helped me with later calculations.

<img width="502" alt="Total_Votes_Increment_In_Loop" src="https://user-images.githubusercontent.com/99457275/159080522-3594eaa7-31ca-4150-819c-e1c445833077.png">

The final tally was 369,711 votes, which matched the number of lines in the CSV file, less the header row.

  -   The next step was to calculate the number of votes by county, and find the percentage by county out of total votes.  After creating a dictionary to hold the counts, I used the for loop to iterate each item based on county.

<img width="587" alt="Track_votes_by_county" src="https://user-images.githubusercontent.com/99457275/159081061-63b6c597-062e-4bed-a0d5-750bcc6cb216.png">

This produced results shown below, which matched what had previously been calculated by vote counting.

<img width="219" alt="Votes_By_County_Terminal_Output ong" src="https://user-images.githubusercontent.com/99457275/159081410-1fe8baf3-eabe-4808-89d9-0336e2b2bf5a.png">

  -   The next requirement was to have the program show which county had the highest turnout.  Once the dictionary had tabulated the raw data, I used an "if" statement to compare each county's totals.  Below are the code used to perform the calculation and the result printed to the terminal.

<img width="548" alt="Largest_County_Code" src="https://user-images.githubusercontent.com/99457275/159082075-dc724775-cf3f-4657-93d6-3f496d60626a.png">

<img width="254" alt="Largest_County_Terminal_Output" src="https://user-images.githubusercontent.com/99457275/159082138-ccdb6a9b-c55c-447c-838c-f1b46c3b6c26.png">

The largest county by voter turnout was Denver County by a wide margin.

  -   Before calculating county data, I was asked to code a porogram to determine the winner of the election.  I was able to use iteration to find which candidates received votes, how many votes each candidate received, and the percentage of total votes each candidate's percentage represented.  The code was similar to how I determined the county breakdown, as can be seen below, along with the results.

<img width="607" alt="Candidate_Vote_Counter_Code" src="https://user-images.githubusercontent.com/99457275/159082951-acaf3db4-e9a0-4728-a078-e21a9730f9b4.png">

<img width="310" alt="Candidate_Results_Terminal_Output" src="https://user-images.githubusercontent.com/99457275/159083076-47cefae2-4c87-438a-81f2-9818510b3585.png">

  -   The final expectation of the program was that it would show who won the election, their total votes, and vote percentage.  This code is similar to determining which county had the highest turnout.  I used an "if" statement to compare to counted statistics and assigned the winning candidate, their total votes, and percentage of votes to their own variables.  Below is the code and output for this requirement.

<img width="658" alt="Winning_Candidate_Code" src="https://user-images.githubusercontent.com/99457275/159083759-9cc3a707-86c5-409a-b48c-74b5cdc1900b.png">

<img width="221" alt="Winning_Candidate_Terminal_Output" src="https://user-images.githubusercontent.com/99457275/159083851-c3c34850-36e0-48ff-9d60-421bcbad493b.png">

And the winner is: Diana DeGette!  Our code was able to confirm the original counts of the election were accurate.  This data was also printed to a text document so that anyone using it can have a permanent record of the outcome.

## Election-Audit Summary
This code was effectively written to handle any number of candiates and counties where an election can take place.  However, this code does not break down candidate data by county.  That is one improvement that could be considered to help candidates understand how their campaigning efforts affected their outcomes.  Another modification that could be helpful is to learn to code visualizations in Python to provide a graphical representation of the results to accompany the output text file.  
