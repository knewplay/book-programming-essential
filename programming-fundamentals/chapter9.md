---
title: "Chapter 9: Best Practices and Readability"
date: "2023-11-08"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - q1-tag: |
      Q1 text
  - q2-tag: |
      Q2 text
  - q3-tag: |
      Q3 text
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

## Commenting Properly

## Activities

**Activity #1:**

**Answer:**

**Activity #2:**

**Answer:**
