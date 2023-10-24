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

[Anatomy of a Function](#anatomy-of-a-function)

- [Parameters and Arguments](#parameters-and-arguments)
- [Return Mechanism](#return-mechanism)

[Designing with Modularity in Mind](#designing-with-modularity-in-mind)

[Activities](#activities)

[Questions](#questions)

## Introduction to Modularization

We learned in Chapter 1 about the importance of breaking down a problem. Remember how we tackled complex challenges by splitting them into smaller, more manageable tasks? This approach mirrors a fundamental principle in the world of programming called modularization. Just as one wouldn't try to build an entire house in a single step, developers don't aim to create an entire program all at once. Instead, they break their code into smaller, self-contained pieces called modules or functions. These modules can be created, refined, and tested individually. This division not only simplifies the coding process but also makes pinpointing and fixing errors much more straightforward.

## Understanding Functions

### Analogy of a Function

Imagine a mysterious black box. You don't know what's inside it, but you're given a manual. The manual tells you what the box needs, and what it will produce. You feed the box what it asks for, and out comes a predictable result, exactly as the manual described. That's the essence of a function in programming. Like this black box, a function takes in certain inputs, processes them internally, and produces an output. You don't always need to know the intricacies of how it works inside, just what you need to give it, and what to expect in return.

Now, consider an airplane-manufacturing plant. You're outside, observing the massive building, and throughout the day, trucks come in loaded with plane parts. By the end of the day, out rolls a brand-new airplane. This entire plant can be visualized as a single function — you input plane parts, and it outputs a ready-to-fly airplane. However, as you correctly guessed, the process isn't that straightforward. Inside, workers aren't scrambling to assemble an entire airplane in one place. The plant is divided into sections, or "sub-functions" if you will. One section assembles the wings, another the fuselage, yet another the engines, and so on. Each section specializes in one aspect, doing its job efficiently. In the end, all these components are combined, resulting in a finished airplane. This reflects the essence of modularization.

Much like the specialized sections in the airplane-manufacturing plant, functions in programming allow developers to break down complex tasks into smaller, more manageable pieces. This not only makes the code more organized but also easier to debug, maintain, and reuse.

[Illustration of [industrial machine which takes in something and outputs something else](https://content.presentermedia.com/content/clipart/00019000/19074/process_conversion_300_nwm.jpg), and on top of it have [illustration of function](https://res.cloudinary.com/practicaldev/image/fetch/s--4bEYLci3--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/kq34mrtitnuolaulcpfz.png)]

### Importance of a Function

Cleaner Code: Modules allow for a clear separation of concerns. Each module handles a specific piece of functionality, making the code within it more focused and easier to understand. When you or someone else revisits the code, it's straightforward to pinpoint where changes or fixes need to be made.

Enhanced Maintainability: As software grows and evolves, modifications become inevitable. With a modular structure, updates can be made to one module without disturbing others. This isolation minimizes unexpected bugs and reduces the risk of unintended consequences elsewhere in the program.

In essence, modularization brings structure and clarity to the programming process. By compartmentalizing tasks and functionalities, we ensure a smoother development experience and pave the way for more robust and maintainable software solutions.

## Anatomy of a Function

Explain in pseudocode

### Parameters and Arguments
I/O

### Return Mechanism

## Designing with Modularity in Mind

Provide clear example w/o use of functions, and then with the use of functions.

## Activities

**Activity #1:**

have student design functions to complete a large task.  Something intuitive