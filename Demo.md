**JavaScript File: Bank Account Management**

**Class-Based Structure:**

The heart of this JavaScript file is the `BankAccount` class, which adheres to Object-Oriented Programming principles. This class encapsulates the data and behavior associated with a bank account.

1. **Properties:**

   - `accountHolder`: This property stores the account holder's name.
   - `accountType`: It holds the account type, such as "Savings" or "Checking."
   - `balance`: This property represents the current balance of the account.

   This class efficiently bundles these properties, ensuring they are logically organized and encapsulated.

2. **Methods:**

   - `deposit(amount)`: This method allows users to deposit funds into their account. It performs essential checks to ensure the amount is valid (greater than zero and not NaN) and updates the account balance accordingly.

   - `withdraw(amount)`: Users can utilize this method to withdraw funds. It performs rigorous validation, ensuring the withdrawal amount is valid (greater than zero, not NaN, and not exceeding the current balance). It then updates the balance accordingly.

This class-based structure not only provides a neat and organized way to manage account-related data but also promotes code reusability and maintainability.

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



# 2
# Bank Account Management Website

This simple website allows users to manage their bank accounts, including making deposits, withdrawals, and checking their account balance. It demonstrates the use of JavaScript classes, switch statements, and try-catch-finally statements for handling various banking operations.

## Instructions

1. **Account Information:** When you load the page, you'll see information about your bank account, including the account holder's name, account type, and the current balance.

2. **Deposit:** To make a deposit, enter the amount you want to deposit in the "Deposit Amount" input field and click the "Deposit" button.

3. **Withdraw:** To make a withdrawal, enter the amount you want to withdraw in the "Withdraw Amount" input field and click the "Withdraw" button.

4. **Check Balance:** To check your account balance, simply click the "Check Balance" button.

5. **Error Handling:** The website includes error handling using try-catch-finally statements. If you enter an invalid amount, attempt to withdraw more than your balance, or encounter any other issues, an error message will be displayed, and the transaction will be rolled back.

### JavaScript Class

The website incorporates a JavaScript class named `BankAccount` to manage bank account operations. The class has the following properties:

- `accountHolderName`: Stores the account holder's name.
- `accountType`: Stores the type of the account (e.g., Savings, Checking).
- `balance`: Tracks the current account balance.

### Switch Statements

A `switch` statement is used to determine the action to be performed based on user input. It handles three main actions:

- **Deposit:** The switch case for deposit updates the account balance by adding the deposited amount.

- **Withdraw:** The switch case for withdrawal validates the withdrawal amount, checks for sufficient funds, and updates the account balance accordingly.

- **Check Balance:** The switch case for checking the balance simply returns the current balance.

### Try-Catch-Finally Statements

- Error handling is implemented using `try-catch` blocks to capture and handle exceptions that may occur during deposit and withdrawal operations. For example, attempting to withdraw more than the available balance or entering an invalid amount will trigger errors.

- The `finally` block is used to perform any necessary cleanup actions and ensure that the input fields are cleared after a transaction, whether it was successful or not.

### Walkthrough Example

Let's walk through an example:

1. **Initial State:** When you load the page, you'll see the account holder's name as "John Doe," the account type as "Savings," and the current balance as "$0.00."

2. **Deposit:** Enter an amount (e.g., $100) in the "Deposit Amount" input field and click the "Deposit" button. The balance will be updated to "$100.00," and a success message will be displayed.

3. **Withdraw:** Enter an amount (e.g., $50) in the "Withdraw Amount" input field and click the "Withdraw" button. The balance will be updated to "$50.00," and a success message will be displayed.

4. **Check Balance:** Click the "Check Balance" button to verify that the balance is "$50.00."

5. **Error Handling:** Try withdrawing more money than the available balance, or entering an invalid amount (e.g., a negative value). You'll see error messages indicating the issues, and the transaction won't be processed.

The website provides a user-friendly interface to manage bank accounts while ensuring that errors are gracefully handled and user feedback is provided.

Feel free to use and explore this website to simulate bank account operations while learning about the use of classes, switch statements, and error handling in JavaScript.


