---
title: "Chapter 2: Algorithms and Flowcharts"
date: "2023-09-26"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - treasure-hunt: |
      Imagine you're setting up a treasure hunt game for your friend. You've buried a treasure and only you know its location. Now, it's your friend's turn to find it. However, there's a twist: your friend, much like a computer, requires precise and unambiguous instructions to accomplish the task.

      Standing at the designated starting point, you hand over a note with the following instructions:

      1. Take 10 steps forward
      2. Turn right and take 3 large steps
      3. Turn left and crawl 5 times
      4. Dig 2 inches down to find the treasure!

      Describe the sequence and decision-making process you would use to turn these instructions into a flowchart. Be sure to mention any symbols and their meanings.
  - cereal: |
      The year is 2053, and you have a humanoid servant robot at home, equipped with advanced visual sensors. You want to ask the robot to make you some cereal, but unfortunately, "making cereal" is too complex of a task for this early version of a servant robot. You've prepped the table with a bowl, cereal, and milk in front of the robot and decided to give it the following instructions (assuming the robot understands the concept of pouring):

      1. Grab the milk carton.
      2. Pour some milk into the bowl.
      3. Grab the box of cereal.
      4. Pour some cereal into the bowl.

      However, the attempt fails. What went wrong? Provide better instructions
  - sandwich: |
      You have a robot chef in your kitchen that can prepare sandwiches based on user preferences. Your task is to provide instructions for the robot chef. The user can choose:

      - The type of bread (white or whole wheat)
      - The type of meat (ham or turkey)
      - Whether they want tomatoes (yes or no)

      Every sandwich also includes lettuce by default.

      Describe in detail the sequence of commands and decision-making process you would provide to the robot to ensure the sandwich is made to the user's preferences, making sure to include the specified decisions.
---

As we venture deeper into the realm of programming and problem-solving, the importance of structured thinking becomes evident. Central to this idea is the concept of algorithms, which act as blueprints for action. Let's dive deeper into what algorithms are and how they can be visually represented using flowcharts.

