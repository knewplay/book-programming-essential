---
title: "Chapter 10: Exploring Further"
date: "2023-11-08"
author: "Andrei Guevorkian"
illustrator: "Dengyijia Liu"
questions:
  - q1-tag: |
      q1-text
  - q2-tag: |
      q2-text
  - q3-tag: |
        q3-text
---

With a solid foundation in programming basics, you're ready to peek into more complex and exciting areas. This chapter will give you a glimpse into advanced fields where programming is making a big impact, inviting you to consider your next steps in the programming landscape.

## Table of Contents

[Introduction to More Advanced Topics](#introduction-to-more-advanced-topics)

- [Artificial Intelligence](#artificial-intelligence)
- [Cybersecurity](#cybersecurity)
- [Game Development](#game-development)
- [Mobile Apps](#mobile-apps)
- [Robotics](#robotics)
- [Web Development](#web-development)

[Learning Resources](#learning-resources)

[Staying Current: The Programmer’s Growth](#staying-current-the-programmers-growth)

## Introduction to More Advanced Topics

### Artificial Intelligence

The term "AI", or "Artificial Intelligence", gets thrown around so much these days that it is impossible to ignore. Companies in all fields are forced to employ AI as a tool if they want to stay competitive and relevant.

But what is AI?

Very simply, AI is about rules and algorithms that help computers perform tasks that would normally require human intelligence. These tasks could be as simple as following a recipe to bake a cake or as complex as driving a car.

For example, think of a simple AI that plays tic-tac-toe:

```typescript
FUNCTION PlayTicTacToe(board)
    // Check if AI can win in the next move
    REPEAT FOR EACH possible move in board
        IF move "leads to victory"
            MAKE move
            RETURN
        END IF
    END REPEAT

    // Otherwise, block opponent from winning
    REPEAT FOR EACH possible move in board
        IF move "blocks opponent victory"
            MAKE move
            RETURN
        END IF
    END REPEAT

    // Otherwise, take one of the remaining free spaces
    MAKE random move from free spaces
END FUNCTION
```

This little snippet shows how AI uses predefined rules to decide what to do next. It's not actually learning or thinking; it's simply following its programming to try and win the game. And while this is a simple example, real-world AI systems can be incredibly complex, using thousands or millions of rules to do things like translating languages or predicting the weather.

However, when most people talk about AI, they actually mean "Machine Learning", or "ML", which is a subset of AI. In other words, all ML is AI, but not all AI is ML.

The key word in ML is "learning", i.e. the machine can improve its performance over time by learning from the data collected.

Here's a simple way to visualize how a computer could learn to tell the difference between cats and dogs using pseudocode:

```typescript
FUNCTION LearnFromPhotos(photoCollection)
    REPEAT FOR EACH photo in photoCollection
        IF photo is labeled 'cat'
            LearnFeatures(cat)
        ELSE IF photo is labeled 'dog'
            LearnFeatures(dog)
        END IF
    END REPEAT
END FUNCTION

FUNCTION GuessAnimal(newPhoto)
    IF newPhoto "matches more features" of 'cat'
        RETURN 'This is probably a cat'
    ELSE
        RETURN 'This is probably a dog'
    END IF
END FUNCTION
```

the features would be things like the shape of the ears, the size of the animal, or the type of fur, and the computer would learn to recognize these features through algorithms that adjust based on whether their predictions are right or wrong. As the computer goes through more and more photos, it gets better at figuring out which features are most important for telling cats and dogs apart.

In summary:

**Traditional AI:**

- Uses hard-coded rules.
- Does not learn from data.
- Makes decisions based on the given rules.

**Machine Learning:**

- Learns from data using algorithms.
- Can improve its performance over time as it is exposed to more data.
- Makes decisions based on patterns it has learned from the data.

### Cybersecurity

### Game Development

### Mobile Apps

### Robotics

### Web Development

## Learning Resources

## Staying Current: The Programmer’s Growth