# 3
## Bank Account Management

This website simulates bank account management. It allows users to deposit, withdraw, and check their balance. The website is built using HTML, CSS, and JavaScript.

### Classes

The website uses a class to represent a bank account. The class has properties for the balance, account holder name, and account type. The class also has methods for depositing, withdrawing, and checking the balance.

### Switch Statements

The website uses a switch statement to handle the different actions that the user can take. The switch statement checks for the value of the `action` variable, which is set when the user clicks one of the buttons. The corresponding `case` statement is then executed.

### Try-Catch-Finally Statements

The website uses try-catch-finally statements to handle exceptions. Exceptions are errors that occur during the execution of the program. The `try` block contains the code that is likely to throw an exception. The `catch` block contains the code that is executed when an exception is thrown. The `finally` block is always executed, regardless of whether an exception is thrown.

### Instructions

To use the website, follow these steps:

1. Enter your account holder name.
2. Select your account type.
3. Click the "Deposit", "Withdraw", or "Check Balance" button.
4. Follow the prompts to complete the action.

### Walkthrough

Here is a walkthrough of how the website works:

1. When the user enters their account holder name and selects their account type, the website creates a new bank account object.
2. When the user clicks the "Deposit", "Withdraw", or "Check Balance" button, the website sets the `action` variable to the corresponding value.
3. The website then calls the `performAction()` function, which uses a switch statement to handle the different actions.
4. The corresponding `case` statement is executed, which performs the desired action.
5. If an exception occurs, the `catch` block is executed.

### Conclusion

The website uses classes, switch statements, and try-catch-finally statements to implement the bank account management functionality. The classes allow the website to encapsulate the data and behavior of a bank account. The switch statements allow the website to handle the different actions that the user can take. The try-catch-finally statements allow the website to handle exceptions.




# 4

## Bank Account Management

This website simulates bank account management. It allows users to deposit, withdraw, and check their balance. The website is built using HTML, CSS, and JavaScript.

### Classes

The website uses a class to represent a bank account. The class has properties for the balance, account holder name, and account type. The class also has methods for depositing, withdrawing, and checking the balance.

### Switch Statements

The website uses a switch statement to handle the different actions that the user can take. The switch statement checks for the value of the `action` variable, which is set when the user clicks one of the buttons. The corresponding `case` statement is then executed.

### Try-Catch-Finally Statements

The website uses try-catch-finally statements to handle exceptions. Exceptions are errors that occur during the execution of the program. The `try` block contains the code that is likely to throw an exception. The `catch` block contains the code that is executed when an exception is thrown. The `finally` block is always executed, regardless of whether an exception is thrown.

### Instructions

To use the website, follow these steps:

1. Enter your account holder name.
2. Select your account type.
3. Click the "Deposit", "Withdraw", or "Check Balance" button.
4. Follow the prompts to complete the action.

### Walkthrough

Here is a walkthrough of how the website works:

1. When the user enters their account holder name and selects their account type, the website creates a new bank account object.
2. When the user clicks the "Deposit", "Withdraw", or "Check Balance" button, the website sets the `action` variable to the corresponding value.
3. The website then calls the `performAction()` function, which uses a switch statement to handle the different actions.
4. The corresponding `case` statement is executed, which performs the desired action.
5. If an exception occurs, the `catch` block is executed.

### Conclusion

The website uses classes, switch statements, and try-catch-finally statements to implement the bank account management functionality. The classes allow the website to encapsulate the data and behavior of a bank account. The switch statements allow the website to handle the different actions that the user can take. The try-catch-finally statements allow the website to handle exceptions.


# 4
# Temperature Converter App

The Temperature Converter app simplifies temperature conversions between Celsius and Fahrenheit, harnessing JavaScript's powerful features such as classes, switch statements, and try-catch statements to enhance user interaction.

## JavaScript Concepts Applied

### Classes

We employ JavaScript classes to structure and manage temperature conversion functions. Our `TemperatureConverter` class streamlines the conversion logic, promoting code organization and reusability.

### Switch Statements

