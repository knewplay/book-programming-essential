---
title: "Chapter 7: Putting It All Together"
date: "2023-11-02"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - age-classifier: |
      Create a function that classifies a person based on their age. The function should take an age as a parameter and return whether they're a "Child", "Teen", "Adult", or "Senior". Then, ask the user for their age and use the function to display their age classification.
  - avg-calc: |
      Request the user to input three numbers. Compute the average of these numbers and display the result.
  - area-func: |
      Write three separate functions: RectangleArea(length, width), TriangleArea(base, height), and CircleArea(radius). Each function should calculate and return the area for its respective shape.
---

Now that we've gone over everything from breaking down problems to using data types, loops, and functions, it's time to put all these pieces together. In this chapter, we're going to combine everything you've learned and solve various problems.

## Table of Contents

[Arithmetic Operations in Programming](#arithmetic-operations-in-programming)

[Example Problems](#example-problems)

- [Example 1: Celsius to Fahrenheit Converter](#example-1-celsius-to-fahrenheit-converter)
- [Example 2: Even or Odd](#example-2-even-or-odd)
- [Example 3: A Basic Calculator](#example-3-a-basic-calculator)
- [Example 4: Guess the Secret Number](#example-4-guess-the-secret-number)

[Activities](#activities)

[Questions](#questions)

## Arithmetic Operations in Programming

When you think of math, the first things that probably come to mind are the basic arithmetic operations. In programming, these operations are just as essential. Let's dive into each of them:

- **\+** : Addition: `3 + 5 = 8`
- **\-** : Subtraction: `9 - 4 = 5`
- **\*** : Multiplication: `4 * 6 = 24`
- **/** : Division: `12 / 3 = 4`

## Example Problems

In this section, we're going to tackle a set of example problems that will take us back through everything we've learned so far. We'll start with simpler examples and gradually ramp up the challenge.

### Example 1: Celsius to Fahrenheit Converter

**Question:** Write a function that converts Celsius temperature to Fahrenheit. After creating this function, demonstrate its use by providing a test case.

![A thermometer](./figures/ch-7-thermometer.jpg)
*A thermometer displaying temperatures in both Celsius and Fahrenheit.*

**Answer:**

To solve this, it's important to understand the relationship between Celsius and Fahrenheit. To convert Celsius to Fahrenheit, you multiply the Celsius temperature by 9/5 and then add 32. In mathematical terms, the formula is: **Fahrenheit = (Celsius × 9/5) + 32**.

**Pseudocode:**

```typescript
function ConvertToFahrenheit(celsius):
    fahrenheit = celsius * 9/5 + 32
    return fahrenheit
END function
```

**Explanation:**

For the `ConvertToFahrenheit` function, the name itself gives away its purpose: to convert a given temperature from Celsius to Fahrenheit. Inside the parentheses, we have a parameter named `celsius`, which is the input temperature we want to convert. Within the function, we use a variable named `fahrenheit` to store the result of our conversion. The math behind this conversion is done using the formula `celsius * 9/5 + 32`, a standard way to change Celsius to Fahrenheit. After the calculation, the function then provides the converted temperature using the `RETURN` statement. Essentially, this function takes in a Celsius value, performs the necessary calculations, and then hands back the Fahrenheit equivalent.

**Function call:**

If we want to test this function, we could call it and pass it an argument, like so:

```typescript
ConvertToFahrenheit(10)
```

On execution, the call `ConvertToFahrenheit(10)` should yield a result of `50` Fahrenheit.

### Example 2: Even or Odd

**Question:** Design a function to identify whether a given integer is even or odd. Create the solution using loops, and afterwards, demonstrate the function with a test case.

**Answer:**

To figure out if a number is even or odd using loops, we'll subtract 2 from the number repeatedly until it becomes less than 2. If the result is 0, then the number is even; otherwise, it's odd.

**Pseudocode:**

```typescript
function IsEvenOrOdd(number):
    while number >= 2:
        number = number - 2

    if number == 0:
        return "Even"
    else:
        return "Odd"
END function
```

**Explanation:**

Think of it like this: if you had 7 apples and you kept giving 2 away at a time, you'd be left with 1 apple. Any time you have 1 apple left (or any number not evenly divisible by 2), that means you started with an odd number. On the other hand, if you kept giving away 2 apples at a time and ended up with none left, you had an even number of apples to start with.

In our loop, we kept subtracting 2 until the number became less than 2. If, after all the subtractions, the number is 0, that means the original number was even. If it's not 0, then it's surely 1. And that's why in our "else" condition, we can confidently say the number is odd.

**Function call:**

To test our function:

```typescript
IsEvenOrOdd(7)
```

Running the above code, `IsEvenOrOdd(7)` should output `Odd`.

### Example 3: A Basic Calculator

**Question:**

Write a program (no need for a function) that prompts the user for two numbers and then for an operation (+, -, *, /). Compute the result based on the given operation.

![A basic calculator](./figures/ch-7-calculator.jpg)
*A basic calculator.*

**Answer:**

We'll be collecting two numbers and an operation from the user. After receiving the inputs, we'll determine which arithmetic operation to perform using conditional statements and then display the result.

**Pseudocode:**

```typescript
PRINT "Enter first number: "
number1 = INPUT
PRINT "Enter second number: "
number2 = INPUT
PRINT "Enter operation (+, -, *, /): "
operation = INPUT

if operation == "+":
    result = number1 + number2
    PRINT result
else if operation == "-":
    result = number1 - number2
    PRINT result
else if operation == "*":
    result = number1 * number2
    PRINT result
else if operation == "/":
    result = number1 / number2
    PRINT result
else:
    PRINT "Unrecognized operation"
```

**Explanation:**

Absolutely! Here's the detailed explanation written as a cohesive paragraph:

In the given pseudocode, we first engage the user by prompting them to provide two numbers and an arithmetic operation. After printing a message asking for the first number, we store the user's input in a variable called `number1`. We follow the same process for the second number, saving it in `number2`. Moving on, we then ask the user to choose an arithmetic operation, and their choice is stored in the `operation` variable. With all our inputs gathered, we use conditional statements to decide which calculation to perform.

If the user selects "+", we compute the sum of the two numbers and store it in the `result` variable, which is then promptly printed to show the user their answer. Similarly, for "-", we subtract `number2` from `number1`, again saving and displaying the result using the same variable. For multiplication (denoted by "*"), the two numbers are multiplied, and for division ("/"), `number1` is divided by `number2`, with the outcomes stored in `result` and shown to the user. Lastly, if the operation input is anything other than the given four choices, a message is printed to inform the user that their chosen operation is not recognized.

### Example 4: Guess the Secret Number

**Question:**

Write a program where you store a secret number between 1 and 10 in a variable, and the user has to guess it. The user should be prompted to guess the number until they get it right. Create a function named Feedback to provide feedback on the user's guess. The function should take in the user's guess and the secret number as inputs and return whether the guess is too high, too low, or correct.

![Guess the number](./figures/ch-7-computer.jpg)
*What number is the computer thinking of?*

**Answer:**

We'll set a predefined secret number, and then use a `WHILE` loop to repeatedly ask the user for their guess. If they guess correctly, we'll exit the loop and congratulate them. If not, the `Feedback` function will provide feedback on their guess, and we'll prompt them to try again.

**Pseudocode:**

```typescript
function Feedback(guess, secret_number):
    if guess < secret_number:
        return "Your guess is too low."
    else if guess > secret_number:
        return "Your guess is too high."
    else:
        return "Congratulations! You've guessed the secret number."
END function

secret_number = 7
guess = 0

PRINT "Guess the secret number between 1 and 10."

while guess != secret_number:
    PRINT "Enter your guess:"
    guess = INPUT
    message = Feedback(guess, secret_number)
    PRINT message
END while
```

**Explanation:**

At the start of the program, the `Feedback` function is defined, ensuring its availability for later use. This doesn't mean the function runs immediately; it simply tells the computer what to do when the function is called later. The actual execution begins with setting the `secret_number` and initializing `guess`. Initializing `guess` with a value, in this case 0, is essential because it provides a starting value that ensures the `WHILE` loop condition is checked properly on the first run. Without initializing `guess`, the program wouldn't know what to compare `secret_number` to during the initial check, which could lead to an error or unintended behavior. The program then prompts the user to guess the secret number. The `WHILE` loop comes into play next; it keeps asking the user for their guess as long as the guess doesn't match the secret number. Within this loop, the `Feedback` function provides hints based on the user's input: if the guess is low, it informs the user to guess higher, and if it's high, it advises guessing lower. Once the correct number is guessed, the loop is exited, and the user is congratulated.

Now why does the program exit the loop once the correct number is guessed? That's because if the user guesses that the secret number is `7`, then when it's time to reevaluate the loops' condition of `guess != secret_number`, we will have `guess = 7` and `secret_number = 7`, meaning that the statement `guess != secret_number` is False (since "*7 is not equal to 7*" is False).

**Example of Execution:**

Imagine a user interacting with the program:

```text
Guess the secret number between 1 and 10.
Enter your guess:
3
Your guess is too low.
Enter your guess:
8
Your guess is too high.
Enter your guess:
7
Congratulations! You've guessed the secret number.
```

In this execution:

- The user first guessed the number 3, which is too low. The program provides feedback accordingly.
- The user then guessed the number 8, which is too high. Again, the program provides feedback.
- Finally, the user guessed 7, which matches the secret number. The program congratulates the user, and the loop exits.

## Activities

**Activity #1:**

In "Chapter 6: Modularizing Your Code with Functions", we explored an airplane manufacturing plant. One of the divisions of this plant is the "Engine Installation".

![Engine](./figures/ch-7-engine.jpg)
*An airplane engine.*

This division is given the wings of the plane and told how many engines it must install in total.

Design a function that represents the process adopted by the engine installation team.

**Answer:**

```typescript
function InstallEngines(wings, numberOfEngines):
    enginesInstalled = 0
    enginesPerWing = numberOfEngines / 2

    while enginesInstalled < numberOfEngines:
        if enginesInstalled == enginesPerWing + 1:
            switch_to_other_wing
        install_engine // Steps to install engine
        enginesInstalled = enginesInstalled + 1
    END while
    
    return "Engine Installation Complete"
END function
```

1. **Function Declaration:** The algorithm starts with the declaration of the `InstallEngines` function. This function models the procedure of attaching engines to an airplane's wings. It accepts two parameters: `wings`, symbolizing the airplane's wings, and `numberOfEngines`, indicating the total number of engines to be installed.
2. **Initializing Variables:** Initially, a counter `enginesInstalled` is set to zero, serving as a tracker for how many engines have been placed. Additionally, `enginesPerWing` calculates the number of engines each wing should ideally hold by dividing the total number of engines by two.
3. **WHILE Loop:** The function then enters a `WHILE` loop, continually installing engines until the desired number, `numberOfEngines`, is met.
    - **Midpoint Check:** The program checks if the current iteration, `enginesInstalled`, is equal to half the total number of engines plus one (`enginesPerWing + 1`, which is the same as `numberOfEngines/2 + 1`). This check determines the midpoint in the engine installation process. When the loop reaches this midpoint, it signifies that half of the engines have already been installed on one wing, and it's time to switch to the other wing. The `switch_to_other_wing` action is then executed, although the specific steps of this action aren't detailed in the provided pseudocode.
    - **Engine Installation:** Immediately after the conditional check (and potentially switching wings), the `install_engine` action is executed. This action represents the actual process of installing an engine. Again, the specific steps to "install an engine" are abstracted away in this snippet and are represented by the comment: // Steps to install each engine.
    - **Counter Increment:** Once `install_engine` is executed, the program then increments the `enginesInstalled` counter.
4. **Function Conclusion:** Once the `WHILE` loop is exited, the function confirms the completion of the installation by returning "Engine Installation Complete".

**Activity #2:**

A local gym wants to implement a promotional discount for its members based on their age and the duration of their membership. They have the following rules:

- Teenagers (younger than 20 years old) who are just about to sign up (0 years of membership) receive a 10% discount.
- Elderly members (55 years and older) who have been a member of the gym for 5 or more years receive a 15% discount.

![Treadmill](./figures/ch-7-thermometer.jpg)
*A treadmill.*

Design a pseudocode algorithm that calculates and displays the eligible discount for a member based on their age and membership duration.

**Answer:**

```typescript
function CalculateDiscount(age, membershipDuration):
    discount = 0

    if age < 20 AND membershipDuration == 0:
        discount = 10
    else if age >= 55 AND membershipDuration >= 5:
        discount = 15
    END if

    return discount
END function

// Main Program
PRINT "Enter your age: "
INPUT age

PRINT "Enter number of years you've been a member: "
INPUT membershipDuration

discountPercent = CalculateDiscount(age, membershipDuration)

PRINT "You are eligible for a " + discountPercent + "% discount!"
```

1. **Function Declaration:** The algorithm starts with the declaration of the CalculateDiscount function. This function takes two parameters: the age and membership duration of a gym member.
2. **Initializing Discount:** Within the function, the discount is initialized to 0%. This ensures that if none of the conditions are met, no discount is given.
3. **Conditional Checks:**
    - The first condition checks if the user's age is less than 20 (meaning they're a teenager) AND they have 0 years of membership. If both these conditions are true, the discount is set to 10%.
    - The next condition, an `ELSE IF`, checks if the user's age is 55 or above (elderly) AND they've been a member for 5 or more years. If both these conditions are satisfied, the discount is set to 15%.
    - These conditions use the logical AND (`AND`) operator, ensuring that both parts of each condition must be true for the discount to be applied.
4. **Return Discount:** The function then returns the determined discount value.
5. **Main Program:** After the function is defined, the main program begins by prompting the user to enter their age followed by the number of years they've been a member of the gym.
6. **Function Call:** The `CalculateDiscount` function is then called with the provided age and membership duration, and the result is stored in the discountPercent variable.
7. **Displaying the Result:** Finally, the program displays the discount the user is eligible for using the `PRINT` statement.
