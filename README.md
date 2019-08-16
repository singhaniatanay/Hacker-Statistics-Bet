# Hacker-Statistics-Bet



# Hacker Statistics

A Statistics problem can faced by 2 methods
- Computing the Sampling Distribution
- Hacker Statistics

By Hacker Statistics we tackle the problem by generating the outcomes of problem and then taking the count of reqd. probability.

Basically we can **SIMULATE**  the sampling distibution (problem) which is easy.
Then count of that simulation would give me the probability.

## Problem Statement

You are in a *BUILDING*. You start with Ground Floor(0). We play a game in which we "Roll a Dice".  

If Dice rolls :
		1 or 2 it takes a step down
		3, 4 or 5 it takes a step up
		6 it again rolls a dice and takes that number of steps up.

It can not go below 0 (*Obviously!*)
There is a chance 0.1% that You fall down to 0 Level.

Bet is will you reach at least 60th Floor.

## Solution
We simulate the problem over 500 times. Get the probability.
More the times we simulate our path (**random walk**) more it will tend to theoritical distibution. Hence more the accuracy of the solution.

#### Random Walk:
By Random Walk, I mean the path we intent to explore.
In this case I will simulate rolling dice by calculating random integer between 1 to 6 which will tell me where to go. This will create a walk.


---


We are only interested in end result of the walk after 100 attempts so we will store the end result. We can plot all walks too.
After Plotting the end results as a Histogram :
![Plot](https://raw.githubusercontent.com/singhaniatanay/Hacker-Statistics-Bet/master/Plot.png "Plot")

By the above histogram we could see the sampling distribution estimate we have created.

Now for the ans we can count the number of end results of walks >=60 and divided by the total  (500) would give us the ans.

i.e
		- 78.4% Chances we will win the bet.
