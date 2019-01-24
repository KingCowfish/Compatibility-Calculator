# Compatibility-Calculator
# My first real project.  A basic calculator to determine the compatibility between two people.

import random
print("Welcome to the Compatibility Calculator!")
print("Here you will learn how suitible you and your crush are for one another!")

user_name = input("To begin, please tell us your first and last name: ")
user_crush = input("Now what is your crush's first and last name? ")

difference = abs(len(user_name) - len(user_crush))

if difference == 0:
    print("You and your crush are " + str(random.randint(80,100)) + "% compatible!")
    print("Go make a move!")
elif difference == 1 or 2:
    print("You and your crush are " + str(random.randint(50,79)) + "% compatible!")
    print("Maybe play it cool for a little while and see how things shake out.")
elif difference == 3 or 4:
    print("You and your crush are " + str(random.randint(30,49)) + "% compatible!")
    print("Doesn't seem like the stars are aligned for you two.")
elif difference >= 5:
    print("You and your crush are " + str(random.randint(0,29)) + "% compatible!")
    print("Yea, go ahead and give that one a miss.")
else:
    print("It appears that you missed a step.  Please start over.")
