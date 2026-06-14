# 🐍 Python for Everybody – Lesson 3: Operators and Expressions

Welcome to Lesson 3! 🎉  
Now that you know how to store data in variables, it’s time to learn how to **do something** with that data. In this lesson, we’ll explore **operators** and **expressions**—the tools Python uses to perform calculations and make decisions.

---

## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Use arithmetic operators to perform calculations  
- Use comparison operators to compare values  
- Use logical operators to combine conditions  
- Write expressions that evaluate to `True` or `False`  
- Build programs that make decisions based on user input

---

## ➕ Arithmetic Operators

These operators let you do math in Python.

| Operator | Meaning        | Example       | Result     |
|----------|----------------|---------------|------------|
| `+`      | Addition        | `2 + 3`       | `5`        |
| `-`      | Subtraction     | `5 - 2`       | `3`        |
| `*`      | Multiplication  | `4 * 3`       | `12`       |
| `/`      | Division        | `10 / 2`      | `5.0`      |
| `**`     | Exponentiation  | `2 ** 3`      | `8`        |
| `%`      | Modulo (remainder) | `7 % 3`   | `1`        //
| `//`     | Floor Division  | `7 // 3`      | `2`        //

### 🧪 Example:

```python
a = 10
b = 3
print("Sum:", a + b)
print("Power:", a ** b)
print("Remainder:", a % b)
```

---

## 🔍 Comparison Operators

These operators compare values and return `True` or `False`.

| Operator | Meaning           | Example       | Result     |
|----------|-------------------|---------------|------------|
| `==`     | Equal to          | `5 == 5`      | `True`     |
| `!=`     | Not equal to      | `5 != 3`      | `True`     |
| `>`      | Greater than      | `7 > 4`       | `True`     |
| `<`      | Less than         | `3 < 8`       | `True`     |
| `>=`     | Greater or equal  | `5 >= 5`      | `True`     |
| `<=`     | Less or equal     | `4 <= 6`      | `True`     |

### 🧪 Example:

```python
age = int(input("Enter your age: "))
print("Are you an adult?", age >= 18)
```

---

## 🔗 Logical Operators

These operators combine multiple conditions.

| Operator | Meaning       | Example                  | Result     |
|----------|---------------|--------------------------|------------|
| `and`    | Both must be true | `True and False`     | `False`    |
| `or`     | At least one true | `True or False`      | `True`     |
| `not`    | Negates a value   | `not True`           | `False`    |

### 🧪 Example:

```python
age = int(input("Enter your age: "))
has_id = input("Do you have an ID? (yes/no): ") == "yes"
print("Can enter club:", age >= 18 and has_id)
```

---

## 🧠 Expressions

An **expression** is any combination of variables, values, and operators that Python can evaluate.

### ✅ Examples:

```python
x = 5
y = 2
result = (x + y) * 3
print("Result:", result)
```

Expressions can be used in `print()`, `if` statements, and anywhere Python expects a value.

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Calculator

Write a program that:

- Asks for two numbers  
- Asks for an operation (`+`, `-`, `*`, `/`)  
- Performs the operation and prints the result

---

### 📝 Exercise 2: Voting Eligibility

Write a program that:

- Asks for age and nationality  
- Checks if the user is eligible to vote (age ≥ 18 and nationality == "Tunisian")  
- Prints `True` or `False`

---

## 🧪 Mini Project: Simple Quiz Checker

Create a program that:

1. Asks the user a question (e.g., "What is 2 + 2?")  
2. Checks if the answer is correct  
3. Prints a message based on the result

### ✅ Example:

```python
answer = int(input("What is 2 + 2? "))
if answer == 4:
    print("Correct!")
else:
    print("Oops, try again.")
```

---

## 💬 Instructor Note

> "Operators are the tools that give your programs logic and intelligence. With just a few symbols, you can build calculators, quizzes, and decision-making systems. Keep practicing, and soon you’ll be writing programs that think for themselves!"

---

## [⏭️ What’s Next?](https://github.com/justMrRyan/python-for-everybody/tree/main/Lessons/lesson4)

In **Lesson 4**, we’ll explore:

- Conditional statements (`if`, `else`, `elif`)  
- How to control the flow of your program  
- Writing programs that respond to different situations

---

## 📚 Bonus Resources

- [Python Docs – Operators](https://docs.python.org/3/reference/expressions.html)
- [Python Tutor – Visualize Code](https://pythontutor.com/)

---

## 🙌 Keep Going!

You’ve now learned how to make Python do math, compare values, and make decisions.  
This is the heart of programming logic—keep experimenting and building!
