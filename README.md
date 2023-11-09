# Intro to NLP - Assignment 3

## Team
|Student name| CCID |
|------------|------|
|Martin Mullappallil Johney  |      |
|Aaron Binoy   |      |

## TODOs

In this file you **must**:
- [ ] Fill out the team table above. Please note that CCID is **different** from your student number.
- [ ] Fill out the table in the [Evaluation](#evaluation) section.
- [ ] Acknowledge all resources consulted (discussions, texts, urls, etc.) while working on an assignment. Non-detailed oral discussion with others is permitted as long as any such discussion is summarized and acknowledged by all parties.
- [ ] Provide clear installation and execution instructions that TAs must follow to execute your code.

## Resources
Resources used: ChatGPT for debugging calculating perplexity

## Execution
Example usage: use the following command in the current directory.

`python3 src/main.py bigram data/training.txt data/dev.txt --laplace`

## Data
- [ ] We have provided the training and dev sets in the [data](data) directory.

## Evaluation

|Model           | Smoothing  | Training set PPL | Dev set PPL |
|----------------|----------- | ---------------- | ----------- |
|unigram         | -          |38.546738412790106|38.22621167306222|
|bigram          | unsmoothed |16.533090308407978|16.789588674738216|
|bigram          | Laplace    |18.99625433814741 |19.090801874848253|
|trigram         | unsmoothed |7.440230413263187 |8.022790772303466 |
|trigram         | Laplace    |19.970915431488635|20.348276377059364|
**Grad student extension**                                           
|bigram (KenLM)  | Kneser-Ney |                  |             |
|trigram (KenLM) | Kneser-Ney |                  |             |

