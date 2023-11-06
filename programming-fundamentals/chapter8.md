---
title: "Chapter 8: Debugging and Problem Solving"
date: "2023-11-08"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - top-three: |
      In your opinion, what are the 3 most commonly used debugging techniques?
  - robot-move: |
      Imagine you have a little robot that can move forward or backward when you press one of two buttons. The "Forward" button should make the robot step forward, and the "Backward" button should make it step backward. Write down the steps (in pseudocode) that describe what the robot should do, inside an infinite loop, so that it continuously responds to the button presses. Then, can you introduce a bug on purpose so that when you press the "Backward" button, the robot moves forward instead?
  - describe-weather: |
      Imagine you're programming your very own weather robot. Your task is to write a function that checks the temperature and tells you how the weather feels. The function will take one input: the temperature in degrees Celsius. It will return a description of the weather, which can be "Too Hot," "Hot," "Just Perfect," "Cold," or "Too Cold." You get to decide what temperature ranges correspond to each of these descriptions.

      Remember to name your function and clearly define the temperature ranges for each description.
---

Debugging, or fixing errors, is a huge part of programming, even for experts. It's as crucial as writing the code itself. In this chapter, we'll concentrate on spotting and fixing errors in pseudocode, a key skill for any coder. As you improve at this, you'll become a more adept and efficient programmer.

## Table of Contents

