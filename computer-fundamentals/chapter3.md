---
title: "Chapter 3: Logic and Decision Making"
date: "2023-10-04"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
---

In our everyday lives, we make countless decisions based on conditions: if it rains, take an umbrella; if it's cold, wear a jacket. Similarly, in programming, decision-making is a crucial aspect, enabling the program to react differently to different inputs or situations.

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

- \> : Greater than. E.g., 5 > 3 is true because 5 is greater than 3.
- < : Less than. E.g., 2 < 4 is true because 2 is less than 4.
- == : Equal to. For instance, 7 == 7 is true because both sides of the operator have the same value.

> Note: We use "==" to check for equality in most programming languages instead of "=". The reason for this will become clearer later when you dive into actual coding. For now, remember to use "==" when making comparisons.

These operators help us compare values and determine the relationship between them. They're fundamental to setting up conditions in our code.

## Practical Problems

**Problem 1:**
Write a program that evaluates a number to determine if it's positive, negative, or zero.

**Possible Answer 1:**
We start by taking an input:

```typescript
INPUT number
```

Next, we must decide what to do based on the number's value. This is where the if construct comes in.

If the number is greater than zero, we can say it's positive:

```typescript
IF number > 0 THEN
    PRINT "The number is positive."
```

But what if it's not? We need another check, and that's where elif proves useful. It's like saying, "if the previous conditions weren't met, then check this."

If the number is less than zero, it's negative:

```typescript
ELSE IF number < 0 THEN
    PRINT "The number is negative."
```

Lastly, if the number isn't positive or negative, it must be zero. That's where else comes in. It's our catch-all for "if none of the above conditions are met, do this":

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

There are multiple ways to solve most problems, depending on the order in you evaluate the conditions.

**Problem 2:**
Imagine you're programming a digital traffic light system. Create a flowchart and corresponding pseudocode that considers vehicle and pedestrian traffic, ensuring safety rules are prioritized.

**Answer:**
If the light is green, vehicles move.
If the light is red, vehicles stop.
If the light is yellow, vehicles slow down in preparation to stop.

[TODO]
COMPLETE ANSWER, OR POSSIBLE REMOVE THIS QUESTION


[ADD SECTION EXPLAINING LOGICAL OPERATORS (and or not)]

**Problem 3:**
Suppose you're organizing an outdoor event. You'll proceed if:

- The forecast does not predict rain.
- The temperature is between 60°F and 85°F.

Write corresponding pseudocode for such a program.

**Answer:**
Using our programming constructs and logical operators, the decision-making part of the program might look like this:

```python
if not raining and (temperature >= 60 and temperature <= 85):
    proceed_with_event()
else:
    reschedule_event()
```
