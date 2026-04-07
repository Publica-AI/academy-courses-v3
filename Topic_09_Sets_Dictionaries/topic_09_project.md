# Topic 9 Project: Word Frequency Analyzer

## Overview

Build a **Word Frequency Analyzer** that reads a paragraph of text and uses sets and dictionaries to analyze word usage patterns.

---

## Part 1 — Text Processing with Sets

Ask the user to enter a paragraph of text (at least 3 sentences).

Then:
- Convert the text to lowercase and split into a list of words
- Create a set of unique words
- Display the total word count and the count of unique words
- Ask the user for two words and check if each appears in the text (use set membership `in`)
- Find all words that appear in the user's text that are NOT common stop words. Use set difference. Stop words to use: `{"the", "a", "an", "is", "are", "was", "were", "and", "or", "but", "in", "on", "at", "to", "of", "it", "this", "that"}`

## Part 2 — Word Frequency with Dictionaries

Build a word frequency dictionary:
- Iterate through the word list
- For each word, add it to the dictionary with count 1 if new, or increment by 1 if existing
- Use `.get()` to safely check current count
- Find the most frequently used word and its count
- Find all words that appear more than once

## Part 3 — Frequency Report

Display a formatted frequency report:
- Header with total stats (words, unique words, distinct words after removing stop words)
- Top 5 most frequent words (sorted by count, descending)
- Words appearing more than once listed in alphabetical order
- The two user-searched words and whether they were found

---

## Instructions

- Save your file as `topic_09_word_analyzer.py`
- Use a set for unique words and for stop word filtering
- Use a dictionary for word frequencies
- Use `.items()` when iterating the dictionary
- Include meaningful comments

---

## Example Output

```
Enter a paragraph: Python is great. Python is easy. Everyone loves Python.

==========================================
       WORD FREQUENCY REPORT
==========================================
Total words      : 9
Unique words     : 6
Non-stop words   : 4 (python great easy everyone loves)

Top 5 Frequent Words:
  1. python     - 3 times
  2. is         - 2 times
  3. great      - 1 time
  ...

Words appearing more than once:
  is, python

Search: 'python' → Found | 'java' → Not found
==========================================
```
