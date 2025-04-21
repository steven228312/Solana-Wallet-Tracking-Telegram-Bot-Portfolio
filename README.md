# Solana Wallet Tracking Telegram Bot

A professional real-time Solana wallet monitoring system that tracks transactions, calculates pnl and delivers instant notifications via Telegram.

<p align="center">
  <img src="https://github.com/stevendev0822/Solana-Wallet-Tracking-Telegram-Bot-Portfolio/blob/main/public/Usage.gif" alt="Home video">
</p>

## Solana Wallet Monitoring Overview

This application monitors Solana wallet activities in real-time, analyzes transactions, and sends detailed notifications through Telegram. It's designed for traders, investors, and developers who need immediate insights into wallet transactions on the Solana blockchain.

## Key Blockchain Tracking Features

- <b>Real-time Transaction Monitoring:</b> Track wallet activities as they happen on the Solana blockchain
- <b>Multi-wallet Support:</b> Track multiple wallets simultaneously through an intuitive Telegram interface
- <b>Detailed Transaction Analysis:</b> Identify buy/sell operations, token transfers, and amounts
- <b>Instant Telegram Notifications:</b> Receive formatted alerts with comprehensive transaction details
- <b>Transaction History:</b> Store and query historical transaction data with MongoDB
- <b>Token Information:</b> Get detailed token data including symbols, names, and amounts
- <b> PNL Tracking:</b> Calculate and display profit and loss for each transaction

## DeFi Monitoring Architecture

The system is built on three core components:

- <b>Helius RPC:</b> Provides reliable Solana blockchain data access with WebSocket connections
- <b>MongoDB:</b> Stores transaction history for analysis and reference
- <b>Telegram Bot API:</b> Delivers real-time notifications and interactive user interface

## Installation for Solana Wallet Tracking Telegram Bot

```bash
# Clone the repository
git clone https://github.com/stevendev0822/Solana-Wallet-Tracking-Telegram-Bot.git

# Navigate to the project directory
cd Solana-Wallet-Tracking-Telegram-Bot

# Install depen dencies
npm install

```

## Blockchain Bot Configuration

Create a `.env` file in the root directory with the following variables:

```bash
# Solana RPC Configuration
RPC_URL=https://mainnet.helius-rpc.com/?api-key=YOUR_API_KEY
WSS_URL=wss://mainnet.helius-rpc.com/?api-key=YOUR_API_KEY

# [Optional] Default Wallet Configuration
WALLET_ADDRESS=YOUR_DEFAULT_WALLET_ADDRESS

# MongoDB Configuration
MONGODB_URI=mongodb://localhost:27017/solana_wallet_tracking

# Telegram Configuration
TELEGRAM_BOT_TOKEN=YOUR_BOT_TOKEN
```

## Setting Up Your Telegram Bot

1. Open Telegram and search for the @BotFather
2. Send `/newbot` command
3. Name your bot (e.g., "SolanaWalletTracker")
4. Choose a username (e.g., "SolanaWalletTrackerBot")
5. Save your bot token


## Crypto Tracking Usage

Once you clone the repository, install dependencies, and configures `.env`, you can simply start the application with the following command:

```
# Start the application
npm start
```

## Solana Wallet Tracking Telegram Bot Commands

The bot supports the following commands:

`/start` - Initialize the bot and see the welcome message
`/help` - Display available commands and usage instructions
`/list` - View all wallets you're currently tracking
`/stop [address]` - Stop tracking a specific wallet
`/stopall` - Stop tracking all 


To track a new wallet, simply send a valid Solana wallet address to the bot.


## Sample Notification

```bash
🔔 New Transaction Detected!

👛 Wallet: AbC1...XyZ9

💰 Sol Amount: 🟢 BUY 1.234 SOL

💸 PNL for this Token: 0.123 SOL

🚀 Token: BONK(Bonk)

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


## Wallet Tracking Performance Considerations

- The bot uses WebSocket connections for efficient real-time monitoring
- Transaction data is cached to minimize RPC calls
- MongoDB indexes optimize query performance
- Telegram message formatting is optimized for readability


## Frequently Asked Questions

- Does this bot require my private keys? 

No, the bot only needs public wallet addresses to monitor transactions.

- Can I track multiple wallets simultaneously? 

Yes, you can track as many wallets as you need through the Telegram interface.

- Will I get notifications for all transaction types? 

The bot focuses on token transfers, swaps, and SOL movements, filtering out less relevant transactions.

- Is historical data available? 

Yes, transaction data is stored in MongoDB for historical analysis.

## License
This project is licensed under the [MIT License](./LICENSE).

## Contact Information

- Gmail: [steven0822.dev@gmail.com](mailto:steven0822.dev@gmail.com)
- GitHub: [Steven Leal(stevendev0822)](https://github.com/stevendev0822)
- Telegram: [@stevendev0822](https://t.me/stevendev0822)
- Twitter: [@stevendev0822](https://twitter.com/stevendev0822)
- Instagram: [@stevendev0822](https://www.instagram.com/stevendev0822/)


## Keywords
<i> Solana, Blockchain, Wallet Tracker, Telegram Bot, Real-time Monitoring, Transaction Analysis, Cryptocurrency, Trading Bot, DeFi Tools, Solana Transactions, Blockchain Monitoring, SPL Tokens, Crypto Alerts, Solana Token Tracking, Crypto PNL Monitoring, Solana Network, Blockchain Notifications, Cryptocurrency Trading, DeFi Monitoring, Solana DeFi, Solana Wallet Notifications, Crypto Transaction Alerts, Blockchain Analytics, Solana Whale Tracking, Token Transfer Monitoring, Crypto Portfolio Tracker</i>