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
 (splat) 
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

#### Exercise III - Timing

 Practice converting inputs to appropiate types
 For empty you could use **if not run_time**

 print(f'{s:.2f} values)

```python
def run_timing():
    number_of_runs = 0
    total_time = 0
    while True:
        run_time = input("Enter 10 km run time: ")
        if not run_time:
            break
        number_of_runs += 1
        total_time += float(run_time)
    
    average_time = total_time / number_of_runs
    print(f"Average of {average_time}, over {number_of_runs} runs")

```

Exercise IV  Hexadecimal

`reversed` and `enumarate` are useful functions
Using `0x` prefix to convert to hexadecimal

```python
def hex_output():
    decnum = 0
    hexnum = input("Enter a hexadecimal number: ")
    for power, digit in enumerate(reversed(hexnum)):
        decnum += int(digit, 16) * (16 ** power)
    print(f"The decimal value of {hexnum} is {decnum}")
```
