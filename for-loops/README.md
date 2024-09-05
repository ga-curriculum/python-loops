<h1>
  <span class="headline">Python Loops</span>
  <span class="subhead">For Loops</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to effectively use for loops to iterate over lists and other collections.

| Lesson    | Duration |
| --------- | -------- |
| For Loops | 50 min   |

## `for` Loop

A `for loop` is geared more toward iterating over lists or collections of data:

- Define a variable to act as our **iterator**.

- Provide the **iterable value**, typically a list.

```python
for number in [0,1,2,3,4,5]:
    print(number)

# outputs 0,1,2,3,4,5
```

> 💡 This is a great chance to break down how the loop works step by step. Use a cross-chart or manually track the values of variables as you go. Talking through each step out loud can help you understand how the loop operates, just like using a debugger.

## The Naming of Things

Remember, clear naming and syntax are one of Python’s great advantages. Don’t spoil it by naming your iterator something vague — be descriptive!

```python
# x is not descriptive!

colors = ["red","yellow"]

for x in colors:
    print(x)
```

```Python
# color is more accurate

colors = ["red","yellow"]

for color in colors:
    print(color)
```

<br>

<div class="activity solo-exercise">
  <h2 class="title">4.2 For Loops</h2>
  <span class="minutes">15 min</span>
</div>

Let's practice some for loops by looping over a list of numbers in **Section 4.2** of the workbook.

<img src="./assets/pencils-cup.png" alt="Pencils in Cup Image" style="width: 300px; height: auto;">

## Using the `range()` Function

Because for loops require an iterable, it's common to use the `range()` function to automatically generate a list of numbers over which to iterate.

```python
for number in range(6):
    print(number)

# outputs 0,1,2,3,4,5
```

> 💡 Why isn't 6 included in the output?

## The Many Faces of `range()`

| #                | Explanation                                                                                                               | Example         |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------- | --------------- |
| One parameter    | A list from zero up to, but not including, the given number.                                                              | `range(5)`      |
|                  |                                                                                                                           | `[0,1,2,3,4]`   |
| Two parameters   | A list including the first number, up to, but not including, the second number.                                           | `range(5, 10)`  |
|                  |                                                                                                                           | `[5,6,7,8,9]`   |
| Three parameters | A list from the first number up to, but not including, the second number, increasing (or "striding") by the third number. | `range(1,10,2)` |
|                  |                                                                                                                           | `[1,3,5,7,9]`   |

## Looping With Indices

If you want to actually modify a list while looping, you must use indices:

```python
numbers = [1,2,3,4]

list_length = len(numbers)

for i in range( len(numbers) ):
    numbers[i] = numbers[i] * 2
```

- Let's break down this code and understand why using `range()` is useful for looping over lists.
- In this example, `range( len(numbers) )` creates a sequence of indices (0, 1, 2, 3) that allow us to access and modify each item in the numbers list.
- If you used `for number in numbers`, you'd be working with a copy of each number, not the original list. This means changes would not be reflected in the `numbers` list.

## Looping Over Dictionaries

Dictionaries have an `.items()` method to help loop through keys and values.

```python
author = { "first_name": "Kazuo", "last_name": "Ishiguro" }

for key, value in author.items():
    print(value)
```

- In this code, `author.items()` is used to loop over the dictionary. It provides a way to access both the keys and values in the dictionary.

- Each item returned by `.items()` is a tuple containing a key and its corresponding value.

- In the loop, `key` and `value` are used to unpack these tuples. Here, we're only interested in `value`, which is why we print it directly.

- This approach allows you to work with both the keys and values of a dictionary, though in this case, we’re focusing on the values.

---

## Nested Loops

Just as it’s possible to nest data structures inside of each other, it is also possible to put loops inside of other loops.

```python
for num_one in range(1,13):
    for num_two in range(1,13):
        print(f"{num_one} times {num_two} = {num_one * num_two}")
```

> 💡 While nested loops are sometimes necessary, this will result in increased complexity, both for you as a programmer and for the computer while executing the program.

## For vs. While: Which One to Use?

| **`while` Loops:**                                                                                                                                                                             | **`for` Loops:**                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| - Great for instances when you have no way of knowing how many times you need to iterate. <br> - Useful for things like random chance or eliminating specific items of an undetermined amount. | - The most common loops, used when you know exactly how many times you need to iterate <br> - If you have a list and need to look through every item, use a for loop. |

<br>

<div class="activity knowledge-check">
  <h2 class="title">For or While?</h2>
  <span class="minutes">2 min</span>
</div>

Which loop type should be used in each of these scenarios?

1. Look through a list to find the largest number.
2. Flip a coin until heads shows up three times in a row.
3. Print every value in a list.
4. Animate a game screen until the player's health is zero.
5. Check the weather every five seconds until it rains.

<details>
<summary>✅ Click to see the answer: </summary>
<hr>

Answers:

<ol>
  <li>For</li>
  <li>While</li>
  <li>For</li>
  <li>While</li>
  <li>While</li>
</ol>

</details>

## List Comprehension

Here’s a neat trick for creating new lists using a loop-like syntax:

```python
numbers = [1,2,3,4,5]

even_numbers = [num * 2 for num in numbers]

# even_numbers is [2,4,6,8,10]
```

> 💡 List comprehension is very common in data analysis applications, and it's important to be able to read the syntax in the examples you'll come across.

<br>

<div class="activity solo-exercise">
  <h2 class="title">4.3 List Comprehension</h2>
  <span class="minutes">15 min</span>
</div>

Shortcuts like list comprehension are what make experienced programmers fall in love with Python.

Let’s try out some challenges using list comprehension instead of loops in **Section 4.3** of the workbook.

<br>

<div class="activity group-exercise">
  <h2 class="title">4.4 Hold on to Your Loops</h2>
  <span class="minutes">20 min</span>
</div>

Things can start getting complicated now that we have loops, conditionals, and data structures!

The challenges in **Section 4.4** will be tough, so be sure to lean on print statements to help navigate your way through these tasks one step at a time.
