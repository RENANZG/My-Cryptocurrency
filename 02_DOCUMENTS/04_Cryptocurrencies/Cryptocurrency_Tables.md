<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cryptocurrency Table of Concepts</title>
<style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 5em;
      max-width: 800px;
      margin-left: auto;
      margin-right: auto;
      background-color: #4D4D4D;
      color: #e0e0e0;
    }
    h1, h2, h3, h4, h5, h6 {
      font-weight: bold;
      margin-bottom: 0.5em;
      color: #F26822;
    }
    h1 {
      font-size: 2.5em;
      line-height: 1.2;
    }
    h2 {
      font-size: 2em;
      line-height: 1.3;
    }
    h3 {
      font-size: 1.8em;
      line-height: 1.4;
    }
    table {
      width: 100%;
      margin-bottom: 20px;
      border-collapse: collapse;
    }
    th, td {
      padding: 10px;
      border: 1px solid #ddd;
      text-align: left;
      color: #ffffff;
    }
    th {
      background-color: #ffffff;
      color: #F26822;
    }
</style>
</head>
<body>
  
  <h1>Cryptocurrency Table of Concepts</h1>
  
  <h2>Cryptocurrency Wallet Concepts</h2>

  <h3>Key Generation and Management</h3>
  
  <table table border="1">
    <thead>
      <tr>
        <th>Concept</th>
        <th>Description</th>
        <th>Category</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Private Key</td>
        <td>A secret cryptographic key used to sign transactions and prove ownership of cryptocurrency.</td>
        <td>Key Management</td>
      </tr>
      <tr>
        <td>Public Key</td>
        <td>A key derived from the private key, used to verify signatures and generate addresses.</td>
        <td>Key Management</td>
      </tr>
      <tr>
        <td>Master Seed (Seed Phrase)</td>
        <td>A random number converted into a human-readable series of words (12-24 words) used to derive all keys.</td>
        <td>Key Generation</td>
      </tr>
      <tr>
        <td>Master Key</td>
        <td>The private key directly derived from the Master Seed; it controls all other keys in the wallet.</td>
        <td>Key Generation</td>
      </tr>
      <tr>
        <td>Extended Private Key (xprv)</td>
        <td>A master private key with additional information (e.g., chain code), allowing derivation of all child keys.</td>
        <td>Key Generation & Derivation</td>
      </tr>
      <tr>
        <td>Extended Public Key (xpub)</td>
        <td>A master public key that can generate all child public keys without revealing private keys.</td>
        <td>Key Generation & Derivation</td>
      </tr>
      <tr>
        <td>Chain Code</td>
        <td>A 256-bit value that helps derive child keys, ensuring uniqueness and security in hierarchical key structures.</td>
        <td>Key Derivation</td>
      </tr>
    </tbody>
  </table>

  <h3>Key Derivation and Hierarchical Structures</h3>

  <table table border="1">
    <thead>
      <tr>
        <th>Concept</th>
        <th>Description</th>
        <th>Category</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>HD Wallet (Hierarchical Deterministic Wallet)</td>
        <td>A wallet structure that generates a tree of private and public keys from a single master seed.</td>
        <td>Key Derivation</td>
      </tr>
      <tr>
        <td>Child Key</td>
        <td>A key derived from the master or parent key using a derivation function.</td>
        <td>Key Derivation</td>
      </tr>
      <tr>
        <td>Grandchild Key</td>
        <td>A key derived from a child key, continuing the hierarchical structure for more key segmentation.</td>
        <td>Key Derivation</td>
      </tr>
      <tr>
        <td>Key Derivation Path</td>
        <td>A standard way of specifying which key in the hierarchical tree to derive (e.g., m/44'/0'/0').</td>
        <td>Key Derivation</td>
      </tr>
      <tr>
        <td>HMAC-SHA512</td>
        <td>A cryptographic function used in HD wallets to derive child keys from the parent key and chain code.</td>
        <td>Key Derivation</td>
      </tr>
    </tbody>
  </table>

  <h3>Security and Backup</h3>

  <table table border="1">
    <thead>
      <tr>
        <th>Concept</th>
        <th>Description</th>
        <th>Category</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Backup Phrase (Seed Phrase)</td>
        <td>A set of words (typically 12 or 24) that can regenerate the master seed and, consequently, the entire wallet.</td>
        <td>Security & Backup</td>
      </tr>
      <tr>
        <td>Recovery Phrase</td>
        <td>Synonym for Backup Phrase. It allows users to restore their wallet if the device is lost or damaged.</td>
        <td>Security & Backup</td>
      </tr>
      <tr>
        <td>Encryption</td>
        <td>Protecting private keys and wallet data using cryptographic algorithms (e.g., AES) for confidentiality.</td>
        <td>Security</td>
      </tr>
    </tbody>
  </table>

  <h3>Public Keys and Addresses</h3>

  <table table border="1">
    <thead>
      <tr>
        <th>Concept</th>
        <th>Description</th>
        <th>Category</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Address</td>
        <td>A string derived from the public key (or public key hash), used to receive cryptocurrency.</td>
        <td>Public Identification</td>
      </tr>
      <tr>
        <td>Public Key Hash</td>
        <td>The result of applying a cryptographic hash (e.g., SHA-256, RIPEMD-160) to a public key to generate a unique address.</td>
        <td>Public Identification</td>
      </tr>
      <tr>
        <td>Address Format (Base58Check, Bech32)</td>
        <td>Encoding schemes used to represent addresses in a more user-friendly format.</td>
        <td>Public Identification</td>
      </tr>
      <tr>
        <td>Stealth Address</td>
        <td>A unique address generated for every transaction to enhance privacy (used in Monero).</td>
        <td>Public Identification & Privacy</td>
      </tr>
      <tr>
        <td>Ring Signature</td>
        <td>A cryptographic technique used to hide the identity of the sender in transactions (used in Monero).</td>
        <td>Privacy</td>
      </tr>
      <tr>
        <td>zk-SNARKs (Zero-Knowledge Proofs)</td>
        <td>Cryptographic proofs used to enable private transactions without revealing sender, recipient, or amount (used in Zcash).</td>
        <td>Privacy</td>
      </tr>
    </tbody>
  </table>

  <h3>Transaction Security and Signing</h3>
  
  <table table border="1">
    <thead>
      <tr>
        <th>Concept</th>
        <th>Description</th>
        <th>Category</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Transaction Signing</td>
        <td>The process of using a private key to sign a transaction, proving the authenticity and ownership of the transaction.</td>
        <td>Transaction Security</td>
      </tr>
      <tr>
        <td>ECDSA (Elliptic Curve Digital Signature Algorithm)</td>
        <td>A cryptographic algorithm used for signing transactions (commonly used in Bitcoin and other cryptocurrencies).</td>
        <td>Transaction Security</td>
      </tr>
      <tr>
        <td>EdDSA (Edwards-curve Digital Signature Algorithm)</td>
        <td>A newer and more secure signature scheme (used in Monero, Stellar).</td>
        <td>Transaction Security</td>
      </tr>
    </tbody>
  </table>

  <h3>Privacy and Confidentiality</h3>
  
  <table table border="1">
    <thead>
      <tr>
        <th>Concept</th>
        <th>Description</th>
        <th>Category</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>RingCT (Ring Confidential Transactions)</td>
        <td>A privacy feature in Monero that hides the transaction amounts using Ring Signatures.</td>
        <td>Privacy & Confidentiality</td>
      </tr>
      <tr>
        <td>Pedersen Commitments</td>
        <td>Cryptographic commitments that are used in Monero and Zcash to hide transaction amounts.</td>
        <td>Privacy & Confidentiality</td>
      </tr>
      <tr>
        <td>Stealth Address</td>
        <td>A method used in Monero to generate a unique address for every transaction, ensuring sender privacy.</td>
        <td>Privacy & Confidentiality</td>
      </tr>
      <tr>
        <td>zk-SNARKs (Zero-Knowledge Proofs)</td>
        <td>A cryptographic proof allowing one to prove knowledge of a fact without revealing the fact itself, used in Zcash for private transactions.</td>
        <td>Privacy & Confidentiality</td>
      </tr>
    </tbody>
  </table>


  <h3>Comparison of Custodial and Non-Custodial Wallets</h3>

  <table border="1">
    <thead>
      <tr>
        <th>Feature</th>
        <th>Custodial Wallet</th>
        <th>Non-Custodial Wallet</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Control of Private Keys</td>
        <td>Third-party service provider (e.g., exchange) holds your keys</td>
        <td>You control your own private keys</td>
      </tr>
      <tr>
        <td>Security</td>
        <td>Dependent on the service provider's security (can be a target for hacking)</td>
        <td>You are responsible for securing your private keys (can be lost and be hacked)</td>
      </tr>
      <tr>
        <td>Ease of Use</td>
        <td>Generally more user-friendly with features like recovery and customer support</td>
        <td>Can be more complex, requiring the user to manage their own private keys, operational security and backups</td>
      </tr>
      <tr>
        <td>Backup and Recovery</td>
        <td>Typically easier (support from the service provider if you lose access)</td>
        <td>Requires manual backup and recovery of the private keys or seed phrase</td>
      </tr>
      <tr>
        <td>Privacy</td>
        <td>Requires trust in the provider (often involves KYC and AML procedures)</td>
        <td>Higher privacy since transactions are not tied to personal information</td>
      </tr>
      <tr>
        <td>Transaction Speed and Fees</td>
        <td>Transactions may be faster or cheaper, depending on the service's structure</td>
        <td>Depends on the blockchain's current load and network conditions</td>
      </tr>
      <tr>
        <td>Risk of Loss</td>
        <td>If the service provider is hacked or goes out of business, you may lose access to funds</td>
        <td>If you lose your private keys or seed phrase, you lose access to your funds permanently</td>
      </tr>
      <tr>
        <td>Examples</td>
        <td>Coinbase, Binance, Kraken</td>
        <td>MetaMask, Trust Wallet, Ledger (hardware wallet)</td>
      </tr>
    </tbody>
  </table>

  <h3>Comparison of Hot Wallets and Cold Wallets</h3>

  <table border="1">
    <thead>
      <tr>
        <th>Wallet Type</th>
        <th>Description</th>
        <th>Security</th>
        <th>Examples</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Hot Wallets</strong></td>
        <td>Internet-connected, easy to access for frequent transactions, but vulnerable to hacking.</td>
        <td>Low to Medium (exposed to online risks)</td>
        <td>MetaMask, Trust Wallet, Coinbase Wallet</td>
      </tr>
      <tr>
        <td>Desktop Wallets</td>
        <td>Installed on a computer. You control the keys, but vulnerable to malware and physical damage.</td>
        <td>Medium (controlled by user but exposed to local threats)</td>
        <td>Electrum, Exodus</td>
      </tr>
      <tr>
        <td>Web Wallets</td>
        <td>Accessed via a web browser. Easy to use but the website controls the keys, making them less secure.</td>
        <td>Medium (website controls keys)</td>
        <td>MyEtherWallet (MEW), Blockchain.info</td>
      </tr>
      <tr>
        <td>Mobile Wallets</td>
        <td>Installed on mobile phones. Convenient but subject to theft or malware.</td>
        <td>Medium (subject to mobile security risks)</td>
        <td>Monerujo, Trust Wallet, Coinomi, Edge Wallet</td>
      </tr>
      <tr>
        <td><strong>Cold Wallets</strong></td>
        <td>Offline storage, providing high security for long-term storage.</td>
        <td>High (offline and immune to online threats)</td>
        <td>Ledger, Trezor, Paper Wallets</td>
      </tr>
      <tr>
        <td>Paper Wallets</td>
        <td>A physical printout of private keys. Highly secure when stored safely but vulnerable to physical loss or damage.</td>
        <td>High (offline, but physical risk)</td>
        <td>Generated via bitaddress.org or similar tools</td>
      </tr>
      <tr>
        <td>Hardware Wallets</td>
        <td>Physical devices storing private keys offline. Offers the highest security even when connected to a computer.</td>
        <td>High (offline, never exposes private keys online)</td>
        <td>Ledger Nano S, Trezor Model T, KeepKey</td>
      </tr>
    </tbody>
  </table>

  <h3>Comparison of Wallet Types and Their Recovery Methods</h3>

  <table border="1">
    <tr>
      <th>Wallet Type</th>
      <th>Recovery Method</th>
      <th>Advantages</th>
      <th>Disadvantages</th>
    </tr>
    <tr>
      <td>Software Wallet (Desktop/Mobile)</td>
      <td>Seed Phrase (12-24 words), Backup File, Private Key</td>
      <td>Easy access, can be used for transactions, user controls keys</td>
      <td>Vulnerable to hacking if not properly secured (malware, phishing, device theft)</td>
    </tr>
    <tr>
      <td>Web Wallet</td>
      <td>Backup File, Email/Account Recovery, Some use Seed Phrase</td>
      <td>Accessible from anywhere, no need for physical device</td>
      <td>Risk of hacking, dependent on service provider, service can be compromised</td>
    </tr>
    <tr>
      <td>Hardware Wallet</td>
      <td>Seed Phrase (12-24 words), Backup File</td>
      <td>Offline, highly secure, resistant to online attacks</td>
      <td>Requires physical device, risk of loss, theft, or damage to the device</td>
    </tr>
    <tr>
      <td>Exchange Wallet (Custodial)</td>
      <td>Account Recovery via Service Provider (e.g., email, 2FA, KYC)</td>
      <td>Convenient, no need to manage private keys, easy to use</td>
      <td>Trusting third party with your funds, exchange can be hacked, limited control over funds</td>
    </tr>
    <tr>
      <td>Crypto Payment Apps (Custodial)</td>
      <td>Account Recovery via Service Provider (e.g., email, 2FA, KYC)</td>
      <td>Easy to use, user-friendly, convenient for daily transactions</td>
      <td>Service provider holds the private keys, potential for service downtime or issues, custodial control</td>
    </tr>
    <tr>
      <td>Paper Wallet</td>
      <td>Private Key or Public Key written down</td>
      <td>No internet exposure, highly secure against online threats, offline storage</td>
      <td>Risk of physical damage or theft, no recovery option if lost, cumbersome for frequent transactions</td>
    </tr>
  </table>

  <h3>Comparison of Centralized Exchanges (CEX), Decentralized Exchanges (DEX), and CBDCs</h3>

  <table border="1">
    <thead>
      <tr>
        <th>Feature</th>
        <th>Centralized Exchange (CEX)</th>
        <th>Decentralized Exchange (DEX)</th>
        <th>Central Bank Digital Currency (CBDC)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Control</strong></td>
        <td>Controlled by a central authority (e.g., Binance, Coinbase)</td>
        <td>Peer-to-peer, no central authority</td>
        <td>Issued and controlled by the central bank of a country</td>
      </tr>
      <tr>
        <td><strong>Transaction Speed</strong></td>
        <td>Fast transactions, typically settled instantly</td>
        <td>Slower, depends on blockchain network congestion</td>
        <td>Fast, depending on the central bank's infrastructure</td>
      </tr>
      <tr>
        <td><strong>Privacy</strong></td>
        <td>Users must submit personal information (KYC, AML)</td>
        <td>More private, no KYC requirements, but still on-chain transactions</td>
        <td>Transactions are traceable, government-controlled, can be monitored</td>
      </tr>
      <tr>
        <td><strong>Security</strong></td>
        <td>Centralized risk, vulnerable to hacks and fraud</td>
        <td>More secure in terms of hacking (no central point of attack), but prone to smart contract bugs</td>
        <td>High security, government-backed, but can be susceptible to centralized risks and government control</td>
      </tr>
      <tr>
        <td><strong>Liquidity</strong></td>
        <td>High liquidity due to large user base</td>
        <td>Lower liquidity, but increasing with popular protocols</td>
        <td>Very high liquidity due to government backing</td>
      </tr>
      <tr>
        <td><strong>Transaction Fees</strong></td>
        <td>Fees depend on the exchange, often relatively low</td>
        <td>Generally low fees, but can be high during network congestion</td>
        <td>No or very low fees, as controlled by the central bank</td>
      </tr>
      <tr>
        <td><strong>Asset Types</strong></td>
        <td>Supports a wide range of cryptocurrencies and tokens</td>
        <td>Supports a range of tokens based on decentralized protocols (e.g., Ethereum, Uniswap)</td>
        <td>Digital versions of fiat currencies, typically limited to the national currency</td>
      </tr>
      <tr>
        <td><strong>Regulation</strong></td>
        <td>Regulated by government financial authorities</td>
        <td>Less regulated, operates in a decentralized manner (but can face regulatory scrutiny)</td>
        <td>Regulated and controlled by the central bank and government financial authorities</td>
      </tr>
      <tr>
        <td><strong>Ownership</strong></td>
        <td>Users don’t hold private keys, the exchange does</td>
        <td>Users retain control of their private keys</td>
        <td>Government retains control of the digital currency</td>
      </tr>
    </tbody>
  </table>

<h3>Comparison of Decentralized Exchange (DEX) Trading, Peer-to-Peer (P2P) Trading, and Over-the-Counter (OTC) Trading</h3>

<table border="1">
  <thead>
    <tr>
      <th>Aspect</th>
      <th>DEX Trading</th>
      <th>P2P Trading</th>
      <th>OTC Trading</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Definition</strong></td>
      <td>A blockchain-based platform where trades occur directly between users using smart contracts.</td>
      <td>Direct trade between two individuals, often facilitated by a platform with escrow services.</td>
      <td>Direct trading of assets between two parties, typically involving larger transactions without a centralized exchange.</td>
    </tr>
    <tr>
      <td><strong>Automation</strong></td>
      <td>Fully automated using smart contracts.</td>
      <td>Often manual or semi-automated, depending on the platform.</td>
      <td>Generally manual negotiation between parties, often facilitated by brokers or dealers.</td>
    </tr>
    <tr>
      <td><strong>Custody of Funds</strong></td>
      <td>Non-custodial: Users retain full control of their funds.</td>
      <td>May involve escrow or custodial services for added security.</td>
      <td>Funds are typically held by the parties involved until the transaction is completed.</td>
    </tr>
    <tr>
      <td><strong>Intermediary</strong></td>
      <td>No intermediary; transactions occur directly via the blockchain.</td>
      <td>Platform acts as a facilitator but does not control funds (except during escrow).</td>
      <td>Often involves brokers or dealers who facilitate the trade between parties.</td>
    </tr>
    <tr>
      <td><strong>Payment Methods</strong></td>
      <td>Crypto only (e.g., ETH, BTC).</td>
      <td>Supports fiat, PayPal, gift cards, and other non-crypto payment methods.</td>
      <td>Typically involves fiat currencies or other assets, negotiated directly between parties.</td>
    </tr>
    <tr>
      <td><strong>Use Case</strong></td>
      <td>Quick, decentralized crypto-to-crypto trades.</td>
      <td>Trading crypto for fiat or fiat for crypto, often across different payment methods.</td>
      <td>Facilitating large trades, often for institutional investors or high-net-worth individuals.</td>
    </tr>
    <tr>
      <td><strong>Examples</strong></td>
      <td>Uniswap, SushiSwap, Bisq.</td>
      <td>LocalCryptos, Paxful, Binance P2P.</td>
      <td>Circle, Genesis Trading, OTC desks at major exchanges.</td>
    </tr>
  </tbody>
</table>


  <h3>Comparison of Cryptocurrency, Fiat Currency, and Digital Currency</h3>

  <table border="1">
    <thead>
      <tr>
        <th>Feature</th>
        <th>Cryptocurrency</th>
        <th>Fiat Currency</th>
        <th>Digital Currency</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Definition</strong></td>
        <td>Decentralized digital assets secured by cryptography</td>
        <td>Government-issued currency that has physical and digital forms (e.g., USD, EUR)</td>
        <td>Digital money that represents a traditional currency, can be issued by government or private entities</td>
      </tr>
      <tr>
        <td><strong>Centralization</strong></td>
        <td>Decentralized, not controlled by any central authority</td>
        <td>Centralized, controlled by the government or central bank</td>
        <td>Can be centralized (e.g., CBDC) or decentralized (private digital currencies)</td>
      </tr>
      <tr>
        <td><strong>Examples</strong></td>
        <td>Bitcoin, Ethereum, Litecoin, etc.</td>
        <td>USD, EUR, GBP, JPY, etc.</td>
        <td>Digital USD (e.g., FedCoin), Digital Euros, Private digital currencies like stablecoins</td>
      </tr>
      <tr>
        <td><strong>Regulation</strong></td>
        <td>Less regulated, with some countries imposing bans or restrictions</td>
        <td>Highly regulated by governments and financial authorities</td>
        <td>Regulation depends on the issuer, with CBDCs being heavily regulated by governments</td>
      </tr>
      <tr>
        <td><strong>Security</strong></td>
        <td>Highly secure via cryptography, but susceptible to exchange hacks, fraud, and wallet theft</td>
        <td>Security relies on financial institutions, central banks, and physical currency infrastructure</td>
        <td>Security depends on the issuer, but can be as secure as the underlying technology (e.g., blockchain, encryption)</td>
      </tr>
      <tr>
        <td><strong>Transaction Speed</strong></td>
        <td>Varies (can take minutes to hours depending on network congestion and blockchain used)</td>
        <td>Instant within countries, but can take longer for international transfers (e.g., wire transfers)</td>
        <td>Varies depending on the system used, but can be fast for domestic digital transactions</td>
      </tr>
      <tr>
        <td><strong>Transaction Costs</strong></td>
        <td>Variable, often depends on network congestion and transaction size</td>
        <td>Usually low or none, but fees exist for certain services like international transfers</td>
        <td>Can vary based on the platform or the type of digital currency (e.g., CBDCs may have no fees, stablecoins may have low fees)</td>
      </tr>
      <tr>
        <td><strong>Ownership</strong></td>
        <td>Ownership is through private keys, and users are responsible for their security</td>
        <td>Ownership is recognized through legal tender and financial systems (banks, cash)</td>
        <td>Ownership depends on the system; CBDCs are controlled by governments, while private digital currencies can be user-owned</td>
      </tr>
      <tr>
        <td><strong>Volatility</strong></td>
        <td>Highly volatile, with prices fluctuating significantly in short periods</td>
        <td>Relatively stable, influenced by inflation rates, interest rates, and government policy</td>
        <td>Depends on the type; CBDCs are stable, but private digital currencies can be volatile (e.g., stablecoins, tokens)</td>
      </tr>
      <tr>
        <td><strong>Physical Form</strong></td>
        <td>Purely digital, no physical counterpart</td>
        <td>Has physical (cash) and digital (bank account) forms</td>
        <td>Purely digital, no physical counterpart (except for fiat-backed digital currencies like CBDCs)</td>
      </tr>
      <tr>
        <td><strong>Global Usage</strong></td>
        <td>Global use, but adoption varies by country and region</td>
        <td>Widely accepted globally, with the exception of some countries (e.g., hyperinflation or bans)</td>
        <td>Limited to regions where issued (e.g., CBDCs within a specific country or currency zone)</td>
      </tr>
    </tbody>
  </table>

</body>
</html>