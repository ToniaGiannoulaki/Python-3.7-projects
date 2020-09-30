"""
This program is basically the game rock, paper, scissors and the winner is the one who will complete 3 points first.
The battle is between you and the computer.
"""
from random import randrange

game = ['rock','paper','scissors']

players_counter = 0
computers_counter = 0

while True:

    # we need an index position of an item along with its value
    random_index = randrange(len(game))
    item = game[random_index]

    # first, we need to check our counter
    if computers_counter == 3 or players_counter == 3:
        break
    else:
        player= input("\nChoose: rock, paper or scissors ")

    # second, we need to check if the player's input is right
    if player not in game:
        print("Invalid input!Please Try again!")
    else:
        print("Computer chose: "+item)

    # and now, we check all the possible conditions
    if player == item:
        print("It's a tie")
        computers_counter += 1
        players_counter += 1
        print("\nComputer's points: "+ str(computers_counter) + "\nPlayer's points: "+ str(players_counter))

    elif player == "scissors" and item == game[0]:
        computers_counter += 1
        print("\nComputer won! Rock smashes the scissors\nComputer's points: "+ str(computers_counter) + "\nPlayer's points: "+ str(players_counter))

    elif player == "scissors" and item == game[1]:
        players_counter += 1
        print("\nYou won! Scissors cut the paper\nComputer's points: "+ str(computers_counter) + "\nPlayer's points: "+ str(players_counter))

    elif player == "paper" and item == game[0]:
        players_counter += 1
        print("\nYou won! Paper covers the rock\nComputer's points: "+ str(computers_counter) + "\nPlayer's points: "+ str(players_counter))

    elif player == "paper" and item == game[2]:
        computers_counter += 1
        print("\nComputer won! Scissors cut the paper\nComputer's points: "+ str(computers_counter) + "\nPlayer's points: "+ str(players_counter))

    elif player == "rock" and item == game[1]:
        computers_counter += 1
        print("\nComputer won! Paper covers the rock\nComputer's points: "+ str(computers_counter) + "\nPlayer's points: "+ str(players_counter))

    elif player == "rock" and item == game[2]:
        computers_counter += 1
        print("\nComputer won! Rock smashes the scissors\nComputer's points: "+ str(computers_counter) + "\nPlayer's points: "+ str(players_counter))

# Sources
# https://pynative.com/python-random-choice/
# https://stackoverflow.com/questions/51252580/how-to-resolve-typeerror-can-only-concatenate-str-not-int-to-str
