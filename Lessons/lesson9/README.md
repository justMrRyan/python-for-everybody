# 🗂️ Lesson 9: Reading and Writing Files in Python

Welcome back! In this lesson, we’ll unlock a powerful new skill: working with files.  
This means your programs can now **store data permanently**—like saving notes, logs, or user input—even after the program ends.

Let’s dive into how Python reads and writes `.txt` files.

---

## 🎯 Objectives

By the end of this lesson, you’ll be able to:

- Open and read text files using Python  
- Write and append content to files  
- Use file modes like `'r'`, `'w'`, and `'a'`  
- Safely manage files using the `with` statement

---

## 📖 Reading Files

To read a file, use the `open()` function with mode `'r'` (read).

```python
file = open("data.txt", "r")
content = file.read()
print(content)
file.close()
```

### 🧠 Key Methods

- `read()` → Reads the entire file as one string  
- `readline()` → Reads one line at a time  
- `readlines()` → Returns a list of all lines

---

## ✍️ Writing to Files

Use mode `'w'` to write. This **overwrites** the file if it exists.

```python
file = open("output.txt", "w")
file.write("Hello, world!\n")
file.write("This is a second line.\n")
file.close()
```

---

## ➕ Appending to Files

Use mode `'a'` to **add** content without deleting existing data.

```python
file = open("output.txt", "a")
file.write("Adding a new line.\n")
file.close()
```

---

## ✅ Best Practice: `with` Statement

Using `with` automatically closes the file after use.

```python
with open("output.txt", "r") as file:
    content = file.read()
    print(content)
```

---

## 🔍 File Modes Summary

| Mode | Action                     |
|------|----------------------------|
| `'r'` | Read (default)             |
| `'w'` | Write (overwrite)          |
| `'a'` | Append                     |
| `'x'` | Create new file (error if exists) |
| `'b'` | Binary mode (for images, etc.) |

---

## 🧪 Practice Time

### 📝 Exercise 1: Save a Message

Write a program that:

- Asks the user for a message  
- Saves it to `message.txt`  
- Confirms the message was saved

---

### 📝 Exercise 2: Read a Poem

Create a file called `poem.txt` with 3 lines of text.  
Write a program that reads and prints each line.

---

## 🛠️ Mini Project: Simple Note Keeper

Build a basic note-taking app:

```python
while True:
    action = input("Choose: write / view / quit: ").lower()
    
    if action == "write":
        note = input("Enter your note: ")
        with open("notes.txt", "a") as file:
            file.write(note + "\n")
    elif action == "view":
        with open("notes.txt", "r") as file:
            print("Your notes:")
            print(file.read())
    elif action == "quit":
        break
    else:
        print("Invalid option.")
```

---

## 💬 Instructor Tip

> “Files are where your programs come alive. They let you save progress, store data, and build real tools. Once you master file handling, you’re ready to build apps that remember.”

---

## [⏭️ Coming Up Next](https://github.com/justMrRyan/python-for-everybody/tree/main/Lessons/lesson10)

In Lesson 10, we’ll explore:

- Handling errors with `try` and `except`  
- Writing programs that don’t crash  
- Making your code more reliable and user-friendly

---

## 📚 Extra Resources

- [Python Docs – File I/O](https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files)  
- [Real Python – Read & Write Files](https://realpython.com/read-write-files-python/)

---

## 🚀 You’re Doing Great!

Reading and writing files is a major milestone.  
Now your programs can interact with the real world—saving notes, logs, and more. Keep practicing and experimenting!
