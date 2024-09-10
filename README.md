# Voting-system-in-c
This repo provides a code for the Tideman voting system using c program.

## What is Tideman Voting System?

The Tideman voting system, also known as the Ranked Pairs method, is a ranked voting system used to determine the winner of an election when voters rank candidates in order of preference. It's designed to reflect voters' preferences more accurately and prevent issues like strategic voting and non-monotonicity.

## How It works?

- *Ranked Ballots*: Voters rank candidates in order of preference. Each rank typically receives a certain number of points, with higher-ranked candidates getting more points.
- *Preference Matrix*: The system constructs a preference matrix from the ballots, showing how many voters prefer each candidate over every other candidate.
- *Pairwise Comparisons*: All possible pairs of candidates are compared based on how many voters prefer one candidate over the other.
- *Pair Sorting*: The pairs are sorted by the strength of their preference, from the most preferred to the least.
- *Locking Pairs*: Pairs are added to the ranking (locked in) in order of their strength, ensuring that no cycles (situations where candidates can be ranked cyclically) are created.
- *Determine Winner*: The final winner is the candidate who is not "locked out" by any other candidate in the final graph.


## How To Give Input

- The program takes in-line arguments.
- These arguments contains the name of the candidates.
- After this the program asks for the number of voters.
- Then the program asks for the input of each voter's preference list.
