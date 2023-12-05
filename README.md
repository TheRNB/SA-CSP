# SA-CSP
An implementation of the Cutting Stock Problem using Simulated Annealing

### INPUT REPRESENTATIONS
We must first come up with a way to represent the input. We define an array with the same length as the number of ordered pieces, and assign each piece the index of its stock. Meaning that if two pieces i and j are to be cut from stock k, then in indices i and j of the array there is value k.

### FITNESS FUNCTION
The fitness of a solution is based on the number of different stocks it has used to cut the ordered pieces. So that a solution with a lower number of stocks used, becomes a "more fit" solution as the problem requires.

### CONTROL PARAMETERS
We must now define the problem specific control variables of the algorithm

### INITIAL SOLUTION
We must also come up with a way to generate new solutions

### NEIGHBOR
Now we should come up with a way to generate neighboring solutions to a specific solution. We can start by checking how much of each stuck is cut, then choose a random piece and a random stock that has enough waste material to fit that piece and assign the piece to that stock. We can also choose a completely new stock to have the new piece cut from there, but that is not beneficial in our case since we want to minimize the number of used stocks.

### ACCEPTANCE PROBABLITY
We should also come up with a function that defines the acceptance probablity of a neighbor as defined in the algorithm.

## INFERENCE
We should now run the algorithm.
