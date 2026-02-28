# SHEET 1 - PYTHON
**Duration:** 1 Hour | **Total Points:** 100

---

## Part I: Theory & Logic (20 Marks)
*Answer the following questions based on your understanding of Python fundamentals.*

1. **(5 pts)** Explain the difference between the `=` operator and the `==` operator. Give a small example of how each is used.
2. **(5 pts)** In Python, the `input()` function always returns data in a specific type. What is that type, and how do you convert it to an integer?
3. **(5 pts)** Describe the difference between a `for` loop and a `while` loop. In what situation would you prefer a `while` loop?
4. **(5 pts)** What is the index of the first element in a list? What is the index of the last element in a list of 10 items?

---

## Part II: Code Tracing (20 Marks)
*What will be the exact output printed on the screen for each code snippet?*

**1. Snippet A (5 pts)**
```python
x = 10
y = 3
if x / y > 3:
    print("Condition Alpha")
else:
    print("Condition Beta")

print(x % y)
```

**2. Snippet B (5 pts)**
```python
total = 0
numbers = [1, 3, 5]
for n in numbers:
    if n == 3:
        total = total + (n * 2)
    else:
        total = total + n
print(total)
```

**3. Snippet C (5 pts)**
```python
def modify_value(a, b):
    result = a - b
    return result

val = modify_value(10, 5)
print(val + 2)
```

**4. Snippet D (5 pts)**
```python
count = 0
while count < 4:
    if count == 2:
        print("Middle")
    else:
        print("Loop")
    count = count + 1
```

---

## Part III: Debugging (15 Marks)
*The following program is supposed to ask the user for 3 numbers, add them to a list, and calculate the sum. However, it contains **three errors**. Identify the line number and provide the fix.*

```python
1  my_list = []
2  i = 0
3  while i < 3
4      num = input("Enter a number: ")
5      my_list.append(num)
6      i = i + 1
7
8  print("The total sum is: " + sum(my_list))
```

---

## Part IV: Short Programming Tasks (20 Marks)

**1. Temperature Assistant (10 pts)**
Write a program that asks the user for the current temperature in Celsius.
- If the temperature is above 30, print "It is hot".
- If it is between 15 and 30 (inclusive), print "It is pleasant".
- If it is below 15, print "It is cold".

**2. List Searcher (10 pts)**
Write a function called `find_in_list(target, items)` that takes a value (`target`) and a list (`items`). 
- The function should loop through the list.
- If the target is found, it should return `True`.
- If the loop finishes and the target was never found, it should return `False`.

---

## Part V: Final Project: The Mini-Store (25 Marks)

Create a program that manages a simple shopping list for a user. Your program must include the following features:

1.  **The Menu:** Use a `while` loop to display a menu that keeps running until the user chooses to "Exit".
    *   1. Add item
    *   2. View list
    *   3. Exit
2.  **Adding Items:** If the user chooses '1', ask for the name of the item and add it to a list called `shopping_cart`.
3.  **Viewing:** If the user chooses '2', use a `for` loop to print every item in the list. If the list is empty, print "Your cart is empty".
4.  **Exit:** If the user chooses '3', print a "Goodbye" message and stop the loop.

**Constraints:** 
- Use at least one function.
- Ensure inputs are handled correctly (e.g., the user enters a number for the menu).
