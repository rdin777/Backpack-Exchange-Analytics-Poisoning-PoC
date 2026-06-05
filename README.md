# Analytics Poisoning via Exposed API Key - Backpack Exchange

*If this research helped you, please consider giving it a ⭐ Star.*


## 🚀 Stay Updated
Found this research useful?
* **Star ⭐** this repo to keep track of it.
* **Follow me** on GitHub for more DeFi security research.
* **Fork** it if you want to run your own experiments.

### ☕ Support the Research
If you appreciate the work and want to support further security research:

<img src="456.PNG" alt="Donate QR" width="200"/>

**Wallet Address (ETH/EVM):** 0xBDDD7973D0DE27B715A4A5cbdb87d0DF78757b3A 


This repository contains a PoC for **Business Logic Corruption** identified on Backpack Exchange. The vulnerability stems from exposing production `Amplitude` API keys on the client-side.

## Business Impact
An attacker can use this key to:
1. **Pollute Analytics Data:** Inject thousands of fake "Deposit" or "Trade" events.
2. **Sabotage Marketing:** Destroy the integrity of Conversion Rates, CAC, and LTV metrics.
3. **Internal Chaos:** Lead the product team to make wrong decisions based on corrupted data dashboards.

## Usage
```bash
pip install requests
python exploit_amplitude.py
