---
title: "Toolset"
date: "31-07-2023"
author: "Andrei Guevorkian"
---
Just as a master carpenter skillfully wields their tools to shape exquisite furniture or a painter expertly selects brushes and colors to create captivating artwork, programmers harness a collection of specialized tools to craft intricate software systems. Let's explore the essential tools that empower programmers to shape the digital world.

# Table of Contents

[Terminal](#terminal)

[Git](#git)

[Search Engine](#google-search)

[Code Editor](#code-editor)


# Terminal
Have you ever seen a movie where a hacker is frantically typing bright green letters on a black screen? Have you ever wanted to do that? As it turns out, that black screen isn't just a Hollywood invention; it really does exist, and it's called a **terminal**. 

## Importance

Back in the days, knowing how to use a terminal was absolutely necessary to communicate with the computer. Today, almost everyone uses the GUI exclusively. That is everyone except for programmers and IT professionals.

To understand why the terminal is important, we must recognize that all programs are ultimately a series of instructions guiding the computer's actions. These instructions can be directly represented to letters and numbers, rather than a graphical component on the screen. It's not like the graphical components of a program just magically appear based on the instructions; someone had to program the corresponding GUI for the program.

For example, if you are playing a video game and click on the "Start Game" button, the game doesn't just start magically; it follows a set of commands set up by the programmers. For example, the underlying commands could be as follows:

- *initializeGame*
- *createPlayerCharacter*
- *setGameParameters*
- *loadGameLevels*
- *spawnEnemiesAndTriggers*
- *startAudio*
- *displayGameInterface*

And each one of these commands will likely call many other commands that take care of the specifics. For example, *displayGameInterface* might call

- *displayHealthBar*
- *displayInventory*
- *displayQuestLog*
- *displayMap*
- *displayScoreboard*

Clearly there is a lot going on beneath the GUI. Just think about it.  What we see as "Start Game" is actually a long list of subprocesses. While everyday users don't need to know all these intricate details, programmers working on games or other apps need to break things down into their smallest components. And that's where the terminal comes in.

The terminal operates at a more fundamental level, granting direct access to the underlying command-line interface (CLI) of the operating system. It's like a secret door that bypasses the graphical user interface altogether. You can do everything you do with a GUI using the terminal, but not everything you can do with the terminal is possible through a GUI. That's because the GUI is written based on the commands, and not all commands might be represented in the GUI.

That's why programmers and IT professionals rely on the terminal. It's a powerhouse of control and functionality. See, while GUIs simplify user interactions, they may not exist or may not be developed for certain specialized technologies or applications. Nobody bothers to create the GUI-equivalent of tools used by programmers and IT professional. Why? Well, developing a GUI takes extra effort, and lots of code has to be written in order to erect a GUI-equivalent of a program. And the assumption is that since tech-savvy folks like programmers are capable of using the terminal, then they can just use the terminal. No need for a GUI-equivalent.

This explanation does make it seem like we're forced to use the terminal because there is no GUI-equivalent, but the truth is that the CLI offers way more functionality than most of its GUI counterparts.

The terminal gives you direct access to the building blocks of a computer's operations. You can run powerful commands, automate tasks, manage files, configure software, and troubleshoot like a pro. By diving into the terminal, programmers and IT professionals gain a deeper understanding of computers and unlock their full potential in the world of technology.

### Some concrete examples

Imagine you are building a website and want to configure the server settings for optimal performance. The terminal becomes invaluable in this scenario. By using specific commands, you can access the server through the terminal and make necessary configurations to improve the website's speed, security, and functionality.

Now consider the example of configuring network devices in a large organization. Network engineers often rely on the terminal to access these devices and execute commands that optimize network performance, establish secure connections, and troubleshoot issues.

Another field where the terminal shines is cybersecurity. Security analysts use various terminal-based tools to detect and investigate potential threats. They can run commands to scan systems, analyze log files, and monitor network traffic, allowing them to identify vulnerabilities and take necessary actions to protect sensitive information.

Finally, the terminal is also crucial in the field of robotics. Even though we sometimes can see young kids "programming" robots within their school curriculum, they often do it using a GUI. These interfaces often feature drag-and-drop functionality and simplified coding blocks that allow students to create basic robot behaviors without delving into the complexities of coding. As students advance in their robotics journey, transitioning to the terminal becomes essential. It allows them to dive deeper into coding, write precise and customized algorithms, and gain a deeper understanding of the mechanics behind their robot's operations.

So whatever your interests, the terminal is crucial tool for programmers and IT professionals. It provides direct access to the underlying command-line interface, allowing for precise control, automation, and efficient workflows. The terminal empowers users to delve into the inner workings of computer operations, unleashing the full potential of their skills and creativity.


## Fundamentals

In this section, we will lay the groundwork for a solid foundation by delving into the essential components of the terminal.

### Terminal-emulator
The terminal used to be an entire device on its own (a display with a keyboard), separate from the mainframe computer. Today, we use software called emulators that replicate the functionality of old-school terminals. But although we technically use terminal-emulators, we simply call the program a terminal.

### Unix
As you delve deeper into the world of computers, you will inevitably encounter the term "Unix." Developed in the 1970s by Ken Thompson and Dennis Ritchie (the latter having created the C programming language for this purpose), Unix was a pioneering operating system that revolutionized the computing landscape. Unix played a significant role in popularizing the use of text-based commands as a primary means of interacting with a computer, and it served as the foundation for many subsequent operating systems, including the widely used Linux.

> To learn more about the history of Unix, read [The Story Behind the Development of the Unix Operating System](https://www.opensourceforu.com/2019/06/the-story-behind-the-development-of-the-unix-operating-system/).

### Linux
Linux is a Unix-inspired, Unix-like operating system widely used today. It was created by Linus Torvalds in the early 1990s. Linux also happens to be open-source, meaning that its software is freely available online, allowing users to view, modify, and distribute its source code.

You'll be surprised to learn that Linux is used everywhere. While the average consumer knows only of Windows and macOS computers, companies across various sectors have embraced Linux's versatility, stability, and cost-effectiveness. From web servers and cloud computing to scientific research, embedded systems, and even space exploration.

I mention Linux here because you will likely encounter it if you continue working with technology, and Linux relies heavily on the use of text-based commands executed through the terminal.

> Fun fact: Linux is used to power 96.3% of the world's top web servers.
[Source](https://www.enterpriseappstoday.com/stats/linux-statistics.html#:~:text=Linux%20is%20used%20to%20power,Linus%20operating%20system%20is%20run)

### Kernel
In the Computer Fundamentals, Software and Hardware section, I mentioned that the operating system is what sits between the hardware components of a computer and the software applications.

In general this is true, however the operating system is large and is made of many components. One of its components is called the kernel.

Just like it's definition in english, the kernel is the core of the operating system. Windows has one, macOS has one, and so too does Linux. Everything previously said that the OS does is actually done specifically by the kernel.

### Shell
As it turns out, we can have direct access to the kernel of an operating system. And that is thanks to the outermost layer of the operating system, known as the shell.

The shell takes in commands, and interprets them. For that reason, it can be called a "command-line interpreter", or "command language interpreter" (not to be confused with the typical abbreviation of CLI being "command-line interface", which refers to the terminal). The shell is a program that takes your typed commands and translates them into instructions that the kernel can understand and execute. It sits between the user and the kernel of the operating system.

But wait, wasn't that the role of the terminal?

Not exactly. The terminal does sit between the user and the operating system, however it is simply an interface; a place where the user can write their commands. The terminal only know how to accept input from the keyboard and display output onto the screen. The terminal itself does not know what to do with the provided input. And that is where the shell comes in.

When you type something into the terminal and press enter, the terminal sends what you wrote to the shell. The shell reads the commands you enter in the terminal, processes them, and communicates with the kernel to carry out the requested actions. The kernel then performs the necessary tasks, such as managing memory, accessing files, or running processes, based on the instructions provided by the shell. 

The terminal and the shell are often used interchangeably, so don't get too caught up on the definitions when reading about it online.

[//]: # "can have an image here such as: http://coewww.rutgers.edu/www1/linuxclass2008/lessons/lesson1/sec_9.html"

[//]: # "can have an image here such as:https://developer.ibm.com/tutorials/l-linux-shells/. and this: https://i.stack.imgur.com/muYsK.jpg"

Since the shell is just a program that interprets commands, there have been many variations created. The default shell on most Linux and on older macOS systems is called the GNU Bash, or just Bash. Newer macOS users use Zsh ("Z shell"), and Windows machines use the Command shell (also known as "cmd") and PowerShell.

### Review of the working directory
I want to mention this topic again, because it is so important. The working directory is important when working with files because it determines the context in which file operations take place. When you create, modify, or access a file without specifying a specific file path, the operating system assumes that the file is located within the working directory.

So if you are in the 

```
Locker > Physics > Quizzes 
```

folder, and you enter a command that translates to "create a file called "quiz8.txt", it will create it in your working directory, i.e. Locker/Physics/Quizzes/. If you do not specify where you want the command to execute, then it will by default execute in the working directory.

### File system navigation
Moving around the file system is a fundamental skill in the terminal. You will need to work with files from different directories, and knowing how to navigate efficiently will save you time and effort.

For macOS and Linux users, you can view the "Basic Navigation" of [this resource for specific commands](https://www.pluralsight.com/guides/beginner-linux-navigation-manual).

For Windows users, you can view [this resource for specific commands](https://riptutorial.com/cmd/example/8646/navigating-in-cmd).

### File manipulation
The terminal enables us to work with files efficiently.

For macOS and Linux users, you can view the "File Manipulation" of [the previous resource for specific commands](https://www.pluralsight.com/guides/beginner-linux-navigation-manual).

[//]: # " for windows have link: talk about creating a file, creating a folder, delete a file or folder, copy a file, move a file, rename a file"

### Working with text
Working with text in the terminal opens up a whole world of possibilities and gives you the power to manipulate, search, and transform text effortlessly. 

For macOS and Linux users, you can view the "Working with Content" of [the previous resource for specific commands](https://www.pluralsight.com/guides/beginner-linux-navigation-manual).

[//]: # " for windows have link. just want to check if this is good way of writing this"

### Understanding relative versus absolute path
In the Computer Fundamentals, Software and Hardware section, I talked about the meaning of a file path. There, I described what is known as "absolute path", i.e. the path it takes to get to a file from the root folder, or in the case of the analogy, the locker.

There is however also the concept of a "relative path". This brings in the concept of a working directory, which I've also covered in that section.

[//]: # "not sure how deep to go into it on my own ^^"

To understand the difference, check out [this article](https://www.redhat.com/sysadmin/linux-path-absolute-relative).

### I/O redirection
When we enter a command into the terminal, we use the keyboard to do so. Hence, the input is text from the keyboard (a.k.a. standard input). Once the command gets executed, we (may) receive an output in the form of text on the terminal (a.k.a. standard output). Commands that do this are ***ls***, ***cat file-name.txt***, ***pwd***, so on and so forth. 

In addition to receiving output on the terminal, we can use I/O redirection to manipulate how commands process data. Let's say you want to take the output of one command and use it as input for another command. This is where pipes come into play. Pipes are represented by the | symbol and allow us to connect multiple commands together, creating a powerful chain of actions.

[//]: # "have image of two functions, output of one going in as input to the other"

See examples of how to use pipes [in this article](https://www.computernetworkingnotes.com/linux-tutorials/pipes-in-linux-explained.html).

It is also possible to redirect an output into a file rather than onto the terminal using the > operator. Learn more about it [in this article](https://learning.lpi.org/en/learning-materials/010-160/3/3.2/3.2_01/#:~:text=To%20redirect%20standard%20output%20to,will%20overwrite%20the%20existing%20file.). 

[//]: # "not sure if I should add a final section (like a conclusion section) ### Additional Utilities There is a lot you can do with the terminal. And for everything that you can do, there is a command for it. So take your time to explore the terminal."

# Git
Imagine investing months, or even years, in developing a remarkable app, only to one day lose your laptop, and thus, your work. Despite such potential setbacks, how do thousands of programmers still manage to collaborate on a single project, and even stay organized? Now that you know about the terminal, we can talk about the wonderful tool called **Git**.

## Importance

Let's say that you are working on a software program. You store all your code in one folder, and name that folder "Project". Anyone who's programmed knows that code can go from "working" to "not working" very quickly. So what you decide to do is whenever you have a working product, you save it in the original "Project" folder. You know that what you have in that folder works.

So now, if you want to add some feature to your project, you duplicate the "Project" folder and name this new folder "Project_v2". Now you have a place where you are safe to experiment in, and if everything completely fails and you end up changing the code so much that it is now unrecognizable, well you will still have the original "Project" folder, so everything's okay.

While this technique might keep you organized, once someone joins the project, working on the same codebase becomes a bit more difficult. Image person A is working on feature A, and that code is partially intertwined with feature B that person B is trying to add. 

## Fundamentals

### Version Control System (VCS)
Version control is the practice of tracking and managing changes, usually to software code.

### Repository

### Committing changes

Concept of a commit
Staging and committing changes
Importance of descriptive commit messages

Cannot directly push code from your working copy to the remote site. Similarly, you cannot directly push your code from the staging area to the remote site. The remote site is only connected to the local repository.


### Branching and Merging

Introduction to branches
Creating, switching, and deleting branches
Merging changes between branches

### Collaborating with Git

Working with remote repositories
Cloning repositories
Pushing and pulling changes

### Resolving conflicts

# Search Engine
They say that Google is a programmer's best friend. With a few keywords and a click of a button, a world of knowledge opens up. Whether it's debugging an error, exploring new libraries, or discovering best practices, programmers can navigate the vast realm of knowledge through a **search engine**.

## Importance
Efficiency, etc


## Fundamentals


# Code Editor
Have you ever wondered where programmers code? On their computers, sure. But do they open Microsoft Word? Do they open their browser and go to some special website where they can code? Programmers use a dedicated software tool designed specifically for coding: the **code editor**.

## Importance

history of vim emacs, why use that instead of google docs or notepadd++

## Fundamentals
