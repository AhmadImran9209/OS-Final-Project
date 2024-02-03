Potion Explosion Game
This is a text-based implementation of the Potion Explosion game in C, incorporating concepts from Operating Systems. In this game, players simulate the process of creating magical potions by combining different ingredients.

How to Play
1. Run the program.
2. Enter the number of players.
3. Players take turns choosing ingredients to form potions.
4. Each potion requires specific ingredients, and players need to collect them strategically.
5. The game continues until a player successfully creates a predefined number of potions.

OS Concepts Integration
The game utilizes various OS concepts, including:
- **Processes**: Each player's turn is handled as a separate process.
- **Synchronization**: Proper synchronization mechanisms are employed to avoid conflicts when multiple players try to access shared resources simultaneously.
- **File I/O**: Player and game data are stored and retrieved using file I/O operations.

Features
- Multiple players can play the game.
- Players can select ingredients strategically to form potions.
- The game keeps track of each player's progress and the overall state of the potion laboratory.

Code Structure
The code is organized into functions for different tasks:
- `initGame()`: Initializes the game, sets up necessary data structures, and spawns player processes.
- `playerTurn()`: Handles a player's turn, allowing them to select ingredients and attempt to create a potion.
- `checkPotion()`: Verifies if a player has successfully created a potion.
- `cleanup()`: Releases resources and concludes the game.

How to Compile
Compile the program using a C compiler. For example:

```bash
gcc potion_explosion.c -o potion_explosion -pthread
How to Run
Run the compiled program:

bash
Copy code
./potion_explosion
Example Gameplay
Here's an example of how the game looks during gameplay:

[Game Board State]

Ingredients:
A: 3
B: 2
C: 1
...

Player 1's turn:
Choose ingredient (A/B/C): A
Choose quantity: 2

...

Potion created by Player 1: Healing Elixir!

Player 1 wins!
