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

- Spacing around a code block (variables are together, can glance at the code and notice them)(space around a function, while loop, if-else block,)

## Commenting Properly

## Activities

**Activity #1:**

**Answer:**

**Activity #2:**

**Answer:**
