---
title: "Chapter 5: Data Types and Variables"
date: "2023-10-19"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - ["", ""]
  - ["", ""]
  - ["",""]
---

In daily life, we deal with different types of data. We classify items by color, size, shape, and various other attributes. Similarly, in programming, understanding data types and how they are managed is paramount to designing efficient and effective programs.

## Table of Contents

[Understanding Data Types](#understanding-data-types)

[Typical Data Types in Programming](#typical-data-types-in-programming)

[Variables: The Storage Units of Data](#variables-the-storage-units-of-data)

- [Purpose of Using Variables](#purpose-of-using-variables)
- [Benefits of Using Variables](#benefits-of-using-variables)
- [Assigning Values to Variables]()
- [Changing Variable Values]()

[Examples with Pseudocode]()

[Side-by-Side: Variables in C and Python]()

[Activities]()

[Questions](#questions)

## Understanding Data Types

Imagine walking into a library. In this library, there are various items: books, CDs, newspapers. Each of these items can be thought of as a different "type" of data in this library.

- Books:
  - Operations: You can read them, bookmark pages, and sometimes write notes.
  - Storage: Kept on specific shelves, categorized by genre or author.
- CDs:
  - Operations: You can listen to them, skip tracks, or repeat songs.
  - Storage: Stored in CD racks or cases.
- Newspapers:
  - Operations: Read articles, check out the classifieds, or solve puzzles.
  - Storage: Kept in stacks or in special newspaper stands.

Just as different items in a library have specific operations and storage methods, data types in programming dictate how data can be manipulated and stored.

Recognizing the "type" of an item or piece of data helps us understand what we can and cannot do with it. In the library, you wouldn't try to "listen" to a book or "read" a CD.

Every piece of data in a program has a 'type'. These types help determine what operations can be performed on the data and how it is stored. So what are some of the common data types in programming?

## Typical Data Types in Programming

At their core, most programming languages support a set of basic or "primitive" data types:

- Integers (int): Whole numbers, both positive and negative. e.g., -3, 0, 42.
- Floating-point numbers (float): Decimal numbers. e.g., 3.14, -0.001.
- Booleans (boolean): Represented by two values, either 'True' or 'False'.
- Strings (string): Sequences of characters. e.g., "Hello, World!" or "I am 15 years old"

> Note: While these are general categories, the exact naming and behavior might differ slightly from one programming language to another.

## Variables: The Storage Units of Data

### Purpose of Using Variables

Continuing with our library analogy, imagine being a librarian responsible for managing the vast amount of items in the library. Over time, you'd realize that just knowing the types of items isn't enough. Every day, people come in and ask for specific books or CDs by name or content. To keep the library organized and to efficiently find items for members, you need a system.

Enter the library catalog system. Each book, CD, or newspaper is given a unique identifier or 'tag'. This tag doesn't just state the type (book, CD, newspaper) but has specific information like title, author, or release date. When a person asks for the book "Animal Farm", you don't just go to the 'book' section. You look up its unique identifier, find its location, and retrieve it. "Animal Farm" is a book, correct, however it is a specific type of book, and so distinguishing it from other books is important.

This 'tagging' system of the library mirrors the concept of 'variables' in programming. A variable is like a tag or label given to a piece of data. It doesn't just tell us the type (integer, float, string) but provides a specific identity so that we can efficiently retrieve, modify, or operate on that data when needed. Just like you wouldn't want to search through all books to find one, in programming, we use variables to directly access and manage specific data.

I like to think of variables as labeled boxes where you can store your items (data). Each box can hold a specific type of item, and you can always replace, remove, or check the item inside.

[Illustration of labeled box]

### Benefits of Using Variables

- Organizing Complexity: Variables are like street names in a city, helping us navigate the complex world of programming by giving data meaningful identifiers.
- Flexibility & Adaptability: Just as preferences change in real life, data can change in programs. Variables allow for dynamic data adjustment, making our programs adaptable.
- Consistency & Safety: Data types set clear rules for what a variable can hold, ensuring data is handled correctly and preventing potential errors.
- Efficiency: Like organizing items in a warehouse, data types help the computer store data optimally, ensuring peak performance.

Utilizing variables and data types lets our programs be organized, adaptable, accurate, and efficient. They're indispensable tools for any developer. Let's now take a look at some pseudocode.

### Assigning Values to Variables

Assigning a value to a variable is like placing an item inside a labeled box.

Imagine finding a box and labelling it "Animal Farm", and then putting the book "Animal Farm" inside it.

[Illustration]

In programming, this is typically done with an "equals" sign (=). The variable name comes on the left, and the value you want to store comes on the right.

As we saw before, programming languages don't have "book", "CD", or "newspaper" as data type. Instead, they have integers, floats, Strings and Booleans just to name a few.

```python
variable_name = value
```

For example:

```python
author = "George Orwell"
```

Notice that author contains a String type.

### Changing Variable Values

A variable's value can be updated or changed throughout a program. This is especially true for weakly typed languages:

```python
variable_name = value
variable_name = new_value
```

### Variable Naming Rules and Conventions

You may have noticed that the variable names follow a certain style. Here are some rules and conventions that programmers follow in order to ensure code clarity and prevent potentials errors.

#### Mandatory Rules

1. **Valid Characters:**
  
    Use only letters (a-z, A-Z), numbers (0-9), and underscores (_).

    Example: *motor_speed*, *axis3_value*.
2. **Starting Character:**

    Always begin with a letter (a-z, A-Z) or an underscore (_). Never start with a number.

    Example: *sensor_reading* (correct), *_backup_value* (correct), *3rd_motor* (incorrect).
3. **Reserved Words:**

    Steer clear of language-specific keywords.

    Example: Avoid naming a variable *int* or *return* as they are common reserved words in many languages.

#### Best Practices

1. **Spacing:**

    It's more readable to place a space before and after the equals sign.

    Example: *wheel_rotation = 45* is preferable to *wheel_rotation=45*.
2. **Capitalization:**

    Start with a lowercase letter. For multi-word names, use camelCase or snake_case.

    Example: *robotArmPosition* (camelCase), *robot_arm_position* (snake_case).
3. **Descriptiveness:**

    Opt for clear names that describe their purpose.
    Example: *battery_voltage* (clear) over *bv* (vague).
4. **Consistency:**

    Stick to a chosen naming style throughout your code.

    Example: If you start with snake_case (*motor_speed*), don't mix with camelCase (*robotArm*) in the same codebase.

> Tip: Although the "Best Practices" aren't strict rules, adhering to them can greatly enhance the clarity and maintainability of your code. Instead of using generic names like *abc* or *var1*, choose descriptive identifiers that convey the variable's purpose.

## Strong vs. Weak Typing: C and Python Examples

In programming, the way languages handle and enforce data types varies. This brings us to the concepts of strong and weak typing.

C (Strong Typing)
In C, you need to specify the data type of a variable when you declare it. Once set

Strongly Typed Languages: In these languages, the data type of a variable is set when the variable is declared, and it can't change unless explicitly redefined. For instance, if you declare a variable to be of type integer, you can't just assign a string value to it later on. C is an example of a strongly typed language.

Weakly Typed Languages: In contrast, weakly typed languages allow variables to take on different data types without explicit redefinition. This provides flexibility but can also lead to unintended consequences if not used carefully. Python can be seen as an example of this
