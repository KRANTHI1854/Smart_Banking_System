# Smart_Banking_System 🏦

A **Java-based console application** designed to simulate basic banking operations. This application allows users to create accounts, log in to their accounts, and perform transactions like deposits, withdrawals, and balance inquiries. The program is structured with a clear focus on modularity, validation, and user-friendly interaction.

---

## Features 🚀

1. **Account Creation**:
   - Users can create a **Savings Account** or a **Fixed Deposit Account**.
   - Input validation for names, mobile numbers, and initial deposit amounts.
   - Automated generation of unique 10-digit account numbers.

2. **Account Login**:
   - Users can log in to their accounts using their unique account numbers.
   - Personalized menus for different account types.

3. **Savings Account Operations**:
   - **Check Balance**: View the current account balance.
   - **Deposit Amount**: Add funds to the account.
   - **Withdraw Amount**: Withdraw funds with validation for sufficient balance.
   - **View Statement**: Display account details like name, balance, and account number.

4. **Fixed Deposit (FD) Account Operations**:
   - **Check Balance**: View the current balance.
   - **View Statement**: Display account details.
   - No withdrawal functionality (fixed deposit constraint).

5. **Data Validation**:
   - Names must contain only letters and spaces.
   - Mobile numbers must be exactly 10 digits.
   - Minimum deposit amount is ₹500.

6. **Error Handling**:
   - Custom exceptions for insufficient balance and invalid account numbers.
   - Input mismatch handling to prevent crashes.

---

## Technologies Used 🛠️

- **Java**: Core programming language.
- **Collections Framework**: Utilized `HashMap` to store accounts.
- **Regular Expressions**: For validating names and mobile numbers.
- **Custom Exceptions**: To enhance user experience by handling specific error scenarios.

---


---

## How It Works 💡

1. **Welcome Screen**:
   - Displays the main menu with options to create an account, log in, or exit.

2. **Account Creation**:
   - Users provide their name, mobile number, and initial deposit amount.
   - System validates inputs and generates a unique account number.
   - Account is created and stored in a `HashMap`.

3. **Login and Operations**:
   - Users log in by entering their account number.
   - Depending on the account type, a specific menu is displayed.
   - Users can perform operations such as checking balance, depositing, or withdrawing money.

4. **Exit**:
   - Users can exit the application at any time.

---

## Code Structure 🧩

### Classes and Their Responsibilities:

1. **`SmartBankApp`**:
   - Main class to initialize and run the application.

2. **`Bank`**:
   - Manages core banking operations such as account creation, login, and transaction menus.

3. **Abstract Class `Account`**:
   - Common attributes and methods for both Savings and FD accounts.
   - Includes functionalities like deposit, withdraw, and view statement.

4. **`SavingsAccount`**:
   - Subclass of `Account` with a menu for balance inquiries, deposits, withdrawals, and statements.

5. **`FDAccount`**:
   - Subclass of `Account` with a limited menu for balance and statements only.

6. **Custom Exceptions**:
   - `InsufficientBalanceException`: Thrown when withdrawal exceeds the balance.
   - `InvalidAccountException`: Thrown when the account number is not found.

---





