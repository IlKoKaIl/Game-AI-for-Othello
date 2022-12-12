# Game-AI-for-Othello
A game AI made to play othello game + a pygame ui. Made using a minimax algorithm
-----------------------------------------

agent.py contains code for the minimax algo agent that plays the game

othello_gui.py contains a simple gui for the othello game

othello_game.py contains the game states. It manages the game by communicating between both players/AI

othello_shared.py contains functions for legal moves, captured tiles and shares information between the game manager, gui, ai and players.

randy_ai.py A test AI named randy that makes random moves as opposed to the minimax using ai in agent.py

-------------------------------------------
Running the code
You can run the Othello GUI by typing $python3 othello gui.py -d board_size -a
agent.py, where the parameter board size is an integer that determines the dimension of the board upon
which you will play and agent.py is the game agent you would like to play against. If you type

$python3 othello gui.py -d board_size -a randy_ai.py

The GUI can take also take two AI programs as command line parameters. When two AIs are specified
at the command line you can watch them play against each other. To see Randy play against itself, type
where board_size is an int representing board size  
$python3 othello gui.py -d board_size -a randy_ai.py -b randy_ai.py

For running the minimax algo using command line using flags do 
$python3 othello gui.py -d 4 -a agent.py -m

For running agent.py on a 4x4 board to play against use
$python3 othello gui.py -d 4 -a agent.py

To make the agent use alpha-beta instead of minimax use this to play
$python3 othello gui.py -d 4 -a agent.py -b randy_ai.py
