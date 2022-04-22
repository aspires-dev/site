

# Number Guessing game


Import the libraries
```{python}
import random
```

Menu - display options to user.
```{python}
print("Welcome to the number guessing game.")
print("Guess the number im thinking of.")
print("you will be givent clues after your first guess.")
print("I have thought of a number from 1 - 100.\n")
```

Generate secret number
```{python}
secretnumber = random.randint(1,100)
```

Input Validation - check that the input is a intager.
```{python}
  while True:
    try:
       userInput = int(input(message))       
    except ValueError:
       print("Not an integer! Try again.")
       continue
    else:
       return userInput 
       break
  ```

Number checker - check guess against generated number.
```{python}
    input = inputNumber("Input your guess!\n")
    print("Guess is", input)
    if input < secretnumber:
        print("Guess too low")
        main()
    elif  input > secretnumber:
        print("Guess too high")
        main()
    elif input == secretnumber:
        print()
```

Main loop - run the 'main' subroutine
```{python}
main()
```
