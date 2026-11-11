# stock-count
The stock count of Selin's warehouse: every product, with its number.
## The count
- The count lives in `count.txt`.
- One product per line: a name, one space, a number.
- Products are in alphabetical order: a new product goes to its place, not to the end.
## Format of new product
- Name Quantity. For example: Apple 10
## How to change it
1. Open an issue.
2. Make a branch.
3. Commit with title "Closed #of issue", push, and open a pull request.
4. Somebody else reviews it before it is merged.

The same steps as a diagram: [docs/workflow.md](docs/workflow.md).
## How to update existing product
1. Open an issue
2. Make a branch
3. Type command "nano count.txt"
4. İn editor change quantity of product
5. Type Ctrl O, then Ctrl X to exist
6. Commit,push,and open pull request.
7. Somebody else reviews it before it is merged.
## Who does what
| Who | What |
|-------|-------------------------------------------|
| Selin | owns the count, merges pull requests |
| Kaan | counts, reviews pull requests |
## Read the history
Every line of the count has a commit behind it:
```
git log --oneline count.txt
git blame count.txt
```
## Decisions
- [0001 - The count is a plain text file](docs/adr/0001-plain-text-count.md)

