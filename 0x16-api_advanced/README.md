
API Advanced Project

In this advanced project, I further developed my skills in querying APIs, specifically focusing on the Reddit API.

## Tests ✔️

**tests:**  
This folder contains test files for all tasks. These tests were provided by ALX.

## Function Prototypes 💾

Below are the prototypes for the functions implemented in this project:

| File           | Prototype                                           |
|----------------|-----------------------------------------------------|
| 0-subs.py      | `def number_of_subscribers(subreddit)`              |
| 1-top_ten.py   | `def top_ten(subreddit)`                            |
| 2-recurse.py   | `def recurse(subreddit, hot_list=[])`               |
| 100-count.py   | `def count_words(subreddit, word_list)`             |

## Tasks 📃

### Task 0: How many subs?

**0-subs.py:**  
Python function that returns the total number of subscribers for a given subreddit.

- **Returns:**  
  `0` if an invalid subreddit is provided.

### Task 1: Top Ten

**1-top_ten.py:**  
Python function that prints the top ten hottest posts for a given subreddit.

- **Prints:**  
  `None` if an invalid subreddit is provided.

### Task 2: Recurse it!

**2-recurse.py:**  
Python function that recursively returns a list of titles for all hot articles on a given subreddit.

- **Returns:**  
  `None` if no results are found for the given subreddit.

### Task 3: Count it!

**100-count.py:**  
Python function that recursively prints a sorted count of given keywords parsed from the titles of all hot articles on a given subreddit.

- **Features:**  
  - Keywords are case-insensitive and separated by spaces.
  - Results are printed in descending order by count.
  - Words with identical counts are sorted alphabetically.
  - Words with no matches are skipped.
  - The count reflects the number of keyword occurrences, e.g., "java java java" counts as three instances of "java."

---
