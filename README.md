# Experiment-8
#Study the system specifications of an ATM system and report any identified bugs.
## Purpose: 
The purpose of this report is to study the system specifications of an Automated Teller Machine (ATM) system, identify potential issues, and report any possible bugs in its design, functionality, or operation.

## Scope:
This report covers the functional and non-functional aspects of an ATM system, including user authentication, transaction processing, cash dispensing, balance inquiry, and system interfaces. The scope includes identification of possible bugs that may affect performance, security, or user experience.

## Intended Audience:
ATM system developers and engineers

Bank IT administrators and software testers

Quality assurance teams

Security analysts

## Product Perspective:
The ATM system is a client-server based system that interacts with a bank’s central database. It provides customers with remote access to their accounts, allowing cash withdrawals, deposits, balance inquiries, and mini-statements. The system is expected to operate reliably in multiple locations and interface securely with the bank’s backend systems.


## Product functions:
User authentication via ATM card and PIN.

Cash withdrawal and deposit.

Balance inquiry and mini-statement printing.

Fund transfer between accounts.

Display of transaction history.

Secure communication with bank servers.

Error handling for failed transactions.

## Operating Environments: 
ATM machines installed in indoor and outdoor locations.

Operating system may be embedded Linux, Windows Embedded, or custom RTOS.

Connectivity via secure network (LAN, WAN, or GSM).

Peripheral devices: card reader, cash dispenser, receipt printer, keypad, and display screen.

## Design/implementation constraints:
Must comply with PCI DSS (Payment Card Industry Data Security Standard).

Limited hardware resources in ATM (memory, CPU).

Real-time processing for transaction requests.

Secure handling of PIN and user data.

Fail-safe operation in case of power/network failure.

## Assumptions and Dependencies:
ATM users have valid bank accounts and authorized ATM cards.

Reliable network connection to the central banking server.

Peripheral devices (card reader, cash dispenser) are properly maintained.

Software updates are performed periodically.

## Some of the possible Bugs on ATM machine:
Authentication Bugs:

PIN validation failure even when correct.

Multiple attempts not handled correctly.

Transaction Bugs:

Cash dispensing errors (shortage or over-dispense).

Balance not updated correctly after withdrawal/deposit.

Fund transfer showing success but not reflected in account.

Interface Bugs:

Screen freezing or incorrect messages.

Buttons or touchscreen not responding.

Hardware Interaction Bugs:

Card stuck in card reader.

Receipt printer failure or incorrect print.

Security Bugs:

Vulnerability to card skimming.

Sensitive data exposure (PIN or account info).

Unauthorized access due to software loopholes.

Network/Server Bugs:

Transaction fails due to timeout but user is charged.

Incorrect error message when network is down.

Concurrency Bugs:

Simultaneous withdrawal requests causing negative balance.

## Result
The study identified several potential bugs that could affect user experience, transaction reliability, and security of the ATM system. Careful testing, secure coding practices, and proper maintenance are required to ensure the ATM functions correctly and securely.
