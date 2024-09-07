# Raydium Volume Bot

This volume bot can mint new SPL token, make a new market on Raydium, create & initialize pool, then start the rasing volume action.

## Screenshots

![image](https://github.com/user-attachments/assets/6c713340-d4fa-4552-b947-a6a928783b5c)


![image](https://github.com/user-attachments/assets/b5c65875-96ba-426e-956a-f4efe5c49d11)


## How to work

<span style="color: #00ff00;">Buy/Sell/Close WSOL in the same transaction</span>

1. Create SPL token

   https://solscan.io/tx/5FaDt6C8cXu7qXEfHaA96bS8DBuqMk6v5gkvZc9kfqa7kPp7DU34AwGtx3MEanxiypZ4VDRGLWVvstexDJbCGHZ4

2. Create Market ID on Raydium

   https://solscan.io/tx/5kLsgZrbcHKmE763u6awrKAr2gABf9dfnA3397ectDhaQq9m9YaJKP8nVNKqii9t4utaeL9bHfRgenhMtSGMxEvt

3. Create & init Pool on Raydium

   https://explorer.jito.wtf/bundle/1c135c60a593a36103b4430496968be6a7e55881f2ee9bc822ef01b746a5102f

4. Create Lookuptable

   https://explorer.jito.wtf/bundle/276ee13e52f4c89896b650dea26844eb2bb9c9226b022b0211d34b7b0913da08

5. Extend Lookuptable

   https://explorer.jito.wtf/bundle/d6ea2f757d3e25caf343a0a5a6b07c05af58077ab58cf8e3772698aefbbf4193

6. Crearte WSOL account and distribute to multi-wallets

   https://explorer.jito.wtf/bundle/68e72c3694fac5046bb4e2c9aa9aedc5795e9f3cc06facb53ae37b15e163bffe

7. Increase its Volume

   https://explorer.jito.wtf/bundle/8463aa4eeb5f63a953647185fdb01a527340a32719cd011ce0d5a3bfccc8e1a9

8. Mint lots of SPL tokens

   https://solscan.io/tx/YB7u7ms1Rvf2w3ih9G2N1qRxtTJeaDq8hMpMvVUhXXfHKrrqNCve1hBvPunxZWtNXcFEry4RjMUCYbhoLThxQy4

9. Sell all tokens

   https://explorer.jito.wtf/bundle/c87f0dffd473804468fecbd2ad1c8af7b50bbff1c8dd0707b5865ec97bc9e24c

10. Remove Liquidty

   https://explorer.jito.wtf/bundle/8c65aa7bdbede537a5ca1bce38bef4fc2aa2032e197393afac38e8a3a66332df



## Tech Stack

- Typescript
- Solana/web3.js
- Raydium SDK
- Jito


## Getting Started

To start this project, follow these steps:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/btcoin23/v_bot.git
   ```

2. Navigate to the project directory:

   ```bash
   cd v_bot
   ```

3. Install the project dependencies:

   ```bash
   npx yarn 
   ```
4. Create a `.env` file in the project root directory and add your wallet's   secret key, RPC URL, and other necessary configuration.
   ```bash
   PRIVATE_KEY=
   RPC_URL=
   WSS_URL=
   ```
5. Edit the `config.ts` file to configure the bot's settings.

   ```bash
   export const SolInPool // SOL amount to init the pool (SOL)
   export const Min_DisAmt // distribute min amount (SOL)
   export const Max_DisAmt // distribute max amount (SOL)
   export const X_Profit // profit amount (%)
   export const JitoTip // jito tip amount (SOL)
   export const NewMintAmt // additional mint amount 

   export const delay // delay time between each transaction (ms)
   export const NumWallets // number of wallets
   ```
6. Start the bot

   Run the following command to start the token creation process:

   ```bash
   npm start
   ```


## Author

- [Github](https://github.com/btcoin23)

- [Telegram](https://t.me/BTC0in23)
