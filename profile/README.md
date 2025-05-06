# 🌍 BeTheNation.Fun - Perpetual Prediction Markets for Countries

**BeTheNation.Fun** is a decentralized platform that enables users to speculate on the long-term economic performance of countries through perpetual prediction markets. Built on blockchain technology, the platform offers transparent, permissionless, and automated trading on country-based markets using real economic indicators.

> ⚡ Built for the [Pharos Builder Base Camp Hackathon](https://pharos.xyz)

---

## 🧭 Overview

BeTheNation.Fun introduces a new type of prediction market: **perpetual, decentralized, and based on economic fundamentals**. Users can trade tokenized representations of country performance — going long or short — based on indicators like inflation, GDP growth, stock indices, and exchange rates. These contracts never expire, allowing positions to be held as long as desired.

Unlike traditional prediction markets where users bet on binary outcomes, BeTheNation.Fun quantifies macroeconomic predictions into tradable indices. For example, instead of predicting "Will interest rates rise?", traders can go long or short on a rate index that reflects central bank decisions. This turns policy speculation into an on-chain asset.

Don’t just bet — trade the future of nations.

---

## 😵 Problem We Are Solving

- ⏳ **Limited Flexibility**: Fixed expiry dates force traders to close positions early.
- 💸 **Risk of Loss**: Positions liquidated, traders lose everything when wrong.
- 🕒 **Expiration Pressure**: Quick decisions limit long-term predictions.
- 🔄 **Lack of Engagement**: Fixed expiry leads to disconnected, short-term focus.

---

## 💡 Solution

BeTheNation.Fun offers:
- 🌀 **Perpetual Markets**: No expiry, hold positions as long as you want.
- 🚫 **No Liquidation Risk**: No total loss when wrong, adjust positions freely.
- 📈 **Continuous Trading**: Speculate on long-term trends without deadlines.
- ⚖️ **Balanced Risk**: Periodic fees keep the market fair and stable.

---

## ⚙️ How It Works

1. **Tokenized Country Markets**  
   Each country is represented by a token linked to its economic performance.

2. **CountryScore Generation**  
   A score is calculated using key economic indicators: inflation, GDP, stock indices, exchange rate, etc.

3. **Open Long/Short Positions**  
   Traders speculate on the direction of the CountryScore by opening long or short positions.

4. **Funding Fee Mechanism**  
   Every 8 hours, funding fees are exchanged between longs and shorts to balance the market.

5. **Automated Profit Sharing**  
   Smart contracts distribute profits to traders and liquidity providers based on their positions.

---

## ✨ Key Features

- 🔁 **Perpetual Contracts** – No expiry dates, stay in the market indefinitely.
- 📈 **CountryScore** – Dynamic score from real macro data.
- 🧠 **Leverage** – Amplify returns (or risks) with leverage trading.
- 🔄 **Funding Fee Model** – Align market incentives between long and short positions.
- 🧑‍🌾 **Liquidity Provider Rewards** – LPs earn from fees and market activity.
- 🤖 **On-Chain Profit Sharing** – No trusted intermediaries required.

---

## 🧪 Tech Stack

| Layer        | Stack / Tools                            |
|--------------|------------------------------------------|
| Frontend     | React.js, Tailwind CSS                   |
| Smart Contracts | Solidity, foundry, Ethers.js          |
| Blockchain   | Base / Pharos (for testnet & launch)     |
| Wallet Auth  | RainbowKit, MetaMask                     |
| Hosting      | Vercel / IPFS                            |

---

## 🔗 Links

- 🔧 GitHub: [BeTheNation Repos](https://github.com/orgs/BeTheNation/repositories)
- 🌐 Website: [bethenation.fun]([https://frontend-eight-mu-77.vercel.app](https://deploy-preview-23--splendid-kringle-e42657.netlify.app/))
- 🛠 Hackathon: [Pharos.xyz](https://pharos.xyz)
- 🎥 Demo Application: [YouTube Video](https://www.youtube.com/watch?v=IU8hBFeg4rI)
- 📊 Presentation: [figma](https://www.figma.com/deck/TuHuBdAIenx2jli1vVD9TK/Slide?node-id=3-121&viewport=-3676%2C-56%2C0.56&t=JISSzZ2uydwcCkDa-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1)

---

## 📚 References & Inspirations

### Noise.xyz
> A decentralized platform where users trade trends and narratives as assets using real-time social data.  
By integrating Kaito, a mindshare oracle, Noise tracks discussions from Twitter and allows speculation on cultural attention using up to 5x leverage.

🔗 [https://noise.xyz](https://noise.xyz)

**Relevance to BeTheNation.Fun**:  
Inspired the concept of turning **non-traditional data (like social trends)** into tradable markets. We adapted this approach to **macro-economic indicators**.

---

### Polymarket
> A decentralized platform for betting on real-world outcomes like elections, weather, and markets.

🔗 [https://polymarket.com](https://polymarket.com)

**Relevance to BeTheNation.Fun**:  
A strong UX/UI and clear example of decentralized prediction markets using oracles to settle markets — key inspiration for execution and structure.

---

## 🛠 How to Contribute

We welcome contributors to help shape the future of BeTheNation.Fun!

```bash
# 1. Fork the repository
# 2. Create a feature branch
git checkout -b feature/your-feature-name

# 3. Implement your changes

# 4. Push your branch
git push origin feature/your-feature-name

# 5. Submit a pull request
