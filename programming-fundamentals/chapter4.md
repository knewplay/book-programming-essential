---
title: "Chapter 4: Repetition and Iteration"
date: "2023-10-10"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - sandwich-loop: Write a program where you make 10 identical sandwiches, all consisting of bread, ham and cheese. Prepare each sandwich sequentially using a loop, ensuring that one sandwich is completed before starting the next.
  - guess-number: |
      You are thinking of a secret number between 1 and 100, and you ask your friend to guess it. If their guess is too high, you respond with "Too high". If their guess is too low, you say "Too low". Your friend continues guessing based on your feedback until they correctly guess the secret number.

      Describe the flow of decisions and responses you would go through until the correct number is identified, as if you were instructing someone to create a flowchart for the game.
  - workout: |
      Is the following program different from the Activity 2 solution. Explain your answer.
  
      REPEAT 5 times:
        REPEAT 10 times:
          do_pushup
          do_situp
          do_squat

---

In our daily lives, we encounter many repetitive tasks, whether it's setting an alarm each night or brushing our teeth every morning. Similarly, in programming, there's a concept that allows us to handle repetitive actions efficiently: loops. Dive into this chapter to discover how loops work in the world of coding.

## Table of Contents

[Understanding the Concept of Loops](#understanding-the-concept-of-loops)

[Use Cases of Looping](#use-cases-of-looping)

[The Intricacies of a Loop](#the-intricacies-of-a-loop)

[Visualizing with Examples](#visualizing-with-examples)

- [Example #1: Repetitive Ball Shots by a Robot](#example-1-repetitive-ball-shots-by-a-robot)
- [Example #2: Rocket Launch Countdown](#example-2-rocket-launch-countdown)

[Nested Loops](#nested-loops)

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

## The Intricacies of a Loop

When you start actually programming, you'll notice that you can't just say "Loop 5 times"; it's a bit more complicated than that.

So in this section, let's take a closer look at the core components of a loop, using a visual guide:

[[Illustration](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.quora.com%2FHow-do-I-visualize-a-loop-in-C-programming&psig=AOvVaw3nEYgUSEy0vJgFHnHPCkYu&ust=1697055905206000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJiF5Iao7IEDFQAAAAAdAAAAABAD) but split "body" and "update" into two boxes]

1. **Starting Point (*`start`*):** This is where our loop begins its journey. It sets the stage for the series of repetitive actions that will follow.
2. **Initialization (*`initialization of loop counter`*):** We set a base or starting value for our loop.
3. **Condition (*`while condition`*):** This is the loop's heartbeat. As long as this condition remains **true**, the loop will continue its iterations. In the flowchart, you can see a decision diamond (the pink one) where the loop checks if the condition is still true. If it's not, the loop will break, and the process will stop.
4. **Execution (*`body of the loop`*):** Here's where the main action of the loop takes place. It's the task or set of tasks that the loop performs with each iteration. Maybe it's adding a number, printing a message, or updating a score in a video game.
5. **Update (*`update the counter`*):** After executing the main action, the loop typically modifies the loop counter, pushing the loop closer to an exiting condition.
6. **Exit Point (*`stop`*)**: All loops must have an end (unless they're meant to run indefinitely). When the loop's condition no longer holds true, it exits, allowing the program to either end or move on to the next task.

## Visualizing with Examples

### Example #1: Repetitive Ball Shots by a Robot

Imagine we're programming a robot for a competition where it needs to shoot a ball into a basket ten times in a row. Using a loop, we can efficiently give the robot this repetitive task.

[Illustration: A flowchart diagram representing a loop where a robot shoots a ball 10 times]

1. **Starting Point (*`Start`*):** Our loop begins at this entry point, initiating the robot's ball shooting sequence.
2. **Initialization (*`Set shotCounter to 0`*):** The loop starts by setting an initial value for the shot counter, which keeps track of how many balls the robot has shot. Initially, the shot counter is set to 0.
3. **Condition (*`Is shotCounter < 10?`*)**: At this step, the loop checks the counter's value. It's asking, "Has the robot shot less than 10 balls?" If the shot counter hasn't reached 10, the loop will continue instructing the robot to shoot. Once the counter reaches 10, the robot stops.
4. **Execution (*`Shoot ball into basket`*):** Here, the loop commands the robot to take a shot, aiming the ball at the basket.
5. **Update (*`Add 1 to shotCounter`*)**: After each successful shot, the loop increments the shot counter by 1, ensuring accurate tracking of the number of shots taken.
6. **Exit Point (*`Exit`*)**: After the robot has shot ten balls, the loop concludes its task, and the robot stops shooting.

> Note: While humans start counting from 1 (1, 2, ..., 8), computers begin at 0 (0, 1, ..., 7). This way of counting is rooted in how early computer systems were designed; starting at 0 was efficient, allowing computers to optimize their memory and processing power. Over time, this zero-based method became the standard in programming. So, in coding, always remember to kick things off with zero!

### Example #2: Rocket Launch Countdown

Rocket launches are thrilling, right? They always start with that dramatic countdown: "10, 9, 8...". Let's break down how a loop might handle this!

1. **Starting Point (*`Start`*):** Our loop's exciting journey begins here, at the launch pad of our mission.
2. **Initialization (*`Set countdown to 10`*):** As we prepare for launch, the loop gets ready by setting the starting point of our countdown at 10.
3. **Condition (*`Is countdown > 0?`*):** At this checkpoint, the loop asks, "Is there still time left on the countdown?" If the countdown is still greater than 0, the loop continues with the countdown. But once it reaches 0, the loop is exited.
4. **Execution (*`Announce countdown`*)**: With every tick of the countdown, the loop announces the current number, letting everyone know how many seconds remain until launch.
5. **Update (*`Subtract 1 from countdown`*):** After each announcement, the loop decreases the 'countdown' by 1. This action ensures that we're progressing toward that exhilarating moment of blast-off.
6. **Exit Point (*`Launch the rocket`*)**: When 'countdown' hits zero, the loop's work is done, and it's time for the rocket to soar into the skies!

**Overview:** The countdown starts at 10, and with each passing second, the number decreases by 1. Once the countdown reaches 0, the rocket launches! In this case, the starting point is `countdown = 10`, the condition to check if is `countdown == 0`, and the update we do is to update `countdown - 1` every passing second.

## Nested Loops

Just as we nest boxes within larger boxes, loops can also be placed inside other loops. This is known as nesting. It's a powerful technique, especially when you need to handle multi-dimensional tasks.

[Illustration [1](https://create.roblox.com/docs/tutorials/fundamentals/coding-4/nested-loops) [2](https://study.com/academy/lesson/nested-while-loops-in-java.html) or img sent in chat]

### Nested Loop Example: Amusement Park

Imagine this: you're on a weekend trip to "WonderWorld Amusement Park" with an all-inclusive two-day ticket pass. You're super excited and have decided that on each day, you'll ride 5 different roller coasters.

This situation is a great example of nested loops. Think of the two-day weekend as the outer loop. Now, inside each day (each cycle of the outer loop), there's another loop for the five times you ride the roller coasters.

Here's a breakdown:

- Day Loop (Outer Loop): This runs for two days (Saturday and Sunday).
- Roller Coaster Ride Loop (Inner Loop): Each day, you ride five roller coasters.

The beauty of nested loops is in their simplicity. You're not doing something drastically different each time; you're repeating the same enjoyable action (riding a roller coaster) within the larger context of the weekend.

Here is what the pseudocode would look like:

```typescript
REPEAT 2 days:
    REPEAT 5 times:
        ride_roller_coaster
        look_for_another_roller_coaster
    rest
```

This logic conveys that for two days, you'll ride a roller coaster, and then decide where to go next five times each day. After those five rides, you might take a break.

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
9. Check if wall is reached. If so, exit loop.
10. Otherwise, repeat from step 1.

```typescript
REPEAT while not endOfRoom
    lift_right_foot_5cm
    move_right_foot_forward_30cm
    lower_right_foot
    transfer_weight_right
    lift_left_foot_5cm
    move_left_foot_forward_60cm
    lower_left_foot
    transfer_weight_left
```

[Illustration of flowchart diagram]

This series of commands instructs the robot on the basic mechanics of walking, step by step. You would then loop the above commands until the robot has reached the end of the room.

### Activity #2

You're working with a new generation humanoid robot that's designed for physical exercises. Unlike previous models, this robot has advanced kinesthetic intelligence, meaning it understands basic exercise commands without needing a breakdown of every movement. For instance, you don't need to instruct it with "bend your arms 90 degrees" for push-ups; you can simply command "Do a push-up", and it will perform the action. However, you cannot ask it to "Do 10 push-ups", as it can only comprehend one push-up at a time.

Instruct your robot to perform a set of 10 push-ups, followed by 10 sit-ups, and then 10 squats. The robot should then loop this set 5 times.

### Answer

To instruct our humanoid robot efficiently, we need to think step-by-step and loop-wise. We want the robot to perform a set of exercises and then repeat that whole set multiple times. This scenario is perfect for nested loops.

Let's break it down:

**Outer Loop:** Represents the entire exercise set we want the robot to repeat. We want the robot to loop through this set 5 times.

```typescript
REPEAT 5 times:
```

**Inner Loops:** Represents each exercise within the set. Since the robot can only comprehend one movement at a time, we'll use a loop for each exercise type:

Push-ups: We want the robot to do a push-up 10 times. Hence, we loop the do_pushup command 10 times.

```typescript
REPEAT 10 times:
    do_pushup
```

Similarly, we instruct the robot to repeat the do_situp and do_squat commands 10 times.

When pieced together in a nested loop structure, the pseudocode becomes:

```typescript
REPEAT 5 times:
    REPEAT 10 times:
        do_pushup
    REPEAT 10 times:
        do_situp
    REPEAT 10 times:
        do_squat
```
