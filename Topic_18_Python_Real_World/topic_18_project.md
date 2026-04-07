# Topic 18 Capstone Project: Real-World Data Reporter

## Overview

Build a **Real-World Data Reporter** — a complete Python application that fetches live data from a web API, processes it using the algorithmic and data skills you have built throughout this course, stores the results as JSON files, and displays a formatted report.

This capstone project combines skills from **all 18 topics**: variables, control flow, functions, error handling, OOP, file handling, algorithms, external libraries, and real-world Python practices.

---

## Part 1 — Fetch Data from the API (4 marks)

**Question:**  
Write two functions to fetch data from the [JSONPlaceholder API](https://jsonplaceholder.typicode.com):
- `fetch_users() -> list` — fetches all users from `https://jsonplaceholder.typicode.com/users`
- `fetch_posts() -> list` — fetches all posts from `https://jsonplaceholder.typicode.com/posts`

**Instructions:**
- Use the `requests` library
- Add a `timeout=10` parameter to each request
- Handle network errors gracefully using try/except:
  - `ConnectionError` — print "No internet connection" and return an empty list
  - `HTTPError` — print the status code and return an empty list
  - `Timeout` — print "Request timed out" and return an empty list
- Each function must have a docstring and type hint on the return value
- Print how many records were fetched for each call

---

## Part 2 — Process and Enrich the Data (6 marks)

**Question:**  
Write a function `build_author_report(users: list, posts: list) -> list` that:

1. Creates a lookup dictionary mapping each `userId` to the user's `name`
2. For each post, adds:
   - `author_name`: the user's name (from the lookup dictionary)
   - `word_count`: the number of words in the post's `body`
3. Groups posts by author and calculates for each author:
   - `post_count`: total number of posts
   - `total_words`: total word count across all their posts
   - `avg_words`: average word count per post (rounded to 1 decimal)
4. Returns a **list of author summary dictionaries**:
   ```python
   {'author': 'Name', 'post_count': 10, 'total_words': 350, 'avg_words': 35.0}
   ```
5. Sorts the list by `post_count` (descending) using **bubble sort** — do NOT use `sorted()` or `.sort()`

**Instructions:**
- Implement bubble sort yourself for the sorting step
- Use a dictionary for the grouping/aggregation
- Include Big O comments on the bubble sort and any O(n²) operations

---

## Part 3 — Save Results to JSON (3 marks)

**Question:**  
Write a function `save_results(enriched_posts: list, author_report: list) -> None` that:

1. Creates an `output/` directory if it does not exist (use `pathlib`)
2. Saves the enriched posts list to `output/posts_enriched.json` (with `indent=2`)
3. Saves the author report list to `output/author_leaderboard.json` (with `indent=2`)
4. Prints confirmation messages showing the file paths and record counts

---

## Part 4 — Display a Formatted Console Report (4 marks)

**Question:**  
Write a function `print_report(author_report: list) -> None` that prints a formatted leaderboard:

```
============================================
          AUTHOR POST LEADERBOARD
============================================
Rank  Author              Posts  Avg Words
----  ------------------  -----  ---------
  1   Leanne Graham          10       51.2
  2   Ervin Howell           10       52.8
  ...
============================================
Total authors: 10 | Total posts: 100
============================================
```

---

## Part 5 — Wire It All Together (3 marks)

**Question:**  
Write a `main()` function that calls all the above functions in the correct order:
1. Fetch users and posts
2. Build the author report (enrich + sort + aggregate)
3. Save results to files
4. Print the formatted report

Guard the entry point with `if __name__ == '__main__': main()`

---

## Instructions

- Save your solution as `topic_18_data_reporter.py` or in a Jupyter notebook
- Apply best practices throughout: **type hints, docstrings, DRY, context managers**
- Do **not** use `sorted()` or `.sort()` for the bubble sort step
- Handle all network errors gracefully
- Each section is worth the marks shown — total: **20 marks**

| Part | Marks |
|------|-------|
| Part 1 — Fetch Data | 4 |
| Part 2 — Process & Enrich | 6 |
| Part 3 — Save to JSON | 3 |
| Part 4 — Formatted Report | 4 |
| Part 5 — Entry Point | 3 |
| **Total** | **20** |

---

## Expected Output (Example)

```
Fetched 10 users
Fetched 100 posts
============================================
          AUTHOR POST LEADERBOARD
============================================
Rank  Author              Posts  Avg Words
----  ------------------  -----  ---------
  1   Leanne Graham          10       51.2
  2   Ervin Howell           10       48.7
  3   Clementine Bauch       10       53.1
  4   Patricia Lebsack       10       49.9
  5   Chelsey Dietrich       10       52.4
  6   Mrs. Dennis Schulist   10       50.8
  7   Kurtis Weissnat        10       47.3
  8   Nicholas Runolfsdottir 10       51.6
  9   Glenna Reichert        10       50.1
 10   Clementina DuBuque     10       49.5
============================================
Total authors: 10 | Total posts: 100
============================================
Report saved → output/posts_enriched.json (100 records)
Report saved → output/author_leaderboard.json (10 records)
```
