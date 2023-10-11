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

[Understanding the Concept of Loops](#understanding-the-concept-of-loops)

[Use Cases of Looping](#use-cases-of-looping)

[The Structure of a Loop](#the-structure-of-a-loop)

[Visualizing with an Example](#visualizing-with-an-example)

[Activities](#activities)

## Understanding the Concept of Loops

Loops are a fundamental concept in programming. They allow us to execute a set of instructions multiple times, which is often referred to as "iteration." Instead of writing the same code over and over again, a loop provides a cleaner way to repeat actions.

Imagine playing your favorite video game. There are certain elements in that game that are repetitive, all thanks to loops. Here are a few:

- **Gameplay Music:** That catchy tune that plays over and over in the background? It's looped to create a consistent ambiance.
- **Non-Playable Characters (NPCs):** Characters like guards that patrol the same route or vendors in a marketplace who follow a fixed path are repeating their actions through loops.
- **Respawning Items:** Ever noticed how some collectible items or power-ups reappear in the same spot after a while? That's a loop ensuring you never run out of challenges or rewards.
- **Animated Backgrounds:** The moving clouds, flying birds, or flowing rivers that bring a game environment to life? These are often looped animations, adding depth without the need for constant new animations.

Using loops, developers can instruct the game to repeat specific actions seamlessly, enhancing the overall gaming experience. It's one of the many nifty tricks in the programmer's toolkit!

### Use Cases of Looping

Loops are incredibly useful in scenarios where:

- A specific action needs to be repeated multiple times.
- An action must be executed until a particular condition is satisfied.
- We have a collection of items and want to perform the same operation on each item.

Using loops not only saves time but also ensures our code remains clean and efficient.

## The Structure of a Loop

Let's take a closer look at the core components of a loop, using a visual guide:

[[Illustration](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.quora.com%2FHow-do-I-visualize-a-loop-in-C-programming&psig=AOvVaw3nEYgUSEy0vJgFHnHPCkYu&ust=1697055905206000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJiF5Iao7IEDFQAAAAAdAAAAABAD)]

1. **Starting Point (*`start`*):** This is where our loop begins its journey. It sets the stage for the series of repetitive actions that will follow.
2. **Initialization (*`initialization of loop counter`*):** We set a base or starting value for our loop.
3. **Condition (*`while condition`*):** This is the loop's heartbeat. As long as this condition remains true, the loop will continue its iterations. In the flowchart, you can see a decision diamond (the pink one) where the loop checks if the condition is still true. If it's not, the loop will break, and the process will stop.
4. **Execution (*`body of the loop`*):** Here's where the main action of the loop takes place. It's the task or set of tasks that the loop performs with each iteration. Maybe it's adding a number, printing a message, or updating a score in a video game.
5. **Update (*`update the counter`*):** After executing the main action, the loop typically modifies the loop counter, pushing the loop closer to an exiting condition.
6. **Exit Point (*`stop`*)**: All loops must have an end (unless they're meant to run indefinitely). When the loop's condition no longer holds true, it exits, allowing the program to either end or move on to the next task.

Consider the countdown for a rocket launch as an example. The countdown starts at 10, and with each passing second, the number decreases by 1. Once the countdown reaches 0, the rocket launches! In this case, the starting point is `countdown = 10`, the condition to check if is `countdown == 0`, and the update we do is to update `countdown - 1` every passing second.

## Visualizing with an Example

Let's say we are tasked with printing "Hello" 8 times onto the screen.

🎨 Illustration: A flowchart diagram representing a loop that prints "Hello" 8 times. As shown [here](https://www.google.com/url?sa=i&url=https%3A%2F%2Fonline.visual-paradigm.com%2Fdiagrams%2Ftemplates%2Fflowchart%2Fflowchart-example-using-loop%2F&psig=AOvVaw3eXjygPKUVObcEHkNF7kqV&ust=1697038491315000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJDMkZbn64EDFQAAAAAdAAAAABAX)

This flowchart begins with the Start. From there, we set our "counter" to 0. Think of this counter as our track lap marker; it helps us keep track of how many times we've said "Hello."

Next, we have a decision point where we check: "Is the counter equal to 7?" If it's not, we go ahead and print "Hello" and then add 1 to our counter. Think of this as completing one lap and taking a sip of water.

If our counter does reach 7, it means we've already printed "Hello" 8 times (remember, we started counting from 0), and we exit the loop. It's like deciding that you've run enough laps for the day and heading home.

> Note: While humans start counting from 1 (1, 2, ..., 8), computers count starting from 0 (0, 1, ..., 7). The reason ...

## Activities

### Activity #1

Recall the humanoid robot from [Chapter 2 Activity #2](./chapter2.md#activity-2). With your understanding of loops from this chapter, describe the commands you would provide to ensure the robot walks across the room. Consider visualizing your solution with a flowchart diagram.

### Answer

To make the robot walk across the room, you would use a series of commands for each step, and then loop through those commands until the robot has crossed the room:

1. Lift the right foot 5 centimeters.
2. Move the right foot 30 centimeters forward.
3. Lower the right foot until it touches the ground.
4. Transfer the weight to the right foot.
5. Lift the left foot 5 centimeters.
6. Move the left foot 60 centimeters forward.
7. Lower the left foot until it touches the ground.
8. Transfer the weight to the left foot.
9. Check for obstacles or the end of the room. If an obstacle or end of the room is detected, exit loop.
10. Otherwise, repeat from step 1.

This series of commands instructs the robot on the basic mechanics of walking, step by step. You would then loop the above commands until the robot has walked the desired distance across the room.

<!-- [Flowchart diagram] -->

### Activity #2

You're working with a new generation humanoid robot that's designed for physical exercises. Unlike previous models, this robot has advanced kinesthetic intelligence, meaning it understands basic exercise commands without needing a breakdown of every movement. For instance, you don't need to instruct it with "bend your arms 90 degrees" for push-ups; you can simply command "Do a push-up", and it will perform the action. However, you cannot ask it to "Do 10 push-ups", as it can only comprehend one push-up at a time.

Instruct your robot to perform a set of 10 push-ups, followed by 10 sit-ups, and then 10 squats. The robot should then loop this set 5 times.

### Answer

```typescript
Repeat 5 times:
    Repeat 10 times:
        Do a push-up
    Repeat 10 times:
        Do a sit-up
    Repeat 10 times:
        Do a squat

```
