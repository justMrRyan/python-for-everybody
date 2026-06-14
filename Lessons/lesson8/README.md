# 🐍 Python for Everybody – Lesson 8: Organizing Data with Dictionaries

Welcome to Lesson 8! 🎉  
You’ve mastered lists—great for storing sequences. Now it’s time to learn about **dictionaries**, which let you store data using **key-value pairs**. Dictionaries are like mini databases: you label each piece of data so you can access it quickly and clearly.

---

## 🎯 Learning Objectives

By the end of this lesson, you will be able to:

- Create and use dictionaries in Python  
- Access, modify, and loop through key-value pairs  
- Use dictionary methods like `get()`, `keys()`, and `values()`  
- Build programs that organize and retrieve labeled data

---

## 📦 What is a Dictionary?

A **dictionary** is a collection of key-value pairs.  
Each key is a label, and each value is the data associated with it.

### ✅ Syntax

```python
person = {
    "name": "Ryan",
    "age": 21,
    "hobby": "coding"
}
```

---

## 🔍 Accessing Values

Use the key to get the value.

```python
print(person["name"])   # Ryan
print(person["age"])    # 21
```

---

## ✏️ Modifying Values

You can change values by assigning a new one to a key.

```python
person["age"] = 22
```

---

## ➕ Adding and Removing Items

### 🔹 Add a new key-value pair

```python
person["city"] = "Tunis"
```

### 🔹 Remove a key-value pair

```python
del person["hobby"]
```

---

## 🔁 Looping Through a Dictionary

### 🔹 Loop through keys

```python
for key in person:
    print(key)
```

### 🔹 Loop through values

```python
for value in person.values():
    print(value)
```

### 🔹 Loop through key-value pairs

```python
for key, value in person.items():
    print(key + ":", value)
```

---

## 🔢 Useful Dictionary Methods

| Method         | Description                          |
|----------------|--------------------------------------|
| `dict.get(key)`| Returns value or `None` if missing   |
| `dict.keys()`  | Returns all keys                     |
| `dict.values()`| Returns all values                   |
| `dict.items()` | Returns all key-value pairs          |

---

## 🧪 Practice Exercises

### 📝 Exercise 1: Student Profile

Write a program that:

- Creates a dictionary with name, age, and grade  
- Prints each item using a loop  
- Updates the grade  
- Adds a new key `"passed"` with value `True`

---

### 📝 Exercise 2: Word Translator

Write a program that:

- Creates a dictionary of English-to-French words  
- Asks the user for an English word  
- Prints the French translation using `get()`

---

## 🧪 Mini Project: Contact Book

Create a program that:

1. Stores contacts in a dictionary (`name: phone number`)  
2. Lets the user add, search, and delete contacts  
3. Prints the contact list after each action

### ✅ Example:

```python
contacts = {}

while True:
    action = input("Add, search, delete, or quit? ").lower()
    
    if action == "add":
        name = input("Enter name: ")
        number = input("Enter phone number: ")
        contacts[name] = number
    elif action == "search":
        name = input("Enter name to search: ")
        print("Number:", contacts.get(name, "Not found"))
    elif action == "delete":
        name = input("Enter name to delete: ")
        if name in contacts:
            del contacts[name]
        else:
            print("Contact not found.")
    elif action == "quit":
        break
    else:
        print("Invalid action.")
    
    print("Contacts:", contacts)
```

---

## 💬 Instructor Note

> "Dictionaries are like labeled boxes for your data. They help you organize information in a way that’s easy to search, update, and manage. Once you master dictionaries, you can build real-world apps like contact books, settings managers, and user profiles."

---

## [⏭️ What’s Next?](https://github.com/justMrRyan/python-for-everybody/tree/main/Lessons/lesson9)

In **Lesson 9**, we’ll explore:

- Working with files  
- Reading and writing data to `.txt` files  
- Saving user input and loading it later

---

## 📚 Bonus Resources

- [Python Docs – Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)
- [Python Tutor – Visualize Dictionaries](https://pythontutor.com/)

---

## 🙌 Keep Going!

You’ve now learned how to label and organize data using dictionaries.  
This opens the door to building smarter, more structured programs. Keep experimenting—you’re building real-world skills!
