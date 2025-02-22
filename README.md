# Online Banking System Using Java

## Overview
This project was part of my Java coursework, where I developed an online banking system based on use cases provided by the professor.

## Features
### Account Creation
To allow customers to open checking and savings accounts, the following features were implemented:

1. **Database Structure:** Created tables:
   - `CheckingAccount (CheckingAccountNumber, CustomerName, Balance, CustomerID)`
   - `SavingsAccount (SavingsAccountNumber, CustomerName, Balance, InterestRate, CustomerID)`
   - `Transactions (TransactionNumber, TransactionAmount, TransactionType, TransactionTime, TransactionDate, FromAccount, ToAccount, CustomerID)`
   - Used `VARCHAR(50)` for non-numerical values (e.g., account numbers and transaction numbers) and `FLOAT` for numerical values. `CustomerID` corresponds to the username.

2. **Entity Class Development:**
   - Analyzed `CheckingAccount.java` and created `SavingsAccount.java` and `Transaction.java`, ensuring transaction recording capabilities.

3. **Bank Account Opening:**
   - Enhanced `OpenBankAccountControl.java` to support both checking and savings account creation while recording opening deposit transactions.

## Further Development
Beyond account creation, additional functionalities were implemented:

### Use Cases
- Developed **Account Overview, Transaction Inquiry, Deposit, and Withdraw** functionalities using real-world banking service examples.
- Created Java programs that fully support these features with database connectivity.
- **Account Overview:** Displays the current balances of a customer’s Checking and Savings accounts.
- **Transaction Inquiry:** Allows customers to search for specific transactions by specifying a date range.

### Key Methods Implemented

#### Banking Operations
1. `deposit()` and `withdraw()` methods in `CheckingAccount` and `SavingsAccount`
2. `getBalance()` and `calculateInterests()` in `SavingsAccount`
3. `searchTransaction()` in `Transactions`
4. Implemented **Transfer, Deposit, and Withdraw** functionalities, modifying the application to show these options post-login instead of the default Open Bank Account window.

#### User Interface Enhancements
- Organized functionalities into **tabs** within a single window.
- Tabs included: **Account Overview, Open Account, Deposit, Withdraw, Transfer, and Inquire Transactions**.
- After a successful login, users are directed to the main application window, which integrates the Open Account feature.

## Conclusion
This project provided hands-on experience in database management, Java programming, and UI development. The banking system efficiently handles multiple accounts, transactions, and customer interactions within a structured and user-friendly interface.

