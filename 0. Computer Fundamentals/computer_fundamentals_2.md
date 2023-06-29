---
title: "Computer Fundamentals: The Operating and File System"
date: "07-06-2023"
author: "Andrei Guevorkian"
---
In the previous article, we explored the fascinating history of computers and their defining characteristics. Now, let's delve deeper into general-purpose computers and their underlying concepts such as Operating Systems and file systems.

# Table of Contents

[Hardware and Software](#hardware-and-software)

[Operating System](#operating-system)

[The File System: A School Analogy](#the-file-system-a-school-analogy)

[The File System](#the-file-system)

# Hardware and Software

As we saw in the last article, a computer, fundamentally, consists of 4 parts:
1. the input, 
2. the processing unit, 
3. the memory (or storage), and 
4. the output.

In the context of a laptop, input devices such as the mouse, keyboard, touchpad, camera, and microphone gather data and transmit it to the computer. For example, during a Zoom meeting, your laptop's camera and microphone capture video and audio data, which is converted into digital signals (1's and 0's) for transmission to other participants' computers. The received bits are then processed (by the CPU) and displayed as an image on their screens (as output). The keyboard and touchpad/mouse are also input devices, allowing you to provide commands and interact with the computer's interface, such as clicking buttons and typing website URLs.

The processing unit, or CPU (central processing unit) in a laptop, is where the computations, data manipulations and instruction executions take place, controlling the overall operation of the system.

When it comes to saving information on a laptop, there are two kinds of methods which are used together: long-term "storage" in the form of a hard disk drive (HDD) or a solid-state drive (SSD), and temporary "memory" in the form of Random Access Memory (RAM).

Finally, we have the output component, which presents the processed information to the user in a user-friendly format. In the case of a laptop, the primary output device is the display screen, where visual information is presented. Additionally, the laptop may have audio output capabilities through built-in speakers or headphone jacks, allowing for the playback of sound or speech. Output devices can also include printers, external monitors, or other devices that provide tangible or perceptible outputs based on the processed data.

All the devices mentioned here, such as the keyboard, the CPU, the hard drive, and the screen, are known as hardware. **Hardware** is "hard" to the touch. In other words, you can actually touch it and hold it. It's also "hard" to change it. If you buy a laptop, the components on the laptop's motherboard are soldered onto the board, making the hardware fixed. 

On the other hand, we have software. **Software** is "soft". In other words, it's not something physical that you can touch and feel. It is also soft in the sense that it is not fixed; one minute you can run Microsoft Word, and then Photoshop five seconds later. It is very flexible, and can be changed or removed easily.

# Operating System

Now the question is, how do we combine hardware with software? Because software without hardware is nothing, and hardware without software is just some piece of metal incapable of anything. You need hardware for the software to exist and to do something, and you need software to give the hardware things to do.

Software is stored in the memory of a computer. You can think of your memory as having memory "slots", and in each slot you can hold a certain amount of information. For simplicity, let's say that one computer instruction (a.k.a. command) can be stored in one memory slot. So if we have 10 commands, then they will be stored in 10 different memory slots, a.k.a. memory locations, a.k.a. memory addresses. The CPU reads memory slot #1, and after executing the command there, it will go to the following memory slot, all the way up to memory slot #10, after which the program is complete (a program is essentially a bunch of commands written for the CPU to execute).

Now let's say I want to write a text editor, something like Microsoft Word. Sure, my application will be able to write and edit text, add and delete images, undo the last action, so on and so forth. Now let's focus on the "write text" portion. How does the computer know that when I press 'P' on my keyboard, this means that 'p' should appear on my screen. Sure, the button says 'P', but that is just printed onto the button. Someone had to have written a program that says "this button on the keyboard corresponds to this letter". That is where the OS comes in.

a computer program that will take the user's keyboard presses, and translate that into text.
Imagine we are in the 1970s, and we happen to have access to a computer. Let's think of some programs (software) that we could write on our computer (hardware). Let's say we want to write a novel. Since it's the 1970s, Microsoft Word doesn't exist yet. To write out a novel on the computer, we need to write a program that will convert a key press into a letter on the screen. So if I press on 'P' on my keyboard, I should see the letter 'p' appear on the screen. I'd have to I'd first have to make a text-editor software, within which I can write my text and add illustrations. So in order to write text, I'd have to connect the keyboard presses,  It should ideally have some buttons which can let me save the text into a file, or "undo" a typo I made. 

Now let's say that I finished writing my book, and

We could make a text-editor program, that allows us to type text and save the text in a file on our computer. We can make a chess 

Taking any computer, whether it's a home desktop PC (personal computer), or a mini-computer powering a robot, 
Essentially, the CPU is waiting for things to do; it's waiting to get instructions on what calculations to perform.

At the most fundamental level, if we have a piece of hardware that is designed to be able to execute "general-purpose" code, then it should 

hardware and software. this will lay a foundation for them that terminal, git, programming, all these things are software
firmware is what connects them. have drivers to help connect external devices to the computer. OS manages all of this -->

Manage/coordinate resources, Hide complexities that we don't need the everyday user to see and interact with. -> GUI

Add recommended reading for details about windows OS

So far we agree that there is a computational complexity spectrum for computers, where on the lower extreme we have some embedded device that is programmable but is limited in its capabilities, and on the other end, we have something like a supercomputer that can process and store ridiculous amounts of data in record-breaking time.

But a computer could have the best CPU in the world, but not be used to its full potential. This all depends on the software.
But no matter the computer's complexity

Mention about the modern OS:
Now talk about how to organize everything, drivers, etc. you want a special software that will manage all of those things that we don't need the user to manage. 


Now the big question is, how are hardware and software linked? How do you run large software programs on compact hardware devices.

Why many flavors. why mac windows linux. whats different. why have OS

hw > OS > Apps > programmer

OS > file system, network, memory, process, multiprocess

# The File System: A School Analogy

what is file (review), what is direcotyr, why need to change it. what is the current working directory, ...

single-level directory
two-level directory => need to navigate

# The File System 
Analogy: can have one big notebook, with history math and physics and chemistry notes. However, we all know that it's much easier to sort through things by having a separate notebook for each subject.
Now what if in history class, you have your notebook with your class notes, but one day the teacher asks you to take out a single piece of paper for the weekly quiz. Now you have a notebook, and a single piece of paper. after 8 weeks, you would have 8 single pieces of paper, which should logically be physically together. You don't want history quiz 1 to be between the math and physics notebooks. That'd be a mess when it's time to find the quiz and review it. --> Folder ...
go back to the profile picture example. or the game graphics. behind all of these visuals, is computer code. and code is just text that get's converted to machine code that the computer can understand.  
For the profile picture, that picture is stored somewhere on facebook's server, and when someone visits your account, the page just has a pointer to the location on the server where your picture resides. its a file. everything is stored in files. A typical program executes sequentially, one command at a time. so technically can have one big chunck of code. but that's just like having one large notebook containing all your class notes from all your courses. and computers have way more information than a year's worth of class notes. computers are very complex today, and it's better to organize and store the different funcitonalities into separate files, just like it's better to put different course material in different folders.

