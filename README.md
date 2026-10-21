# Banking Management System in C++

A console-based Banking Management System developed in C++ that demonstrates object-oriented programming concepts, especially **inheritance** and **polymorphism**. Users can create savings or current accounts and perform basic banking operations through a menu-driven interface.

## Project Description

The application manages bank accounts during program execution. Each account stores an account number, account holder name, account type, and balance.

### Features

- Create a **Savings Account** or **Current Account**.
- Automatically assign account numbers, starting from `1001`.
- Deposit money into an existing account.
- Withdraw money from an existing account.
- Check the balance of an account.
- Display all accounts.
- Validate positive transaction amounts and account numbers.
- Prevent withdrawals that exceed the available balance.
- Enforce a minimum initial deposit of **₹500** for savings accounts.
- Maintain a minimum balance of **₹500** in savings accounts after withdrawals.

### Object-Oriented Concepts Used

- **Inheritance:** `SavingsAccount` and `CurrentAccount` inherit from the abstract base class `BankAccount`.
- **Abstraction:** `BankAccount` declares `getAccountType()` as a pure virtual function.
- **Polymorphism:** Account operations such as `withdraw()` and `displayAccount()` use virtual functions.
- **Encapsulation:** Account data is stored in class members and accessed through class methods.
- **Smart pointers:** `unique_ptr` manages account objects stored in a vector.

## Requirements

- A C++ compiler that supports **C++14 or later** (for example, GCC or Clang).
- A terminal or command prompt.

## Execution

### 1. Save the source file

Save the source code as `banking_system.cpp`.

### 2. Compile the program

Using GCC:

```bash
g++ -std=c++14 banking_system.cpp -o banking_system
```

### 3. Run the program

**Linux / macOS:**

```bash
./banking_system
```

**Windows (Command Prompt):**

```bat
banking_system.exe
```

If you are using VS Code, open the project folder in the terminal and run the compile and run commands there.

## Sample Execution

The following is an example session. Your output will depend on the choices and values you enter.

```text
====================================
       BANKING MANAGEMENT SYSTEM
====================================
1. Create Account
2. Deposit Money
3. Withdraw Money
4. Check Balance
5. Display All Accounts
6. Exit
====================================
Enter your choice: 1
Enter Account Holder Name: Sai Pawar

Select Account Type:
1. Savings Account
2. Current Account
Enter choice: 1
Enter Initial Deposit: Rs. 1000

Account created successfully!
Your Account Number: 1001

====================================
       BANKING MANAGEMENT SYSTEM
====================================
1. Create Account
2. Deposit Money
3. Withdraw Money
4. Check Balance
5. Display All Accounts
6. Exit
====================================
Enter your choice: 2
Enter Account Number: 1001
Enter Deposit Amount: Rs. 500
Deposit successful!
Updated Balance: Rs. 1500.00

====================================
       BANKING MANAGEMENT SYSTEM
====================================
1. Create Account
2. Deposit Money
3. Withdraw Money
4. Check Balance
5. Display All Accounts
6. Exit
====================================
Enter your choice: 3
Enter Account Number: 1001
Enter Withdrawal Amount: Rs. 200
Savings account withdrawal successful!
Updated Balance: Rs. 1300.00

====================================
       BANKING MANAGEMENT SYSTEM
====================================
1. Create Account
2. Deposit Money
3. Withdraw Money
4. Check Balance
5. Display All Accounts
6. Exit
====================================
Enter your choice: 4
Enter Account Number: 1001

Current Balance: Rs. 1300.00

====================================
       BANKING MANAGEMENT SYSTEM
====================================
1. Create Account
2. Deposit Money
3. Withdraw Money
4. Check Balance
5. Display All Accounts
6. Exit
====================================
Enter your choice: 6
Thank you for using our banking system!
```

## Project Structure

```text
Banking-Management-System/
├── banking_system.cpp
└── README.md
```

## Author

**Sai Pawar**
