# rockpaperscissors
import random

options = ["Rock", "Paper", "Scissors"]

def play_game():
    
    user_choice = input("Enter your choice (Rock, Paper, or Scissors): ")
    while user_choice not in options:
        user_choice = input("Invalid choice. Please enter Rock, Paper, or Scissors: ")

    
    computer_choice = random.choice(options)

  
    if user_choice == computer_choice:
        print("It's a tie!")
    elif user_choice == "Rock" and computer_choice == "Paper":
        print("Computer wins!")
    elif user_choice == "Rock" and computer_choice == "Scissors":
        print("You win!")
    elif user_choice == "Paper" and computer_choice == "Rock":
        print("You win!")
    elif user_choice == "Paper" and computer_choice == "Scissors":
        print("Computer wins!")
    elif user_choice == "Scissors" and computer_choice == "Rock":
        print("Computer wins!")
    elif user_choice == "Scissors" and computer_choice == "Paper":
        print("You win!")


play_game()
