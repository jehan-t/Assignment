# 📚 Library Management System (Procedural + OOP Hybrid)

This project implements a **simple Library Management System** written
in Python, using a combination of **procedural style** and
**object-oriented design**.\
The system simulates:

-   Adding books\
-   Registering members\
-   Borrowing & returning books\
-   Tracking transactions\
-   Displaying available books and borrowed books

The development was done **step-by-step**, adding one class at a time:

1.  **Book class**\
2.  **Member class**\
3.  **Library class**\
4.  **test_library_system()** for full automated testing

------------------------------------------------------------------------

## ✅ 1. Book Class

The **Book** class represents the blueprint for a book in the library.

### Features

-   Stores book ID, title, author, and number of available copies\
-   Provides a `__status__()` method to print current book info

### Attributes

  Attribute            Description
  -------------------- --------------------------
  `book_id`            Unique ID of the book
  `title`              Title of the book
  `author`             Author of the book
  `available_copies`   How many copies are left

------------------------------------------------------------------------

## ✅ 2. Member Class

The **Member** class stores information about library users.

### Features

-   Tracks the member's name, ID, email\
-   Stores a list of borrowed books\
-   Limits borrowing to **3 books per member**
-   Includes methods to borrow and return books

### Methods

  Method                    Purpose
  ------------------------- ------------------------------
  `__status__()`            Shows member info
  `can_borrowed()`          Checks if below borrow limit
  `borr_book(book_id)`      Borrow a book
  `return_books(book_id)`   Return a borrowed book

------------------------------------------------------------------------

## ✅ 3. Library Class

The core class that manages the entire system.

### Responsibilities

-   Add books to the library\
-   Register members\
-   Find books & members\
-   Borrowing and returning logic\
-   Displaying data (books available, member's books)

### Internals

The system uses three global lists: - `books` --- list of all book
dictionaries\
- `members` --- list of all member dictionaries\
- `borrowed_books` --- transaction history

------------------------------------------------------------------------

## ✅ 4. test_library_system() --- Full Automated Testing

This function performs a **complete functional test** of the system.

### What it tests:

1.  Adding books\
2.  Adding members\
3.  Borrowing books\
4.  Returning books\
5.  Borrowing limits\
6.  Error handling\
7.  Displaying library status\
8.  Re-borrowing after return\
9.  Handling invalid input\
10. Showing final report of all members & books

It prints all results to the console so you can visually verify the
system's behavior.

------------------------------------------------------------------------

## ▶️ Running the Program

Run this file directly:

``` bash
python your_file_name.py
```

This triggers:

``` python
if __name__ == "__main__":
    test_library_system()
```

You will see a full test simulation with step-by-step output.

------------------------------------------------------------------------

## 📂 Project Structure

    Library_System/
    │── library_system.py       # Main script
    │── README.md               # Documentation

------------------------------------------------------------------------

## 🌟 Summary

This project demonstrates a growing system where each class is added
step-by-step:

1.  **Book class** → data structure for books\
2.  **Member class** → structure for users\
3.  **Library class** → manages all operations\
4.  **Test system** → validates every functionality

It is perfect for practicing **OOP**, **procedural logic**, and **system
design**.
