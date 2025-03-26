# Blockchain Simulation  

## Overview  
This project simulates a **peer-to-peer blockchain network** with four users, demonstrating how transactions are validated, added to the blockchain, and secured against unauthorized modifications. The blockchain is implemented in **C++**, using **linked lists** to connect blocks and **Merkle trees** to compute hash values. The project also simulates hacker attempts to modify transactions, showcasing how blockchain security mechanisms prevent tampering.  

## Features  
- **Decentralized Ledger**: Each user maintains a local copy of the blockchain.  
- **Transaction Validation**: Transactions require a majority consensus to be added.  
- **Tamper Detection**: Unauthorized changes trigger a verification process.  
- **Blockchain Structure**: Blocks store transaction data, previous hashes, and Merkle tree-based integrity checks.  

## How It Works  
1. **User Setup**: Four usernames are entered at the start to create a P2P network.  
2. **Menu Options**:  
   - **Add a Transaction**: Enter sender, receiver, and amount; approval is required from a majority of users.  
   - **Display a Local Copy**: View the blockchain state for any user.  
   - **Simulate an Attack**: Modify a local blockchain copy and test its resistance to tampering.  
3. **Security Check**: Any unauthorized changes are detected by comparing blockchain copies across the network.  

## Implementation Details  
- **Linked List**: Used for maintaining an ordered chain of blocks.  
- **Merkle Tree**: Ensures data integrity by hashing transactions hierarchically.  
- **Consensus Algorithm**: Transactions are only added if a majority approves them.  
- **Hashing**: SHA-512 is used for cryptographic security.  

## Compilation & Execution  
To compile the project:  
```sh
g++ blockchain_simulation.cpp -o blockchain_simulation
```
