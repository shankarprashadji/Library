# Simple Library Website

This website allows users to manage their Books, which includes add, remove, and sort their Books.


**Class-Based Structure:**

***Book*** 
class encapsulates the details of book.


```
class Book {
  constructor(title, author, ISBN) {
    this.title = title;
    this.author = author;
    this.ISBN = ISBN;
  }
}
```
1. **Properties:**

   - `title`: This property stores the book's title
   - `author`: This property stores the book's author
   - `ISBN`: This property stores the book's ISBN

   This class efficiently bundles these properties, ensuring they are logically organized and encapsulated.


***Library***
class encapsulates the data of book list and method that manipulate book.
1. **Properties:**
```
static books = [];
```

- `Books`: this property Store list of books object 


2. **Methods:**

```
static getBooks() {
    if (
      localStorage.getItem("books") === null ||
      localStorage.getItem("books") === undefined
    ) {
      {
        this.books = bookData;
        localStorage.setItem("books", JSON.stringify(this.books));
      }
    } else {
      this.books = JSON.parse(localStorage.getItem("books"));
    }
    return this.books;
  }
```

   - `getBooks()`: This method allows users to get Books from localStorage,if user first time open this website than localStorage empty for this website then Some books Stores on localStorage. If user already use this website than this method return already store books

 ```
 static addBook(book) {
    this.books.push(book);

    localStorage.setItem("books", JSON.stringify(this.books));
  }
  ```

   - `addBook(book)`: Users can utilize this method to add book. It then updates the localstorage and UI accordingly.

```
static removeBook(ISBN) {
    this.books = this.books.filter((book) => book.ISBN !== ISBN);
    localStorage.setItem("books", JSON.stringify(this.books));
  }
```
- `removeBook(ISBN)`: Users can utilize this method to remove book. 

```
static removeAllBooks() {
    this.books = [];
    localStorage.setItem("books", JSON.stringify(this.books));
  }
```
- `removeAllBooks()`: Users can use this method to remove all books.

```
 static sort(headName) {
    switch (headName) {
      case "title":
        this.books.sort((a, b) => {
          if (a.title > b.title)
            return 1
          else if (a.title < b.title)
            return -1
          else return 0
        })
        break;
      case "author":
        this.books.sort((a, b) => {
          if (a.author > b.author)
            return 1
          else if (a.author < b.author)
            return -1
          else return 0
        })
        break;
      case "bookId":
        this.books.sort((a, b) => {
          if (a.ISBN > b.ISBN)
            return 1
          else if (a.ISBN < b.ISBN)
            return -1
          else return 0
        })
        break;
    }
    localStorage.setItem("books", JSON.stringify(this.books));
  }
}
```

- `sort(headName)`: This method use for sort books by `title`, `author` and `book id`

**Switch Statements for User Actions:**

The JavaScript file effectively uses a `switch` statement to handle different user actions:

- **Deposit**: When the user selects "Deposit" from the action dropdown, the corresponding case executes the `deposit` method of the `BankAccount` class, facilitating the addition of funds to the account.

- **Withdraw**: The "Withdraw" case invokes the `withdraw` method, enabling users to withdraw funds, provided the withdrawal amount is valid.

- **Check Balance**: The "Check Balance" case does not perform any specific action but allows users to view their current balance.

- **Default**: In the default case, an error message is generated for invalid actions, ensuring that the user receives clear feedback.

This `switch` statement enhances code readability and maintainability by neatly organizing action-related logic.

**Try-Catch-Finally Statements for Error Handling:**

Robust error handling is a key feature of this JavaScript file, which employs `try-catch-finally` statements to ensure a smooth and secure user experience:

- **Try Block**: Within the `try` block, each user action is attempted. This includes depositing, withdrawing, and checking the balance.

- **Catch Block**: In the event of an error, such as an invalid amount or insufficient funds, the `catch` block captures the error and generates user-friendly error messages. This ensures that users receive clear and informative feedback about the nature of the issue.

- **Finally Block**: The `finally` block guarantees that specific actions are taken regardless of whether an error occurred or not. It clears the input fields after each transaction, offering users a seamless and clean interface for subsequent actions.

These error-handling mechanisms contribute to the website's robustness, enhancing user trust and confidence in the platform.


git add . 
git commit -m "update"  
git push