[Understanding Algorithms](#understanding-algorithms)

[Introduction to Flowcharts](#introduction-to-flowcharts)

[Convert a Problem into a Flowchart](#convert-a-problem-into-a-flowchart)

[Activities](#activities)

[Questions](#questions)

## Understanding Algorithms

An algorithm is a well-defined series of steps to solve a specific problem or accomplish a task. Algorithms are everywhere, not just in computing. They're essentially a recipe: a series of discrete, step-by-step instructions that, when followed precisely, leads to a predictable outcome.

Imagine you're teaching someone to tie their shoelaces. The instructions you give them, starting from holding the two ends of the laces to the final tightening of the knot, constitute an algorithm.

Now, consider a more complex scenario: robots in a competition. In such a contest, a robot might be tasked to collect a ball from the ground and shoot it into a basket.

![Shooting robot](./figures/ch-2-robot-shoot-image.jpg)
*A robot shooting a basketball during a competition.*

The robot doesn't act on instinct or intuition; instead, it follows a strict set of instructions - its algorithm. The algorithm could look something like this:

1. Scan the surroundings for a ball.
2. Navigate towards the ball while avoiding obstacles.
3. Pick up the ball.
4. Identify the location of the basket.
5. Calculate the right angle and force to shoot the ball into the basket.
6. Shoot the ball.

Even though it might seem simple to us, each of these steps needs to be meticulously defined for a robot to perform them. How does it "scan" or "pick up the ball"? Each of these larger tasks can be further decomposed into smaller, more precise actions, each constituting part of the overall algorithm.

## Introduction to Flowcharts

While algorithms can be written down as a list of instructions, for complex tasks, a visual representation can be more intuitive. Enter flowcharts.

A flowchart uses symbols to represent different types of actions or steps. Key symbols include:

- Oval: Represents the start or end of a process.
- Rectangle: Denotes a process or action step.
- Diamond: Used for decisions, often questions that yield 'yes' or 'no' answers.
- Arrow: Dictates the flow of the process.

### Convert a Problem into a Flowchart

Converting a problem into a flowchart involves breaking down the problem into individual steps or processes, then representing those steps graphically. Let's take a straightforward example: making a cup of tea.

#### Step 1: Define the problem

Understand what you're trying to achieve. In our example, the problem or task is: Make a cup of tea.

#### Step 2: List down the steps

Write down every step involved in the process. For our tea example, it might look like this:

- Fill the kettle with water.
- Boil the water.
- Place a teabag in the cup.
- Pour the boiled water into the cup.
- Wait a couple of minutes.
- Remove the teabag from the cup.

#### Step 3: Start drawing the flowchart

**Begin at the start:**
Draw an oval labeled "Start". This will be the entry point of your flowchart.

**Go step-by-step:**
Now, take your first step ("Fill the kettle with water.") and represent it with a rectangle. Draw an arrow from "Start" to this rectangle.

From this rectangle, draw another arrow leading to the next step ("Boil the water.") represented by another rectangle. This intuitive method is like walking through the process yourself and marking down each step as you complete it.

**Incorporate decisions:**
When you encounter a step that involves making a decision, use a diamond shape. For instance, after removing the teabag, there might be a decision: "Add sugar?". If "Yes", you'd show the steps to add sugar; if "No", you'd proceed to the end.

**Continue until the end:**
Keep drawing arrows from one rectangle to the next as you move through your list of steps. After the last step, draw an arrow to a rounded rectangle labeled "End".

![Completed flowchart](./figures/ch-2-tea-making.jpg)
*Complete flowchart of the tea-making process.*

#### Step 4: Review

Once you've drawn out each step from your list, take a moment to review the flowchart. Walk through each step and decision in your mind to ensure nothing is missing and the flow is logical.

The intuitive approach is like narrating a story to yourself. You're recounting the tale of making a cup of tea, from start to finish. By following each step as you would in real life and drawing it out in sequence, you create a visual representation of the process.

![Tea making](./figures/ch-2-tea-makeing-image.jpg)
*Tea being poured into a cup.*

By using this systematic approach, you can turn any problem or process into a clear, visual flowchart.

Remember, algorithms and flowcharts are all about breaking down problems and representing solutions in a structured manner. As you become more familiar with them, they'll become invaluable tools in your problem-solving toolkit!

## Activities

### Activity #1

Think of a daily routine. Describe the sequence and decision-making process of your routine as if you were guiding someone through the steps. For instance, consider the routine of getting ready for work in the morning.

![Getting ready for school](./figures/ch-2-getting-ready-for-school.jpg)
*A student headed to school.*

### Answer

Routine: Getting ready for work in the morning

1. Wake up when the alarm rings.
2. Turn off the alarm.
3. Check the weather.
4. Put on basic clothing.
5. Go to the bathroom to brush teeth and wash face.
6. Eat breakfast.
7. Decision: Is it raining?
    - Yes: Wear rain-appropriate attire and carry an umbrella.
    - No: Wear regular attire.
8. Grab your schoolbag, ensuring the essentials are inside.
9. Leave the house and head to school.

This sequence lists out the steps and includes a decision-making point regarding the weather, which affects the choice of attire for the day.

### Activity #2

Imagine you have a humanoid robot. This robot can flawlessly execute every command you give but understands only fundamental commands, such as "lift your right foot 5 centimeters" or "turn your head 90 degrees left". It's unable to process abstract or compound actions like "walk forward".

You want to instruct the robot to move 30 centimeters forward. Describe in detail the series of commands you would provide to ensure the robot moves the desired distance.

### Answer

To instruct the robot to move 30 centimeters forward with each leg, one after another, you would give the following commands:

1. Lift the right foot 5 centimeters.
2. Move the right foot 30 centimeters forward.
3. Lower the right foot until it touches the ground.
4. Transfer the weight to the right foot.
5. Lift the left foot 5 centimeters.
6. Move the left foot 30 centimeters forward.
7. Lower the left foot until it touches the ground.
8. Distribute the weight evenly between both legs, achieving a 50/50 balance.

These commands ensure the robot takes a single step with each leg, moving a total of 30 centimeters forward.
