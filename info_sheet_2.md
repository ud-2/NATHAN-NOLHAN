# 🐍 Python Programming Exam - Level 2
**Total Points:** 20 marks

---

## Part I: Conceptual Logic (4 Marks)
*Provide concise and clear answers.*

**1. (2 pts) Variable Swapping:**
You have two variables: `a = 10` and `b = 20`. Without assigning the numbers 10 and 20 directly, write a short Python snippet (2-3 lines) to swap their values so that `a` becomes 20 and `b` becomes 10. Briefly explain how your code works.

**2. (2 pts) Loop Mechanics:**
Explain the difference between iterating *directly over the items* in a list versus iterating *over the indices* using `range()`. Provide a one-line code example of how to start each type of loop.

---

## Part II: Code Tracing (5 Marks)
*Read the following snippets and write down the **exact** output that will be printed on the screen.*

**Snippet A (3 pts):**
```python
x = 5
y = 0
while x > 0:
    if x % 2 == 0:
        y = y + x
    x = x - 1
print(y)
```

**Snippet B (2 pts):**
```python
data = [10, 20, 30]
result =[]
for i in range(len(data)):
    result.append(data[i] + i)
print(result)
```

---

## Part III: Logic Debugging (4 Marks)
*The following function is supposed to find and return the **smallest** number in a list of temperatures. However, when we run it with the list provided, it outputs `0` instead of `3`. There are no syntax errors, but there is a **logic error**.*

```python
def find_minimum(temperatures):
    minimum = 0
    for temp in temperatures:
        if temp < minimum:
            minimum = temp
    return minimum

daily_temps =[12, 5, 8, 3, 22]
print(find_minimum(daily_temps))
```

**Task:** 
1. **(2 pts)** Explain *why* the code currently prints `0`.
2. **(2 pts)** How would you fix the logic? Write down the corrected line(s) of code.

---

## Part IV: Practical Programming Challenge (7 Marks)

**The Scenario: Cocoa Harvest Analysis in Cameroon**
A local cooperative in Cameroon needs a program to analyze the daily cocoa harvest brought in by different farmers. You are given a list of weights (in kilograms). 

**The Task:**
Write a program containing a function called `analyze_harvest(harvest_list, threshold)`. 
**Constraint:** You are **NOT allowed** to use Python's built-in mathematical functions like `sum()`, `max()`, or `min()`. You must build the logic yourself using loops.

Inside your function, use a **single loop** to go through the list and find:
1. The **total weight** of all the cocoa collected.
2. The weight of the **heaviest single harvest** (the maximum value).
3. The **count** of how many farmers brought in an amount equal to or greater than the `threshold`.

After the loop, the function should print these three statistics clearly.

**Test your code by writing a call to the function at the bottom:**
Assuming `harvests =[45, 12, 60, 33, 85, 20]`, call your function to analyze this list with a threshold of `40` kg.
