<h1>
  <span class="headline">Python Loops</span>
  <span class="subhead">While Loops</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to understand and use while loops to execute code repeatedly while a condition is true, recognize and avoid infinite loops, and apply these concepts in practical coding exercises.

| Lesson      | Duration |
| ----------- | -------- |
| While Loops | 30 min   |

## `while` Loop

A while loop is very straightforward. It continues executing while the condition you've given it is still true. Once the condition is false, it stops!

```python
number = 0
while number < 10:
    number = number + 1
    print(number)
```

## Discussion: What Will This Code Do? TKTK

```python
number = 1
while number > 0:
    number = number + 1
    print(number)
```

> 🍎 Take a moment to think about how the loop works and keep track of the number's value. Remember, the loop goes "back to the top" and checks the condition again before continuing. If the condition is always true, it creates an infinite loop!

## Caution! Infinite Loops Ahead

Be careful with while loops! If the _condition is never broken_, you'll have an unending loop that will devour your computer's processing power.

```python
number = 1
while number > 0:
    number = number + 1
    print(number)
```

## Solo Exercise: 4.1 While Loops 20 min TKTK

Use while loops to complete the challenges in **Section 4.1** of the Jupyter Notebook.

![Image Placeholder](TKTK)
