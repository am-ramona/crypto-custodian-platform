<a id="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h1 align="center">CryptoCustodian Platform</h3>

  <p align="center">
A production-style crypto portfolio dashboard creating CryptoCustodian architecture with intuitive UX, scalable Next.js frontend, API-driven Node Backend, real-time data visualization, and testing-first engineering.
    <br />
    <a href="https://github.com/am-ramona/crypto-custodian-portfolio-dashboard"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/am-ramona/crypto-custodian-portfolio-dashboard">View Demo</a>
    &middot;
    <a href="https://github.com/am-ramona/crypto-custodian-portfolio-dashboard/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    &middot;
    <a href="https://github.com/am-ramona/crypto-custodian-portfolio-dashboard/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#why-this-project-matters">Why This Project Matters</a></li>
        <li><a href="#system-architecture">System Architecture</a></li>
        <!-- <li><a href="#my-contribution">My Contribution </a></li> -->
         <li><a href="#web3-analytics-engine">Web3 Analytics Engine</a></li>
        <li><a href="#key-features">Key Features</a></li>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#architecture-overview">Architecture Overview</a></li>
        <li><a href="#architecture-highlights">Architecture Highlights</a></li>
        <li><a href="#example-workflow">Example Workflow</a></li>
        <li><a href="#what-i-learned">What I Learned</a></li>
        <li><a href="#repositories">Repositories</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <!-- <li><a href="#usage">Usage</a></li> -->
    <li><a href="#roadmap">Roadmap</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

