**NAME:** MONISHA B

**COMPANY:** CODTECH IT SOLUTIONS

**OFFER LETTER ID:** CT08DS7229

**DOMAIN:** "JAVA PROGRAMMING"

**DURATION:** SEPTEMBER to OCTOBER 2024



Description of Task-2:

**Overview**:

This Java program simulates a basic online banking system. It allows users to:
Create Accounts

i)Deposit and Withdraw Funds

ii)Transfer Money Between Accounts

iii)View Transaction History

iv)Manage Personal Information

The program operates via a command-line interface and uses in-memory data storage to manage accounts and transactions.

**Program Components**:
1. Account Class

Attributes:

**accountNumber:** Unique identifier for the account.

**accountHolder:** Name of the account holder.

**balance:** Current balance of the account.

**transactionHistory:** List of transaction records.

2. Methods:

**Constructor (Account(String accountNumber, String accountHolder)):** Initializes a new account with a given account number and account holder name. Sets the initial balance to 0.0 and logs this in the transaction history.

**deposit(double amount):** Deposits a specified amount into the account. The amount must be positive. Updates the balance and records the transaction.

**withdraw(double amount):** Withdraws a specified amount from the account if sufficient funds are available. The amount must be positive and less than or equal to the balance. Updates the balance and records the transaction.

**transfer(Account target, double amount):** Transfers a specified amount from the current account to a target account. The amount must be positive and less than or equal to the balance. Updates the balance of both accounts and records the transactions in both account histories.

**printTransactionHistory():** Prints all transactions related to this account.

**updateAccountHolder(String newHolder):** Updates the account holder’s name and logs this change in the transaction history.

2. BankingSystem Class

Attributes:

**accounts:** A HashMap storing Account objects with their account numbers as keys.

**scanner:** A Scanner object for reading user input.

Methods:

**createAccount():** Prompts the user to enter an account number and account holder name. Creates a new account if the account number does not already exist.

**depositFunds():** Prompts the user to enter an account number and an amount to deposit. Deposits the amount into the specified account if the account exists.

**withdrawFunds():** Prompts the user to enter an account number and an amount to withdraw. Withdraws the amount from the specified account if sufficient funds are available.

**transferMoney():** Prompts the user to enter source and target account numbers and an amount to transfer. Transfers the amount from the source account to the target account if both accounts exist and there are sufficient funds in the source account.

**viewTransactionHistory():** Prompts the user to enter an account number and displays the transaction history for that account.

**managePersonalInformation():** Prompts the user to enter an account number and a new account holder name. Updates the account holder's name for the specified account if it exists.

How It Works
**Account Management:** Users can create new accounts with unique numbers and names. Each account starts with a zero balance and records all transactions.

**Fund Management:** Users can deposit and withdraw funds from their accounts. Deposits increase the balance, while withdrawals decrease it, provided there are sufficient funds.

**Money Transfer**: Users can transfer money between accounts. The system updates the balance for both the source and target accounts and records these transactions.

**Transaction History:** Users can view the history of all transactions for a specific account, including deposits, withdrawals, and transfers.

**Personal Information:** Users can update the account holder’s name, which is recorded in the transaction history.
