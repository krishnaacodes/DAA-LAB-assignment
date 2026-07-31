# DAA-LAB-assignment



# Lab Task 2

## Part 1. Trace It Yourself

### Input:
List = [8, 3, 15, 6, 2]

### Output:
Largest Number = 15

### Comparisons made:
4

### Dry Run:

Initial:
max = 8


|1|3|3 < 8|8|
|2|15|15 > 8|15|
|3|6|6 < 15|15|
|4|2|2 < 15|15|

### Sorting method used:
Bubble Sort

### Sorting Steps:

Initial:
8 3 15 6 2

Pass 1:
3 8 6 2 15

Pass 2:
3 6 2 8 15

Pass 3:
3 2 6 8 15

Pass 4:
2 3 6 8 15

Sorted List:
2 3 6 8 15

### Explanation:

To find the largest element, every number is compared with the current maximum once. Since every element must be checked, the algorithm performs n−1 comparisons, giving a time complexity of **O(n)**.

---

# Part 2. Stack or Queue

### Stack order:

Task5

Task4

Task3

Task2

Task1

### Queue order:

Task1

Task2

Task3

Task4

Task5

### Printer should use:

Queue

### Reason:

A printer should print jobs in the same order they arrive. Queue follows the FIFO (First In First Out) principle, ensuring fairness.

### Dry Run:

Stack (LIFO)

Push:
Task1

Task2

Task3

Task4

Task5

Pop:

Task5

Task4

Task3

Task2

Task1

Queue (FIFO)

Enqueue:

Task1

Task2

Task3

Task4

Task5

Dequeue:

Task1

Task2

Task3

Task4

Task5

### Explanation:

A stack removes the most recently added item first (LIFO). A queue removes the oldest item first (FIFO), making it suitable for printer scheduling.

---



# Part 4. Count the Steps

### Single loop runs:

5 times

### Nested loop total prints:

25 times

### Dry Run

Single Loop

i = 1 → Print

i = 2 → Print

i = 3 → Print

i = 4 → Print

i = 5 → Print

Total = 5 prints

Nested Loop

For i = 1:

j = 1 to 5 → 5 prints

For i = 2:

5 prints

For i = 3:

5 prints

For i = 4:

5 prints

For i = 5:

5 prints

Total = 25 prints

### For n = 10

Single loop runs:

10 times

Nested loop runs:

100 times

### Explanation

A single loop performs one operation per iteration, so it grows linearly (**O(n)**). A nested loop performs n operations for each of n iterations, resulting in **O(n²)** growth.

---

# Acceptance Criteria

## Part 1

**Input:**

List of integers

**Output:**

Largest number and sorted list

**Data Structure Used:**

Array (List)

**Growth:**

Linear (**O(n)**) for finding maximum.

Bubble sort grows quadratically (**O(n²)**).

---

## Part 2

**Input:**

Task1, Task2, Task3, Task4, Task5

**Output:**

Order of execution

**Data Structure Used:**

Stack and Queue

**Growth:**

Proportional (**O(n)**), because each task is processed once.

---

## Part 3

**Input:**

Subject hierarchy

**Output:**

Tree and level-order traversal

**Data Structure Used:**

Tree (Queue for level-order traversal)

**Growth:**

Proportional (**O(n)**), since each node is visited once.

---

## Part 4

**Input:**

Loop limits

**Output:**

Number of iterations

**Data Structure Used:**

None

**Growth:**

Single loop → Linear (**O(n)**)

Nested loops → Quadratic (**O(n²)**)

If the input size increases by 100×:

- Linear algorithms take about **100×** more work.
- Quadratic algorithms take about **10,000×** more work, so they grow much faster.

---

# How to Run

```bash
python part1_trace.py
python part2_stack_queue.py
python part3_tree.py
python part4_complexity.py
```
