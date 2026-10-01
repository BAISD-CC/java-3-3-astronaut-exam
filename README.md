# Ch. 3 Challenge 3: Astronaut Exam

## Mission Briefing

We have developed an exam of five tasks for our astronauts, and we need to convert each astronaut's raw score into a percentage that we can later use to rank them. Your program reads how many tasks an astronaut completed and reports the percentage from the scoring table, or reports that the number is not valid.

## What You'll Practice

- `Scanner` input of an `int` (Chapter 2)
- A `switch` with `case`, `break`, and `default` (Day 3 notes, E3-B)
- An if-else-if chain with a trailing else also works (Day 1 notes, E1-C)

## Starter Code

Edit `src/AstronautExam.java`. The class is named `AstronautExam`. Do not rename the file or the class.

The comments in `main` list the steps in order. You may follow them or solve the problem your own way.

## Inputs

| Order | Input | Type |
|---|---|---|
| 1 | Number of tasks completed | `int` |

## Rules

### 1. Convert tasks to a percentage

| Tasks completed | Percentage |
|---|---|
| 0 | 0 |
| 1 | 10 |
| 2 | 25 |
| 3 | 45 |
| 4 | 70 |
| 5 | 100 |

### 2. Reject an invalid number of tasks

| Tasks completed | Result |
|---|---|
| **below** 0 | Print the invalid message only. |
| 0 **through** 5 | Print the score line. |
| **above** 5 | Print the invalid message only. |

## What to Use

These tools fit this problem. They are suggestions: any approach that produces the correct output earns full credit.

- A `switch` on the number of tasks, one `case` per row of the table, and `default` for everything else.
- Or an if-else-if chain with a trailing else.

## Exact Output

Spelling, capitalization, and punctuation must match exactly.

Prompt (on its own line; the user types on the next line):

```text
How many tasks did the astronaut complete?
```

Then exactly one of these:

```text
The astronaut's score is [percentage] percent.
Invalid number of tasks. Enter 0 through 5.
```

## Sample Runs

```text
How many tasks did the astronaut complete?
4
The astronaut's score is 70 percent.
```

```text
How many tasks did the astronaut complete?
7
Invalid number of tasks. Enter 0 through 5.
```

## Test Your Program

Run every row before you submit. The autograder uses these values.

| Tasks | Expected output |
|---|---|
| 0 | The astronaut's score is 0 percent. |
| 1 | The astronaut's score is 10 percent. |
| 2 | The astronaut's score is 25 percent. |
| 3 | The astronaut's score is 45 percent. |
| 4 | The astronaut's score is 70 percent. |
| 5 | The astronaut's score is 100 percent. |
| -1 | Invalid number of tasks. Enter 0 through 5. |
| 6 | Invalid number of tasks. Enter 0 through 5. |

## How It's Checked

| Category | Points |
|---|---|
| Prompt | 2 |
| Scores for 0 through 5 (6 tests) | 18 |
| Invalid numbers rejected (2 tests) | 6 |
| **Total** | **26** |

Grading is by output only. Any approach that prints the correct lines earns full credit. Your results must come from the number the user types; a program that prints fixed answers will fail the tests that use other values.

## Where to Look

- Day 3 notes, E3-B: a switch that sets a value for each exact choice, with a default.
- Day 3 notes, Fall-Through and Stacked Labels: what happens when a break is missing.
- Day 1 notes, E1-C: an if-else-if chain with a trailing else.
