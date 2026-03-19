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


 ![img](https://github.com/SumanMoharana24/Path-to-web3/blob/2d3a191c8b4eb6ad6cc1e07aba45656f5d256d9a/Chainlink_Randomness/assets/carbon%20(1).png)


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
