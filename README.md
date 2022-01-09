# Fortune Teller

## To Run This Application

- `git clone` the app
- `cd` into the application
- `npm install` to install the dependencies

### Working with the Application

- `npm test` will run your tests
- `npm start` will spin up the application


# Fortune Teller

## Overview

Develop a console application that will tell the user’s fortune based on data received from the user.

## Skills Required

- Variables and Basic Types
- Operators and Expressions
- Conditionals
- Strings

## Tasks

### Part 1

- [ ] Ask the user for the user’s first name.
- [ ] Ask the user for the user’s last name.
- [ ] Ask the user for the user’s age.
- [ ] Ask the user for the user’s birth month (as an 'int').
- [ ] Ask the user for the user’s favorite ROYGBIV color.
  - [ ] If the user does not know what ROYGBIV is, ask the user to enter “Help” to get a list of the ROYGBIV colors.
- [ ] Ask the user for the user's number of siblings.

### Part 2

For each of the below, you will select your own value for each condition. The table will give the conditions and an example for each. Don't steal our examples—be creative!

#### Retirement Years

The user's number of years until retirement will be based on whether the user's age is odd or even.

| _(condition)_ If the user's age is… | _(example)_ then the user will retire in… |
| ----------------------------------- | ----------------------------------------- |
| odd                                 | _14_ years                                |
| even                                | _12_ years                                |

#### Vacation Home Location

The location of the user's vacation home will be based on how many siblings the user has. If the user enters a number less than zero, give the user a _bad_ location!

| _(condition)_ If the user's number of siblings is… | _(example)_ then the user's vacation home will be in… |
| -------------------------------------------------- | ----------------------------------------------------- |
| 0                                                  | Boca Raton, FL                                        |
| 1                                                  | Nassau, Bahamas                                       |
| 2                                                  | Ponta Negra,Brazil                                    |
| 3                                                  | Portland, Oregon                                      |
| greater than three                                 | Baton Rouge, LA                                       |
| less than zero                                     | Chernobyl, Ukraine                                    |

#### Mode of Transportation

The user's mode of transportation will determined by the user's favorite color.

| _(condition)_ If the user's favorite color is… | _(example)_ then the user's mode of transportation will be… |
| ---------------------------------------------- | ----------------------------------------------------------- |
| red                                            | Maserati                                                    |
| orange                                         | stallion                                                    |
| yellow                                         | chariot                                                     |
| green                                          | taxi                                                        |
| blue                                           | rickshaw                                                    |
| indigo                                         | motor scooter                                               |
| violet                                         | flying saucer                                               |

#### Bank Balance

The user's bank balance at retirement will be based on the user's birth month. If the user enters something other than 1-12 for birth month, the user's balance will be \$0.00.

| _(condition)_ If the user's birth month is… | _(example)_ The user's balance will be… |
| ------------------------------------------- | --------------------------------------- |
| 1-4                                         | \$256,000.76                            |
| 5-8                                         | \$3,687,105.42                          |
| 9-12                                        | \$86.23                                 |
| anything else                               | \$0.00                                  |

### Part 3

Display the user's fortune in this format:

    *[First Name]* *[Last Name]* will retire in *[# of years]* with *[bank balance]* in the bank,
    a vacation home in *[location]*, and travel by *[mode of transportation]*.

Your program should be able to process input whether a user enters capital or lowercase letters.

## Stretch Tasks (Optional)

- [ ] Give the user the ability to quit the program by typing "Quit" (should not be case sensitive) at any point where the program is looking for user input. The program should print “Nobody likes a quitter...” before ending. - _Tip_: To do this with the prompts that expect an integer, you will need to read in a `String`, check for "Quit", then _"parse the string to an int"_ (google it!) to convert the user input string to an `int`.
- [ ] Research `while` or `do/while` loops and use them to check whether a user typed "Help" for favorite color, printing the list of colors each time the user types "Help".

      	```bash
      	What is your favorite ROYGBIV color?
      	Help
      	The ROYGBIV colors are red, orange, yellow, green, blue, indigo, violet.
      	Help
      	The ROYGBIV colors are red, orange, yellow, green, blue, indigo, violet.
      	Blue
      	```
