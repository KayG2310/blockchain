# Basic Simulation of a Blockchain System

## Overview
This project simulates a **basic blockchain network** for a fixed **four-user** peer-to-peer (P2P) system. It is implemented in **C++** and compiled using the **GNU compiler**. The blockchain uses the **SHA-512** hashing function for encryption and maintains security through a consensus mechanism.

## Features
- **Transaction Management**: Users can securely add transactions to the blockchain.
- **Decentralized Ledger**: Each user maintains a local copy of the blockchain.
- **Security Mechanism**: Valid transactions require majority approval.
- **Tamper Detection**: A hacker simulation feature checks the blockchain’s resistance to tampering.

## Installation & Compilation
To compile the code, use the following command:
```sh
g++ blockchain_simulation.cpp -o blockchain_simulation -lcrypto
```
To run the program
```sh
./blockchain_simulation
```
