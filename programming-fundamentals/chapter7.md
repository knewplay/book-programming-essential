---
title: "Chapter 7: Putting It All Together"
date: "2023-11-02"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - tag1: |
      q1 text,
  - tag2: |
      q2 text.
  - tag3: |
      q3 text.
---

Now that we've gone over everything from breaking down problems to using data types, loops, and functions, it's time to put all these pieces together. In this chapter, we're going to combine everything you've learned and build a complete program.

## Table of Contents

[Arithmetic Operations in Programming](#arithmetic-operations-in-programming)

[Example 1: Celsius to Fahrenheit Converter](#example-1-celsius-to-fahrenheit-converter)

[Example 2: Even or Odd](#example-2-even-or-odd)

[Example 3: A Basic Calculator](#example-3-a-basic-calculator)

[Example 4: Something with loopings](#example-4-something-with-looping)

[Activities](#activities)

[Questions](#questions)

## Arithmetic Operations in Programming

When you think of math, the first things that probably come to mind are the basic arithmetic operations. In programming, these operations are just as essential. Let's dive into each of them:

- **\+** : Addition: `3 + 5 = 8`
- **\-** : Subtraction: `9 - 4 = 5`
- **\*** : Multiplication: `4 * 6 = 24`
- **/** : Division: `12 / 3 = 4`

## Example Problems

In this section, we're going to tackle a set of example problems that will take us back through everything we've learned so far. We'll start with simpler examples and gradually ramp up the challenge.

### Example 1: Celsius to Fahrenheit Converter

**Question:** Write a function that converts Celsius temperature to Fahrenheit. After creating this function, demonstrate its use by providing a test case.

**Answer:**

To solve this, it's important to understand the relationship between Celsius and Fahrenheit. To convert Celsius to Fahrenheit, you multiply the Celsius temperature by 9/5 and then add 32. In mathematical terms, the formula is: **Fahrenheit = (Celsius × 9/5) + 32**.

**Pseudocode:**

```typescript
FUNCTION ConvertToFahrenheit(celsius):
    fahrenheit = celsius * 9/5 + 32
    RETURN fahrenheit
```

**Explanation:**

For the `ConvertToFahrenheit` function, the name itself gives away its purpose: to convert a given temperature from Celsius to Fahrenheit. Inside the parentheses, we have a parameter named `celsius`, which is the input temperature we want to convert. Within the function, we use a variable named `fahrenheit` to store the result of our conversion. The math behind this conversion is done using the formula `celsius * 9/5 + 32`, a standard way to change Celsius to Fahrenheit. After the calculation, the function then provides the converted temperature using the `RETURN` statement. Essentially, this function takes in a Celsius value, performs the necessary calculations, and then hands back the Fahrenheit equivalent.

**Function call:**

If we want to test this function, we could call it and pass it an argument, like so:

```typescript
ConvertToFahrenheit(10)
```

On execution, the call `ConvertToFahrenheit(10)` should yield a result of `50` Fahrenheit.

### Example 2: Even or Odd

**Question:** Design a function to identify whether a given integer is even or odd. Create the solution using loops, and afterwards, demonstrate the function with a test case.

**Answer:**

To figure out if a number is even or odd using loops, we'll subtract 2 from the number repeatedly until it becomes less than 2. If the result is 0, then the number is even; otherwise, it's odd.

**Pseudocode:**

```typescript
FUNCTION IsEvenOrOdd(number):
    WHILE number >= 2:
        number = number - 2
    IF number == 0:
        RETURN "Even"
    ELSE:
        RETURN "Odd"
```

**Explanation:**

Think of it like this: if you had 7 apples and you kept giving 2 away at a time, you'd be left with 1 apple. Any time you have 1 apple left (or any number not evenly divisible by 2), that means you started with an odd number. On the other hand, if you kept giving away 2 apples at a time and ended up with none left, you had an even number of apples to start with.

In our loop, we kept subtracting 2 until the number became less than 2. If, after all the subtractions, the number is 0, that means the original number was even. If it's not 0, then it's surely 1. And that's why in our "else" condition, we can confidently say the number is odd.

**Function call:**

To test our function:

```typescript
IsEvenOrOdd(7)
```

Running the above code, `IsEvenOrOdd(7)` should output `Odd`.

### Example 3: A Basic Calculator

### Example 4: Something with looping

## Activities
