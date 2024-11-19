 ATM Machine Simulation:


---

Overview

The code simulates the basic functionalities of an ATM machine using object-oriented programming in Python. It provides functionalities like:

1. Balance inquiry


2. Cash deposit


3. Cash withdrawal


4. PIN change


5. Transaction history




---

Components of the Code

1. ATM Class

This is the core of the program where all ATM functionalities are implemented.

__init__(self, pin, balance=0)

Initializes an ATM account with a PIN (pin) and an optional balance (default is $0).

Maintains a transaction history as a list (self.transaction_history).

Example:

atm = ATM(pin=1234, balance=1000)

Creates an account with a balance of $1000 and a PIN 1234.


authenticate(self, entered_pin)

Validates the user's input PIN against the stored PIN.

Returns True if the PIN matches, otherwise False.


check_balance(self)

Returns the current account balance.

Example:

atm.check_balance()  # Output: 1000


deposit(self, amount)

Adds the specified amount to the account balance.

Updates the transaction history with a log like "Deposited: $amount".

Returns success or error messages based on the input.

Example:

atm.deposit(500)  # Deposits $500


withdraw(self, amount)

Deducts the specified amount from the balance if sufficient funds are available.

Updates the transaction history with a log like "Withdrew: $amount".

Returns success or error messages based on conditions.

Example:

atm.withdraw(300)  # Withdraws $300


**`


