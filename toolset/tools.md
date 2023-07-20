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

## Some concrete examples

Imagine you are building a website and want to configure the server settings for optimal performance. The terminal becomes invaluable in this scenario. By using specific commands, you can access the server through the terminal and make necessary configurations to improve the website's speed, security, and functionality.

Now consider the example of configuring network devices in a large organization. Network engineers often rely on the terminal to access these devices and execute commands that optimize network performance, establish secure connections, and troubleshoot issues.

Another field where the terminal shines is cybersecurity. Security analysts use various terminal-based tools to detect and investigate potential threats. They can run commands to scan systems, analyze log files, and monitor network traffic, allowing them to identify vulnerabilities and take necessary actions to protect sensitive information.

Finally, the terminal is also crucial in the field of robotics. Even though we sometimes can see young kids "programming" robots within their school curriculum, they often do it using a GUI. These interfaces often feature drag-and-drop functionality and simplified coding blocks that allow students to create basic robot behaviors without delving into the complexities of coding. As students advance in their robotics journey, transitioning to the terminal becomes essential. It allows them to dive deeper into coding, write precise and customized algorithms, and gain a deeper understanding of the mechanics behind their robot's operations.

So whatever your interests, the terminal is crucial tool for programmers and IT professionals. It provides direct access to the underlying command-line interface, allowing for precise control, automation, and efficient workflows. The terminal empowers users to delve into the inner workings of computer operations, unleashing the full potential of their skills and creativity.


## Fundamentals

In this section, we will lay the groundwork for a solid foundation by delving into the essential components of the terminal.

## Terminal-emulator
The terminal used to be an entire device on its own (a display with a keyboard), separate from the mainframe computer. Today, we use software called emulators that replicate the functionality of old-school terminals. But although we technically use terminal-emulators, we simply call the program a terminal.

## Unix
As you delve deeper into the world of computers, you will inevitably encounter the term "Unix." Developed in the 1970s, Unix was a pioneering operating system that revolutionized the computing landscape. Unix played a significant role in popularizing the use of text-based commands as a primary means of interacting with a computer, and it served as the foundation for many subsequent operating systems, including the widely used Linux.

> To learn more about the history of Unix, read [The Story Behind the Development of the Unix Operating System](https://www.opensourceforu.com/2019/06/the-story-behind-the-development-of-the-unix-operating-system/).

## Linux

Linux is a Unix-like operating system that is widely used today. 

## Shell
talk about shell,  commonly used shells bash csh, zsh, powershell
link with unix

## Kernel


## File system navigation

The working directory is the current directory or folder in which a user is actively working within a file system. It is the default location where a command or program will execute and search for files unless a specific file path is provided.

The working directory is important when working with files because it determines the context in which file operations take place. When you create, modify, or access a file without specifying a specific path, the operating system assumes that the file is located within the working directory. This allows for relative file referencing, making it easier to work with files within a specific project or directory structure.

The working directory helps maintain organization and streamline file management. It ensures that related files and resources are easily accessible and allows for the execution of commands or programs without explicitly specifying the full file path. By understanding and utilizing the concept of the working directory, users can navigate through the file system more efficiently and perform file operations with greater ease.

talk about pwd, cd, ls other

## File manipulation

talk about creating a file, creating a folder, delete a file or folder, copy a file, move a file, rename a file

## Text editing

display contents of a file (cat), add text to a file,

## I/O redirection
- mention pipe (O > I) I/O redirection
Redirecting input and output streams
Using pipes to chain commands together

## Additional Utilities
Exploring additional useful terminal tools (e.g., tar, zip, ssh)
Installing and managing software through package managers (e.g., apt, Homebrew)
display user manual of a command




what is the relation between unix/linux and the temrinal
ChatGPT
Unix and Linux are operating systems that utilize a command-line interface known as the terminal. The terminal, also referred to as a shell or command-line interface (CLI), is a program that allows users to interact with the operating system by typing commands. Unix and Linux systems typically provide multiple terminal applications, such as Bash, Zsh, or Csh, each with its own features and functionalities.

The terminal provides a text-based environment where users can execute commands, navigate the file system, manage processes, and perform various system operations. It serves as an alternative to graphical user interfaces (GUIs) commonly found in desktop environments, allowing users to perform tasks efficiently through typed commands.

Unix, which was developed in the 1970s, was one of the first operating systems to introduce the concept of a command-line interface and provided a foundation for subsequent systems like Linux. Linux, created in the early 1990s, was developed as a free and open-source operating system that follows the design principles of Unix. It adopted many of Unix's concepts, including the use of the terminal as a primary means of interacting with the system.

In the Unix and Linux environments, the terminal plays a crucial role in system administration, software development, and general user tasks. It offers powerful capabilities for automation, scripting, and remote access, making it a preferred choice for advanced users and professionals.

While Unix and Linux systems often have graphical interfaces available, the terminal remains an essential tool for tasks that require precise control, scripting, or operating in server environments without a GUI. Many system administration tasks, programming workflows, and software development practices rely heavily on the use of the terminal.

In summary, Unix and Linux operating systems provide the foundation for the terminal, which is a command-line interface allowing users to interact with the system through typed commands. The terminal is a powerful tool for system administration, development, and automation in Unix and Linux environments.














# Git
Imagine investing months, or even years, in developing a remarkable app, only to one day lose your laptop, and thus, your work. Despite such potential setbacks, how do thousands of programmers still manage to collaborate on a single project, and even stay organized? Now that you know about the terminal, we can talk about the wonderful tool called **Git**.

## Importance

Let's say that you are working on a software program. You store all your code in one folder, and name that folder "Project". Anyone who's programmed knows that code can go from "working" to "not working" very quickly. So what you decide to do is whenever you have a working product, you save it in the original "Project" folder. You know that what you have in that folder works.

So now, if you want to add some feature to your project, you duplicate the "Project" folder and name this new folder "Project_v2". Now you have a place where you are safe to experiment in, and if everything completely fails and you end up changing the code so much that it is now unrecognizable, well you will still have the original "Project" folder, so everything's okay.

While this technique might keep you organized, once someone joins the project, working on the same codebase becomes a bit more difficult. Image person A is working on feature A, and that code is partially intertwined with feature B that person B is trying to add. 

## Fundamentals

### Version Control System (VCS)
Version control is the practice of tracking and managing changes, usually to software code.


---
Cannot directly push code from your working copy to the remote site. Similarly, you cannot directly push your code from the staging area to the remote site. The remote site is only connected to the local repository.

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
