# Bandit Level 0 > 1

## Description:
The password for the next level is stored in a file called ```readme``` located in the home directory. Use this password to log into ```bandit1``` using ```SSH```. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Tips to help to solve this Level:
ls, cd, cat, file, du, find

## Solution:
The solution for this level was fairly simple. First thing was to list out the contents within bandit0, this is where the ```readme``` file resided. So there were 2 methods to read the file and it was either using ```cat``` or ```vim``` and this will display/read what is stored within the file.

![](bandit0to1.png)
