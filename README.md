# Library Management System

The Library Management System is a Java-based application that allows users to manage a library's collection of books. It provides functionality for adding new books, displaying available books, borrowing books, and returning borrowed books.

## Features

- **Add New Books**: Users can add new books to the library by providing details such as title, author, and ISBN.
- **Display Available Books**: Users can view a list of all available books in the library.
- **Borrow Books**: Users can borrow books from the library by providing the book's ISBN.
- **Return Books**: Users can return previously borrowed books by providing the book's ISBN.

## Classes

### `Book`
The `Book` class represents a book in the library. It has the following attributes:
- `title`: The title of the book.
- `author`: The author of the book.
- `isbn`: The ISBN (International Standard Book Number) of the book.
- `available`: A boolean indicating whether the book is available for borrowing.

### `FictionBook` and `NonFictionBook`
These are subclasses of the `Book` class, representing fiction and non-fiction books, respectively.

### `Library`
The `Library` class represents the library itself. It has the following methods:
- `addBook(Book book)`: Adds a new book to the library.
- `displayAvailableBooks()`: Displays a list of all available books in the library.
- `borrowBook(User user, String isbn)`: Allows a user to borrow a book from the library by providing the book's ISBN.
- `returnBook(User user, String isbn)`: Allows a user to return a previously borrowed book by providing the book's ISBN.

### `User`
The `User` class represents a user of the library. It has the following attributes and methods:
- `userId`: A unique identifier for the user.
- `borrowedBooks`: A list of books currently borrowed by the user.
- `borrowBook(Book book)`: Adds a book to the user's list of borrowed books.
- `returnBook(Book book)`: Removes a book from the user's list of borrowed books.

### `AddNewBook`
The `AddNewBook` class provides a utility method `createNewBook()` that prompts the user to enter details about a new book and returns a `Book` object representing the new book.

### `LibraryManagementSystem`
The `LibraryManagementSystem` class is the main class that runs the Library Management System application. It creates instances of the `Library` and `User` classes and provides a menu-driven interface for users to interact with the system.

## Usage

1. Compile and run the `LibraryManagementSystem` class.
2. Follow the on-screen instructions to navigate through the menu options and perform various operations, such as adding new books, displaying available books, borrowing books, and returning borrowed books.

## Example