Switch statements guide the app through diverse conversion scenarios. When you choose a temperature scale (Celsius or Fahrenheit), a switch statement directs the app to the corresponding conversion method. This versatile control flow structure efficiently handles different cases.

### Try-Catch Statements

For robust error handling, we implement try-catch statements. Should you input an invalid temperature value or face a conversion error, the try-catch block captures and gracefully manages the issue. This safeguards user experience amidst unexpected inputs or errors.

## Step-by-Step Usage

### Step 1: Open the App

Access the Temperature Converter web page in your browser:


[Live Demo](https://sg75-temperature-converter-app.netlify.app/)


### Step 2: Enter Temperature Value

1. Locate the "Temperature Value" input field.
2. Input your temperature value, ensuring it's a valid number.

### Step 3: Select Conversion Scale

1. Find the "Convert to" dropdown below the temperature input.
2. Click the dropdown to reveal your scale choices:
   - **Celsius**: Converts to degrees Celsius.
   - **Fahrenheit**: Converts to degrees Fahrenheit.

### Step 4: Perform the Conversion

1. After entering the temperature and choosing the scale, spot the "Convert" button.
2. Click "Convert" to trigger the conversion.

### Step 5: View the Result

1. Upon completion, the converted temperature, along with the chosen scale, is displayed on the web page.
2. Any errors appear in red text beneath the result.

### Step 6: Start a New Conversion

For another conversion:

1. Enter a fresh temperature value.
2. Pick your desired conversion scale.
3. Click "Convert" again for the new conversion.

## Notes

- Invalid temperature entries (e.g., non-numeric characters) trigger an error message. Ensure valid numbers for accurate conversions.

- The app utilizes JavaScript's classes, switch statements, and try-catch statements for conversion and error handling.

- Employ this app effortlessly to convert temperatures between Celsius and Fahrenheit, serving diverse purposes.


# 5

# JavaScript Intermediate Campaign Bounty Submission

## Project Overview

For this bounty, I have created a website that simulates bank account management. The website utilizes classes, switch statements, and try-catch-finally statements, as required by the bounty guidelines.

## Instructions

To use the website, follow these steps:

1. Visit the website by clicking [here](https://unified-bank-stackup-bounty.netlify.app).

2. On the website, you will see two sections: **Account Information** and **Actions**.

### Account Information

- **Account Holder**: Displays the name of the account holder (initially set to "John Doe").
- **Account Type**: Shows the type of the account (initially set to "Savings").
- **Balance**: Displays the current account balance (initially set to $1000.00).

### Actions

- **Select Action**: Choose an action from the dropdown list. You can select from "Deposit," "Withdraw," or "Check Balance."

- **Amount**: Enter the amount for the selected action. Ensure that you enter a valid positive number.

- **Submit**: Click the "Submit" button to perform the selected action on the account.

## Incorporating JavaScript Concepts

Here's how I incorporated the required JavaScript concepts:

### Classes

I created a `BankAccount` class with the following properties:
- `accountHolder`: Stores the name of the account holder.
- `accountType`: Represents the type of the account.
- `balance`: Maintains the account balance (initialized to $1000.00).

### Switch Statements

I used a switch statement to handle user-selected actions. Depending on the chosen action, the switch statement executes the corresponding functionality, such as depositing, withdrawing, or checking the balance.

### Try-Catch-Finally Statements

I implemented try-catch-finally statements to handle exceptions gracefully. For instance, if a user attempts to withdraw more than the available balance or enters an invalid amount, the try-catch-finally block ensures that appropriate error messages are displayed.

## Additional Information

- I added a dark mode feature to enhance user experience. Users can toggle dark mode on and off using the "Dark Mode" switch in the header.

Thank you for considering my submission for the JavaScript Intermediate Campaign Bounty.

---
**Submission Details**

- X (formerly Twitter) Handle: @AdityaJamdade08

- Discord Handle: @aditya_jamdade08

- [GitHub Repository](https://github.com/AdityaJamdade/unified-bank-stackup-project)

- [Website](https://unified-bank-stackup-bounty.netlify.app)