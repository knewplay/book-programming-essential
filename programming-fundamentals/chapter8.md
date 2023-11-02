---
title: "Chapter 8: Debugging and Problem Solving"
date: "2023-11-08"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - tag1: |
      q1 text
  - tag2: |
      q2 text
  - tag3: |
      q3 text
---

Debugging, or fixing errors, is a huge part of programming, even for experts. It's as crucial as writing the code itself. In this chapter, we'll concentrate on spotting and fixing errors in pseudocode, a key skill for any coder. As you improve at this, you'll become a more adept and efficient programmer.

## Table of Contents

[Recognizing Common Errors in Pseudocode](#recognizing-common-errors-in-pseudocode)

[Strategies for Identifying Errors](#strategies-for-identifying-errors)

[Correcting Errors in Pseudocode](#correcting-errors-in-pseudocode)

[Activities](#activities)

## Recognizing Common Errors in Pseudocode

## Strategies for Identifying Errors

Spotting errors in your code doesn't have to be overwhelming. With a few smart strategies, you can make the process more systematic and manageable. Here's how:

1. **Read Aloud:** Reading your code out loud can sometimes highlight issues that you might not notice while reading silently. If something sounds off, it's worth a closer look.
2. **Check for Completeness:** Go through each line of your pseudocode and ask yourself, "Does this instruction make sense?" and "Is this step complete?" Make sure each part of your pseudocode does exactly what it's supposed to do.
3. **Work Backwards:** Start from the end of your code and trace your way back. This can provide a fresh perspective and help you spot errors that you might have missed initially.
4. **Simplify Complex Statements:** Break down any long or complex instructions into smaller, manageable pieces. This can make errors more apparent and easier to fix.
5. **Peer Review:** A second pair of eyes can often catch mistakes you've missed. Ask a friend or classmate to look over your code and provide feedback.
6. **Test with Examples:** Plug in actual values and mentally walk through the steps of your code. This can help you verify whether the logic produces the expected outcome.
7. **Take a Break:** If you've been staring at your code for hours and can't seem to spot the problem, step away and come back with fresh eyes. It's amazing what a good night's sleep or even a short break can do for your problem-solving abilities. It's like hitting the restart button on your computer; sometimes, the issues just seem to fix themselves.

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

**Check for Completeness:** Each statement appears to address different temperature ranges, but is there any range missing? What happens if the temperature is exactly 30?

**Work Backwards:** Starting from the `ELSE` statement, which captures temperatures 20 and below, one might trace back to ensure all other possibilities are correctly addressed.

**Simplify Complex Statements:** The `ELIF` statement uses 'and', a logical operator that requires both conditions to be true. Make sure this logic correctly includes all intended values, especially at the boundaries.

**Peer Review:** A classmate might not spot the boundary issue immediately, but a discussion could lead to questions about temperatures at the exact transition points.

**Test with Examples:** Trying out specific temperatures like 25 or 15 might not reveal the issue, but testing the boundary values, such as 20 or 30, would highlight the gap.

**Take a Break:** If nothing stands out, a break and a fresh look later might make it obvious that you need to specify what happens at exactly 30 degrees.

## Correcting Errors in Pseudocode

## Activities
