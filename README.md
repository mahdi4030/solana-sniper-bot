## solana-sniper-bot

## Overview

The Solana Trading Bot helps you trade tokens on the Pump.fun on Solana blockchain based on bonding curves and market cap changes. The bot scrapes data to identify new tokens with favorable bonding curves, monitors market cap changes, and makes decisions on when to sell to maximize profits.

## Trading Strategy

- **Initial Buy**: The bot scrapes pump.fun to identify new token pairs with favorable bonding curves.
- **Monitoring**: Once a token is bought, the bot monitors the market cap and bonding curve progress.
- **Profit Targets**: 
  - The bot aims to take profit at a 25% increase and then again at another 25% increase.
  - It sells 50% of the tokens at the first 25% increase and 75% of the remaining tokens at the next 25% increase.
- **Stop Loss**: The bot will sell all tokens if the market cap falls by 10%.
- **Bonding Curve**: The bot will sell 75% of the tokens if the bonding curve reaches a critical level and keep 25% as a moon bag.
- **Timing**: The bot resets the timer if the price goes up and monitors the trade for a set period, adjusting its actions based on market conditions.

## Requirements

- **Node.js**: JavaScript runtime built on Chrome's V8 JavaScript engine.
- **Solana CLI**: Command-line interface for interacting with the Solana blockchain.
- **Selenium WebDriver (Chrome)**: Automated web browser.
- 
