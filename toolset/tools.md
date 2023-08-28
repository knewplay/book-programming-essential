---
title: "Toolset"
date: "2023-08-18"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
---
Just as a master carpenter skillfully wields their tools to shape exquisite furniture or a painter expertly selects brushes and colors to create captivating artwork, programmers harness a collection of specialized tools to craft intricate software systems. Let's explore the essential tools that empower programmers to shape the digital world.

# Table of Contents

[Terminal](#terminal)

[Git](#git)

[Search Engine](#search-engine)

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

Not exactly. The terminal does sit between the user and the operating system, however it is simply an interface; a place where the user can write their commands. The terminal only knows how to accept input from the keyboard and display output onto the screen. The terminal itself does not know what to do with the provided input. And that is where the shell comes in.

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
They say that Google is a programmer's best friend.  With a few keywords and a click of a button, a world of knowledge opens up at the palm of our hands. Whether it's debugging an error, exploring new libraries, or discovering best practices, programmers can navigate the vast realm of knowledge through a **search engine**.

## Importance
In the world of programming, one thing remains certain: programmers, even those with decades of experience, will face hurdles, encounter challenges, and have moments of confusion.

This is especially important for beginners, because it could be very discouraging to not be able to move forward with a project because of some error. It is quite common for beginners to get stuck, not know how or even who to ask for help, and simply abandon on their learning journey.

Even more experienced programmers ask for help. Programming is a dynamic field that constantly evolves with technology. Some programming languages that were once considered cutting-edge have evolved, while new ones have emerged. As a result, programmers often find themselves working on diverse projects with varying technical requirements. While their experience serves as a solid foundation, they may still encounter unfamiliar details or bugs.

The key to overcoming these obstacles is to be resourceful and skilled in the art of searching for answers effectively. The internet has almost all the answers, but you need to be able to extract them. This is where the power of a search engine comes into play.

## Fundamentals
We all wish that computers could just read our minds and give us the exact solution to our problem, in the exact context that we need it in. However, past the most rudimentary of programming questions, things aren't always that easy. Searching is somewhat of an art, and it's not always intuitive.

While there are alternative search engines such as Bing, Yahoo, DuckDuckGo, we will stick with the Google search engine, as it is the most widely used, notably among programmers. However, the advice provided will be relevant for all search engines.

### How Google Search works
The internet is a global network of interconnected computers and servers. It is a vast infrastructure that allows various devices and networks to communicate with each other using a common set of rules known as protocols. 

One of the subsets of the internet is called the World Wide Web, or simply "web" for short. The web refers to a collection of interconnected websites and web pages that are accessible through the internet.

Google Search is a powerful tool that helps users navigate the vast landscape of the web to find relevant information. When you enter a query ("query" is a fancy word for "question") into Google's search bar and hit the search button, a complex and fascinating process is set in motion.

1. Crawling: Google uses specialized software known as "web crawlers" to systematically browse the web. These crawlers follow hyperlinks from one web page to another, collecting data about each page they visit. This process is known as "crawling."

2. Indexing: The data collected by the web crawlers is then indexed, which means it is organized and stored in Google's vast database. This index allows Google to quickly retrieve relevant information when a user performs a search.

3. Ranking: When you perform a search, Google's (secret) search algorithms come into play. These algorithms analyze the indexed data and consider numerous factors to determine the most relevant and useful results for your query. Google takes into account factors like the words used in your search, the freshness of the content, the quality of the web page, and the number of other websites linking to that page (known as PageRank).

### When to google
The truth is that you can google anything, anytime you want. Google is never going to tell you "that was a dumb question". Once you start googling, you will notice that there have been many people before you who have had the same questions, and those questions are answered on the internet. However, here are some more specific cases when it is appropriate to google.

1. As someone learning a new programming language, googling can help you find tutorials, guides and online courses to expand your knowledge.

2. If you come across the use of a function in a tutorial, and would like to see more examples of that function being used, then googling for examples is a great idea.

3. When you compile or run your code, errors are innevitable, and copy-pasting the error message will often lead you to either a blog post solving the error, a discussion forum where others have faced the same issue and found solutions, or most commonly, a Q&A website such as Stack OverFlow. However, do not forget to read and try to understand the error message yourself before automatically copy-pasting it.

4. Just like when learning a new programming language, there may be a new library that you must use. Learn more about the library by googling it.

### How to google
Googling is an art. There is no one way to enter your query. I might ask it one way, and you might ask it slightly differently. And that's okay. But here are some general guidelines on how to do it.  

#### **Be simple but precise**
The important thing is to find a balance between concise and descriptive queries. You need to use the minimum number of words, but also give enough information for Google to understand what it needs to show you. Never add any information that is not important. Being too specific is not good either, as it will limit your search result and Google will return fewer quality examples of what you really want to know.

> If you want to know how to write a Hello World program in C, don't mention your operating system, your location, or your programming environment. All of these things are unrelated to the problem, and will negatively affect the search result as it will take the focus away from *"how to write a hello world program in c"*.

When it comes to simplifying your query, think of the resulting websites' titles and contents. Google will match your query with the website title and contents.

> Instead of writing *"I'm confused by when I should use semicolons in C"*, write *"semicolon use in c"*, or just simply *"semicolons in c"*. If Google shows results of semicolon use in regular English (for example), and didn't pick up the *"in c"* portion of the query, then specify: *"semicolon use in c programming language"*.

> Sidenote: Google searched are case-insensitive, meaning it doesn't matter if you write *C* of *c*.

#### **Use autocompletion**
When you start typing words into the search bar, always pay attention to what Google is suggesting. It can help you complete your queries faster, but it can also better word a query for you, taking the guesswork of what to type away. This is a perfect feature to use when you have an idea of what you are looking for, but not sure how to phrase it.

#### **It's okay to be messy**
This is not a beauty contest. You do not get a prize for coming up with the nicest and cleanest way to ask a question. Sometimes, the perfect words just aren't coming into your mind, and that's okay. Use the English language as best you can to describe the problem.

> Let's say you know that there is a function that *prints out* the argument as a message onto the screen. So you can write *"function to print message in c"*. But what if you forgot the terms "function" and "print". Well, just simplify it into English: *"how to output onto the screen in c"*. Now what if you forgot the term "output"? Simplify the query further: *"how to write onto the screen in c"*.

Part of the programming journey is to go from using purely English terms, to using more technical and precise programming terms. As long as you read the results, learn more about the topic and get used to the correct terms, you are on the right path.

#### **When to check the second page**
Sometimes, you search a query, and Google gives results for a different topic with similar vocabulary. If that happens, don't go looking for your topic on the second or third page of Google. The first page was Google's best guess at what you asked for, so instead of looking for what you need, word your query differently.

The only time you should consider checking Google's second result's page is when Google is displaying the correct general topic, but the articles provided are missing some detailed information that you need. This rarely happens though if you were specific enough in the query.

#### **Don't just click and stay**
After entering their query, most people will automatically click on the first search result and just read that. What I like to do is skim through the search results' titles and snippets, and see how well they match my query. If they match, I typically open a few of them in separate tabs (by holding *ctrl/cmd* and clicking on the websites), and skim through them. If the websites all provide the same solution, then I will use it with confidence. If not, then I might dig a bit into the different solutions and learn about the differences.

#### **Use matching operators**
1. Using double quotes ("") around any term acts as an **inclusion operator** and will force Google to match it exactly. E.g. ***"html" "css" website development***
2. Using the minus symbol (-) before a word acts as an **exclusion operator** and will filter out any results containing that word. Use this when you are looking for a solution for something but, for one reason or another, you don't want to use some particularly popular tool; maybe it doesn't work on your system, maybe it's too bulky for your project, etc. E.g. rather than searching ***robotics programming without python***, which is going to give python-related results, search for  ***robotics programming -python***.
3. Using the asterisk (*) within a query acts as a **wildcard operator** and will be replaced with any word or phrase. E.g. you run your code, and receive an error message which contains your local directory (which will only be relevant to you). Instead searching for the entire error message, you could replace that section with an asterisk.

#### **Use date operators**
If you are typing ***"c programming tutorial"*** and are getting results from 2010, you may want to limit the search to more recent articles.

You can use the complete format of ***yyyy-mm-dd***, or just type in the year. For example, ***"c programming tutorial after:2020"***.

Similarly, you can use ***"before"*** to search for articles before a certain date.

#### **Honorable mention: Stack Overflow**
One website that you will commonly encounter through your google search results will be StackOverflow. Stack OverFlow is a question-and-answer website for programmers. 

For beginners, Stack Overflow is an excellent place to learn from others' experiences and to gain insights into best practices. Reading through questions and answers related to topics you're interested in can provide valuable exposure to real-world coding scenarios.

### Veterans google differently
While experienced programmers do use Google a lot, there is a big difference in the way that they use it as opposed to how a complete beginner uses it. In the world of cybersecurity, there is this idea of a "script kiddie"; this is a person who uses existing code and copy-pastes his way through to whatever he wants to do. An experienced programmer will never simply take a piece of code and use it without fundamentally understanding what it does. They may do so to try to see if it works, but then they will try to understand it to potentially improve it and customize it.

So do not blindly follow or copy-paste any solutions you come across. Check to see if there are other avenues you could take. If you found a function that does what you need, learn more about how the function works; i.e. what arguments can it take, how will the result change if you give it different arguments, etc.

You must learn to carefully evaluate solutions you find online. Because at the end of the day, it's just people writing them. And people can also be faulty, or not provide the full picture. And this is where critical thinking comes into play.

# Code Editor
Have you ever wondered where programmers code? On their computers, sure. But do they open Microsoft Word? Do they open their browser and go to some special website where they can code? Programmers use a dedicated software tool designed specifically for coding: the **code editor**.

## Importance
In the early days of computing, programming was done using punch cards. Each card represented a line of code, and programmers had to feed a stack of these cards into a machine to run a program. This method was tedious and error-prone: a single misplaced hole in a card meant the whole stack might be rendered useless.

As computers evolved and became more interactive, the need for a more efficient way to program them became evident. This led to the development of the first code editors. These were rudimentary tools, basic environments for writing and editing text. However, they marked a significant leap from punch cards, allowing programmers to type in their code, make edits, and save their work electronically.

One of the earliest and most influential of these editors was vi, created in the 1970s. It was purely keyboard-driven, mainly because the mouse wasn't a common tool yet. Other editors like vim (an improved version of vi) and emacs emerged around this era. They prioritized speed and efficiency, and their influence can still be seen in many of the code editors we use today.

While you can technically use any text editor, like Google Docs or Notepad++, to write code, specialized code editors are preferred for several reasons. They're designed with coding in mind, providing features like syntax highlighting, auto-completion, error detection, and integrated debugging. 

> Fun fact: In computing, we often refer to programming errors as "bugs." The term "bug" actually has a fascinating origin. Back in 1947, a moth found its way into one of the components of the Mark II computer at Harvard University. When the team, led by Grace Hopper, discovered it, they commented that they were "debugging" the system. That's how we got the term "debugging." So, a "bug" refers to an error or flaw in software that produces unexpected results, and "debugging" is the process of finding and fixing these issues to ensure the program works correctly.

These tools make the coding process faster, more efficient, and less prone to error. In today's world, with these editors, you can write, test, and see the results of your code almost instantly, a far cry from the days of punch cards.

## Fundamentals
<!-- - mention google docs, notepad++ again
- give examples of popular editors (vi, vim, emacs, vs code, visual stodio, pycharm, eclipse). name them but categorize. What field are they used for, and why.
- show how its a spectrum of complexity: can go from vim (basic command-line editor) to visual studio (advanced cloud-based integrated environment)
- mention how programmers who use Vim swear by it (or emacs), without a mouse is faster. 
- explain IDE (it include code editor, but also much more)
- tell them where they can get started from. include some links to resources

At the end of the day, you can get the same result from whatever editor you use. Important thing is to start programming.  -->

