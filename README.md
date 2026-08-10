# Astronaut Exam

We have developed an exam consisting of five tasks for our astronauts, and we need to convert their raw score into a percentage that we can later use to rank astronauts.

## Scoring Table

Convert the number of completed tasks into a percentage using this table:

| Tasks Completed | Percentage |
|------------------|------------|
| 0                | 0          |
| 1                | 10         |
| 2                | 25         |
| 3                | 45         |
| 4                | 70         |
| 5                | 100        |

## What You Are Building

Write a program that:

1. Uses a `Scanner` to ask the user how many tasks the astronaut completed.
2. Uses `if` / `else if` statements to determine the correct percentage from the table above.
3. Displays the percentage earned.

Do not hard-code a single output value — your program must use `if` / `else if` logic to look up the correct percentage for whatever number of tasks the user enters.

## Expected Input and Output

Your program must print the prompt exactly as shown below:

```
How many tasks did the astronaut complete?
```

After the user enters a number, display the result exactly as shown below (with the correct percentage in place of `[percentage]`):

```
The astronaut's score is [percentage] percent.
```

For example, if the user enters `4`, your program should display:

```
The astronaut's score is 70 percent.
```

## Requirements

- Use a `Scanner` to read the number of tasks completed from the user as an `int`.
- Use `if` / `else if` statements to determine the percentage based on the table above.
- Display the result using the exact wording shown above.
