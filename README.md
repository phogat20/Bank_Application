# Bank Backend Application

–	The bank application provides users with features such as account creation, transaction history, loans, and balance.
–	Build this application on monolithic architecture.
–	The bank application uses hashing for sensitive data like passwords and session management to ensure security. Roles-based authorization is also added.
–	Implemented CSRF Cookie Filter and BCrypt Password encoder is used for password hashing and storage.

## Tools & Technologies used:  
- Spring Boot
- Spring JPA
- Spring Security
- MySQL
- Maven
- Postman

This is a backend application for a bank, developed using Spring Boot. It provides various features such as transactions, withdrawals, deposits, and loans. 
The application also incorporates complete security using Spring Security.

## Features

- Transactions: Users can initiate transactions, view transaction details, and update existing transactions.
- Withdrawals: Users can withdraw from their accounts and view their withdrawal history.
- Deposits: Users can make deposits to their accounts and view their deposit history.
- Loans: Users can apply for loans, view loan details, and make loan repayments.

## Security

The application ensures complete security using Spring Security. The following security measures have been implemented:

- Authentication: Users are required to authenticate themselves before accessing any functionality.
- Authorization: Different user roles (such as admin, employee, and customer) have different levels of access to the application's features.
- Password Encryption: User passwords are securely encrypted using password encoders to protect sensitive information.
- CSRF Protection: Cross-Site Request Forgery (CSRF) protection is in place to prevent unauthorized requests.
- Session Management: Sessions are managed securely to prevent session-related attacks.

## Prerequisites

Before running the application, make sure you have the following prerequisites:

- Java Development Kit (JDK) installed (version 8 or above)
- Apache Maven installed
- MySQL or any other supported database management system installed

## Project Structure

```
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── your company
│   │   │           ├── config
│   │   │           │   ├── SecurityConfig.java
│   │   │           │   └── WebConfig.java
│   │   │           ├── controller
│   │   │           │   ├── TransactionController.java
│   │   │           │   ├── WithdrawalController.java
│   │   │           │   ├── DepositController.java
│   │   │           │   └── LoanController.java
│   │   │           ├── model
│   │   │           │   ├── Transaction.java
│   │   │           │   ├── Withdrawal.java
│   │   │           │   ├── Deposit.java
│   │   │           │   └── Loan.java
│   │   │           ├── repository
│   │   │           │   ├── TransactionRepository.java
│   │   │           │   ├── WithdrawalRepository.java
│   │   │           │   ├── DepositRepository.java
│   │   │           │   └── LoanRepository.java
│   │   │           ├── service
│   │   │           │   ├── TransactionService.java
│   │   │           │   ├── WithdrawalService.java
│   │   │           │   ├── DepositService.java
│   │   │           │   └── LoanService.java
│   │   │           ├── BankApplication.java
│   │   │           └── SecurityInitializer.java
│   │   └── resources
│   │       ├── application.properties
│   │       └── data.sql
│   └── test
│       └── java
│           └── com
│               └── your company
│                   └── controller
│                       ├── TransactionControllerTest.java
│                       ├── WithdrawalControllerTest.java
│                       ├── DepositControllerTest.java
│                       └── LoanControllerTest.java
├── .gitignore
├── pom.xml
└── README.md







