# source-GoL
A small version of Conway's game of life that runs in the source console. 

## Installation
Unzip the release (or download the source code), and place the 'life' folder into the cfg folder for whichever game you wish to use. That's it!

## Running
Open the console in the game and type the command 'exec life/life'. This should display some text on how to use the program, and display the grid with a glider on it. Read that text to get started. Use the 'help_life' command if you need to see it again. The text is also provided below.

I have had issues with running the program while in a game, even with sv_allow_wait_command 1, due to the very high volume of commands sent. Because of this, I suggest running the file from the title screen.

### Help text

    This is a version of Conway's game of life in the TF2 console. This version is a 13x13 grid that wraps around, due to hardware constraints.

    Type 'start_life' into the console to start with the current setup.

    To change the state of a cell, use the <row>_<col>_t (for alive, or true) or <row>_<col>_f (for dead, or false).

    Cells are 0-indexed (Base 10, despite the grid) starting in the top-right corner, and a preview of the screen can be seen with 'outputAll'

    The loop can be paused with 'stop_life' and restarted with 'start_life'.

    The game can also be played 1 generation at a time with the 'next_gen' command. The 'help_life command brings up this message'

## Performance issues
If your computer is having issues with running the program, try increasing the wait amount in the 'gen_delay' alias in the life.cfg file. This will make the computer render generations more slowly, potentially helping performance slightly.
