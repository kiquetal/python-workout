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

#### Formatting text

Using f" templates to format text

```python
 name = f"Hello {name}"
```

#### Exercise II

 Using *args, to receive an arbitrary number of arguments

 you can call a list with a prefix *
 sum(*[1,2])

```python

def sum(*args):
    total = 0
    for arg in args:
        total += arg
    return total

```

