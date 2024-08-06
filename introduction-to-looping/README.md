<h1>
  <span class="headline">Python Loops</span>
  <span class="subhead">Introduction to Looping</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to understand the importance of loops in programming and recognize the need for iterative solutions in coding.

# Loops

| Lesson                  | Duration |
| ----------------------- | -------- |
| Introduction to Looping | 15 min   |

## Today’s Learning Objectives

In this Module, you will:

- Use loops to iterate over code blocks repeatedly.
- Differentiate between while and for loops.
- Use list comprehension to generate lists using loop syntax.

## What We’ll Practice Today

This Module connects to and reinforces topics that you encountered in the pre-work.
We’re going to return to topics covered in the pre-work and build upon them:

- For loops
- While loops

## Solo Exercise: Jupyter Notebook (10 min) TKTK

Let’s dive right in and use what we learned in the pre-work! We want to understand where you are in your learning journey so that we can give the best possible experience in class.

- Look over the exercises in today's Jupyter Notebook and attempt any that seem immediately doable to you.

- Then, rate your confidence level on today's subjects from 1–5.

## Discussion: Life Without Loops TKTK

Imagine that we have a list of colors and we want to print each one:

```python
colors = ["red", "orange", "yellow"]
print(colors[0])
print(colors[1])
print(colors[2])
```

Does this seem sustainable?

- Remember the "Don't repeat yourself" mantra—it’s a key principle in coding.
- Repeating the same code over and over can be time-consuming, especially if the list changes and requires constant updates.
- Plus, repeating code increases the risk of making mistakes, like typos, which can cause errors in your program.

---

## What is a Loop?

> Loop: A control flow statement allowing for the **_repeated execution of a code block_** until a specific condition is reached.

![Image Placeholder](TKTK)

## Why Loops?

Loops take advantage of what computers do best: evaluate instructions across organized sets of data very quickly.

Computers excel when working in isolated patterns, which is exactly how a loop works.
You can avoid needlessly copying or re-typing code by repeating it in a loop.

![Image Placeholder](TKTK)

- When dealing with lists of data from databases or other web apps, we often don’t know how many items there will be, so hard-coding operations isn’t practical.

- Instead of copying and pasting code, we can use tools like `len()` and loops to handle any number of items efficiently!
