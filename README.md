# NoobChain - Java Blockchain

My own cryptocurrency implementation built from scratch in Java.

## What I Built

A complete blockchain system that creates "NoobCoin" - featuring secure wallets, signed transactions, and mining capabilities.

## Getting Started

### Requirements

- Java 8+
- Bouncy Castle library (for cryptography)
- GSON library (for JSON)

### Quick Start

```bash
# Compile
javac -cp "lib/*:src" src/noobchain/*.java

# Run
java -cp "lib/*:src" noobchain.NoobChain
```

## Project Files

```
src/noobchain/
├── NoobChain.java    # Main blockchain
├── Block.java        # Block structure  
├── Transaction.java  # Transaction logic
├── Wallet.java       # Digital wallets
└── StringUtil.java   # Helper functions
```

## Key Features

- **Digital Wallets** - Generate secure key pairs
- **Signed Transactions** - ECDSA digital signatures
- **Mining** - Proof-of-work block creation
- **Validation** - Complete blockchain verification

## Usage Example

```java
// Create wallets
Wallet walletA = new Wallet();
Wallet walletB = new Wallet();

// Send coins
Transaction tx = walletA.sendFunds(walletB.publicKey, 25f);

// Mine block
Block block = new Block(previousHash);
block.addTransaction(tx);
block.mineBlock(difficulty);
```

## Sample Output

```
Starting NoobChain...
Wallet A balance: 100.0
Sending 40 coins...
Wallet A balance: 60.0
Wallet B balance: 40.0
✅ Blockchain valid
```

## What It Demonstrates

- Blockchain fundamentals
- Cryptographic security
- Java programming skills
- UTXO transaction model

This project shows how cryptocurrencies work under the hood, built entirely in Java with proper cryptographic security.
Made by Manish Lakkavatri
