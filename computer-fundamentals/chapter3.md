# Chapter 3: Logic and Decision Making
In our everyday lives, we make countless decisions based on conditions: if it rains, take an umbrella; if it's cold, wear a jacket. Similarly, in programming, decision-making is a crucial aspect, enabling the program to react differently to different inputs or situations.

## A Brief Review of Transistors
Imagine a tiny switch, so small that millions of them could fit on the tip of your finger. This is a transistor. It's a device that can either allow an electric current to flow through it (like turning on a light) or stop it entirely (like turning the light off).

In essence, a transistor has two primary states:

- On: This is when it allows electricity to pass through. We can liken this to opening a faucet and letting water flow.
- Off: This is when it prevents electricity from flowing, similar to closing a faucet to stop the water.

### The Binary Nature of Transistors
The fact that a transistor has only two states introduces us to a fundamental concept: "binary." In the realm of computers, binary refers to the system of representing values using only two symbols, usually 0 and 1. In the case of our transistor, "on" can be thought of as "1", and "off" as "0".

> Note: The term 'binary' focuses on two states. In contrast, "unary" describes one state, "ternary" represents three states, and "quadrinary" means four states. However, computers primarily use binary logic because of the inherent on/off, true/false nature of electrical circuits and transistors.

### Connecting Transistors to Programming: Boolean Values
When you start programming, you'll encounter a concept called "boolean values." Named after George Boole, a 19th-century mathematician, booleans in programming have just two values: "True" and "False".

Do you see the parallel? Just as a transistor can be "on" (1) or "off" (0), a boolean value can be "True" (equivalent to 1) or "False" (equivalent to 0).

To grasp the significance of booleans, think about how we evaluate statements in our daily life. For instance, the statement "The sky is blue" can be true during a clear day, but false during the night. Similarly, in programming, boolean values emerge from evaluating conditions or statements.

> Note: A statement is a sentence or expression that can be evaluated as either true or false but not both. In programming, statements provide a way to represent facts or conditions that the computer can then use to make decisions.

Take the example "5 is greater than 4." When a computer processes this statement, it evaluates the condition and concludes it to be "True." In contrast, the statement "6 is greater than 4 and less than 3" is contradictory, and thus, it evaluates to "False."

In the realm of programming, these boolean evaluations become crucial. They serve as the bedrock for decision-making in code. A program can execute specific tasks based on whether a statement is true or false. This binary approach to decision-making, deeply rooted in the fundamental operation of transistors, showcases the elegant bridge between hardware (transistors) and software (boolean logic).


## Practical Problems

**Problem 1:**
Imagine you're programming a digital traffic light system. Create a flowchart and corresponding pseudocode that considers vehicle and pedestrian traffic, ensuring safety rules are prioritized.

**Answer:**
If the light is green, vehicles move.
If the light is red, vehicles stop.
If the light is yellow, vehicles slow down in preparation to stop.

**Problem 2:**
Suppose you're organizing an outdoor event. You'll proceed if:

- The forecast does not predict rain.
- The temperature is between 60°F and 85°F.

Write corresponding pseudocode for such a program.

**Answer:**
Using our programming constructs and logical operators, the decision-making part of the program might look like this:

```
if not raining and (temperature >= 60 and temperature <= 85):
    proceed_with_event()
else:
    reschedule_event()
```


## Exercises

**Questions 1:**


**Question 2:**


**Question 3:**
Create a flowchart and the corresponding pseudocode for a program that checks whether a given number is positive, negative, or zero.