# Bank-Management-System
Bank management system designed using Python and SQL

## Introduction
The Bank Management System (BMS) is a comprehensive program designed to manage and track clients' bank accounts. This project automates various banking operations, providing a seamless experience for both bank employees and customers. The system allows for the creation and management of accounts, transactions, and loan requests, among other functionalities.

## Features
- User Authentication: Login and registration system.
- Account Management: Create, update, and delete bank accounts.
- Transactions: Perform deposits and withdrawals.
- Customer Details: View detailed account information.
- Transaction History: View transaction details for any account.
- Loan Management: Request and manage loans.
- Low Balance Alerts: Automated alerts for low account balances using triggers.

## Objectives
1. Creating and managing bank accounts.
2. Handling transactions effectively.
3. Storing and managing bank details.
4. Providing detailed transaction history.
5. Facilitating loan requests and management.
6. Deleting accounts securely.

## Design
### Data Dictionary
- **User_detail**: Stores user login information.
- **Customer_detail**: Stores customer account details.
- **Transaction_detail_credit**: Records credit transactions.
- **Transaction_detail_debit**: Records debit transactions.
- **Low_bala_account**: Tracks accounts with low balances.
- **Loan**: Manages loan details.

### ER Diagram
The system uses entity-relationship diagrams to map out the relationships between different entities like customers, transactions, and loans.

### Flow Chart
A detailed flow chart illustrates the system's workflow from registration/login to various banking operations.

## Stored Procedures and Triggers
- **Stored Procedures**: Implemented for error handling, crediting, and debiting amounts.
- **Triggers**: Automated alerts for specific conditions such as low balance and high withdrawal amounts.

## Installation
To run the Bank Management System locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bank-management-system.git
   ```
2. Navigate to the project directory:
   ```bash
   cd bank-management-system
   ```
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up the MySQL database and import the bank1 database schema.
5. Update the database connection details in main.py:
   ```python
   sql_data = sqltor.connect(host='localhost', user='root', password='123456', database='bank1')
   ```
6. Run the application:
   ```bash
   python3 main.py
   ```

## Usage
Login/Register: Start the application and choose to log in if you already have an account or register to create a new one.
Main Menu: After logging in, you will see options to create an account, perform transactions, view details, request loans, and more.
Transactions: Choose to deposit or withdraw money from your account.
Account Management: View account details, transaction history, and delete accounts if necessary.
Output
The system provides various outputs such as successful login messages, account details, transaction histories, and more. Each action performed is followed by a confirmation message to ensure successful operation.

## Conclusion
The Bank Management System aims to virtualize traditional banking processes, making them more efficient and user-friendly. The system's automated features improve transaction time and overall system efficiency.

## Future Developments
Implementation of OTP (One-Time Password) for enhanced security.
Transaction alert SMS notifications.
Additional constraint checks on user inputs.
Authors
Rahul Markasserithodi
Sahil Sharma
Gopit Singhal
Anish Saha

