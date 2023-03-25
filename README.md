# Mancala Board Game
A terminal-based version of the board game Mancala in Python.

## Functionality
The program supports the following commands:

**Register New Player**
```
RJ <player_name>
```

**List Existing Players**
```
LJ
```
The output is of the form
```
<player_name> <games_played> <num_of_victories> <num_of_draws> <num_of_defeats>
```
  
**Start a Game Between Two Existing Players**
```
IJ <player_one_name> <player_two_name>
```

**Start a Game Against CPU**
```
IJA <player_name> <difficulty>
```  
Where difficulty can be `Normal` or `Avançado` (Advanced)

**Check the State of the Game**
```
DJ
``` 
The output is of the form
```
<player_one_name> [num_seeds] [num_seeds] [num_seeds] [num_seeds] [num_seeds] [num_seeds] (num_seeds)
<player_two_name> [num_seeds] [num_seeds] [num_seeds] [num_seeds] [num_seeds] [num_seeds] (num_seeds)
```
Where the number of seeds in the six square brackets represents the number of seeds in the six pits for each player (left to right), and the number of seeds in the round brackets represents the number of seeds in each of the player's mancala.

**Make a Turn**
```
J <player_name> <position>
```
Where `position` is a number between 1 and 6 (inclusive).

**Save the State of the Program to a File**
```
G <filename>
```

**Recover the State of the Program from a File**
```
L <filename>
```

## Start the program
```
python program.py
```
