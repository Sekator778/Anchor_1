# Escrow Program

This project implements an Escrow program using the Anchor framework for the Solana blockchain. The program allows users to create and accept token exchange offers in a secure manner.

## Prerequisites

- Rust
- Solana CLI
- Anchor CLI
- Node.js and npm

## Project Structure

- `programs/escrow/src/lib.rs`: Main program file.
- `programs/escrow/src/constants.rs`: File for storing constants.
- `programs/escrow/src/state/mod.rs`: Module for connecting state definitions.
- `programs/escrow/src/state/offer.rs`: State definition for the offer.
- `programs/escrow/src/instructions/mod.rs`: Module for connecting instructions.
- `programs/escrow/src/instructions/make_offer.rs`: Instruction for creating an offer.
- `programs/escrow/src/instructions/take_offer.rs`: Instruction for accepting an offer.
- `tests/escrow.ts`: Tests for the Escrow program.

## Setup

1. Initialize a new Anchor project:
    ```sh
    anchor init escrow --template=multiple
    ```

2. Navigate to the project directory:
    ```sh
    cd escrow
    ```

3. Install dependencies:
    ```sh
    npm install @solana/spl-token
    npm install @solana-developers/helpers
    ```

4. Build the project:
    ```sh
    anchor build
    ```

## Instructions

### Create an Offer

Defines the structure and logic for creating a token exchange offer.

- **File**: `programs/escrow/src/instructions/make_offer.rs`
- **Function**: `make_offer`

### Take an Offer

Defines the structure and logic for accepting a token exchange offer.

- **File**: `programs/escrow/src/instructions/take_offer.rs`
- **Function**: `take_offer`

## Running Tests

Run the tests to ensure the program works as expected:

```sh
anchor test
