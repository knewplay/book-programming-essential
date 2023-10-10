---
title: "Chapter 4: Repetition and Iteration"
date: "2023-10-10"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - ["sandwich-loop", ""]
  - ["guess-number", "You are thinking of a secret number between 1 and 100, and you ask your friend to guess it. If their guess is too high, you respond with \"Too high\". If their guess is too low, you say \"Too low\". Your friend continues guessing based on your feedback until they correctly guess the secret number.

  Describe the flow of decisions and responses you would go through until the correct number is identified, as if you were instructing someone to create a flowchart for the game."]
---

In our daily lives, we encounter many repetitive tasks, whether it's setting an alarm each night or brushing our teeth every morning. Similarly, in programming, there's a concept that allows us to handle repetitive actions efficiently: loops. Dive into this chapter to discover how loops work in the world of coding.

## Table of Contents

[A Brief Review of Transistors](#a-brief-review-of-transistors)

- [The Binary Nature of Transistors](#the-binary-nature-of-transistors)
- [Connecting Transistors to Programming: Boolean Values](#connecting-transistors-to-programming-boolean-values)

## Understanding the Concept of Loops

Loops are a fundamental concept in programming. They allow us to execute a set of instructions multiple times, which is often referred to as "iteration." Instead of writing the same code over and over again, a loop provides a cleaner way to repeat actions.

Imagine playing your favorite video game. There are certain elements in that game that are repetitive, all thanks to loops. Here are a few:

- **Gameplay Music:** That catchy tune that plays over and over in the background? It's looped to create a consistent ambiance.
- **Non-Playable Characters (NPCs):** Characters like guards that patrol the same route or vendors in a marketplace who follow a fixed path are repeating their actions through loops.
- **Respawning Items:** Ever noticed how some collectible items or power-ups reappear in the same spot after a while? That's a loop ensuring you never run out of challenges or rewards.
- **Animated Backgrounds:** The moving clouds, flying birds, or flowing rivers that bring a game environment to life? These are often looped animations, adding depth without the need for constant new animations.

Using loops, developers can instruct the game to repeat specific actions seamlessly, enhancing the overall gaming experience. It's one of the many nifty tricks in the programmer's toolkit!

## Use Cases of Looping

Loops are incredibly useful in scenarios where:

- A specific action needs to be repeated multiple times.
- An action must be executed until a particular condition is satisfied.
- We have a collection of items and want to perform the same operation on each item.

Using loops not only saves time but also ensures our code remains clean and efficient.

## The Structure of a Loop

A loop generally consists of three main components:

- Starting Point: This is where the loop begins.
- Condition: The loop continues as long as this condition holds true.
- Update: After each loop iteration, there's typically an update or an action that leads us closer to exiting the loop.

Consider the countdown for a rocket launch as an example. The countdown starts at 10, and with each passing second, the number decreases by 1. Once the countdown reaches 0, the rocket launches! In this case, the starting point is `countdown = 10`, the condition to check if is `countdown == 0`, and the update we do is to update `countdown - 1` every passing second.

[Have an illustration [like this one](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.quora.com%2FHow-do-I-visualize-a-loop-in-C-programming&psig=AOvVaw3nEYgUSEy0vJgFHnHPCkYu&ust=1697055905206000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJiF5Iao7IEDFQAAAAAdAAAAABAD)]

## Activities

**Activity #1:** ...

Now that we've learned about loops let's visualize them!

🎨 Illustration: A flowchart diagram representing a loop that prints "Hello" 8 times. As shown [here](https://www.google.com/url?sa=i&url=https%3A%2F%2Fonline.visual-paradigm.com%2Fdiagrams%2Ftemplates%2Fflowchart%2Fflowchart-example-using-loop%2F&psig=AOvVaw3eXjygPKUVObcEHkNF7kqV&ust=1697038491315000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJDMkZbn64EDFQAAAAAdAAAAABAX)

This flowchart begins with the Start. From there, we set our "counter" to 0. Think of this counter as our track lap marker; it helps us keep track of how many times we've said "Hello."

Next, we have a decision point where we check: "Is the counter equal to 7?" If it's not, we go ahead and print "Hello" and then add 1 to our counter. Think of this as completing one lap and taking a sip of water.

If our counter does reach 7, it means we've already printed "Hello" 8 times (remember, we started counting from 0), and we exit the loop. It's like deciding that you've run enough laps for the day and heading home.

Loops, whether in flowcharts or code, provide a visual and structured way to handle repetitive tasks. With this fun activity, you should now have a clearer picture of how loops operate!

Hope this helps deepen your understanding and makes the concept fun!

**Activity #2:** Imagine you possess another humanoid robot. Resembling an adult human, this robot can flawlessly hear and execute every command you give. However, it's limited to understanding only the most fundamental commands, like "lift your right foot 5 centimeters" or "turn your head 90 degrees left". It's unable to process abstract or compound actions like "walk across the room."

Describe in detail the series of commands you would give to instruct the robot on how to walk forward step by step. Additionally, you can draw the corresponding flowchart diagram.

**Answer:**
To make the robot walk forward, a series of commands can be given, focusing on one step at a time:

1. Lift the right foot 5 centimeters.
2. Move the right foot 30 centimeters forward.
3. Lower the right foot until it touches the ground.
4. Transfer the weight to the right foot.
5. Lift the left foot 5 centimeters.
6. Move the left foot 30 centimeters forward.
7. Lower the left foot until it touches the ground.
8. Transfer the weight to the left foot.
9. Repeat steps 1-8 for continued walking.

This series of commands instructs the robot on the basic mechanics of walking, step by step.

<!-- [Flowchart diagram] -->

