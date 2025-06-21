# ATM System Simulator

A simple command-line ATM (Automated Teller Machine) simulator built in Python that provides basic banking operations with user authentication.

## Features

- User Authentication with username and PIN verification
- Account lockout after 3 failed PIN attempts
- Check account balance (Statement)
- Withdraw money
- Deposit money (Lodgement)
- Change PIN
- Transaction validation (amounts must be multiples of 10)

## Prerequisites

- Python 3.x
- No external dependencies required

## Installation

1. Clone this repository
2. Run the program:
```bash
python atm_system.py
```

## Default Test Accounts

| Username | PIN  | Initial Balance |
|----------|------|-----------------|
| user     | 1234 | €1000          |
| user2    | 2222 | €2000          |
| user3    | 3333 | €3000          |

## Available Operations

- **S** - Statement: View current account balance
- **W** - Withdraw: Remove money from account
- **L** - Lodgement: Deposit money into account
- **P** - Change PIN: Update your account PIN
- **Q** - Quit: Exit the system

## Security Features

- Hidden PIN input using `getpass` module
- Account lockout after 3 unsuccessful attempts
- 4-digit PIN validation
- Transaction limits (multiples of 10 Euro)

## Limitations

- Account data is not saved between sessions
- User accounts are hardcoded
- Basic error handling

## License

This project is open source and available under the MIT License.
