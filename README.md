# 💳 ATM System in C (Linked List + CSV-Based)

This project is a simple C-based ATM (Automated Teller Machine) system **entirely implemented using singly linked lists** for dynamic in-memory management of users and transactions. It simulates user login, account access, and basic banking operations like deposit, withdrawal, and balance inquiry.

All persistent data — such as user credentials and account balances — are stored in **CSV (Comma-Separated Values) files**, making the system lightweight, portable, and human-readable. The program also applies **password encryption** to enhance security during user authentication.

---

## 🚀 Features

- 🔐 **User Authentication**  
  Users must enter a valid username and password to log in. Passwords are encrypted and stored securely in a CSV file.

- 📂 **Data Storage Using CSV**  
  - `users.csv`: Stores usernames and encrypted passwords  
  - `transactions.csv`: Maintains balances and transaction history

- 🧮 **Core Banking Operations**
  - Balance Inquiry
  - Deposit
  - Withdraw

- ❌ **Error Handling**
  - Invalid login attempts trigger an error message: `"Wrong information"`

---

## 🔁 Data Structure

- 🧷 **Linked Lists**
  
  The system is completely implemented using **singly linked lists** to manage all user accounts and transactions in memory. This enables:
  - Dynamic allocation of user and transaction nodes
  - Easy data traversal and updates
  - Better structure and separation from persistent storage (CSV files)

---

##🔐 Password Encryption

Passwords are encrypted before being saved to users.csv. You can see the original (plain) passwords in passwordsBeforeEnc.txt — this file is for testing purposes only and should be removed or excluded in production.

---

## 🧱 Project Structure
```
ATM_program/
├── main.c # Main function, menu logic
├── user.c / user.h # Handles login, password encryption, user validation
├── transaction.c / .h # Deposit, withdraw, balance check
├── util.c / util.h # Utility functions (e.g., password hashing)
├── users.csv # User data with encrypted passwords
├── transactions.csv # Account balances and transaction history
├── passwordsBeforeEnc.txt# (Optional) Plain passwords (for setup/testing)
```

