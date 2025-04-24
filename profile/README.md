# Hackathon Semarang - Pharos Builder Base Camp

## Project Description

This project is part of the Pharos Builder Base Camp hackathon, focusing on decentralized finance (DeFi) and perpetual prediction markets. The goal of BeTheNation.Fun is to provide a platform where users can trade country markets based on economic indicators, such as inflation, stock indices, and GDP growth, using perpetual contracts. These contracts never expire, allowing traders to speculate on the long-term economic performance of countries. The platform leverages blockchain technology for secure, transparent, and decentralized trading.

## Key Features

- **Perpetual Prediction Markets**: Trade country-based markets that have no expiration. Open long or short positions and hold them indefinitely.
- **CountryScore**: A unique score generated from key economic indicators like inflation, stock indices, exchange rates, and GDP to drive trading decisions.
- **Leverage**: Use leverage to amplify potential returns on country market trades.
- **Funding Fee Mechanism**: Every 8 hours, a funding fee is charged or paid to maintain a balanced market between long and short positions.
- **Liquidity Provider Rewards**: Liquidity providers (LPs) earn rewards from trading fees and funding fees for supporting market liquidity.

## Hackathon Project Criteria

### Theme Focus:
This project bridges the gap between traditional finance (TradFi) and decentralized finance (DeFi) through perpetual prediction markets based on real-time country economic data. The integration of blockchain technology allows us to provide a transparent and secure platform for data-driven financial speculation.

### Utilizing Pharos Infrastructure:
The project leverages Pharos' modular stack, including L1Core, L1Extension, and L1Base, to provide fast, scalable, and secure market execution. By utilizing Pharos's infrastructure, we ensure high-speed performance and transaction efficiency.

### Viable Business Potential:
BeTheNation.Fun has the potential to be a disruptive platform in the DeFi space, offering an innovative way for users to engage in economic forecasting and trade based on real-world data. It creates new investment opportunities in the form of country market prediction, which appeals to both retail traders and institutional investors.

### Alignment with Available Tracks:
This project fits into the DeFi track, focusing on economic forecasting, perpetual trading, and data-driven financial markets.

### Presentation and Pitch:
Clear and interactive documentation, an engaging demo of the trading platform, and showcasing its scalability, security, and user experience will be key during judging.

## Profit Sharing Mechanism

The platform will implement an automated profit-sharing system via smart contracts. Here's the workflow:

- **Token Issuance**: Countries issue tokens representing their economic performance, linked to CountryScore.
- **Trading**: Users can buy or sell positions (long/short) on country markets based on their predictions of economic indicators.
- **Funding Fees**: Fees are periodically distributed to traders and liquidity providers based on market positions.
- **Automated Profit Distribution**: The platform automatically distributes profits to users according to their trading positions and liquidity contributions, ensuring fairness and transparency.

## References & Inspirations

Some platforms that serve as inspiration for this concept include:

- **Noise.xyz**: A decentralized platform that allows users to trade trends and narratives as assets. By leveraging real-time social data and decentralized finance (DeFi), Noise enables users to speculate on the popularity and attention of various topics or ideas. The platform turns cultural trends into tradable assets, allowing users to engage in markets based on public interest. Noise's integration with Kaito, a mindshare oracle, tracks discussions on platforms like Twitter, and users can speculate on trends with up to 5x leverage. This innovative approach to trend trading has inspired BeTheNation.Fun in its goal to create decentralized prediction markets based on economic indicators and real-time data.

## Project Architecture

### Frontend:
Web interface built with React.js and Tailwind CSS, providing a seamless and responsive experience for trading and viewing economic data.

### Backend:
Node.js with Express to manage API requests, handle user authentication, and interact with smart contracts.

### Smart Contracts:
Developed in Solidity, the smart contracts govern the perpetual prediction markets, ensuring decentralized and automated trading.

## How to Contribute

1. Fork this repository.
2. Create a new branch:
   ```
   git checkout -b feature/your-feature-name
   ```
3. Implement your changes.
4. Push your branch:
   ```
   git push origin feature/your-feature-name
   ```
5. Submit a pull request for review.

We welcome contributions to enhance and expand BeTheNation.Fun!
