# 🐍 Python for Everybody – Lesson 1: Communicating with Python (`print()` and `input()`)

Welcome to your first real Python lesson! 🎉  
In this module, we’ll explore how to **talk to your computer** and make it talk back. You’ll learn how to display messages, ask questions, and create your first interactive program using two essential functions: `print()` and `input()`.

---

## 📘 Why Start Here?

Every program begins with communication. Whether you're building a game, a website, or a data analysis tool, you need to:

- Show information to the user (`print()`)
- Receive information from the user (`input()`)

These two functions are the **foundation** of all interactive Python programs.

---

## 🖨️ Part 1: Using `print()` to Display Output

The `print()` function is used to show messages, results, or any kind of output on the screen.

### ✅ Syntax

```python
print("Your message here")
```

### 🧪 Examples

```python
print("Hello, world!")
print("Python is fun!")
print("2 + 2 =", 2 + 2)
```

### 🧠 What You Should Know

- Text must be inside quotes: `" "` or `' '`
- You can print numbers, strings, and even math expressions
- You can combine text and variables using commas or `+`

### 🔍 Tip: Printing Multiple Items

```python
name = "Ryan"
age = 21
print("Name:", name, "| Age:", age)
```

Or using `+`:

```python
print("Name: " + name + " | Age: " + str(age))
```

---

## 🎤 Part 2: Using `input()` to Get User Input

The `input()` function lets your program ask the user for information.

### ✅ Syntax

```python
variable = input("Your question here: ")
```

### 🧪 Examples

```python
name = input("What's your name? ")
print("Hello, " + name + "!")

age = input("How old are you? ")
print("You are " + age + " years old.")
```

### 🧠 What You Should Know

- `input()` always returns a **string**
- You can store the result in a variable
- You can use that variable later in your program

---

## 🔄 Combining `print()` and `input()`

Let’s build a simple conversation:

```python
print("Welcome to the Python chatbot!")
name = input("What's your name? ")
color = input("What's your favorite color? ")
print("Nice to meet you, " + name + "!")
print("I like " + color + " too!")
```

---

## 🧠 Concept Check

Try answering these questions:

1. What does `print()` do?
2. What does `input()` return?
3. How do you store user input in a variable?
4. How can you combine text and variables in `print()`?

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Greeting Program

Write a program that:

- Asks for the user's name
- Asks for their city
- Prints: `"Hello [name], how's the weather in [city]?"`

---

### 📝 Exercise 2: Simple Math

Write a program that:

- Asks for two numbers
- Prints their sum

Hint: You’ll need to convert the input to numbers using `int()` or `float()`:

```python
num1 = int(input("Enter a number: "))
num2 = int(input("Enter another number: "))
print("The sum is", num1 + num2)
```

---

## 🧪 Mini Project: Personal Introduction Generator

Create a program that:

1. Asks for the user's name, age, and hobby
2. Prints a short paragraph introducing them

### ✅ Example Output:

```
What's your name? Ryan  
How old are you? 21  
What's your favorite hobby? Coding  

Nice to meet you, Ryan!  
You're 21 years old and you love coding.  
That's awesome!
```

---

## 💬 Instructor Note

> "This lesson is all about starting a conversation—with your computer and with your future as a coder. `print()` and `input()` may seem simple, but they’re the gateway to building real applications. Keep experimenting, and don’t be afraid to break things. That’s how you learn!"

---

## [⏭️ What’s Next?](https://github.com/justMrRyan/python-for-everybody/edit/main/Lessons/lesson2)

In **Lesson 2**, we’ll dive into:

- Variables and data types  
- How Python stores information  
- Writing cleaner, smarter code

You’ll learn how to make your programs more powerful and flexible.

---

## 📚 Bonus Resources

- [Python Official Docs – `print()`](https://docs.python.org/3/library/functions.html#print)
- [Python Official Docs – `input()`](https://docs.python.org/3/library/functions.html#input)
- [Replit – Online Python Editor](https://replit.com/)

---

## 🙌 Keep Going!

If you’ve made it this far, you’ve already written your first Python program. That’s a huge win! 🎉  
Now go ahead and customize your code, try new questions, and make it your own.

