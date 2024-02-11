# Echo-Chess-Engine

An original chess engine that was inspired by Dr. Robert Hyatt's original chess engine "Crafty".
This is my first experience with work of this kind, and some of its attributes include:

* **120 square array board representation** - to handle out of bounds cases for piece movement and to avoid having to limit specific types of movements in specific positions on the board, and thus increasing computing time for the program considerably, I have chosen to work with a 120 square array board that contained within it the actual 64 squares that the game was played in.

* **Bitboards** - a type of data structure that allowed me to represent the positions of pieces on the board and look them up effectively by seperating the board into Files (A through H) and a ranks (1 to 8) and all of their positions could thus be contained within a single 64 bit representation of all of the positions acress the board by rank and file and lookup through bitwise operations alone.

* **Data structures and algorithms** - The engine made considerable use of hashing (via XOR) and hash tables (With a consitent replacement scheme for move search), search trees, arrays, Alpha-Beta search and quiescence search among others

*  **Communication protocols** - Supports two different communication protocols and thus allows it to run on multiple types of GUI 

The engine is capable of basic MVV/LVA move ordering, killer heuristic, History Table (via FEN notation and hash code look-up), and basic move evaluation as well as reading a premade opening moves book (polyglot)
In general, most of what the engine does is look-up.

Although it can be played via console, I recommend using a suitable GUI (I used Winboard)
