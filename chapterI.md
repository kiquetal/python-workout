#### Numeric types

  Exercise 1

  Number guessing game

 ```python

def guessing_number():
    guess = random.randint(1, 100)
    number = int(input("Enter a number: \n"))
    attempts = 1
    while number != guess and attempts < 3:
        if number > guess:
            print("Too high")
        else:
            print("Too low")
        number = int(input("Enter a number:\n"))
        attempts += 1
    if number == guess:
        print("You guessed it")
    else:
        print("You lost")



 ```
