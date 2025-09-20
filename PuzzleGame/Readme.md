Java Sliding Puzzle GameA classic command-line implementation of the sliding tile puzzle (also known as the 15-puzzle or n-puzzle). This project is written in pure Java and is designed to be a simple, robust, and fun console application.The game creates a shuffled, yet always solvable, puzzle of a user-defined size and prompts the player to slide tiles until the board is in its sorted, winning state.FeaturesVariable Board Size: Players can choose a puzzle size from 2x2 up to 5x5.Guaranteed Solvable Puzzles: The shuffling algorithm starts with a solved board and makes thousands of random, valid moves to ensure every generated puzzle is solvable.Robust User Input: The game handles various user inputs, validating player names, board sizes, and tile numbers.Clear Console UI: The puzzle board is displayed in a clean, easy-to-read format in the console.Java 8 Compatible: The code is written to be compatible with Java Development Kit (JDK) 8 and later versions.How to Compile and RunTo play the game, you need to have a Java Development Kit (JDK) version 8 or higher installed on your system.Place the Files: Make sure all three .java files (Player.java, Board.java, and PuzzleGame.java) are in the same directory.Compile the Code: Open a terminal or command prompt, navigate to the directory containing the files, and run the Java compiler:javac PuzzleGame.java Player.java Board.java
This will create the corresponding .class files.Run the Game: Execute the main class to start the game:java PuzzleGame
Code StructureThe project is logically separated into three classes, each with a distinct responsibility:Player.java: A simple data class that models a player. It is responsible for validating and storing the player's name.Board.java: The core engine of the game. This class manages the puzzle's state, including the grid of tiles, initializing and shuffling the board, checking for the solved state, and validating tile movements.PuzzleGame.java: The main controller and entry point for the application. It handles the primary game loop, processes all user input from the console, and coordinates the interactions between the Player and Board objects to create the game experience.Example GameplayHere is a sample of what a game session looks like:=== Welcome to the Sliding Puzzle Game! ===
Enter your name: aayush
Enter puzzle size (between 2 and 5): 2
Okay aayush, here’s your puzzle:
+--+--+
| 1| 3|
+--+--+
| 2|  |
+--+--+
aayush, which tile do you want to slide? 3
+--+--+
| 1|  |
+--+--+
| 2| 3|
+--+--+
aayush, which tile do you want to slide? 1
+--+--+
|  | 1|
+--+--+
| 2| 3|
+--+--+
aayush, which tile do you want to slide? 2
+--+--+
| 2| 1|
+--+--+
|  | 3|
+--+--+
aayush, which tile do you want to slide? 3
+--+--+
| 2| 1|
+--+--+
| 3|  |
+--+--+
...
