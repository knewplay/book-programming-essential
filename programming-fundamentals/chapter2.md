---
title: "Chapter 2: Algorithms and Flowcharts"
date: "2023-09-26"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
exercises:
  - ["treasure-hunt", "Imagine you're setting up a treasure hunt game for your friend. You've buried a treasure and only you know its location. Now, it's your friend's turn to find it. However, there's a twist: your friend, much like a computer, requires precise and unambiguous instructions to accomplish the task.

  Standing at the designated starting point, you hand over a note with the following instructions:

  1. Take 10 steps forward
  2. Turn right and take 3 large steps
  3. Turn left and crawl 5 times
  4. Dig 2 inches down to find the treasure!

  Draw the corresponding flowchart for these instructions."]
  - ["daily-routine", "Think of a daily routine, and map it out on a flowchart. It could be your morning routine, making a cup of tea, or even how you decide what to wear!"]
  - ["simon-says", "You're playing a game of \"Simon Says\" with a group of children. The goal is for you to call out commands and for the children to follow, but only if you first say \"Simon Says.\" If you don't use the phrase \"Simon Says\" before a command and they still execute it, they're out of the game. Given this set of rules:
  1. Listen for the phrase \"Simon Says.\"
  2. If \"Simon Says\" is heard, execute the following command.
  3. If \"Simon Says\" is not heard, do not execute the command.
  4. If a command is executed without the preceding \"Simon Says\", the player is out.

  Convert this rule set into a flowchart."]
  - ["guess-number", "You are thinking of a secret number between 1 and 100, and you ask your friend to guess it. If their guess is too high, you respond with \"Too high\". If their guess is too low, you say \"Too low\". Your friend continues guessing based on your feedback until they correctly guess the secret number.

  Create a flowchart to visually represent this process, ensuring you account for each decision and response until the correct number is identified."]
---

As we venture deeper into the realm of programming and problem-solving, the importance of structured thinking becomes evident. Central to this idea is the concept of algorithms, which act as blueprints for action. Let's dive deeper into what algorithms are and how they can be visually represented using flowcharts.

## What is an algorithm?

An algorithm is a well-defined series of steps to solve a specific problem or accomplish a task. Algorithms are everywhere, not just in computing. They're essentially a recipe: a series of discrete, step-by-step instructions that, when followed precisely, leads to a predictable outcome.

Imagine you're teaching someone to tie their shoelaces. The instructions you give them, starting from holding the two ends of the laces to the final tightening of the knot, constitute an algorithm.

Now, consider a more complex scenario: robots in a competition. In such a contest, a robot might be tasked to collect balls from the ground and shoot them into a basket. The robot doesn't act on instinct or intuition; instead, it follows a strict set of instructions - its algorithm. The algorithm could look something like this:

1. Scan the surroundings for a ball.
2. Navigate towards the ball while avoiding obstacles.
3. Pick up the ball.
4. Identify the location of the basket.
5. Calculate the right angle and force to shoot the ball into the basket.
6. Shoot the ball.
7. Repeat until no balls are left or a set period expires.

Even though it might seem simple to us, each of these steps needs to be meticulously defined for a robot to perform them. How does it "scan" or "pick up"? Each of these larger tasks can be further decomposed into smaller, more precise actions, each constituting part of the overall algorithm.

## Introduction to flowcharts and their symbols

While algorithms can be written down as a list of instructions, for complex tasks, a visual representation can be more intuitive. Enter flowcharts.

A flowchart uses symbols to represent different types of actions or steps. Key symbols include:

- Oval: Represents the start or end of a process.
- Rectangle: Denotes a process or action step.
- Diamond: Used for decisions, often questions that yield 'yes' or 'no' answers.
- Arrow: Dictates the flow of the process.

[Illustration of these symbols with labels: For the robot example, a flowchart could visually depict the process from scanning the environment to shooting the ball, highlighting decisions (like whether a ball is found) and actions (like navigating or shooting).]

## How to convert a problem into a flowchart

Converting a problem into a flowchart involves breaking down the problem into individual steps or processes, then representing those steps graphically. Let's take a straightforward example: making a cup of tea.

### Step 1: Define the Problem

Understand what you're trying to achieve. In our example, the problem or task is: Make a cup of tea.

### Step 2: List Down the Steps

Write down every step involved in the process. For our tea example, it might look like this:

- Fill the kettle with water.
- Boil the water.
- Place a teabag in the cup.
- Pour the boiled water into the cup.
- Wait a couple of minutes.
- Remove the teabag from the cup.

### Step 3: Start Drawing the Flowchart

**Begin at the Start:**

Draw the rounded rectangle labeled "Start". This will be the entry point of your flowchart.

**Go Step-by-Step:**

Now, take your first step ("Fill the kettle with water.") and represent it with a rectangle. Draw an arrow from "Start" to this rectangle.

From this rectangle, draw another arrow leading to the next step ("Boil the water.") represented by another rectangle. This intuitive method is like walking through the process yourself and marking down each step as you complete it.

**Incorporate Decisions:**

When you encounter a step that involves making a decision, use a diamond shape. For instance, after removing the teabag, there might be a decision: "Add sugar?". If "Yes", you'd show the steps to add sugar; if "No", you'd proceed to the end.

**Continue Until the End:**

Keep drawing arrows from one rectangle to the next as you move through your list of steps. After the last step, draw an arrow to a rounded rectangle labeled "End".

### Step 4: Review

Once you've drawn out each step from your list, take a moment to review the flowchart. Walk through each step and decision in your mind to ensure nothing is missing and the flow is logical.

The intuitive approach is like narrating a story to yourself. You're recounting the tale of making a cup of tea, from start to finish. By following each step as you would in real life and drawing it out in sequence, you create a visual representation of the process. This method can be particularly useful for those who are new to flowcharts or who think best in linear, sequential terms.

[Illustration of tea making process]

By using this systematic approach, you can turn any problem or process into a clear, visual flowchart.

Remember, algorithms and flowcharts are all about breaking down problems and representing solutions in a structured manner. As you become more familiar with them, they'll become invaluable tools in your problem-solving toolkit!

## Practice Problems

**Problem 1:**
The year is 2053, and you have a servant robot at home, equipped with advanced visual sensors. You want to ask the robot to make you some cereal, but unfortunately, "making cereal" is too complex of a task for this early version of a servant robot. You've prepped the table with a bowl, cereal, and milk in front of the robot and decided to give it the following instructions (assuming the robot understands the concept of pouring):

1. Grab the milk carton.
2. Pour some milk into the bowl.
3. Grab the box of cereal.
4. Pour some cereal into the bowl.

However, the attempt fails. What went wrong?

**Answer:**
The instructions provided lacked specificity in several areas:

- The robot wasn't instructed to open the milk carton or cereal box before pouring.
- There was no indication of how long to pour the milk or cereal, leading to potential overflow or inadequate amounts.

A robot, especially an early version, requires precise, step-by-step instructions to successfully complete tasks.

Here is a possible solution:

1. Grab the milk carton.
2. Open the milk carton.
3. Pour milk into the bowl until it's 1/4 full.
4. Close the milk carton.
5. Grab the box of cereal.
6. Open the cereal box.
7. Pour cereal into the bowl until it covers the milk.
8. Close the cereal box.

But then again, what is likely to happen here is that the robot closes the milk carton, but never let's go of it. And when asked to grab the cereal, is uses its other hand to do so.

[Illustration of robot with milk in one hand, and cereal box in the other]

**Problem 2:** Imagine you possess a state-of-the-art humanoid robot. Resembling an adult human, this robot can flawlessly hear and execute every command you give. However, it's limited to understanding only the most fundamental commands, like "lift your right foot 5 centimeters" or "turn your head 90 degrees left". It's unable to process abstract or compound actions like "walk across the room."

Draw a flowchart diagram to instruct the robot on how to walk forward.

**Answer:**

[Flowchart diagram]
