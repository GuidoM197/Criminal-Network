# Criminal-Network
## TP3 of Algorithms and Data structure

### This project simulates, through the use of graphs, various functionalities to help FBI agents track convicts or obtain information.

### The program must receive as a parameter and load into memory the data set ($ ./algopoli messages.tsv) and then wait for the reception of commands by standard input, of the style <command> parameter1, parameter2.

### Once the file has been processed and the graph has been assembled, instructions are requested, which can be:

- __*Command -> min_seguimientos and Parameters -> origin and destination:*__ prints a list with the criminals (their identification code) with which we go from the origin criminal to the destination criminal in the fastest way. In case of not being able to track (i.e. there is no path), print Tracking impossible.

- __*Command -> mas_imp and Parameters -> cant:*__ Prints, from highest to lowest importance, the most important number of criminals.

- __*Command -> persecution and Parameters -> criminal1, criminal2, ..., criminalN and K:*__ Given each of the past criminals (undercover agents), obtain the shortest path to get from one of the criminals passed by parameter, to one of the K most important criminals. In case of having paths of equal length, prioritize those that go to a more important criminal.

- __*Command -> communities and Parameters -> n:*__ Prints a list of communities with at least n members.

- __*Command -> disclose and Parameters -> criminal and n:*__ Prints a list with all the criminals who end up receiving a rumor that begins with the criminal passed by parameter, and at most makes n jumps (then, the message begins to be distorted too much), taking into account that all the criminals will transmit the rumor to their relatives.

- __*Command -> disclose_cycle and Parameters -> criminal:*__ Allows you to find the shortest simple path that begins and ends with the criminal passed by parameter. If no cycle is found, print No cycle found.

- __*Command -> cfc and Parameters -> none:*__ Prints each set of delinquents among which all are connected to all.
