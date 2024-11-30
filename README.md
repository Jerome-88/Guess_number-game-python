import random

print("Welcome to the Number Guessing Game!\nI'm thinking of a number between 1 and 100.\nYou have 5 chances to guess the correct number.")
print("Please select the difficulty level:\n1. Easy (10 chances)\n2. Medium (5 chances)\n3. Hard (3 chances)")
a=int(input("Enter your choice: "))
b = random.randint(1,100)
if a==1:
    print("Great! You have selected the Easy difficulty level.\nLet's start the game!")
    for i in range(10):
        user=int(input("Enter your guess: "))
        if(user<b):
            print(f"Incorrect! The number is greater than {user}.")
        elif(user>b):
            print(f"Incorrect! The number is less than {user}.")
        else:
            print(f"Congratulations! You guessed the correct number in {i} attempts.")
elif a==2:
    print("Great! You have selected the Medium difficulty level.\nLet's start the game!")
    for i in range (5):
        user=int(input("Enter your guess: "))
        if(user<b):
            print(f"Incorrect! The number is greater than {user}.")
        elif(user>b):
            print(f"Incorrect! The number is less than {user}.")
        else:
            print(f"Congratulations! You guessed the correct number in {i} attempts.")
else:
    print("Great! You have selected the Hard difficulty level.\nLet's start the game!")
    for i in range (3):
        user=int(input("Enter your guess: "))
        if(user<b):
            print(f"Incorrect! The number is greater than {user}.")
        elif(user>b):
            print(f"Incorrect! The number is less than {user}.")
        else:
            print(f"Congratulations! You guessed the correct number in {i} attempts.")

