# Analytics Poisoning via Exposed API Key - Backpack Exchange

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
