
# 🏦 Bank Account Management System

A console-based **Bank Account Management System** built using Python.
This project demonstrates **Object-Oriented Programming (OOP), Exception Handling, CSV File Handling, and CRUD Operations**.

---

## 📌 Project Overview

The Bank Account Management System allows users to create and manage bank accounts through a simple command-line interface.

Users can:

* Create a bank account
* View all accounts
* Search for an account
* Deposit money
* Withdraw money
* Delete an account
* Handle invalid inputs and banking errors
* Store account data permanently in a CSV file

---

## 🚀 Features

### 1. Create Account

Create a new bank account with:

* Account ID
* Account Holder Name
* Initial Balance

### 2. View Accounts

Display all registered bank accounts with their current balances.

### 3. Search Account

Search for a specific account using its Account ID.

### 4. Deposit Money

Add money to an existing account.

### 5. Withdraw Money

Withdraw money while checking whether sufficient balance is available.

### 6. Delete Account

Remove an existing bank account from the system.

### 7. Exception Handling

The project handles errors such as:

* Invalid input
* Negative amounts
* Invalid account IDs
* Insufficient balance
* Missing accounts

---

## 🛠️ Technologies Used

* **Python 3**
* Object-Oriented Programming (OOP)
* Exception Handling
* Custom Exceptions
* CSV File Handling
* File Handling
* CRUD Operations

---

## 📂 Project Structure

```text
Day-09-Bank-Management/
│
├── bank_management.py
├── accounts.csv
└── README.md
```

---

## 🧠 OOP Concepts Used

### Class

```python
class Bank:
```

The `Bank` class contains all banking operations.

### Object

```python
bank = Bank()
```

An object of the `Bank` class is created to run the application.

### Constructor

```python
def __init__(self):
```

The constructor initializes the bank system and creates the CSV file if it doesn't exist.

### Custom Exception

```python
class InsufficientBalanceError(Exception):
    pass
```

A custom exception is used when a customer tries to withdraw more money than their available balance.

---

## ⚠️ Exception Handling

The project uses:

```python
try
except
else
finally
raise
```

Example:

```python
try:
    amount = float(input("Enter Withdrawal Amount: "))

    if amount <= 0:
        raise ValueError("Amount must be greater than zero.")

except ValueError as e:
    print("Invalid amount:", e)
```

---

## 💾 Data Storage

Account information is stored in:

```text
accounts.csv
```

Example:

```csv
Account_ID,Name,Balance
101,Rohit,5000.0
102,Amit,7500.0
103,Rahul,3000.0
```

CSV storage allows the data to remain available even after the program is closed.

---

## ▶️ How to Run

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Open the project

```bash
cd Day-09-Bank-Management
```

### Step 3: Run the program

```bash
python bank_management.py
```

---

## 🖥️ Sample Menu

```text
================================
   BANK ACCOUNT MANAGEMENT
================================
1. Create Account
2. View Accounts
3. Search Account
4. Deposit Money
5. Withdraw Money
6. Delete Account
7. Exit

Enter Choice:
```

---

## 🧪 Example

### Create Account

```text
Enter Choice: 1

Enter Account ID: 101
Enter Name: Rohit
Enter Initial Balance: 5000

✅ Account created successfully!
```

### Deposit

```text
Enter Choice: 4

Enter Account ID: 101
Enter Deposit Amount: 2000

✅ Deposit successful!
New Balance: 7000.0
```

### Withdraw

```text
Enter Choice: 5

Enter Account ID: 101
Enter Withdrawal Amount: 1500

✅ Withdrawal successful!
Remaining Balance: 5500.0
```

### Insufficient Balance

```text
Enter Choice: 5

Enter Account ID: 101
Enter Withdrawal Amount: 10000

❌ Transaction Failed: Insufficient balance.
```

---

## 📊 CRUD Operations

| Operation | Feature               |
| --------- | --------------------- |
| Create    | Create Account        |
| Read      | View / Search Account |
| Update    | Deposit / Withdraw    |
| Delete    | Delete Account        |

---

## 🔐 Error Handling

The application protects against:

* Negative account balance
* Negative deposit
* Negative withdrawal
* Invalid numeric input
* Duplicate Account IDs
* Non-existent accounts
* Insufficient balance
* Invalid menu choices

---

## 🔮 Future Improvements

Planned improvements:

* [ ] Money Transfer between accounts
* [ ] Update Account Name
* [ ] Transaction History
* [ ] Transaction Date & Time
* [ ] Total Bank Balance
* [ ] Admin Login
* [ ] User Authentication
* [ ] Password/PIN protection
* [ ] SQLite database
* [ ] GUI using Tkinter
* [ ] Monthly transaction reports

---

## 📚 What I Learned

Through this project, I practiced:

* Python OOP
* Classes and Objects
* Constructors
* Methods
* Custom Exceptions
* Exception Handling
* File Handling
* CSV module
* CRUD operations
* Input Validation
* Building a menu-driven application

---

## 👨‍💻 Author

**Rohit**

This project was created as part of my **Python & Data Science Interview Preparation – Day 9**.

---

## ⭐ If You Like This Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.
