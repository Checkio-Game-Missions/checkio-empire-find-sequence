Let's upgrade our troop line recognize algorithms.

You are given a matrix of NxN.
You should check if there is a sequence of 4 or more matching digits.
The sequence may be positioned horizontally, vertically or diagonally (NW-SE or NE-SW diagonals).

![Find](find-sequence.png)

**Input:** A matrix as a list of lists with integers. 

**Output:** Whether or not a sequence exists as a boolean.

**Example:**

```python
has_sequence([
    [1, 2, 1, 1],
    [1, 1, 4, 1],
    [1, 3, 1, 6],
    [1, 7, 2, 5]
]) == True
has_sequence([
    [7, 1, 4, 1],
    [1, 2, 5, 2],
    [3, 4, 1, 3],
    [1, 1, 8, 1]
]) == False
has_sequence([
    [2, 1, 1, 6, 1],
    [1, 3, 2, 1, 1],
    [4, 1, 1, 3, 1],
    [5, 5, 5, 5, 5],
    [1, 1, 3, 1, 1]
]) == True
has_sequence([
    [7, 1, 1, 8, 1, 1],
    [1, 1, 7, 3, 1, 5],
    [2, 3, 1, 2, 5, 1],
    [1, 1, 1, 5, 1, 4],
    [4, 6, 5, 1, 3, 1],
    [1, 1, 9, 1, 2, 1]
    ]) == True
```
**How it is used:**

This concept is useful for games where you need to detect various lines of the same elements (match 3 games for example).
This algorithm can be used for basic pattern recognition.

**Precondition:**

```python
0 <= len(matrix) <= 10
all(all(0 &lt; x Б 10 for x in row) for row in matrix)
```
