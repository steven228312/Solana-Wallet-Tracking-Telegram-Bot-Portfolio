# Solana-Wallet-Tracking-Telegram-Bot-Portfolio

A professional Solana wallet monitoring system that tracks transactions and delivers real-time notifications via Telegram.

<p align="center">
  <img src="https://github.com/stevendev0822/Solana-Wallet-Tracking-Telegram-Bot-Portfolio/blob/main/public/telegram-bot.PNG" alt="Main Menu">
</p>

## Overview

This application monitors Solana wallet activities in real-time, analyzes transactions, and sends detailed notifications through Telegram. It's designed for traders, investors, and developers who need immediate insights into wallet transactions.

## Key Features

- <b>Real-time Transaction Monitoring:</b> Track wallet activities as they happen
- <b>Detailed Transaction Analysis:</b> Identify buy/sell operations, token transfers, and amounts
- <b>Instant Telegram Notifications:</b> Receive formatted alerts with transaction details
- <b>Transaction History:</b> Store and query historical transaction data
- <b>Token Information:</b> Get detailed token data including amounts and addresses

## System Architecture

The system is built on three core components:

- <b>Helius RPC:</b> Provides reliable Solana blockchain data access
- <b>MongoDB:</b> Stores transaction history for analysis and reference
- <b>Telegram Bot API:</b> Delivers real-time notifications

## Installation

```bash
# Clone the repository
git clone https://github.com/stevendev0822/Solana-Wallet-Tracking-Telegram-Bot.git

# Navigate to the project directory
cd Solana-Wallet-Tracking-Telegram-Bot

# Install dependencies
npm install

```

## Configuration

Create a `.env` file in the root directory with the following variables:

```bash
# Solana RPC Configuration
RPC_URL=https://mainnet.helius-rpc.com/?api-key=YOUR_API_KEY
WSS_URL=wss://mainnet.helius-rpc.com/?api-key=YOUR_API_KEY

# Wallet Configuration
WALLET_ADDRESS=YOUR_WALLET_ADDRESS

# MongoDB Configuration
MONGODB_URI=mongodb://localhost:27017/solana_wallet_tracking

# Telegram Configuration
TELEGRAM_BOT_TOKEN=YOUR_BOT_TOKEN
TELEGRAM_CHAT_ID_CLIENT=YOUR_CLIENT_CHAT_ID
TELEGRAM_CHAT_ID_MINE=YOUR_PERSONAL_CHAT_ID
```


## Usage

```
# Start the application
npm start
```

## Setting Up Your Telegram Bot

1. Open Telegram and search for the @BotFather
2. Send `/newbot` command
3. Name your bot (e.g., "SolanaWalletTracker")
4. Save your bot token
5. Add your bot to your channel or start a direct conversation
6. Send a message to the bot
7. Access: `https://api.telegram.org/bot<YOUR_TOKEN>/getUpdates`
8. Extract the `chat_id` from the response

## Sample Notification

```bash
🔔 New Transaction Detected!

👛 Wallet: AbC1...XyZ9

💰 Sol Amount: 📤 BUY 1.234 SOL

💸 PNL for this Token: 0.123 SOL

🚀 Token: TokenName

🔗 View Transaction

⏰ 2025-04-01 12:34:56
```

## Technical Implementation

The system:

- Establishes WebSocket connections to Solana via Helius
- Listens for transaction logs in real-time
- Parses transaction data to extract relevant information
- Analyzes token transfers and SOL movements
- Formats and sends notifications via Telegram
- Stores transaction data in MongoDB for historical reference

## Development

```bash
# Run in development mode
npm run dev

# Build the project
npm run build

# Run tests
npm test
```

## License
This project is licensed under the [MIT License](./LICENSE).

## Contact Information

- Gmail: [stevenpiao0822@gmail.com](mailto:stevenpiao0822@gmail.com)
- GitHub: [Steven Leal](https://github.com/stevendev0822)
- Telegram: [@stevendev0822](https://t.me/stevendev0822)
- Twitter: [@stevendev0822](https://twitter.com/stevendev0822)
- Instagram: [@stevendev0822](https://www.instagram.com/stevendev0822/)
