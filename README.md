# PSO
Particle Swarm Optimization Algorithm for Cost optimization

## Problem Description

The scenario is such that the person needs to vacate the current accommodation and move to a new place. The optimal time to move, which will be between Monday 00 00 and Sunday 23 59, needs to be calculated.

Also, the optimal time to vacate depends upon the price of moving service which is the price that the moving service charges us and it fluctuates throughout the day. 
A fitness function should be formulated that takes in account all the variables to calculate the optimal time for us to move from the current accommodation to the new place. 


## Problem Formulation

To tackle this problem, the concept of Particle Swarm Optimisation (PSO) has been used. Between Monday 00 00 and Sunday 23 59, there are numerous possibilities of day and time to move from the current accommodation to the new one. The swarm of particles in the PSO Algorithm represents the various possibilities where each particle represents a potential solution. In the search space, the particle having the best position is identified. Using the experience of the neighbours and that of the particle itself, the best position is found. This is done by comparing the current position with the previous best position based on the fitness of both positions.

The proposed fitness function is,

10000 / ((current rental price + new rental price + price of moving) * renovation level)  

where, the lower the cost, the higher the fitness.



## Result

During the run of the algorithm, each iteration the program prints out the iteration number alongside the particle positions for that iteration. While the algorithm termination threshold is not achieved the algorithm continues to print the position values of each iteration. Furthermore the algorithm prints out the particle with the highest fitness out of all the particles from all the iterations. This position will provide in terms of Time T the most optimal time to move out from the current apartment to the new one relative to the price of moving and renovation level of the new apartment.

The output produced by the algorithm varies according to the parameters initialized, therefore any changes to these parameters brings about change to the output and the optimal position printed by the algorithm. 
