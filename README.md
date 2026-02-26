  # Creating-a-Smart-Contract-Repo-on-Base
Use BaseScan (Base equivalent of Etherscan) to verify your contract after deployment.
🛠 Step 1: Set Up Your Development Environment
Install:
Node.js (v18+)
npm or yarn
Git
Then install Hardhat:
Initialize project:
Create a JavaScript project
🛠 Step 2: Add Base Network to Hardhat
Edit hardhat.config.js:
  require("@nomicfoundation/hardhat-toolbox");

module.exports = {
  solidity: "0.8.20",
  networks: {
    base: {
      url: "https://mainnet.base.org",
      accounts: ["YOUR_PRIVATE_KEY"]
    },
    baseGoerli: {
      url: "https://goerli.base.org",
      accounts: ["YOUR_PRIVATE_KEY"]
    }
  }
};
🛠 Step 3: Write Your Smart Contract
