---
title: "Chapter 6: Modularizing Your Code with Functions"
date: "2023-10-26"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
---

In daily tasks, we often break things down into steps: making a sandwich involves selecting ingredients, assembling, and finally eating. Similarly, in programming, we modularize our code using "functions", turning complex tasks into manageable, step-by-step processes.

## Table of Contents

[Introduction to Modularization](#introduction-to-modularization)

[Understanding Functions](#understanding-functions)

- [Analogy of a Function](#analogy-of-a-function)
- [Importance of a Function](#importance-of-a-function)
- [Anatomy of a Function](#anatomy-of-a-function)

[Designing with Modularity in Mind](#designing-with-modularity-in-mind)
[Activities](#activities)

[Questions](#questions)

## Introduction to Modularization

We learned in Chapter 1 about the importance of breaking down a problem. ...

## Understanding Functions

### Analogy of a Function

Blackbox system. Don't need to know the inner workings in order to use it. As long as you know give what the device needs, it will do its thing and output the final product.

Give analogy of airplane-making plant. One day, you decide to sit by the plant, and watch what goes in and out for the entire day. In the morning and early afternoon, you see trucks bringing various plane parts. Occasionally, you see a complete plane coming out of it from the back. You can think of the entire building as one large function. It gets pieces to come in, and a completed airplane comes out. But we know, looking from the outside, that the workers inside aren't just assembling all the pieces in one shot. There are different divisions. One group is working on assembling the wings, one on the main frame, one on XYZ. And then all those pieces come together. So there are multiple "mini-powerplants" inside the building which all work separately, but they do come back together to build and complete the overall plane. Imagine 1000 people in your class. Could you imagine everyone working on one thing? No. Instead, you split up into smaller groups (2-4 people is usually manageable), and then when you all complete your own parts, you combine your work together to get the final project.

[Illustration of [industrial machine which takes in something and outputs something else](https://content.presentermedia.com/content/clipart/00019000/19074/process_conversion_300_nwm.jpg), and on top of it have [illustration of function](https://res.cloudinary.com/practicaldev/image/fetch/s--4bEYLci3--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/kq34mrtitnuolaulcpfz.png)]

### Importance of a Function

Cleaner Code: Modules allow for a clear separation of concerns. Each module handles a specific piece of functionality, making the code within it more focused and easier to understand. When you or someone else revisits the code, it's straightforward to pinpoint where changes or fixes need to be made.

Enhanced Maintainability: As software grows and evolves, modifications become inevitable. With a modular structure, updates can be made to one module without disturbing others. This isolation minimizes unexpected bugs and reduces the risk of unintended consequences elsewhere in the program.

In essence, modularization brings structure and clarity to the programming process. By compartmentalizing tasks and functionalities, we ensure a smoother development experience and pave the way for more robust and maintainable software solutions.

### Anatomy of a Function

Explain in pseudocode

#### Arguments, parameters, input output, return

## Designing with Modularity in Mind

## Activities

**Activity #1:**

have student design functions to complete a large task.  Something intuitive