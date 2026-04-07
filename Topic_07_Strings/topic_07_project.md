# Topic 7 Project: Text Analyzer

## Overview

Build a **Text Analyzer** that accepts a sentence from the user and performs a series of text analysis and transformation tasks using string indexing, methods, and f-string formatting.

---

## Part 1 — Text Collection and Cleaning

Ask the user to enter a sentence of their choice (at least 5 words).

Clean the input:
- Strip leading/trailing whitespace
- Convert to title case (capitalize first letter of each word)
- Replace any occurrence of the word "bad" with "good" (case-insensitive)

Display the cleaned version of the sentence.

## Part 2 — Text Analysis

On the cleaned sentence, compute and display:
- Total number of characters (including spaces)
- Number of characters excluding spaces
- Number of words (hint: use `.split()`)
- The first word and the last word
- Whether the sentence starts with a vowel (a, e, i, o, u — case-insensitive)
- The sentence reversed (character by character)
- Number of times the letter "a" or "A" appears

## Part 3 — Formatted Summary Report

Use f-strings to display a formatted analysis report that includes all the results from Part 2 in a clear, labeled layout. The report must:
- Have a header with `=` borders
- Display every metric with a label
- Include a footer that shows the first 3 and last 3 characters of the cleaned sentence

---

## Instructions

- Save your file as `topic_07_text_analyzer.py`
- Use string indexing and slicing at least twice
- Use at least 3 different string methods
- Use f-strings for ALL output in Part 3
- Include meaningful comments

---

## Example Output

```
==========================================
         TEXT ANALYSIS REPORT
==========================================
Original (cleaned)  : Hello World This Is Python
Characters (total)  : 25
Characters (no spaces): 20
Word count          : 5
First word          : Hello
Last word           : Python
Starts with vowel   : False
Reversed sentence   : nohtyP sI sihT dlroW olleH
Count of 'A/a'      : 0
------------------------------------------
First 3 chars : Hel
Last 3 chars  : hon
==========================================
```
