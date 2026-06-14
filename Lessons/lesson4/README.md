# 🐍 Python for Everybody – Lesson 4: Making Decisions with `if`, `else`, and `elif`

Welcome to Lesson 4! 🎉  
So far, you’ve learned how to store data, do math, and compare values. Now it’s time to teach Python **how to make decisions**. In this lesson, you’ll learn how to use `if`, `else`, and `elif` to control the flow of your program.

This is where your code starts to think for itself.

---

## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Use `if` statements to run code conditionally  
- Use `else` to handle alternative outcomes  
- Use `elif` to check multiple conditions  
- Write programs that respond dynamically to user input

---

## 🔍 What is a Conditional Statement?

A **conditional statement** lets your program choose what to do based on a condition.

### ✅ Syntax

```python
if condition:
    # code to run if condition is True
```

### 🧪 Example:

```python
age = int(input("Enter your age: "))
if age >= 18:
    print("You are an adult.")
```

If the condition is `True`, Python runs the indented code. If not, it skips it.

---

## 🔁 Adding `else`

Use `else` to run code when the condition is `False`.

### ✅ Example:

```python
age = int(input("Enter your age: "))
if age >= 18:
    print("Welcome to the club!")
else:
    print("Sorry, you're too young.")
```

---

## 🔄 Adding `elif` (Else If)

Use `elif` to check **another condition** if the first one is `False`.

### ✅ Example:

```python
score = int(input("Enter your score: "))
if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
else:
    print("Grade: F")
```

Python checks each condition in order and runs the first one that’s `True`.

---

## 🧠 Indentation Matters!

Python uses **indentation** (spaces or tabs) to know which code belongs to which block.

### ❌ Incorrect:

```python
if age >= 18:
print("Adult")  # This will cause an error!
```

### ✅ Correct:

```python
if age >= 18:
    print("Adult")
```

Always indent code inside `if`, `else`, and `elif` blocks.

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Even or Odd

Write a program that:

- Asks for a number  
- Prints `"Even"` if the number is divisible by 2, otherwise `"Odd"`

Hint: Use `%` and `==`

---

### 📝 Exercise 2: Temperature Checker

Write a program that:

- Asks for the temperature  
- Prints a message based on the range:

| Temperature | Message         |
|-------------|------------------|
| ≥ 30        | "It's hot!"      |
| 20–29       | "Nice weather."  |
| < 20        | "It's cold!"     |

---

## 🧪 Mini Project: Login System

Create a program that:

1. Asks for a username and password  
2. Checks if they match predefined values  
3. Prints `"Login successful"` or `"Access denied"`

### ✅ Example:

```python
username = input("Username: ")
password = input("Password: ")

if username == "admin" and password == "1234":
    print("Login successful!")
else:
    print("Access denied.")
```

---

## 💬 Instructor Note

> "Conditional statements are the brain of your program. They let your code respond to different situations and make decisions. With `if`, `else`, and `elif`, you’re building logic that adapts to the user and the world."

---

## [⏭️ What’s Next?](https://github.com/justMrRyan/python-for-everybody/tree/main/Lessons/lesson5)

In **Lesson 5**, we’ll explore:

- Loops (`while` and `for`)  
- How to repeat actions automatically  
- Writing programs that run until a condition is met

---

## 📚 Bonus Resources

- [Python Docs – `if` Statements](https://docs.python.org/3/tutorial/controlflow.html#if-statements)
- [Python Tutor – Visualize Conditionals](https://pythontutor.com/)

---

## 🙌 Keep Going!

You’ve now unlocked the power of decision-making in Python.  
Try building your own interactive programs, quizzes, or games using `if`, `else`, and `elif`. You’re officially coding with logic!
