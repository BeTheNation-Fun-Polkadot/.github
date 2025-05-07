# 🌍 BeTheNation.Fun - Perpetual Prediction Markets for Countries
Speculate on macroeconomics like never before — on-chain, perpetual, and open to everyone.


🧠 Predict the long-term fate of nations using real economic indicators — not hype.
----(Ganti dengan link GIF atau image dari demo nanti)----

---

## 🧭 Overview
BeTheNation.Fun introduces a new type of prediction market: **perpetual, decentralized, and based on economic fundamentals**.
Users can trade tokenized representations of country performance — going long or short — based on indicators like inflation, GDP growth, stock indices, and exchange rates.
These contracts never expire, allowing positions to be held as long as desired.

Unlike traditional prediction markets where users bet on binary outcomes, 
BeTheNation.Fun quantifies macroeconomic predictions into tradable indices. 
For example, instead of predicting "Will interest rates rise?", traders can go 
long or short on a rate index that reflects central bank decisions. This turns 
policy speculation into an on-chain asset.

---

## 😵 Problem We Are Solving
- ⏳ Expiring prediction markets limit long-term forecasting.
- 💸 High liquidation risk on leveraged positions.
- 🧩 No financial product for directly trading macro trends of countries.
- 🌐 Prediction markets too focused on events, not economic fundamentals.

---

## 💡 Solution
We introduce Perpetual Country Positions, where traders can:
- 📈 Open long/short positions on countries based on real indicators.
- 🌀 Keep positions perpetually — no expiry.
- ⚖️ Avoid full liquidations — positions decay over time, not explode.
- 🤝 Trade with transparent funding fees and no centralized intermediaries.

---

## ⚙️ How It Works
1. **CountryScore Calculation**
   Based on CPI, GDP, Stock Index, Exchange Rate — hardcoded (PoC) or via oracle.
2. **Position Contracts**
   Users open long or short using openPosition(), and can set takeProfit / stopLoss.
3. **Funding Fee Model**
   Balances incentives between longs/shorts every 8 hours.
4. **Profit/Loss Sharing**
   All handled by smart contracts — no need to trust us.

---   

## ✨ Key Features
- 🔁 **Perpetual Markets** – Positions never expire.
- 📊 **CountryScore** – Derived from economic data (PoC = hardcoded).
- 🧠 **Leverage Trading** – Predict with 2x–10x impact.
- 🤖 **On-Chain Settlement** – All logic in Solidity (EVM) — migrating to   Ink! (Rust).
- 🧑‍🌾 **Liquidity Provider Rewards** – For market makers.
- 🔄 **No Total Liquidation** – Reduce risk, improve fairness.

---

## 🧪 Tech Stack
| Layer          | Stack / Tools                                           |
| -------------- | ------------------------------------------------------- |
| Frontend       | React.js, Tailwind CSS                                  |
| Wallet Auth    | Polkadot.js Extension, WalletConnect (via Talisman SDK) |
| Smart Contract | **Ink! (Rust)** via Substrate Contracts pallet          |
| Blockchain     | **Polkadot Ecosystem** (Testnet: Rococo / Local)        |
| Dev Tools      | cargo-contract, Substrate Playground, Phala Dev Tools   |
| Hosting        | Vercel, IPFS, Static Web Deployment                     |

---

## ⚙️ Smart Contracts on Polkadot
Our smart contracts are built using ink!, a Rust-based language designed specifically for the Polkadot ecosystem. Unlike traditional Ethereum-based contracts written in Solidity, ink! runs natively on the Substrate Contracts Pallet, enabling far more efficient execution in terms of speed and cost.

## ⚡ Why Polkadot + ink!
- **Low to Zero Gas Fees**
  On Polkadot, contract execution is significantly cheaper than on EVM-based chains. In some testnets or parachains, gas fees can be effectively zero, enabling more experimentation and frequent interaction without cost barriers.
  
- **High Performance**
  Contracts compiled from Rust into WebAssembly (Wasm) are inherently faster and safer. This means smart contracts on Polkadot are not only cheaper but also more performant, making them suitable for complex applications like perpetual prediction markets.

- **Solidity vs. ink!**
  During early development, we experimented with Solidity on an EVM-compatible chain. However, we faced unexpected high gas costs and execution errors, especially when simulating state-heavy logic like perpetual funding and leverage. Switching to ink! resolved these issues and unlocked native integration with Substrate’s features.

