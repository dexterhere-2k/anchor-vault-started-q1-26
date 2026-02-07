# Anchor Vault Program

A simple Solana smart contract built with **Anchor**. This program implements a basic vault mechanism allowing users to securely manage SOL deposits and withdrawals using Program Derived Addresses (PDAs).

## Features

* **Initialize:** Create a vault PDA with a state account to store canonical bumps.
* **Deposit:** Transfer SOL from a user's wallet into the secure vault.
* **Withdraw:** Withdraw specific amounts of SOL from the vault back to the user (signed by the vault's PDA).
* **Close:** Close the vault account, transferring all remaining SOL back to the initializer and closing the state account.

## Prerequisites

Ensure you have the following tools installed before running the project:

* **Anchor CLI** (v0.32.1 or later) - Installed via AVM.
* **Solana CLI** - For interacting with the Solana cluster.
* **Node.js & Yarn** - For running integration tests.


## Running Tests

You can run tests using  the standard Anchor local validator.



### Standard Anchor
You can run the full test suite with a single command:

```bash
anchor test