![Product Name Screen Shot][product-screenshot] <!-- (https://url.com)  -->
<span>Production-grade Web3 portfolio analytics platform combining a scalable React dashboard, API-driven on-chain analytics, and performance-focused UX for digital asset management.

Built as part of the CryptoCustodian project architecture to demonstrate real-world Web3 system design across frontend, backend, and data layers.</span>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Why This Project Matters

Managing digital assets requires clarity, performance, and trust.

This platform shows how to build a real production-style Web3 analytics system that:

* Aggregates on-chain data
* Computes portfolio intelligence
* Presents insights through fast, intuitive dashboards
* Maintains scalability and clean architecture

It reflects the kind of systems used by DAO treasuries, custodians, and Web3 asset platforms.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### System Architecture

This project is organized into three repositories:

* crypto-custodian-dashboard → Next.js React dashboard
* crypto-custodian-api → Node.js analytics API
* crypto-custodian-platform → Architecture, documentation, orchestration

Each repo demonstrates a different layer of a production Web3 system.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Web3 Analytics Engine

On the API layer, I implemented a portfolio analytics pipeline that fetches on-chain data from Etherscan APIs and computes structured portfolio insights used by the dashboard UI.

##### Key analytics modules

🔹 <strong>1. Portfolio Calculation</strong>

Transforms raw transaction history into a normalized portfolio summary.

Returns:

* ```tokenName```
* ```tokenSymbol```
* ```amount```

Used for wallet summaries and treasury dashboards.

Purpose:

✔ Build accurate wallet holdings view
✔ Support multi-token dashboards
✔ Normalize heterogeneous on-chain data


🔹 <strong>2. Asset Allocation Engine</strong>

Calculates token distribution across the portfolio.

Returns:

* ```tokenSymbol```
* ```allocationPercentage```
* 
Used for diversification analysis and risk visualization.

Purpose:

✔ Visualize diversification
✔ Support DAO treasury decisions
✔ Power allocation charts in frontend

🔹 <strong>3. Performance Metrics Engine</strong>

Computes activity and efficiency metrics:
Aggregates transaction-level analytics into portfolio performance insights.

Returns:

* ```transactionCount```
* ```totalGasUsed```
* ```totalEtherTransferred```
* ```tokenTransfers```
* ```averageGasPrice```
* ```averageTransactionValue```
* ```maxGasUsed```
* ```minGasUsed```
* ```errorRate```

Used for treasury performance monitoring and cost optimization.

Purpose:

✔ Measure wallet activity
✔ Analyze gas efficiency
✔ Detect abnormal transaction behavior
✔ Provide performance dashboards

👉 Full implementation details in <strong>crypto-custodian-api</strong> repo.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ### Key Features

<ul>
<li>AI-generated NFT assets using Pollinations AI</li>
<li>Smart contract minting with Solidity + Hardhat</li>
<li>Wallet interaction via Ethers.js</li>
<li>IPFS storage via Pinata</li>
<li>Full-stack architecture (frontend + backend + smart contracts)</li>
<li>Responsive UI with loading/error states</li>
<li>Scalable minting workflow with clear user feedback</li>
</ul>

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->

### Built With

#### Frontend

* Next.js
* React
* TypeScript
* Chart.js
* TailwindCSS
* Jest

#### Backend

* Node.js
* Express
* Sequelize
* SQLite / MySQL
* Supertest

#### Web3

* Etherscan API
* Ethereum transaction analytics

<!-- * [![React][React.js]][React-url]
* [![Javascript][javascript.com]][Javascript-url]
* [![Web3 UX flows][web3uxflows.js]][Web3UXFlows-url]
* [![Solidity][Soliditylang.org]][Solidity-url]
* [![Hardhat][Hardhat.org]][Hardhat-url]
* [![Ethers.js][Ethers.io]][Ethers-url]
* [![Pinata][Pinata.cloud]][Pinata-url]
* [![Pollinations AI][Pollinations.ai]][Pollinations-url]
* [![Node][Node.js]][Node-url] -->

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Architecture Overview

![Product Architecture Screen Shot][architecture-screenshot]

* Frontend → Smart Contract interaction
* Backend → IPFS + AI generation
* Wallet → Transaction signing

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Architecture Highlights
  
* Modular full-stack design
* Clear separation of concerns
* API-driven frontend
* Scalable analytics layer
* Performance-first UI
* Production-ready engineering practices  

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Example Workflow

1. Fetch wallet transactions via Etherscan API
2. Compute portfolio analytics
3. Store processed data
4. Serve insights via REST API
5. Render dashboard charts and allocation views

This mirrors real Web3 custody platform pipelines.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### What I Learned

* Designing Web3 analytics pipelines
* Translating on-chain data into user insights
* Performance-first frontend dashboards
* Clean API architecture for Web3 platforms
* Balancing UX clarity with complex blockchain data

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

* Install [NodeJS](https://nodejs.org/en/)
* Install [npm](https://nodejs.org/en/)
* Install [Git](https://git-scm.com/)

### Installation

1. Clone/Download and run each repository
   

   ```
   git clone https://github.com/am-ramona/crypto-custodian-dashboard
   git clone https://github.com/am-ramona/crypto-custodian-api
   ```
Follow each repo’s README.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE -->
<!-- ## Usage

This space is to show useful examples of how a project can be used. Additional screenshots, code examples, demos and more resources work well in this space. 

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->

<!-- ROADMAP -->
### Repositories

* Dashboard → ```crypto-custodian-dashboard```
* API → ```crypto-custodian-api```
* Architecture → ```crypto-custodian-platform```

<p align="right">(<a href="#readme-top">back to top</a>)</p>
   
## Roadmap

<!-- - [x] Add Changelog -->
* [ ] Multi-chain analytics
* [ ] Real-time websocket updates
* [ ] Advanced risk metrics
* [ ] Gas optimization recommendations
* [ ] Wallet clustering analysis

See the [open issues](https://github.com/am-ramona/crypto-custodian-portfolio-dashboard/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
<!-- ## License

Distributed under the Unlicense License. See `LICENSE.txt` for more information.

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[product-screenshot]: images/crypto-custodian-dashboard.png
[architecture-screenshot]: src/assets/images/Miro_design-architecture.png

[React.js]: https://img.shields.io/badge/React%20-%20Frontend%20Framework-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[web3uxflows.js]: https://img.shields.io/badge/UX-8A2BE2?style=for-the-badge&logo=ux&logoColor=61DAFB&label=Web3%20UX%20flows
[Web3UXFlows-url]: https://coinbound.io/web3-ux-design-guide/
[Javascript.com]: https://img.shields.io/badge/JavaScript-React%20and%20Testing-F7DF1E?style=for-the-badge&logo=javascript
[Javascript-url]: https://javascript.com
[Hardhat.org]: https://img.shields.io/badge/Hardhat%20-%20Development%20Framework-8C8C8C?style=for-the-badge&logo=hardhat
[hardhat-url]: https://hardhat.org/
[Ethers.io]:  https://img.shields.io/badge/Ethers.js%20-%20Blockchain%20Interaction-2B2B2B?style=for-the-badge&logo=ethers
[Ethers-url]: https://docs.ethers.io/v5/
[Soliditylang.org]: https://img.shields.io/badge/Solidity%20-%20Smart%20Contracts-3DDC84?style=for-the-badge&logo=solidity
[Solidity-url]: https://soliditylang.org/
[Pinata.cloud]:  https://img.shields.io/badge/Pinata%20-%20IPFS-4A90E2?style=for-the-badge&logo=ipfs
[Pinata-url]: https://pinata.cloud/
[Pollinations.ai]: https://img.shields.io/badge/Pollinations%20AI%20-%20AI%20Models-6A5ACD?style=for-the-badge&logo=ai
[Pollinations-url]: https://pollinations.ai/
[Node.js]: https://img.shields.io/badge/Node-Server-58a846?style=for-the-badge&logo=node.js&logoColor=58a846
[Node-url]: https://nodejs.org/
