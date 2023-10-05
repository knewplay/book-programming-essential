---
title: "Chapter 3: Logic and Decision Making"
date: "2023-10-05"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - ["plant", "You're creating an automatic plant watering system. The plant should be watered if:

- The soil is dry.
- It's daytime.

Write pseudocode to determine whether the plant should be watered or not."]
  - ["alarm", "You're building an alarm system for your home. The alarm should sound if:

- A window or door is opened.
- The system is armed.

Write pseudocode for this scenario."]
  - ["grade","Design a program that categorizes a student's grade. The program should:

- Display \"Excellent\" for scores 90 and above.
- Display \"Good\" for scores between 70 and 89.
- Display \"Average\" for scores between 50 and 69.
- Display \"Fail\" for scores below 50.

Write the corresponding pseudocode to determine and display the student's category based on the score."]
---

In our everyday lives, we make countless decisions based on conditions: if it rains, take an umbrella; if it's cold, wear a jacket. Similarly, in programming, decision-making is a crucial aspect, enabling the program to react differently to different inputs or situations.

## Table of Contents

[A Brief Review of Transistors](#a-brief-review-of-transistors)

- [The Binary Nature of Transistors](#the-binary-nature-of-transistors)
- [Connecting Transistors to Programming: Boolean Values](#connecting-transistors-to-programming-boolean-values)

[Introducing Pseudocode and Decision-Making in Programs](#introducing-pseudocode-and-decision-making-in-programs)

- [Comparison Operators](#comparison-operators)
- [Logical Operators](#logical-operators)

[From Math to Everyday Decisions](#from-math-to-everyday-decisions)

[Practical Problems](#practical-problems)

[Questions](#questions)

## A Brief Review of Transistors

Imagine a tiny switch, so small that millions of them could fit on the tip of your finger. This is a transistor. It's a device that can either allow an electric current to flow through it (like turning on a light) or stop it entirely (like turning the light off).

In essence, a transistor has two primary states:

- On: This is when it allows electricity to pass through. We can liken this to opening a faucet and letting water flow.
- Off: This is when it prevents electricity from flowing, similar to closing a faucet to stop the water.

### The Binary Nature of Transistors

The fact that a transistor has only two states introduces us to a fundamental concept: "binary." In the realm of computers, binary refers to the system of representing values using only two symbols, usually 0 and 1. In the case of our transistor, "on" can be thought of as "1", and "off" as "0".

> Note: The term 'binary' focuses on two states. In contrast, "unary" describes one state, "ternary" represents three states, and "quadrinary" means four states. However, computers primarily use binary logic because of the inherent on/off nature of electrical circuits and transistors.

### Connecting Transistors to Programming: Boolean Values

When you start programming, you'll encounter a concept called "boolean values." Named after George Boole, a 19th-century mathematician, booleans in programming have just two values: "True" and "False".

Do you see the parallel? Just as a transistor can be "on" (1) or "off" (0), a boolean value can be "True" (equivalent to 1) or "False" (equivalent to 0).

To grasp the significance of booleans, think about how we evaluate statements in our daily life. For instance, the statement "The sky is blue" can be **true** during a clear day, but **false** during the night. Similarly, in programming, boolean values emerge from evaluating conditions or statements.

> Note: A statement is a sentence or expression that can be evaluated as either true or false, but not both. In programming, statements provide a way to represent facts or conditions that the computer can then use to make decisions.

Take the example "5 is greater than 4." When a computer processes this statement, it evaluates the condition and concludes it to be "True." In contrast, the statement "6 is greater than 4 and less than 3" is contradictory, and thus, it evaluates to "False."

Programming uses this true or false approach for decision-making. And it all circles back to transistors—the link between the physical (transistors) and the logical (booleans).

## Introducing Pseudocode and Decision-Making in Programs

Pseudocode is a method to design and represent algorithms without the strict structure of a particular programming language. It allows programmers to focus on logic and flow, without worrying about the syntax of any specific programming language.

An integral part of pseudocode, and programming in general, is decision-making. This is achieved using specific patterns or templates known as constructs.

> Note: In programming, a "construct" is a fundamental piece or feature of the language that serves a building block. Constructs provide a way to introduce structure, repetition, decision-making, and more into our code.

For decision-making, common constructs are **if**, **else**, and **else if** (or 'else-if' or 'elif').

### Comparison Operators

Before delving into the pseudocode, let's familiarize ourselves with some basic comparison operators used in decision-making:

- **\>** : Greater than.
  - 5 > 3 is a true statement because 5 is greater than 3.
  - 2 > 8 is a false statement because 2 is not greater than 8.
- **<** : Less than.
  - 2 < 4 is a true statement because 2 is less than 4.
  - 6 < 3 is a false statement because 6 is not less than 3.
- **==** : Equal to.
  - 7 == 7 is a true statement because both sides of the operator have the same value.
  - 5 == 8 is a false statement because 5 is not equal to 8.

> Note: We use "==" to check for equality in most programming languages instead of "=". The reason for this will become clearer later when you dive into actual coding. For now, remember to use "==" when making comparisons.

These operators help us compare values and determine the relationship between them. They're fundamental to setting up conditions in our code.

### Logical Operators

Beyond simple comparisons, we often need to check multiple conditions at once or invert the logic of a condition. This is where logical operators come in. The three primary logical operators are **and**, **or**, and **not**.

- **and** : Both conditions must be true.
  - The statement "5 > 3 and 6 > 4" is true because both individual conditions are true.
  - However, "5 > 3 and 6 < 4" is false because, even though the first condition is true, the second is false.
- **or** : At least one condition must be true.
  - The statement "5 > 3 or 6 < 4" is true because at least one of the conditions (the first one) is true.
  - "2 < 1 or 3 < 2" is false because both conditions are false.
- **not** : Inverts the truth value of the condition.
  - If we have a statement like "5 > 3", its truth value is true. Using **not** inverts this, making the statement "not(5 > 3)" false.
  - Similarly, for the statement "2 > 3" which is false, "not(2 > 3)" will be true.

These operators allow for more complex conditions and evaluations. For instance, imagine you're programming a system that checks if a user is allowed to view a specific piece of content. You might have conditions like:

- The user must be logged in **and** the user must have a premium subscription.
- The content must be available in the user's region **or** the user has a "global pass".

Using logical operators like **and** and **or** lets us create these multifaceted conditions to guide decision-making in our programs. They provide the flexibility and nuance to mirror real-world decisions within the digital realm of programming.

## From Math to Everyday Decisions

Until now, our examples have primarily focused on numbers. However, programming isn't confined to mathematical operations. Often, the conditions we evaluate are abstract, representing real-world scenarios. The logical structure remains consistent, regardless of whether you're comparing numbers or determining whether it's raining.

For instance:

**Mathematical comparison**: 5 > 3 evaluates to True because 5 is, indeed, greater than 3.

**Real-world condition:** *'raining'* might be a variable in our program representing whether it's raining or not. If it's raining, *'raining'* is **True**; if not, *'raining'* is False. Another variable, *'temperature'*, could represent the current temperature.

> Note: Think of these variables as containers. Instead of always having a fixed value, like the number 5, they can hold different values at different times. For instance, today the variable *'raining'* might be True, but tomorrow it might be False. Similarly, *'temperature'* could be 25°C today and 23°C the next day. The term "variable" essentially means something that can "vary" or change.

In both cases, the underlying principle is evaluating the accuracy or truthfulness of a statement or condition.

When programming real-world applications, we use variables like *'raining'* or *'temperature'* to symbolize and manage real-world data. Our decision-making constructs and logical operators interact with these variables in the same way they would with pure numbers.

<!-- [4-part Illustration: 1. 3>2 (True), 2. 4>4 (False), 3. raining (True), 4. not raining (False)] -->

This dynamic nature of variables lets our programs react and make decisions based on the current situation or data, whether that data represents numbers, weather conditions, user inputs, or any other conceivable scenario.

With this understanding, we can now delve into real-world problems like deciding whether to hold an outdoor event based on the weather forecast.

## Practical Problems

**Problem 1:**

Write a program that evaluates a number to determine if it's positive, negative, or zero.

**Possible Answer 1:**

We start by taking an input:

```typescript
INPUT number
```

Next, we must decide what to do based on the number's value. This is where the **if** construct comes in.

If the number is greater than zero, we can say it's positive:

```typescript
IF number > 0 THEN
    PRINT "The number is positive."
```

But what if it's not? We need another check, and that's where **else if** proves useful. It's like saying, "if the previous conditions weren't met, then check this."

If the number is less than zero, it's negative:

```typescript
ELSE IF number < 0 THEN
    PRINT "The number is negative."
```

Lastly, if the number isn't positive or negative, it must be zero. That's where **else** comes in. It's our catch-all for "if none of the above conditions are met, do this":

```typescript
ELSE
    PRINT "The number is zero."
```

And, to neatly conclude our decision-making constructs, we use:

```typescript
END IF
```

Putting it all together, we have

```typescript
INPUT number

IF number > 0 THEN
    PRINT "The number is positive."
ELSE IF number < 0 THEN
    PRINT "The number is negative."
ELSE
    PRINT "The number is zero."
END IF
```

By outlining logic in pseudocode, transitioning to actual coding in any programming language becomes a smoother process, as the core logic remains consistent.

**Possible Answer 2:**

Without going into all the steps, here is the final pseudocode.

```typescript
INPUT number

IF number == 0 THEN
    PRINT "The number is zero."
ELSE IF number > 0 THEN
    PRINT "The number is positive."
ELSE
    PRINT "The number is negative."
END IF
```

There are multiple ways to solve most problems, depending on the order in which you evaluate the conditions.

**Problem 2:**

Suppose you're organizing an outdoor event. You'll proceed if:

- The forecast does not predict rain.
- The temperature is between 18°C and 30°C.

Write corresponding pseudocode for such a program.

**Answer:**

**Evaluating Rain Forecast:**
We want to check if it's NOT raining. Here's how we can understand the NOT raining condition:

- The *'raining'* variable would be **True** if it's raining and **False** if it isn't.
- Using "NOT" in front of *'raining'* inverts its truth value. So, if *'raining'* is **True**, *'NOT raining'* becomes **False**, and vice versa.
- For our event to proceed, we want it to be the case where it's not raining, so we're looking for the scenario where *'NOT raining'* is **True**.

In pseudocode:

```typescript
IF NOT raining
```

**Evaluating Temperature:**
We want the temperature to be between 18°C and 30°C. This condition can be represented as:

```typescript
temperature > 18 AND temperature < 30
```

Combining both conditions, our complete decision-making pseudocode becomes:

```typescript
IF NOT raining AND (temperature > 18 AND temperature < 30):
    proceed_with_event
ELSE
    reschedule_event
```

By breaking down our conditions in this way, we ensure that the event only proceeds if it's not raining and the temperature is within our desired range.
