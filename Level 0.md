# Bandit Level 0

## Description:
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

## Tips to help to solve this Level:
ssh

## Solution:
The first step I took was to read through the man pages of the ```ssh``` command to understand what options are available. I then tried the options `-W`, `-L` and `-J` and `-l' for login_name so like this:

```ssh -W bandit.labs.overthewire.org -l bandit0```

After a few attempts I finally was able to work out the command:

```ssh bandit0@bandit.labs.overthewire.org -p2220```

![alt text](bandit0-loginSrini.png)