---

## 🔗 Links

- 🔧 GitHub: [BeTheNation Repos](https://github.com/orgs/BeTheNation-Fun-Polkadot/repositories)

- 🌐 Website: [bethenation.fun](https://deploy-preview-23--splendid-kringle-e42657.netlify.app/)

- 🎥 Demo Application: [YouTube Video](https://www.youtube.com/watch?v=IU8hBFeg4rI)

- 📊 Presentation: [figma](https://www.figma.com/deck/TuHuBdAIenx2jli1vVD9TK/Slide?node-id=3-121&viewport=-3676%2C-56%2C0.56&t=JISSzZ2uydwcCkDa-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1)
---

## 🤖 AI Tools Used
| Tool     | Purpose                                |
| -------- | -------------------------------------- |
| ChatGPT  | Idea clarification, writeup, structure |
| Claude 3 | Draft refinement, insight suggestion   |

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

## 🛠️ Feedback on Polkadot Tooling and Documentation
Throughout the development of our project using Polkadot’s smart contract stack—primarily ink!, cargo-contract, and Polkadot.js UI—our team encountered a number of friction points that hindered the onboarding experience for new developers. Below are the most notable issues, along with suggestions based on our direct experience:

1. 🚫 Missing Critical Setup Step in Ink! Docs
    Issue: The official setup guide on use.ink omits the rustup target add wasm32-unknown-unknown command. Without this target, compiling contracts fails with an unclear error (target not found).
    Impact: This is a major barrier for new developers and leads to unnecessary confusion.
    Suggested Fix: Include the required command explicitly at the top of the setup instructions.
    Evidence:

```bash
error: target 'wasm32-unknown-unknown' not found    
#   Command that resolves it:
rustup target add wasm32-unknown-unknown
```

2. 🔄 No End-to-End Contract + Front-End Example
    Issue: While the ink! docs provide decent examples for writing and deploying smart contracts, they lack an end-to-end tutorial demonstrating integration with a frontend (e.g., using Polkadot.js + React).
    Impact: This gap slows down teams trying to build full-stack dApps on Polkadot.
    Suggested Fix: Provide a beginner-friendly example repository that includes:
- Smart contract in ink!
- Deployment script
- Frontend (React or plain JS) interacting with contract via @polkadot/api
Evidence: Documentation provides contract examples but no frontend integrations. We had to manually bridge data and experiment with Polkadot.js API calls.

3. ⚙️ Tooling Version Compatibility Issues
    Issue: We encountered build failures due to incompatible versions between cargo-contract, ink!, and Rust. The documentation assumes these tools "just work together," but in reality, minor mismatches break the pipeline.
    Impact: Wasted time debugging environment inconsistencies.
    Suggested Fix: Provide a version compatibility matrix (like this) or a version-check script (cargo-contract doctor) to validate the local setup.
        Evidence:
```bash
error[E0433]: failed to resolve: maybe a missing crate?
###
note: the `ink_lang` crate is not compatible with current cargo-contract
```

4. 🧮 Unclear Gas & Deposit Behavior in UI
    Issue: When deploying contracts using cargo-contract instantiate, we had to manually tweak gas limits and storage deposits in the Polkadot.js UI. However, the documentation doesn’t mention expected defaults or recommended values.
    Impact: New users may set incorrect values, leading to failed deployments or wasted funds on testnet.
    Suggested Fix: Add documentation of typical gas/storage ranges or provide presets in the UI that align with cargo-contract deployments.
        Evidence:
- cargo-contract instantiate works with default limits
- But Polkadot.js UI deploy fails unless gas is manually increased
- No documentation suggests what "safe defaults" are for common contracts

📌 Summary & Suggestion
    Polkadot’s native smart contract tooling is extremely powerful, especially when using ink! and deploying via cargo-contract. However, the developer experience currently assumes prior Rust and blockchain familiarity.
    We recommend the following:
- Clearer, step-by-step onboarding for beginners
- Synchronization between CLI tooling and Polkadot.js UI
- Improved full-stack developer examples
- A diagnostic tool for environment validation
We hope these insights can help make Polkadot more accessible to the broader Web3 builder community.

---

🛠 How to Contribute

```bash
# 1. Fork this repo
# 2. Create a new branch
git checkout -b feature/your-feature

# 3. Make your changes
# 4. Push and open a PR
git push origin feature/your-feature
```