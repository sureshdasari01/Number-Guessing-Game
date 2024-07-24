# Number-Guessing-Game
Enjoy a fun guessing game with computer hints for added excitement.
Here's a simple Python guessing game where the computer gives hints to make it more exciting. The game will prompt the user to guess a number between 1 and 100, and the computer will provide hints such as "Too high" or "Too low" to guide the user.

python
import random

def guessing_game():
    print("Welcome to the Guessing Game!")
    print("I'm thinking of a number between 1 and 100.")
    
    number_to_guess = random.randint(1, 100)
    attempts = 0
    
    while True:
        guess = input("Take a guess: ")
        
        if not guess.isdigit():
            print("Please enter a valid number.")
            continue
        
        guess = int(guess)
        attempts += 1
        
        if guess < number_to_guess:
            print("Too low!")
        elif guess > number_to_guess:
            print("Too high!")
        else:
            print(f"Congratulations! You guessed the number in {attempts} attempts.")
            break

if __name__ == "__main__":
    guessing_game()
Explanation
import random: This imports the random module, which we use to generate a random number.
guessing_game(): The main function that contains the game logic.
The computer generates a random number between 1 and 100.
The game continues in a loop until the user guesses the correct number.
The user is prompted to enter a guess.
The computer checks if the guess is too low, too high, or correct and provides the appropriate hint.
If the guess is correct, the game congratulates the user and displays the number of attempts.
if name == "main": This ensures that the game runs only when the script is executed directly, not when it's imported as a module.
Running the Program
Save the code to a file, for example, guessing_game.py.
Open a terminal or command prompt.
Navigate to the directory where you saved guessing_game.py.
Run the program by typing python guessing_game.py.
This game is a fun and interactive way to practice Python programming and familiarize yourself with loops, conditionals, and user input handling.






