# Experiment-3
## ATM System Overview:
An ATM (Automated Teller Machine) is used by bank customers to perform a range of financial transactions without needing to visit a bank branch. Common tasks include checking balances, withdrawing cash, and transferring money between accounts. The ATM is typically connected to the bank's central system that holds customer data, account balances, and transaction histories.

## System Specifications:
The ATM system should have the following specifications:
•	User Interface:
o	Pin entry screen for user authentication.
o	Options for account types (e.g., checking, savings).
o	Transaction options (withdraw, deposit, check balance, transfer).
o	Transaction status updates (success or failure messages).
o	Printing option for receipts.
•	Security:
o	User authentication via PIN number.
o	Encryption for PINs and transaction data.
o	Lockout after several failed attempts.
o	Logging of all transactions for audit purposes.
•	Database:
o	Stores user data: account numbers, balances, transaction history.
o	Updates balances after each transaction.
o	Handles request for new PIN, account creation, etc.
•	Transaction Types:
o	Balance Inquiry: Shows the available balance.
o	Cash Withdrawal: Allows the user to withdraw a specified amount.
o	Transfer: Moves funds between accounts.
o	Deposit: Accepts money (cash or checks) and updates the account balance.
•	Error Handling:
o	Insufficient funds for withdrawal.
o	ATM running out of cash.
o	Connection issues to the bank’s central server.
o	Invalid account number or PIN.

## Aim
•	Ease of Access: Provide users with 24/7 access to banking services.
•	User-friendly interface: The system should be simple and intuitive to use.
•	Security: Ensure secure transactions using encryption and PIN validation.
•	Efficient Transactions: Complete transactions quickly, minimizing user wait time.
•	Reliability: Ensure the ATM works without frequent downtime.
•	Compliance: The system should comply with banking regulations for security and transaction logging.

## Bugs in ATM System:
Bugs may occur in various parts of the ATM system. Here are a few examples:
1.	Authentication Issues:
o	Bug: Incorrect PIN validation (e.g., allowing incorrect PIN after multiple failed attempts).
o	Impact: Unauthorized access to the user's account.
2.	Transaction Failures:
o	Bug: Withdrawal amount greater than available balance not flagged correctly.
o	Impact: The user may attempt to withdraw more money than available.
3.	Network Failure Handling:
o	Bug: In case of network failure, the ATM does not notify the user properly and might hang.
o	Impact: User confusion and incomplete transactions.
4.	Cash Dispensing:
o	Bug: ATM dispensing a lower amount of money than requested.
o	Impact: Financial loss to the customer, user dissatisfaction.
5.	Receipt Generation:
o	Bug: Receipt does not print after a successful transaction or prints the wrong details.
o	Impact: Lack of proof of transaction, inconvenience to users.
6.	Database Update:
o	Bug: Transaction history not correctly updated after a transfer.
o	Impact: Incorrect balance information provided.
7.	Multi-Threading Issues:
o	Bug: Multiple transactions happening concurrently (like withdrawal and transfer at the same time) causing race conditions.
o	Impact: Data corruption and incorrect transaction outcomes.

## Algorithm for ATM System:
Here is a simplified algorithm for a user to perform a withdrawal:
1.	Start.
2.	Display "Enter your ATM PIN".
3.	User inputs PIN.
4.	If PIN is correct, proceed, otherwise show "Invalid PIN" and allow up to 3 attempts before locking the account.
5.	Display Main Menu (Balance Inquiry, Withdrawal, Deposit, Transfer).
6.	User selects Withdraw option.
7.	Display "Enter amount to withdraw".
8.	If Amount > Account Balance, show "Insufficient funds".
9.	Otherwise, proceed with withdrawal:
o	Deduct amount from account balance.
o	Check if the ATM has sufficient cash.
o	Dispense money.
o	Print receipt (optional).
10.	Show "Transaction Successful" and display the remaining balance.
11.	End session after user confirms.

## Program

## Output

## Result
