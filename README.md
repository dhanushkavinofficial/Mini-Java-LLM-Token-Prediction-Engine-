# Mini-Java-LLM-Token-Prediction-Engine-
# Mini Java LLM (Token Prediction Engine)

A simplified Large Language Model simulation written in pure Java.

This project demonstrates the internal architecture of language models using basic algorithms.

It focuses on:

- Tokenization
- Vocabulary building
- Probability modeling
- Next-token prediction

The goal of this project is educational: to understand how language models generate text.

---

# Architecture

User Input
     |
Tokenizer
     |
Vocabulary Builder
     |
Probability Model (Bigram Model)
     |
Prediction Engine
     |
Generated Output

---

# Components

Tokenizer
Converts raw text into tokens.

Example:
"Java is powerful"

Becomes:

["java", "is", "powerful"]

---

Vocabulary

Stores unique tokens.

Example:

java
is
powerful
software
engineers

---

Probability Model

Builds token relationships using a bigram model.

Example:

java -> is
is -> powerful
is -> used

Counts transitions between words.

---

Prediction Engine

Generates text by predicting the most probable next token.

Example:

Input:
java

Output:
java is powerful

---

# Algorithm

The system uses a simple bigram probability model.

P(next_word | current_word)

Example:

java -> is (3 times)
java -> powerful (1 time)

Probability:

P(is | java) = 3 / 4

---

# How To Run

Compile

javac Main.java

Run

java Main

---

# Example Training Data

java is powerful
java is fast
java is used for backend
software engineers love java

---

# Future Improvements

Possible upgrades:

Add neural embeddings
Add transformer attention
Add temperature sampling
Add dataset loader
Add REST API
Add vector search

---

# Learning Goals

This project helps developers understand:

LLM internal architecture
Token prediction
Probability models
Java system design
Algorithmic thinking

---

# Author

Created for learning low-level design and language model fundamentals.
