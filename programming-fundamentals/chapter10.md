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

However, when most people talk about AI, they are often referring to "Machine Learning" (ML), which is a specific subset of AI. The key aspect of ML is "learning," which means the machine improves over time by learning from data. The critical factor here is that the machine is provided with labeled data—this is like giving the machine a filled-out quiz to study from, so it knows what the correct answers (or classifications) should be.

In ML, we give the computer examples of labeled data, such as pictures that are already tagged as 'cat' or 'dog'. The machine uses these examples to learn the distinctive features of each animal.

Here's a simplified pseudocode example of how a machine could learn from labeled photos to tell the difference between cats and dogs:

```typescript
FUNCTION LearnFromPhotos(photoCollection)
    REPEAT FOR EACH photo in photoCollection
        IF photo is labeled 'cat'
            LearnFeatures('cat', photo)
        ELSE // Photo is labeled 'dog'
            LearnFeatures('dog', photo)
    END REPEAT
END FUNCTION

FUNCTION GuessAnimal(newPhoto)
    IF newPhoto "matches more features" of 'cat'
        RETURN 'This is probably a cat'
    ELSE
        RETURN 'This is probably a dog'
END FUNCTION
```

The 'LearnFeatures' function is where the machine learning algorithm examines each labeled photo, identifying and cataloging features such as ear shape, fur pattern, or tail length. Over time, as the algorithm encounters more labeled photos, it gets better at understanding which features are most likely to signify 'cat' or 'dog'. This process is called "training the model."

Once trained, the machine can then look at new, unlabeled photos (data it hasn't seen before) and use what it has learned to guess whether they contain a cat or a dog. This guessing is based on the presence and strength of the features it learned during training.

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
