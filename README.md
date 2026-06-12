Chat Application

A Java application with user registration, login, and messaging functionality.

Part 1: Registration & Login
- Username validation (underscore, max of 5 characters)
- Password validation (8+ characters, capital, number, special characters)
- South African cellphone validation (+27 format)
- Login with retry capability

Part 2: QuickChat Messaging
- Send messages after successful login
- Message ID generation (10-digit random)
- Message Hash creation (XX:X:WORDWORD format)
- Recipient cell validation (international code)
- Message length validation (max 250 characters)
- Send / Store / Disregard options
- JSON file storage for messages

Part 3: Store Data and Display Task Report

- Five dynamic arrays for message management:
  - Sent Messages
  - Stored Messages
  - Disregarded Messages
  - Message Hashes
  - Message IDs
- Stored Messages submenu with six functions:
  - Display sender and recipient of all stored messages
  - Display the longest stored message
  - Search for a message by ID
  - Search all messages by recipient
  - Delete a message using its hash
  - Display full report (hash, recipient, message)
- Read stored messages from JSON file into arrays
- Populate test data with no hard-coding

Files
- `Login.java` - User authentication
- `Message.java` - Message handling
- `Main.java` - Application entry point
- `LoginTest.java` - Part 1 unit tests
- `MessageTest.java` - Part 2 unit tests

How to Compile and Run

Compile:
```bash
javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar *.java
