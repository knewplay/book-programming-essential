---
title: "Chapter 6: Modularizing Your Code with Functions"
date: "2023-10-26"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
- birthday-song: 
Happy Birthday song is repetitive. have a function call for the "Happy birthday to you" line. Write the happy birthday song in pseudocode.
---

In daily tasks, we often break things down into steps: making a sandwich involves selecting ingredients, assembling, and finally eating. Similarly, in programming, we modularize our code using "functions", turning complex tasks into manageable, step-by-step processes.

## Table of Contents

[Introduction to Modularization](#introduction-to-modularization)

[Understanding Functions](#understanding-functions)

[Benefits of Using Functions](#benefits-of-using-functions)

[Anatomy of a Function](#anatomy-of-a-function)

- [Function Definition and its Parameters](#function-definition-and-its-parameters)
- [Function Call and its Arguments](#function-call-and-its-arguments)
- [Return Mechanism](#return-mechanism)

[Designing with Modularity in Mind](#designing-with-modularity-in-mind)

[Activities](#activities)

[Questions](#questions)

## Introduction to Modularization

We learned in Chapter 1 about the importance of breaking down a problem. We learned to tackled complex challenges by splitting them into smaller, more manageable tasks. This approach mirrors a fundamental principle in the world of programming called modularization. Just as one wouldn't try to build an entire house in a single step, developers don't aim to create an entire program all at once. Instead, they break their code into smaller, self-contained pieces called modules or functions. These modules can be created, refined, and tested individually. This division not only simplifies the coding process but also makes pinpointing and fixing errors much more straightforward.

## Understanding Functions

Imagine a mysterious black box. You don't know what's inside it, but you're given a manual which tells you what the box needs, and what it will produce. You feed the box what it asks for, and out comes a predictable result, exactly as the manual described. That's the essence of a function in programming. Like this black box, a function takes in certain inputs, processes them internally, and produces an output. You don't always need to know the intricacies of how it works inside, just what you need to give it, and what to expect in return.

[Illustration of [industrial machine/BLACK BOX which takes in something and outputs something else](https://content.presentermedia.com/content/clipart/00019000/19074/process_conversion_300_nwm.jpg), and on top of it have [illustration of function](https://res.cloudinary.com/practicaldev/image/fetch/s--4bEYLci3--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/kq34mrtitnuolaulcpfz.png)]

Now, consider an airplane-manufacturing plant. You're outside, observing the massive building, and throughout the day, trucks come in loaded with plane parts. By the end of the day, out rolls a brand-new airplane. This entire plant can be visualized as a single function: you input plane parts, and it outputs a ready-to-fly airplane.

[Illustration of building, with plane parts going in, and a plane coming out]

However, as you correctly guessed, the process isn't that straightforward. Inside, workers aren't scrambling to assemble an entire airplane in one place. The plant is divided into sections. One section assembles the wings, another the fuselage, yet another the engines, and so on. Each section specializes in one aspect, doing its job efficiently. In the end, all these components are combined, resulting in a finished airplane. This reflects the essence of modularization.

[Illustration of inside the building (maybe have building be transparent, we can see its silhouette) with different components being produced.
OR Somehow show that the pieces that come in from the trucks, then get distributed/separated into different sections.]

[OR illustration of the entire building being one large function, and inside have sub-functions]

Much like the specialized sections in the airplane-manufacturing plant, functions in programming allow developers to break down complex tasks into smaller, more manageable pieces. This not only makes the code more organized but also easier to debug, maintain, and reuse.

### Benefits of Using Functions

When I described to you this airplane-manufacturing plant, I hope to have given to you the picture that it is very organized thanks to the different sections. Each section has its own workspace, tools, and materials, ensuring that there's no clutter. When each section is clean and organized, the whole process runs smoother and more efficiently.

Similarly, in programming, by having separate functions for different tasks, the code is 'cleaner'. It's organized in a way that's easier to read and understand, just like an organized workspace makes it easier to build an airplane.

Now imagine that one day, at this airplane-manufacturing plant, a batch of airplane tires were found to be defective. Instead of halting the entire assembly line, the tire section just focuses on addressing that particular issue. Meanwhile, the wings, engines, and other parts continue to be built as usual.

Similarly, in programming, when there's an issue in a specific part of the program, you can dive into that specific function to fix it, without having to touch the rest of the code. It's easier to maintain, and its easier to pinpoint where changes or fixes need to be made in case of an error.

Furthermore, as your program grows and evolves, modifications become inevitable. With a modular structure, updates can be made to one module without disturbing others.

In essence, modularization brings structure and clarity to the programming process. By modularizing tasks and functionalities, we ensure a smoother development experience and pave the way for more robust and maintainable software solutions.

## Anatomy of a Function

Now that we've seen the overall system, let’s dive deeper to understand one of its core sections: the fuselage assembly area. This is where the main body of the plane gets pieced together.

### Function Definition and its Parameters

Imagine a section of the plant where the fuselage is assembled. Before assembly starts, the fuselage-assembly team needs some key details like the size of the airplane (small, medium, large) and the number of windows it should have. Without these details, the fuselage-assembly team cannot do their work. Because remember, we have purposefully separated the plane building process, so one group does not have direct access to what the other groups are doing. They are all working independently. So this information needs to be fed to them from the general manager.

In programming, it's the same story. The programmer (general manager) needs to provide the "input" to the function in order for the function to do its job. And these inputs are known as "parameters".

For our fuselage assembly example, the code might look like this:

```typescript
FUNCTION AssembleFuselage(size, numberOfWindows)
    // Here the fuselage gets assembled.
END FUNCTION
```

- `FUNCTION`: This is a keyword indicating that we're defining a new function. Think of it as announcing, "Hey, we're setting up a new section of the assembly line here!"
- `AssembleFuselage`: This is the name of the function, much like naming the "fuselage assembly" section. By using this name in our code, we can instruct the function to start its task, just as a project manager would say *"Hey Fuselage-Assembly team, get to work!"*
- `(size, numberOfWindows)`: Inside these parentheses, we have our parameters – the essential details the function needs. In this case, the two parameters are:
- `size`: This parameter expects a value that indicates the size of the airplane, like "small", "medium", or "large".
- `numberOfWindows`: This parameter expects a number, indicating how many windows the fuselage should have.
Think of these parameters as the instruction manual or blueprint for the fuselage assembly team. Without these specifics, the team won't know how to proceed.
- `// Here the fuselage gets assembled.`: This is a comment in the pseudocode. It doesn't affect the functionality but is a note to anyone reading the code (or for our analogy, a reminder for the assembly team) about what happens in this section of the function. In a real code setting, this is where the steps or operations to assemble the fuselage would be detailed.
- `END FUNCTION`: This keyword indicates the function's conclusion. It's a signal that the process defined in this function is complete. Think of it as the signal that the fuselage assembly job is complete.

The beauty of this approach is that once this function is set up, we can call upon it multiple times with various inputs. If we need a large plane with 20 windows, we simply provide those specific details (arguments) when we call the function. It's like telling the assembly team to start a new project with a new set of blueprints.

### Function Call and its Arguments

### Return Mechanism

## Designing with Modularity in Mind

Provide clear example w/o use of functions, and then with the use of functions.

## Activities

**Activity #1:**

have student design functions to complete a large task.  Something they are familiar with and have an intuition for.

**Activity #2:**

Pseudocode of 3 functions, and make functions calls.
