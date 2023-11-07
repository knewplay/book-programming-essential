---
title: "Chapter 9: Best Practices and Readability"
date: "2023-11-08"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - function-use: |
      When might you choose to create a function in your code instead of writing out the steps each time? Can you think of an example from a game or an app?
  - commenting: |
      3. What's the difference between a comment that is helpful and one that is unnecessary? Provide examples.
  - logical-segmentation: |
      What does "logical segmentation" mean in the context of writing code, and why is it helpful?
---

When writing code, it's important not just to make it work, but also to make it readable and maintainable for others (and your future self). This chapter will guide you through the best practices to achieve clean, understandable code.

## Table of Contents

[Some Review: Descriptive Names](#some-review-descriptive-names)

[Code Structure and Formatting](#code-structure-and-formatting)

- [Spacing and Indentation](#spacing-and-indentation)
- [Organizing Variables](#organizing-variables)
- [Logical Segmentation](#logical-segmentation)
- [Avoiding Deep Nesting](#avoiding-deep-nesting)
- [Using Functions to Reduce Repetition](#using-functions-to-reduce-repetition)

[Commenting Properly](#commenting-properly)

- [Bad Commenting Examples](#bad-commenting-examples)
- [Good Commenting Examples](#good-commenting-examples)

[Activities](#activities)

[Questions](#questions)

## Some Review: Descriptive Names

In some of the previous chapters, we've touched upon some good coding practices already, notably that of providing clear and descriptive names to functions and variables.

Good naming is like giving clear, easy-to-follow instructions. When naming functions, we use verbs to describe actions, making it obvious what the function does. So is this good enough?

```typescript
FUNCTION DoThing()
    ...
END FUNCTION
```

No, because what this function does just by looking at its name is anyone's guess. Now just to understand what the function does, we'd have to go inside the function and try to understand the code.

Instead, you should call it something like:

```typescript
FUNCTION CalculateTotalScore()
    ...
END FUNCTION
```

Now, we're not forced to read the code inside this function to understand what it does; we can simply read its name.

When it comes to variables, the names should reflect their content or purpose as well. For instance:

```typescript
playerScore = 0
```

This variable clearly represents the player's score.

> Note: In our made up pseudocode programming language, we have function names follow the `P`ascal`C`ase notation, and variables follow either camel`C`ase or snake`_`case, making sure to stay consistent throughout your code.

## Code Structure and Formatting

How you structure and format your code can greatly influence how easy it is to read and maintain. Here's how to keep your code looking neat and organized:

### Spacing and Indentation

Just like paragraphs in a story, code needs to be organized with proper spacing and indentation to tell the computer (and our friends) what steps to follow and in what order. Indentation helps to show which pieces of code are connected. For example, everything inside a loop should be indented one level deeper:

```typescript
FUNCTION PrepareTea(numOfGuests)
    i = 0
    WHILE i < numOfGuests:
        AddWater()
        SteepTea()
    END WHILE
END FUNCTION
```

Notice how the actions inside the for loop (adding water and steeping the tea) are indented, showing they are part of the looping action.

### Organizing Variables

Think of variables like ingredients in a recipe. You want to lay them all out before you start cooking. By grouping related variables at the start, you make your "recipe" easier to follow. Here's an example:

```typescript
FUNCTION BakeCake()
    eggs = 3
    sugar = "1 cup"
    flour = "2 cups"
    
    MixIngredients(eggs, sugar, flour)
    PourBatter()
    Bake()
END FUNCTION
```

All the "ingredients" are listed at the top, so it's clear what we need to bake the cake.

### Logical Segmentation

When writing a story, we use paragraphs to separate ideas; in coding, we use blank lines to break up our code into sections. Each part does something different, like setting up the game, playing a round, or ending the game:

```typescript
FUNCTION PlayGame()
    SetupGame()

    WHILE not gameOver
        PlayRound()
    END WHILE
    
    EndGame()
END FUNCTION
```

### Avoiding Deep Nesting

When we write stories, if we have too many stories within stories, it can become confusing. Similarly, in programming, having too many loops or conditions inside of each other (nested) can make code hard to follow. Try to keep things simple:

```typescript
// Try to avoid this
IF conditionA
    IF conditionB
        IF conditionC
            // Code here is deeply nested 
            //and harder to read.
        END IF
    END IF
END IF


// Better approach
IF conditionA AND conditionB AND conditionC
    // Code here is easier to understand.
END IF
```

### Using Functions to Reduce Repetition

Just like we don't want to repeat the same story over and over again, we don't want to write the same code repeatedly. If you're doing the same thing in multiple places, consider making a function for it:

```typescript
// Instead of this
IF conditionA
    AddSugar()
    AddFlour()
    Mix()
END IF

IF conditionB
    AddSugar()
    AddFlour()
    Mix()
END IF

// Do this
FUNCTION MakeMixture()
    AddSugar()
    AddFlour()
    Mix()
END FUNCTION

IF conditionA
    MakeMixture()
END IF

IF conditionB
    MakeMixture()
END IF
```

## Commenting Properly

While not strictly part of the code's functionality, comments are part of the overall structure. Use them to explain why you're doing something, not what you're doing (which should be clear from the code itself). Over-commenting with obvious information can clutter the code, while under-commenting can leave readers puzzled.

### Bad Commenting Examples

```typescript
// Bad: States the obvious
counter = 0 // Set counter to zero

// Bad: Explains 'how' instead of 'why', which should be evident from the code
FUNCTION addNumbers(a, b)
    // Add a and b and return the sum
    RETURN a + b
END FUNCTION

// Bad: Comment is redundant because the code is self-explanatory
IF temperature >= 100
    // If temperature is greater than or equal to 100, print 'It's very hot!'
    PRINT "It's very hot!"
END IF
```

### Good Commenting Examples

```typescript
// Good: Explains why a specific value is chosen
maxLoginAttempts = 3 // Limit attempts to prevent brute force attacks

// Good: Describes the purpose of a complex function
FUNCTION calculateOptimalPath()
    // Finds the quickest route through the network.
    ...
END FUNCTION

// Good: Clarifies the reason behind a particular logic choice
IF temperature < 0
    // Check for sub-zero temperatures to trigger the anti-freeze protocol
    activateAntiFreeze()
END IF
```

## Activities

**Activity #1:**

Here’s a snippet of code where everything is jumbled together. Can you reorganize it using proper spacing and indentation?

```typescript
FUNCTION MakePizza(topping1,topping2)
dough = 'wheat'
AddToPan(dough)
AddToPan(topping1)
AddToPan(topping2)
ovenTemp = 475
Bake(ovenTemp)
END FUNCTION
```

**Answer:**

When making a pizza in code, just like in the kitchen, organization is key. You gather your ingredients, prepare your dough, add the toppings, and finally, bake your pizza to perfection. Let's take this step-by-step approach to our `MakePizza` function:

```typescript
FUNCTION MakePizza(topping1,topping2)
    // Prepare the base ingredients
    dough = 'wheat'
    ovenTemp = 475
    
    // Start the pizza-making process
    AddToPan(dough)
    AddToPan(topping1)
    AddToPan(topping2)
    
    // Bake the pizza at the desired temperature
    Bake(ovenTemp)
END FUNCTION
```

With the ingredients and steps laid out clearly, anyone reading this code will understand the process of making a pizza. The comments provide additional context, making the function accessible even for those who might be new to coding.

**Activity #2:**

Here’s a long piece of code that repeats the same steps several times. Can you create a function to avoid repetition and make the code cleaner?

```typescript
Display("Welcome, playerone!")
// ...
// 10 more lines of code for setting up the game for user "playerone". 
// These might include initializing scores, setting positions, etc.

Display("Welcome, zombieXZ!")
// ...
// Same 10 lines of code for setting up the game for user "zombieXZ" 

Display("Welcome, IronHeart007!")
// ...
// Same 10 lines of code for setting up the game for user "IronHeart007"
```

**Answer:**

We want to make a function that handles the setup process for a player. This way, we can call the same function for all players without repeating those 11 (the `PRINT` as well as the 10 other lines) lines of code. Here's how you might structure that function and call it for all players:

```typescript
FUNCTION SetUpGame(player)
    Display("Welcome, " + player + "!")
    // ...
    // 10 more lines of code for setting up the game for a player
    // These might include initializing scores, setting positions, etc.
END FUNCTION

// Call the function for each player
SetUpGame("playerone");
SetUpGame("zombieXZ");
SetUpGame("IronHeart007")
```

This setup not only simplifies your code, making it easier to read and maintain, but also makes your game setup more flexible. If you wanted to add 100 more players or change the setup process, you'd only need to update it in one place.
