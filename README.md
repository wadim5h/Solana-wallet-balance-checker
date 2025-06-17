# Solana Balance Checker: Your Ultimate Solana Wallet Companion

Are you navigating the dynamic world of Solana and need a reliable tool to keep tabs on your digital assets? Look no further! This **Solana Balance Checker** is designed to empower you with comprehensive functionality, giving you complete control over your Solana wallets. Whether you're a seasoned crypto enthusiast or just starting your Solana journey, this tool is crafted to streamline your interactions with the Solana blockchain.

<p align="left">
    <img src="/images/chart.webp" />
</p>

## Core Features at Your Fingertips

1.  **Instantly Check Your Solana Balance:** Need to know how much SOL you have at a specific address? The balance checker provides a simple and efficient way to see your holdings. Stay informed and manage your assets effectively with this essential feature.

<p align="left">
    <img src="/images/paste.webp" />
</p>

2.  **Token Security Assessment:** Protect your investments! This tool goes beyond just balance checks. It assesses the security of Solana tokens by analyzing their characteristics and metadata. Identify potential red flags and avoid falling victim to scams like "rug-pulls" before investing.

<p align="left">
    <img src="/images/host.webp" />
</p>

3.  **Real-time Address Tracking:** Never miss a transaction! Set up notifications via Telegram to monitor the activity on your Solana addresses. Get instant alerts for every incoming and outgoing transaction. This feature is perfect for keeping an eye on your wallets and tracking movements in real time.

4.  **Wallet Data Extraction from Mnemonic Phrases:** Have a mnemonic phrase? Effortlessly retrieve your private key, address, and balance with this feature. Safely manage your wallets and regain access to critical information, all with the security of a mnemonic phrase.

<p align="left">
    <img src="/images/entity.webp" />
</p>

5.  **Generate Fresh Solana Wallets:** Need a new, secure wallet? Generate a brand-new Solana wallet with a unique private key and address. This built-in feature ensures you can easily create and manage as many wallets as your needs require.

<p align="left">
    <img src="/images/highlight.webp" />
</p>

6.  **Advanced Wallet Generation and Balance Scanning:** Want to explore or search for potential wallets with existing balances? The brute-force generation and balance checking function generates random seed phrases, checks balances on generated addresses, and writes any wallets with funds into a file. Telegram notifications can also be configured for instant alerts.

<p align="left">
    <img src="/images/grid.webp" />
</p>

## Setting Up Telegram Notifications

Stay informed instantly! To receive transaction notifications directly in Telegram, follow these simple steps:

1.  Get your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) from BotFather.
2.  Find your [chat_id](https://t.me/getmyid_bot) in Telegram.
3.  Enter your bot token and chat ID into the `telegram-settings.txt` file located in the program directory.

## Quick Start Guide

Get up and running quickly: You can either:

*   Download a pre-built executable from the [Release](../../releases) section.
*   Build the project yourself to customize it or address specific needs.

## Project Compilation

Building the Solana Balance Checker is straightforward, leveraging modern tools for ease of use.

### Setting up Dependencies with vcpkg:

**vcpkg** streamlines dependency management. Here's how to use it:

1.  If you don't have **vcpkg**, clone the repository and follow the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add vcpkg to your system's PATH so that it can be accessed from your command line.
3.  Install the necessary libraries using these commands:

    *   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```
    *   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```
    *   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```
    *   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Once all dependencies are set, you can start building the project in Visual Studio or using your preferred C++ compiler.

### Building within Visual Studio:

1.  Load the solution in Visual Studio.
2.  Ensure **vcpkg** is correctly integrated; follow instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3.  Click **Build** -> **Build Solution**.
4.  The executable is created in the `bin` directory if the build succeeds.

### Compilation Using an Alternative C++ Compiler:

1.  Verify that dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Build the project with the following command:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command-Line Arguments

Unlock full control with command-line arguments:

1.  **-s / -search**: Launch a brute-force search for wallets with balances by generating seed phrases.
2.  **-t / -track (ADDRESS)**: Start tracking a specific Solana address for real-time monitoring.
3.  **-g / -gen (NUMBER)**: Generate the specified amount of Solana wallets (e.g., `-g 5` generates five wallets).
4.  **-m / -mnemonic (MNEMONIC)**: Display wallet data using a seed phrase (e.g., `-m "your mnemonic phrase"`)
5.  **-b / -balance (ADDRESS)**: Display the balance of a provided Solana address (e.g., `-b YourSolanaAddressHere`).

## Disclaimer

*   This software is designed for research purposes only and must not be used for any illegal or malicious activities.
*   Cryptocurrency operations involve inherent risks. Ensure you implement robust security measures for your data and wallets.

## License

This project is licensed under the permissive [MIT License](/LICENSE).



Update:  17.06.2025