# 🔗 Chainlink VRF v2 Plus – Developer Guide

A complete guide to using **Chainlink VRF v2 Plus** for generating secure, verifiable randomness in smart contracts.

---

## 📌 What is Chainlink VRF?

Chainlink VRF (Verifiable Random Function) is a service that provides **provably fair and tamper-proof randomness** on-chain.

Unlike traditional randomness (which can be manipulated), VRF ensures:

- 🎲 Unpredictability  
- 🔍 Verifiability  
- 🔒 Security against manipulation  

---

## 🚀 What is VRF v2 Plus?

VRF v2 Plus is an improved version of VRF v2 with:

- Flexible payment options (LINK + Native tokens)  
- Better gas efficiency  
- Easier subscription management  
- Enhanced developer experience  

---

## 🤔 Why Use Chainlink VRF?

### ❌ Problem with Randomness in Smart Contracts

Smart contracts are deterministic. That means:

- `block.timestamp` → manipulatable  
- `blockhash` → predictable to miners  

👉 This leads to exploits in games, lotteries, NFTs  

---

### ✅ Solution: Chainlink VRF

- Random number generated off-chain  
- Cryptographic proof provided  
- Verified on-chain before use  

---

## 🧠 Use Cases

- 🎮 Blockchain Games (loot, outcomes)  
- 🎟️ Lotteries & Raffles  
- 🖼️ NFT minting randomness  
- 🎯 Random airdrops  
- 🧪 Fair selection systems  

---

## ⚙️ How It Works (Simple Flow)

1. Contract requests randomness  
2. Chainlink oracle generates random number  
3. Proof is created  
4. Smart contract verifies proof  
5. Random number is returned  

---

## 🛠️ Prerequisites

- Node.js  
- Hardhat / Foundry  
- Solidity basics  
- Wallet with test ETH  
- Chainlink subscription  

---

## 🔧 Installation

```bash
# 🎲 Chainlink VRF v2.5 (VRF v2 Plus) Guide

A practical guide to integrating Chainlink VRF v2 Plus for secure and verifiable randomness in smart contracts.

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/vrf-v2-plus-guide.git
cd vrf-v2-plus-guide
npm install
```

---

## 🔑 Setup

### 1. Create Subscription

- Go to: https://vrf.chain.link  
- Create a subscription  
- Fund it with LINK or native tokens  
- Add your contract as a consumer  

---

### 2. Environment Variables

Create a `.env` file:

```
SEPOLIA_RPC_URL=your_rpc_url
PRIVATE_KEY=your_wallet_private_key
VRF_SUBSCRIPTION_ID=your_subscription_id
VRF_COORDINATOR=coordinator_address
KEY_HASH=gas_lane_key_hash
CALLBACK_GAS_LIMIT=500000
```

---

## 📜 Smart Contract Example

<p align="center">
  <img src="/carbon.png" width="600"/>
</p>

---

## 🚀 Deployment (Hardhat)

```bash
npx hardhat compile
npx hardhat run scripts/deploy.js --network sepolia
```

---

## ▶️ Usage Flow

1. Deploy contract  
2. Add contract as consumer in VRF subscription  
3. Call requestRandomNumber()  
4. Wait for fulfillment  
5. Read randomNumber  

---

## ⚠️ Important Notes

- Set enough callback gas limit  
- Use correct network coordinator  
- Avoid pseudo-random values  
- Ensure contract is added as consumer  

---

## 🌐 Supported Networks

- Sepolia  
- Ethereum Mainnet  
- Polygon  
- Arbitrum  
- Avalanche  

---

## 📈 Best Practices

- Use multiple confirmations  
- Handle failed callbacks  
- Optimize gas usage  
- Store randomness properly  

---

## ❗ Common Errors & Fixes

| Issue | Fix |
|------|-----|
| 403 Push Error | No permission → fork repo |
| Callback failed | Increase gas limit |
| No random number | Add contract as consumer |
| Transaction stuck | Check balance |

---

## 📚 Resources

- https://docs.chain.link/vrf  

---

## 🧠 Final Thought

Randomness in Web3 must be secure. One mistake can make your contract predictable.
