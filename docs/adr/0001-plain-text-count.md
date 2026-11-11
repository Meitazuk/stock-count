# 0001 - The count is a plain text file
## Context
The auditors need to see every change to the count: which line, who, when, why.
Git shows changes line by line, but only in text files. An Excel file is a
binary file: Git can only say that it changed, not what changed.
## Decision
The count is one plain text file, `count.txt`, with one product per line.
## Consequences
- Every change shows as a line in the history, and two people can change
different lines at the same time.
- No formulas: a total has to be computed by hand or with a command.
