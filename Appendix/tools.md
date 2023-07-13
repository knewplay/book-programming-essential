---
title: "Toolset"
date: "31-07-2023"
author: "Andrei Guevorkian"
---
At the end of the day, programmers are creators. They create software. And creators 


# Table of Contents

[Terminal](#terminal)

[Git](#git)

[Search Engine](#google-search)

[Code Editor](#code-editor)


# Terminal
Have you ever seen a movie where a hacker is frantically typing bright green letters on a black screen? Have you ever wanted to do that? As it turns out, that black screen isn't just a Hollywood invention; it really does exist, and it's called a **terminal**. 

## Importance

Back in the days, knowing how to use a terminal was absolutely necessary to communicate with the computer. Today, almost everyone uses the GUI exclusively. That is everyone except for programmers and IT professionals.

We have to understand that fundamentally, all programs are a sequence of instructions for the computer to execute. It's not like the graphical components of a program just magically appear based on the instructions; someone had to program the corresponding graphical interface for the program.

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

Clearly there is a lot going on beneath the GUI. And it is exactly at this low level where the terminal resides and operates. The terminal provides direct access to the underlying command-line interface (CLI) of the OS, skipping the graphical user interface altogether.



-talk about how terminal is used
-which fields is it mandatory (places where gui is not an option)
-how is it faster, more efficient. give concrete examples

There are several reasons why the terminal is impo

## Fundamentals
The terminal used to be an entire device on its own (a display with a keyboard), separate from the mainframe computer. Today, we use software called emulators that replicate the functionality of the old-school terminals. But although we technically use terminal-emulators, we simply call the program a terminal.


talk about shell,  

- mention pipe (O > I)

# Git
Have you ever wondered how thousands of programmers can collaborate and work on the same codebase, yet still be organized and not overwrite each other's work? This is the perfect time to introduce this tool, because it is typically used within the terminal. It is called **Git**.

## Importance

Let's say that you are working on a software program. You store all your code in one folder, and name that folder "Project". Anyone who's programmed knows that code can go from "working" to "not working" very quickly. So what you decide to do is whenever you have a working product, you save it in the original "Project" folder. You know that what you have in that folder works.

So now, if you want to add some feature to your project, you duplicate the "Project" folder and name this new folder "Project_v2". Now you have a place where you are safe to experiment in, and if everything completely fails and you end up changing the code so much that it is now unrecognizable, well you will still have the original "Project" folder, so everything's okay.

While this technique might keep you organized, once someone joins the project, working on the same codebase becomes a bit more difficult. Image person A is working on feature A, and that code is partially intertwined with feature B that person B is trying to add. 

## Fundamentals

### Version Control System (VCS)
Version control is the practice of tracking and managing changes, usually to software code.

# Search Engine
They say that Google is a programmer's best friend. With a few keywords and a click of a button, a world of knowledge opens up. Whether it's debugging an error, exploring new libraries, or discovering best practices, programmers can navigate the vast realm of knowledge through a **search engine**.

## Importance

## Fundamentals


# Code Editor
Have you ever wondered where programmers code? On their computers, sure. But do they open Microsoft Word? Do they open their browser and go to some special website where they can code? Programmers use a dedicated software tool designed specifically for coding: the **code editor**.

## Importance


## Fundamentals
