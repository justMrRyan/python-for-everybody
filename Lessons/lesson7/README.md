# 🐍 Python for Everybody – Lesson 7: Working with Lists

Welcome to Lesson 7! 🎉  
So far, you’ve learned how to write functions and organize your code. Now it’s time to explore **lists**—Python’s way of storing multiple values in a single variable. Lists are perfect for handling collections like names, scores, or items in a shopping cart.

---

## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Create and use lists in Python  
- Access, modify, and loop through list items  
- Use built-in list methods like `append()`, `remove()`, and `len()`  
- Write programs that manage collections of data

---

## 📦 What is a List?

A **list** is a container that holds multiple values in a specific order.

### ✅ Syntax

```python
my_list = [value1, value2, value3]
```

### 🧪 Example:

```python
fruits = ["apple", "banana", "cherry"]
print(fruits)
```

This prints:  
```
['apple', 'banana', 'cherry']
```

---

## 🔍 Accessing List Items

Use **indexing** to access items. Indexes start at `0`.

```python
print(fruits[0])  # apple
print(fruits[2])  # cherry
```

---

## ✏️ Modifying List Items

You can change items using their index.

```python
fruits[1] = "blueberry"
print(fruits)  # ['apple', 'blueberry', 'cherry']
```

---

## ➕ Adding and Removing Items

### 🔹 `append()` – Add to the end

```python
fruits.append("orange")
```

### 🔹 `remove()` – Remove by value

```python
fruits.remove("apple")
```

### 🔹 `pop()` – Remove by index

```python
fruits.pop(0)
```

---

## 🔁 Looping Through a List

Use a `for` loop to go through each item.

```python
for fruit in fruits:
    print("I like", fruit)
```

---

## 🔢 Useful List Functions

| Function     | Description                     |
|--------------|---------------------------------|
| `len(list)`  | Returns the number of items     |
| `sorted(list)` | Returns a sorted version      |
| `list.append(x)` | Adds item to the end        |
| `list.remove(x)` | Removes item by value       |
| `list.pop(i)`    | Removes item by index       |

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Favorite Movies

Write a program that:

- Creates a list of 3 favorite movies  
- Prints each one using a loop  
- Adds a new movie using `append()`  
- Removes one using `remove()`

---

### 📝 Exercise 2: Number Stats

Write a program that:

- Asks the user for 5 numbers  
- Stores them in a list  
- Prints the total, average, and largest number

Hint: Use `sum()`, `len()`, and `max()`.

---

## 🧪 Mini Project: To-Do List Manager

Create a program that:

1. Starts with an empty list  
2. Asks the user to add tasks  
3. Lets them remove tasks  
4. Prints the updated list after each change

### ✅ Example:

```python
tasks = []

while True:
    action = input("Add, remove, or quit? ").lower()
    
    if action == "add":
        task = input("Enter a task: ")
        tasks.append(task)
    elif action == "remove":
        task = input("Enter task to remove: ")
        if task in tasks:
            tasks.remove(task)
        else:
            print("Task not found.")
    elif action == "quit":
        break
    else:
        print("Invalid action.")
    
    print("Current tasks:", tasks)
```

---

## 💬 Instructor Note

> "Lists are the backbone of data management in Python. Whether you're building a game, a survey, or a data processor, lists help you store and organize information. Practice looping, modifying, and managing lists—you’ll use them everywhere."

---

## [⏭️ What’s Next?](https://github.com/justMrRyan/python-for-everybody/tree/main/Lessons/lesson8)

In **Lesson 8**, we’ll explore:

- Dictionaries: storing data with labels  
- Key-value pairs and how to use them  
- Building programs that organize complex information

---

## 📚 Bonus Resources

- [Python Docs – Lists](https://docs.python.org/3/tutorial/datastructures.html)
- [Python Tutor – Visualize Lists](https://pythontutor.com/)

---

## 🙌 Keep Going!

You’ve now learned how to manage collections of data using lists.  
This unlocks a whole new level of programming power—keep experimenting and building!
