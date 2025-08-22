# Brokex Protocol Auto BOT


"This is an automated bot for interacting with the Brokex Protocol on the Pharos testnet. The bot provides functionality to claim faucet tokens, open and close positions with leverage, and manage liquidity pools.

## Features

- 🚰 **Claim Faucet**: Claim testnet USDT tokens
- 📊 **Open Positions**: Trade with Long/Short & select leverage 1-50
- 🔒 **Close Positions**: Automatically close open positions
- 💧 **Liquidity Management**: Deposit and withdraw from liquidity pools
- 🔄 **Proxy Support**: Rotate proxies for improved reliability
- ⏱️ **Randomized Delays**: Avoid detection with configurable delays
- 📊 **Real-time Logging**: Color-coded terminal output with timestamps

## Installation

1. Clone the repository:
```bash
git clone https://github.com/dicoderin/Brokex-BOT.git
cd Brokex-BOT
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Create necessary files:
```bash
touch accounts.txt proxy.txt
```

## Configuration

### accounts.txt
Add your private keys (one per line):
```
0xYourPrivateKey1
0xYourPrivateKey2
...
```

### proxy.txt (optional)
Add your proxies (one per line):
```
http://user:pass@ip:port
socks5://user:pass@ip:port
...
```

## Usage

Run the bot:
```bash
python bot.py
```

### Menu Options
1. **Claim Faucet** - Claim testnet USDT tokens
2. **Open Position** - Open leveraged trading positions
   - Set position count per wallet
   - Set position amount (min 10 USDT)
3. **Close Position** - Close open positions
4. **Deposit Liquidity** - Add funds to liquidity pool
5. **Withdraw Liquidity** - Remove funds from liquidity pool
6. **Run All Features** - Execute all actions sequentially

### Proxy Options
1. Use free proxies from Proxyscrape
2. Use private proxies from proxy.txt
3. Run without proxies

## Supported Pairs
- BTC/USDT
- ETH/USDT
- SOL/USDT
- XRP/USDT
- AVAX/USDT
- TRX/USDT
- ADA/USDT
- SUI/USDT
- LINK/USDT

## Leverage Options
The bot randomly selects leverage from:
- 1x
- 2x
- 5x
- 10x Up to 50x

## Disclaimer
⚠️ **This is experimental software.** Use at your own risk. ⚠️

- Only use testnet accounts
- Do not use mainnet private keys
- The developers are not responsible for any losses
- This bot is for educational purposes only
