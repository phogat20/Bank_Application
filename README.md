# Bank Backend Application

–	The bank application provides users with features such as account creation, transaction history, loans, and balance.
–	Build application on monolithic architecture.
–	To ensure security, the bank application uses hashing for sensitive data like passwords and session management. Roles-based authorization is also added.
–	Implemented CSRF Cookie Filter and BCrypt Password encoder is used for password hashing and storage.

Tools & Technologies used:  Spring Boot, Spring JPA, Spring Security, MySQL, Maven, Postman.


This is a backend application for a bank, developed using Spring Boot. It provides various features such as transactions, withdrawals, deposits, and loans. 
The application also incorporates full security using Spring Security.

## Features

- **Transactions**: Users can initiate transactions, view transaction details, and update existing transactions.
- **Withdrawals**: Users can make withdrawals from their accounts and view their withdrawal history.
- **Deposits**: Users can make deposits to their accounts and view their deposit history.
- **Loans**: Users can apply for loans, view loan details, and make loan repayments.

## Security

The application ensures full security using Spring Security. The following security measures have been implemented:

- **Authentication**: Users are required to authenticate themselves before accessing any functionality.
- **Authorization**: Different user roles (such as admin, employee, and customer) have different levels of access to the application's features.
- **Password Encryption**: User passwords are securely encrypted using password encoders to protect sensitive information.
- **CSRF Protection**: Cross-Site Request Forgery (CSRF) protection is in place to prevent unauthorized requests.
- **Session Management**: Sessions are managed securely to prevent session-related attacks.

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
│   │   │       └── yourcompany
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
│               └── yourcompany
│                   └── controller
│                       ├── TransactionControllerTest.java
│                       ├── WithdrawalControllerTest.java
│                       ├── DepositControllerTest.java
│                       └── LoanControllerTest.java
├── .gitignore
├── pom.xml
└── README.md
```



## Project Components

1. **`SecurityConfig.java`**: This class is responsible for configuring Spring Security. It includes settings for authentication and authorization, such as user roles and password encoders.

2. **`WebConfig.java`**: This class is used to configure additional settings for the Spring Web application, such as enabling CORS and setting up view resolvers.

3. **`TransactionController.java`**: This controller handles requests related to transactions, such as retrieving transaction details, creating new transactions, and updating existing transactions.

4. **`WithdrawalController.java`**: This controller handles requests related to withdrawals, such as initiating a withdrawal and retrieving withdrawal history.

5. **`DepositController.java`**: This controller handles requests related to deposits, such as initiating a deposit and retrieving deposit history.

6. **`LoanController.java`**: This controller handles requests related to loans, such as applying for a loan, retrieving loan details, and making loan repayments.

7. **`Transaction.java`**: This class represents a transaction entity, with attributes such as transaction ID, amount, date, and associated account details.

8. **`Withdrawal.java`**: This class represents a withdrawal entity, with attributes such as withdrawal ID, amount

, date, and associated account details.

9. **`Deposit.java`**: This class represents a deposit entity, with attributes such as deposit ID, amount, date, and associated account details.

10. **`Loan.java`**: This class represents a loan entity, with attributes such as loan ID, amount, interest rate, duration, and associated account details.

11. **`TransactionRepository.java`**: This interface provides methods to interact with the transaction data in the database.

12. **`WithdrawalRepository.java`**: This interface provides methods to interact with the withdrawal data in the database.

13. **`DepositRepository.java`**: This interface provides methods to interact with the deposit data in the database.

14. **`LoanRepository.java`**: This interface provides methods to interact with the loan data in the database.

15. **`TransactionService.java`**: This service class contains the business logic for handling transactions.

16. **`WithdrawalService.java`**: This service class contains the business logic for handling withdrawals.

17. **`DepositService.java`**: This service class contains the business logic for handling deposits.

18. **`LoanService.java`**: This service class contains the business logic for handling loans.

19. **`BankApplication.java`**: This is the main class that serves as the entry point for the Spring Boot application.

20. **`SecurityInitializer.java`**: This class initializes the Spring Security filter chain.

21. **`application.properties`**: This file contains the application-level configuration properties, such as database connection settings.

22. **`data.sql`**: This file contains SQL statements to initialize the database with some sample data.

23. **`TransactionControllerTest.java`**: This is a test class that contains unit tests for the `TransactionController` class.

24. **`WithdrawalControllerTest.java`**: This is a test class that contains unit tests for the `WithdrawalController` class.

25. **`DepositControllerTest.java`**: This is a test class that contains unit tests for the `DepositController` class.

26. **`LoanControllerTest.java`**: This is a test class that contains unit tests for the `LoanController` class.

27. **`.gitignore**`: This file specifies which files and directories should be ignored by Git.

28. **`pom.xml`**: This is the Maven configuration file that defines the project dependencies.

29. **`README.md`**: This is the file where you can provide documentation and instructions for running the application.



