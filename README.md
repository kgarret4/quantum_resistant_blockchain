# Quantum-Resistant Blockchain Module

## Overview
The **Quantum-Resistant Blockchain Module** is a Rust-based blockchain framework designed to be resistant to quantum computing threats. It integrates **post-quantum cryptography (PQC)** to secure transactions and smart contracts.

## Features
-  **Quantum-resistant cryptographic signatures** using **NTRU** and **Falcon**.
-  **Blockchain ledger with secure transaction validation**.
-  **Integration with Solana SDK for execution**.
-  **Smart contract execution with PQ-safe keys**.
-  **Efficient storage and transaction verification**.

## Installation
1. **Clone the repository**:
   git clone https://github.com/kgarret4/quantum_resistant_blockchain.git
   cd quantum_resistant_blockchain

## Usage
The module allows users to create quantum-safe transactions and store them securely on a blockchain ledger.

Example:

let (public_key, private_key) = keypair();
let transaction = QuantumTransaction::new("Alice".to_string(), "Bob".to_string(), 100, &private_key);
let mut blockchain = QuantumBlockchain::new();
blockchain.add_transaction(transaction.clone());
assert!(blockchain.verify_transaction(&transaction, &public_key));

## Contributors
Co-authored by:

 Orly (orlychikka@gmail.com)
 Shaul (shaulong717@gmail.com)
 Harry (zharry420@gmail.com)
 Hanson (hansonp303@gmail.com)
