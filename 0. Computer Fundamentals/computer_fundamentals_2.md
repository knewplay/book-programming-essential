---
title: "Computer Fundamentals: The File System"
date: "07-06-2023"
author: "Andrei Guevorkian"
---
In the previous article, we explored the fascinating history of computers and their defining characteristics. Now, let's delve deeper into general-purpose computers and their underlying concepts such as Operating Systems and file systems.

# Table of Contents

[Hardware and Software](#)

talk about the computational complexity spectrum, what are the extremes (maybe). talk about software and hardware, talk how can connect external devices using drivers. can get complicated. 


Mention about the modern OS:
Now talk about how to organize everything, drivers, etc. you want a special software that will manage all of those things that we don't need the user to manage. 


[The File System](#the-file-system)

# Deconstructing a Laptop

As we saw in the last article, a computer, fundamentally, consists of 4 parts: 
1. the input, 
2. the processing unit, 
3. the memory (or storage), and 
4. the output.

In the context of a laptop, input devices such as the mouse, keyboard, touchpad, camera, and microphone gather data and transmit it to the computer. For example, during a Zoom meeting, your laptop's camera and microphone capture video and audio data, which is converted into digital signals (1's and 0's) for transmission to other participants' computers. The received bits are then processed and displayed as an image on their screens. The keyboard and touchpad/mouse are also input devices, allowing you to provide commands and interact with the computer's interface, such as clicking buttons and typing website URLs.

The processing unit, or CPU (central processing unit) in a laptop, is where the computations, data manipulations and instruction executions take place, controlling the overall operation of the system.

When it comes to saving information on a laptop, there are two kinds of methods which are used together: long-term "storage" in the form of a hard disk drive (HDD) or a solid-state drive (SSD), and temporary "memory" in the form of Random Access Memory (RAM).

Finally, we have the output component, which presents the processed information to the user in a usable form. In the case of a laptop, the primary output device is the display screen, where visual information is presented. Additionally, the laptop may have audio output capabilities through built-in speakers or headphone jacks, allowing for the playback of sound or speech. Output devices can also include printers, external monitors, or other devices that provide tangible or perceptible outputs based on the processed data.

All the devices which we saw here, such as the keyboard, the CPU, the hard drive, and the screen, are known as hardware. Hardware is "hard" to the touch. In other words, you can actually touch it and hold it. It's also "hard" to change it. If you buy a laptop, the components on the laptop's motherboard are soldered into the board, making the hardware fixed. On the other hand, we have software. Software is "soft". In other words, it's not something physical that you can touch and feel. It is also soft in the sense that it is not fixed; one minute you can run Microsoft Word, and then Photoshop five seconds later. It is very flexible, and can be changed or removed easily.

# Operating Systems

Why many flavors. why mac windows linux. whats different. why have OS

hw > OS > Apps > programmer

OS > file system, network, memory, process, multiprocess

# School Analogy

what is file (review), what is direcotyr, why need to change it. what is the current working directory, ...

single-level directory
two-level directory => need to navigate

# Files and Folders in the Digital World

# The File System 
Analogy: can have one big notebook, with history math and physics and chemistry notes. However, we all know that it's much easier to sort through things by having a separate notebook for each subject.
Now what if in history class, you have your notebook with your class notes, but one day the teacher asks you to take out a single piece of paper for the weekly quiz. Now you have a notebook, and a single piece of paper. after 8 weeks, you would have 8 single pieces of paper, which should logically be physically together. You don't want history quiz 1 to be between the math and physics notebooks. That'd be a mess when it's time to find the quiz and review it. --> Folder ...
go back to the profile picture example. or the game graphics. behind all of these visuals, is computer code. and code is just text that get's converted to machine code that the computer can understand.  
For the profile picture, that picture is stored somewhere on facebook's server, and when someone visits your account, the page just has a pointer to the location on the server where your picture resides. its a file. everything is stored in files. A typical program executes sequentially, one command at a time. so technically can have one big chunck of code. but that's just like having one large notebook containing all your class notes from all your courses. and computers have way more information than a year's worth of class notes. computers are very complex today, and it's better to organize and store the different funcitonalities into separate files, just like it's better to put different course material in different folders.

