# ! /usr/bin/env python3
# Author: Sabrina Hossain, Sahil Blayson, Hil Patel, Jugal Gajjar


# importing the random module

import random

# Listing options available for the computer
# Taking input from a user using the variable user_option
# Choosing an random option by the computer

player_option = input("Please enter an appropriate choice (rock, paper or scissors): ")

options = ["rock", "paper", "scissors"]
computerOption = random.choice(options)

# Adding the print statement to guide the user from the beginning to the end of the game

# Using print to illustrate the user and computer options
print("The user chose: " + player_option)
print(" The computer chose: " + computerOption)

# Using a if/else/else block to illustarte comparison of the user playing and to find a potential winner in this game.

# If condition if the both the players chose the same option.
if player_option == computerOption:
	print("Both the playeres have selected the option. " + player_option + "The game has been declared as a tie!")

# The condition where player choses paper and computer choses rock.
elif player_option == "paper":
	if computerOption == "rock":
		print("Yeah, the paper will envelop the rock. The player will win!!!")
	else:
		print("The scissors will tear the paper. The player will lose!!!")

# The condition where player choses scissors and computer choses paper.
elif player_option == "scissors":
	if computerOption == "paper":
		print("The scissors will cut the paper. The player will win!!!")
	else:
		print("The rock will crush the scissors. The player will lose!!!")

# The condition where player choses rock and computer choses scissors.
elif player_option == "rock":
	if computerOption == "scissors":
		print("The rock will crush the scissors. The player will win!!!")
	else:
		print("The paper will envelop the rock. The player will lose!!!")