[Recognizing Common Errors in Pseudocode](#recognizing-common-errors-in-pseudocode)

- [Spelling and Syntax Errors](#spelling-and-syntax-errors)
- [Logic Errors](#logic-errors)
- [Runtime Errors](#runtime-errors)

[Strategies for Identifying Errors](#strategies-for-identifying-errors)

[Activities](#activities)

[Questions](#questions)

## Recognizing Common Errors in Pseudocode

When you're learning a new language, it's normal to make mistakes. Let's take a look at some of the common types of errors you might encounter in writing code:

### Spelling and Syntax Errors

These are the easiest to spot and fix. They happen when you misspell a command or forget to include a necessary part of the code structure. For example:

**Incorrect Pseudocode:**

```typescript
IF x > 10
    PRIT "X is a big number!"
```

Can you spot the mistake?

**Corrected Pseudocode:**

```typescript
IF x > 10
    PRINT "X is a big number!"
```

### Logic Errors

These can be trickier. Logic errors happen when your pseudocode doesn't do what you intend it to do. Here's an example:

**Incorrect Pseudocode:**

```typescript
IF x < 10
    PRINT "X is a big number!"
ELSE
    PRINT "X is a small number!"
```

The messages are mixed up! If x is less than 10, it should say that it's a small number.

**Corrected Pseudocode:**

```typescript
IF x < 10
    PRINT "X is a small number!"
ELSE
    PRINT "X is a big number!"
```

### Runtime Errors

Runtime errors are like unexpected pitfalls that crop up while your program is running, hence the name "runtime". They can be particularly tricky because your code looks correct at first glance, but when you try to run it, things don't work as expected. For instance:

**Incorrect Pseudocode:**

```typescript
x = 5
result = x / 0
PRINT result
```

Dividing by zero is something you just can't do—it's like trying to share five cookies with zero friends. It just doesn't work!

By being able to recognize these common errors in pseudocode, you're well on your way to becoming a more efficient and effective programmer. All it takes is some practice.

## Strategies for Identifying Errors

Next, we'll explore strategies for identifying errors in your code.

Spotting errors in your code doesn't have to be overwhelming. With a few smart strategies, you can make the process more systematic and manageable. Here's how:

1. **Read Aloud:** Reading your code out loud can sometimes highlight issues that you might not notice while reading silently. If something sounds off, it's worth a closer look.
2. **Check for Completeness and Edge Cases:** Go through each line of your pseudocode and ask yourself, "Does this instruction make sense?" and "Is this step complete?". Ensure that you've considered the boundary values or extreme scenarios, making sure each part of your pseudocode does exactly what it's supposed to do.
3. **Simplify Complex Statements:** Break down any long or complex instructions into smaller, manageable pieces. This can make errors more apparent and easier to fix.
4. **Peer Review:** A second pair of eyes can often catch mistakes you've missed. Ask a friend or classmate to look over your code and provide feedback.
5. **Test with Examples:** Plug in actual values and mentally walk through the steps of your code. This can help you verify whether the logic produces the expected outcome.
6. **Take a Break:** If you've been staring at your code for hours and can't seem to spot the problem, step away and come back with fresh eyes. It's amazing what a good night's sleep or even a short break can do for your problem-solving abilities. It's like hitting the restart button on your computer; sometimes, the issues just seem to fix themselves.

To illustrate, let's consider a simple piece of pseudocode:

```typescript
IF temperature > 30
    PRINT "It's hot outside!"
ELIF temperature > 20 and temperature < 30
    PRINT "It's warm outside!"
ELSE
    PRINT "It's a cold day."
```

Using our strategies:

**Read Aloud:** "*If temperature is greater than 30, print 'It's hot outside!' Else if temperature is greater than 20 and less than 30, print 'It's warm outside!' Otherwise, print 'It's cold outside.'*" Reading this aloud, everything seems in place at first glance.

**Check for Completeness and Edge Cases:** Each statement appears to address different temperature ranges, but is there any range missing? What happens if the temperature is exactly 20? What about 30?

**Simplify Complex Statements:** The `ELIF` statement uses 'and', a logical operator that requires both conditions to be true. Make sure this logic correctly includes all intended values, especially at the boundaries.

**Peer Review:** A classmate might not spot the boundary issue immediately, but a discussion could lead to questions about temperatures at the edge cases.

**Test with Examples:** Trying out specific temperatures like 25 or 15 might not reveal the issue, but testing the boundary values, such as 20 or 30, would highlight the gap.

**Take a Break:** If nothing stands out, a break and a fresh look later might make it obvious that you need to specify what happens at exactly 30 degrees.

## Activities

**Activity #1:**

Your friend wrote the following code:

```typescript
x = INPUT
IF x < 10
    PRINT "x is less than 10"
ELSE IF x < 5
    PRINT "x is less than 5"
ELSE
    PRINT "x is not less than 10 and 5"
```

Are there any problems with this code? Explain.

**Answer:**

The code your friend wrote doesn't work as intended. To figure out why, we need to test it with a variety of numbers, especially paying attention to the edge cases - the points at which the behavior of the program might change.

Let's run through some numbers:

- **Above 10 (e.g., 12):** It prints "x is not less than 10 and 5". This is correct.
- **Exactly 10:** It prints "x is not less than 10 and 5". This is correct.
- **Between 5 and 10 (e.g., 8):** It prints "x is less than 10". This is correct.
- **Exactly 5:** It prints "x is less than 10". This is correct.
- **Below 5 (e.g., 3):** It prints "x is less than 10" instead of printing "x is less than 5", which is what we actually want. This is a case that the code fails to handle correctly.

The flaw lies in the sequence of the conditions. When we input a number, for example, 3, the program first checks if `x < 10`. Since 3 is indeed less than 10, the program outputs "x is less than 10" and bypasses the subsequent conditions. As a result, the second condition `ELSE IF x < 5` is never executed, which means the program will never print "x is less than 5", even though it's accurate.

The code should be rearranged so that it checks for the smaller value first. Here's a corrected version:

```typescript
x = INPUT
IF x < 5
    PRINT "x is less than 5"
ELSE IF x < 10
    PRINT "x is less than 10"
ELSE
    PRINT "x is not less than 10 and 5"
```

Now, the code checks if `x` is less than 5 first. If it's not, then it checks if it's less than 10. This way, all possibilities are covered correctly.

**Activity #2:**

Your friend was asked to write a program that will count numbers from 1 to 10. They wrote the following code:

```typescript
i = 1         // Initialize variable i
WHILE i < 10
    PRINT i   // Display i onto the screen
    i = i + 1 // Increment i by 1
END WHILE
```

Comment on this code. Does it do what it is intended to do? What would you change, if anything?

**Answer:**

The code is close to achieving the goal but falls short due to a common oversight. It's meant to count from 1 to 10, yet it stops at 9. The loop's condition, i < 10, causes it to halt prematurely.

To better understand and catch such issues, it's essential to mentally simulate the program's execution, especially paying attention to edge cases. Let's mentally run the code:

- Start with `i = 1`, the loop runs, and it prints 1.
- Then `i` becomes 2, and so forth. It's clear that the pattern continues.
- Fast forward to when `i = 8` and then `i = 9`, everything works as expected.
- But at `i = 10`, the loop condition `i < 10` is no longer true, so the loop stops, and 10 isn't printed. This is an edge case, i.e. the boundaries of our counting range.

To correct this, we can change the loop's condition to `i <= 10` so that it includes 10 in the count. The revised code looks like this:

```typescript
i = 1         // Initialize variable i
WHILE i <= 10
    PRINT i   // Display i onto the screen
    i = i + 1 // Increment i by 1
END WHILE
```

Now, if you mentally run through the code again, you'll see that it counts all the way up to 10, fixing the original issue and ensuring that the program works as intended.
