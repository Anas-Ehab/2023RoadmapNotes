# Mastery Level 02
Since the course focuses on how to use the terminal I will be making a cheatsheet for the commands.

**Format is command : description**

## Commands
echo Hello : displays Hello to the screen can be quoted ("Hello") or not.

cal : Shows the calendar of the current month can take a parameter of the year (cal 2023) to display all the months in the year can use the option -y 2023 to do the same.

date : Shows the current date and time.

clear : Used to clear the terminal.

history: Shows history of commands after typing history !NumberOfCommand can be used to rerun the command.

history -c; history -w : Clears the history.

which command : Will display the path of the command

echo $PATH : Will print the path of $PATH which is used to identify the runable commands from the terminal.

man command : Used to show the manaul for a command.

ls : shows the content of the working directory (-l to get long fromat and -h to get human readable sizes).

cd path : changes working directory to path (. means the working directory, .. means the previous directory).

help command : similar to man (shows how to use a command) but shorter.

pwd : prints the current working directory path.


## Keyboard Shortcuts
Ctrl + Alt + T : Opens a new terminal.

Ctrl + D : Used in terminal to close it.

Ctrl + C : Used to cancel the running command.

Ctrl + L : Used similar to the clear command to clear the terimnal.

Tab : Used to auto-complete the commands.

Double Tab: Used to list down all possible auto-complete options.

Arrow-Up : Used to browse the pervious commands.

Ctrl + Shift + C : Used to copy from a terminal.

Ctrl + Shift + V : Used to paste into a terminal.

## Extra Information
- The shell is what's used to interpret the commands.
- The terminal is a window to type your commands
- There are different types of shells, the most common is bash.
- The command format is CommandName (cal) options (-y) and input (2023).
- In general an option is written using a dash - when using the shortform(only 1 letter) and two dashes (--) when typing the longform(the whole word).
- The manaul (man) command is used to understand how a command work and and its options/inputs/etc... It has different levels as shwon below 

| Section | Contains                     |
|---------|------------------------------|
| 1       | User Commands                |
| 2       | System Calls                 |
| 3       | C Library Functions          |
| 4       | Devices and Special Files    |
| 5       | File Formats and Conventions |
| 6       | Games                        |
| 7       | Miscellaneous                |
| 8       | System Administration        |

- The pipe (|) in man options part means "OR" (one or the other but not both).
- The [] in the man of a command means that it's optional.
