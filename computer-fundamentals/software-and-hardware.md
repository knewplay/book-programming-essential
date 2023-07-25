---
title: "Computer Fundamentals: Software and Hardware"
date: "2023-07-06"
author: "Andrei Guevorkian"
---
In the previous article, we explored the history of computers and their defining characteristics. Now, let's delve deeper into general-purpose computers and their underlying concepts such as Operating Systems and file systems.

# Table of Contents

[Hardware and Software](#hardware-and-software)

[Operating System](#operating-system)

[The File System: A School Analogy](#the-file-system-a-school-analogy)

[The File System](#the-file-system)
 - [File Naming](#file-naming)
 - [File Path](#file-path)
 - [Working Directory](#working-directory)

[Questions](#questions)

# Hardware and Software

As we saw in the last article, a computer, fundamentally, consists of 4 parts:

1. the input, 
2. the processing unit, 
3. the memory (or storage), and 
4. the output.

In the context of a laptop, input devices such as the mouse, keyboard, touchpad, camera, and microphone gather data and transmit it to the computer. For example, during a Zoom meeting, your laptop's camera and microphone capture video and audio data, which is converted into digital signals (1's and 0's) for transmission to other participants' computers. The received bits are then processed (by the CPU) and displayed as an image on their screens (as output). The keyboard and touchpad/mouse are also input devices, allowing you to provide commands and interact with the computer's interface, such as clicking buttons and typing website URLs.

The processing unit, or CPU (Central Processing Unit) in a laptop, is where the computations, data manipulations and instruction executions take place, controlling the overall operation of the system.

When it comes to saving information on a laptop, there are two kinds of methods which are used together: long-term "storage" in the form of a hard disk drive (HDD) or a solid-state drive (SSD), and temporary "memory" in the form of Random Access Memory (RAM). 

> There is a difference between storage and memory when we talk about a computer. To learn more about it, I recommend you read [this short article](https://student.cs.uwaterloo.ca/~cs100/F21content/02-03-secondary-storage.html), followed by [this article](https://student.cs.uwaterloo.ca/~cs100/F21content/02-04-memory.html) containing a great analogy. However, please note that the author of the article refers to "memory" as "primary memory", and "storage" as "secondary storage". Do not get lost/confused by this terminology.

Finally, we have the output component, which presents the processed information to the user in a user-friendly format. In the case of a laptop, the primary output device is the display screen, where visual information is presented. Additionally, the laptop may have audio output capabilities through built-in speakers or headphone jacks, allowing for the playback of sound or speech. Output devices can also include printers, external monitors, or other devices that provide tangible or perceptible outputs based on the processed data.

All the devices mentioned here, such as the keyboard, the CPU, the hard drive, and the screen, are known as hardware. **Hardware** is "hard" to the touch. In other words, you can actually touch it and hold it. It's also "hard" to change it. If you buy a laptop, the components on the laptop's motherboard are soldered onto the board, making the hardware fixed. 

On the other hand, we have software. **Software** is "soft". In other words, it's not something physical that you can touch and feel. Can you "touch" a video game, or the Google search engine? Nope. It is also soft in the sense that it is not fixed; one minute you can run Microsoft Word, and then Photoshop five seconds later. It is very flexible, and can be changed or removed easily.

# Operating System

Now the question is, how do we combine hardware with software? Because software without hardware is just theory, and hardware without software is just some piece of metal worth little. You need hardware for the software to exist and have purpose, and you need software to give the hardware things to do (and have purpose).

Software is stored in the memory of a computer. You can think of the memory as having many "slots", and in each slot you can hold a certain amount of information. For simplicity, let's say that one computer instruction (a.k.a. command) can be stored in one memory slot. So if we have 10 commands, then we will need 10 different memory slots, a.k.a. memory locations, a.k.a. memory addresses. The CPU reads memory slot #1, and after executing the command there, it will go to the following memory slot, all the way up to memory slot #10, after which the program is over (a program is essentially a bunch of commands written for the CPU to execute).

Sounds simple, right? The problem is that a Mac computer, an iPhone, a Samsung smartphone, and a Lenovo laptop all use different hardware from different companies (think of the processors being made by Intel, AMD, Apple, etc.), and so they execute programs differently. On top of the internal hardware differences, we also want to connect external devices such as a mouse, keyboard, monitor, printer, and much more.

It would be ridiculous to ask software developers to write one program for Lenovo laptops, one for Apple, one for smartphones that use the Qualcomm processor, so on and so forth. Software shouldn't be "machine-specific". This is how things were in the 1970s and part of the 1980s.

To address these challenges and facilitate the seamless interaction between hardware and software, we rely on operating systems (OS). The operating system acts as an intermediary layer, bridging the gap between the hardware and software components of a computer system. In essense, an operating system is low-level software, meaning that it interacts more closely with the physical hardware components.

The operating system abstracts the complexities of hardware, providing a uniform environment for software developers to create applications. It also provides regular everyday computer users with their familiar view of the computer: the GUI, or Graphical User Interface. When we turn on a Windows computer there is a style that we expect to see, and it's a similar story when we turn on a device running macOS, iOS, or Android.

Whether it's creating a new folder on our computer, running two programs simultaneously, saving a text document on our computer, or pluging a brand new mouse into the usb, the operating system takes care of all this for us. Anything that the user shouldn't have to worry about is taken care of by the operating system. For example, when was the last time that you told the computer how to allocate its memory space, i.e. Microsoft Word should have memory slots #1 - #10000 and Adobe Photoshop should take memory slots #10001 - #21000? When was the last time you wondered where in storage you should save your essay file? Never. Just click "Save", and the operating system will take care of the rest.

All in all, operating systems play a vital role in harmonizing hardware and software components. They provide the necessary abstractions, services, and interfaces to ensure compatibility, efficient resource utilization, and seamless communication between different devices and software applications.

> Do you know of any operating systems? What kind of devices do they run on, i.e. can these operating systems run on devices made by different companies? Think of Apple devices, a Samsung smartphone, a Lenovo laptop, etc.

> What could be some reasons for why multiple operating systems exist?
P.S. Consider factors such as market demand, target user demographics, and specialized functionalities that drive the development of distinct operating systems.

The operating systems of Microsoft's Windows, Apple's macOS/iOS, and Google's Android are popular. What is less known but still as widely used (although mostly unknowingly) is Linux. To learn more about Linux, [read this](https://opensource.com/resources/linux).

# The File System: A School Analogy

Imagine this. It's 8:27AM, and you just reached your school locker. You have a strict Physics teacher who closes the classroom door at 8:30AM. No ifs, buts or maybes. You frantically turn the lock combination, open the door, and a bunch of books and papers come crashing down on your feet. You kneel down, pick up a paper, and "oh no, this ones yesterday's History quiz! This one's the Math book, ugh it looks so similar to the Physics book!"... long story short, you're late for class.

Now imagine a different scenario. It's 8:27AM, and you just reached your school locker. You turn the lock combination, open the locker, read the folder labels "History, no. Math, no. Chemistry, no. Physics, perfect!". You pull out the "Physics" folder, which you know contains everything already, lock the door, and head to class. It's 8:28AM by the way.

Continuing from this "more organized version of you", you sit down at your desk, and open the folder. Inside this "Physics" folder, you have two more folders, two notebooks, a couple of blank sheets of papers (in case there's a pop-quiz or you just want to jot something down) and the Physics book which your teacher follows. The "subfolders" are labeled "Quizzes" and "Homework", and they have notebooks and separate papers inside of them too.

Something to realize is that there is no "right" and definitive way to organize your files. You may be organized with your method, and maybe your classmate is also organized, but he has his Physics folder insider of a larger folder called "Science", which contains both "Physics" and "Chemistry" folders, and he holds his blank sheets of paper inside a "Quizzes" folder.

# The File System

Let's now transition to the computer's way of organizing files and folders. This is a crucial aspect that the operating system takes care of, ensuring that information is not all jumbled together. Remember, all data is stored as a sequence of 1's and 0's, but the operating system creates a virtual boundary between one piece of data and the next.

We have an idea of what a folder is in real life, and it's no different when it comes to computers; it's a way to separate and organize data. Sometimes, a folder is called a directory. Keep that in mind. Now what is a "file"?

> The term "folder" is a relatively new term in the computer world, introduced with the advent of the GUI. Whenever you see "directory", in your head, replace it with the word.

In the realm of computers, a file resembles the items you'd find inside your school locker. It is a named collection of data stored on a computer's storage system. Just like your school book, notebook, or piece of paper, a computer file can hold various types of information, such as text, images, videos, audio, program instructions, or configuration data.

> To get a better understanding of how computers view and represent images, [read this](http://www.lakelandscomputing.com/binary-images.html).

While folders are used to group related files together, a file is the data itself. Think of it as the content of a specific book, notebook, or piece of paper in your locker.

## File Naming

In school, if you open your Physics folder, you can distinguish between a sheet of paper and a notebook. You can see the difference, and you can touch the difference. Both contain information, but they are clearly different.

When it comes to computer files, they aren't actual objects which we can hold and say "this is a JPG image file" or "this one's a simple text file". Calling some file "image1" doesn't make it an image, because maybe it's a text file where we describe some image in text.

So, rule number one is that you must always specify the file type. How? By adding a filename extension. Foe example, "image1.png", or "image1.jpg", or "image1.txt".

> Note: Most people use applications which automatically do this for them. For example, when we write and save a Microsoft Word file, clearly it get's saved as a "doc" file. When you work with images in Adobe Photoshop, they will never suggest ".txt" as a potential filename extension. But we will see in the next series of articles how programmers use a tool where they must specify the file type themselves.

The second thing to realize is that in your Physics folder, you will not have two sheets of paper, both named "Quiz 1". That would be confusing. But if you had a notebook that's labeled "Quiz 1" and a loose sheet of paper labeled "Quiz 1", then there is some distinction and you can distinguish them. Furthermore, you can have a paper labeled "Quiz 1" in the Physics folder, and one in the History folder, and that is okay as well, as long as you don't mix the contents up.

It's a similar story with computer files. The file has a name that uniquely identifies it within a folder. So you can have a file called "quiz1.txt" in both the "Document" folder and in the "Desktop" folder, but you cannot have the exact same name within the same folder.

## File Path

If you want to review your Quiz 1 for your Physics class, there is an underlying path to get to Quiz 1: open your locker (you can think of it as a folder containing all your course folders), open the Physics folder, and grab the loose sheet of paper labeled "Quiz 1". If your folder structure is different, then you'll have to take a different path: open your locker, open the Science folder, open the Physics folder, open the Quizzes folder, then grab "Quiz 1". It all depends on the structure of the folder system.

A simple way to represent the path that you took to get to your Physics Quiz 1 in the first case is as follows: 
```
Locker > Physics > Quiz 1
``` 

In the second case, it is as follows: 

```
Locker > Science > Physics > Quizzes > Quiz 1.
```

The computer's file system works in the exact same way. Computers always have a folder called the root folder which is like the locker in the school example: a folder (or box) that contains all other folders. The root folder is denoted by a forward slash (/) on Linux and macOS, while Windows uses the drive (HDD or SSD) letter followed by a colon (e.g., "C:").

> Task: Try to find the root folder on your computer! See what it holds. Don't be afraid to Google if you don't know how!

Within the root folder, you will have subfolders. To these subfolders, the root folder is called the "parent folder", or "parent directory".

## Working Directory

Let's go back to the school analogy. Say you have the following file path to get to the Physics Quiz 1.

```
Locker > Physics > Quizzes > Quiz 1.
```

Let's now say that you are in the middle of opening your locker. In other words, you are at this step:

```
Locker > 
```

If you take a look at all the folders directly available to you, you may find folders such as Physics, Chemistry, History, Math, English, Ethics, so on and so forth. At the Locker level, you are not able to access the Quiz 1.

In order to get to the quiz, you will have to, one by one, go through the folders as follows:

```
Locker > Physics > 
```

```
Locker > Physics > Quizzes 
```

At which point you will have direct access to Quiz 1.

The working directory is the folder which you are "in" and have opened in front of you; this is the folder whose subfolders and files you can directly access. For instance, in order to access Quiz 1, the working directory had to be the Quizzes folder. In order to view all the different courses you are taking, you must go to the Locker "folder" and have that be your working directory.

# Questions
- What are some examples of hardware components in a computer?

- Can you give examples of software applications you use on a daily basis?

- (Multiple choice question) Which of the following is the OS tasked with?

    1. Memory Management: Manages computer memory, allocating and tracking memory resources for programs, ensuring efficient utilization and preventing conflicts between different processes.

    2. Process Management: Controls the execution of processes, scheduling CPU time and handling process creation and termination, ensuring fair allocation of resources and maximizing overall system performance.

    3. File System Management: Organizes and manages data storage, allowing users to create, read, write, and delete files, providing a hierarchical structure and access control for efficient data management.

    4. Device Management: Handles input and output devices, providing drivers and protocols for communication and coordinating I/O operations, ensuring seamless interaction between the computer and peripheral devices.

    5. All of the above.

    <details><summary>Hint</summary>
    The purpose of the OS is to abstract all the complex interactions between hardware and software, providing a unified interface and essential services to manage memory, processes, file systems, and devices.
    </details>

- What is the purpose of file naming conventions?