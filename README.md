# Slot Machine Game

This is a simple command-line-based slot machine game implemented in Python. The game simulates a slot machine with 3 rows and 3 columns, where players can place bets on multiple lines and try to win based on symbol combinations.

## How to Play

1. Run the `main()` function to start the game.
2. Enter the initial deposit amount when prompted. The game will not start until a valid positive deposit amount is provided.
3. You can choose the number of lines to bet on (1 to 3) for each spin. Each line will have a separate bet amount.
4. Place your bet for each line. The bet amount must be between $1 and $100.
5. The slot machine will randomly generate symbols on each row of the 3x3 grid.
6. If any line contains the same symbol in all three columns, you win based on the symbol's value and the bet amount for that line.
7. The game will display the outcome of each spin, including any winnings and the line number(s) you won on.
8. You can continue playing as long as you have a positive balance. Press 'q' and then Enter to quit the game.

## Game Rules

- The maximum number of lines you can bet on is 3.
- The minimum and maximum bet amount allowed is $1 and $100, respectively.
- Each symbol has a predefined count and value. The count represents how many times a symbol appears in the slot machine, while the value determines the payout when you win.
- The game calculates the total bet based on the number of lines and the bet amount for each line. If the total bet is higher than your current balance, the game will not proceed, and you will be prompted to deposit more funds or quit the game.

## Code Organization

The code is organized into several functions:

- `deposit()`: Asks the player to deposit an initial amount before starting the game.
- `get_number_of_lines()`: Asks the player to choose the number of lines to bet on (1 to 3).
- `get_bet()`: Asks the player to choose the bet amount for each line (between $1 and $100).
- `spin(balance)`: Handles the game mechanics for each spin, including generating random symbols, calculating winnings, and updating the balance.
- `main()`: The main function that runs the game loop, allowing players to continue playing until they choose to quit.

## Customization

Feel free to customize the `symbol_count` and `symbol_value` dictionaries to change the game's symbols and their corresponding counts and values.

Enjoy playing the slot machine game! 🎰💰
