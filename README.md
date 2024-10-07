
# Token Faucet - Sepolia Network

This repository provides a simple token faucet service for the Sepolia network. It enables users to send a specified amount of tokens to a wallet address after verifying their previous transactions. 

## Features

- **Token Transfer**: Users can request a token transfer to their wallet address.
- **Transaction Check**: The faucet verifies the user's transaction history to prevent daily abuse.
- **Easy Integration**: The service can be easily integrated into existing applications.

## Technologies Used

- **Node.js**: For the server-side implementation.
- **Express**: A web framework for building APIs.
- **Axios**: For making HTTP requests.
- **Alchemy Web3**: For interacting with the Ethereum blockchain.
- **dotenv**: For environment variable management.
- **BigNumber.js**: For precise financial calculations.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/krmrr/TOKEN-FAUCET-BACKEND.git
   ```
2. Navigate to the project directory:
   ```bash
   cd token-faucet
   ```
3. Install the dependencies:
   ```bash
   npm install
   ```
4. Create a `.env` file in the root directory and add the following variables:
   ```plaintext
   API_URL=<YOUR_ALCHEMY_API_URL>
   TOKEN_ADDRESS=<YOUR_TOKEN_CONTRACT_ADDRESS>
   FROM_ADDRESS=<YOUR_WALLET_ADDRESS>
   WALLET_PK=<YOUR_WALLET_PRIVATE_KEY>
   ETHERSCAN_API=<YOUR_ETHERSCAN_API_KEY>
   PORT=<YOUR_PORT_NUMBER>
   ```

## Usage

1. Start the server:
   ```bash
   npm start
   ```
2. Send a GET request to the faucet endpoint with the wallet address as a query parameter:
   ```plaintext
   GET /api/send?wallet=<WALLET_ADDRESS>
   ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Alchemy for providing the Web3 infrastructure.
- Etherscan for the token transaction data.

## Author

- **Ömerfaruk Karaömer** - Co-Founder of Qoalaa
