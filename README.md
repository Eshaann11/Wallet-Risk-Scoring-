# Compound Wallet Risk Scoring Pipeline

This repository contains a Python-based scoring pipeline designed to evaluate DeFi wallets interacting with the **Compound V2/V3 lending protocol**. The model assigns a **risk score (0–1000)** to each wallet based on historical lending and borrowing behavior.

---

## 🚀 Project Overview

Using wallet addresses as input, the pipeline:
1. Retrieves transaction activity from the Compound protocol
2. Engineers wallet-level behavioral and collateral features
3. Calculates a composite risk score using weighted metrics
4. Flags behavioral outliers using an Isolation Forest
5. Outputs final scores to a clean CSV file for downstream analysis

---

## 📂 Project Structure

```bash
.
├── Wallet id.xlsx              # Input file containing wallet addresses
├── score_pipeline.py           # Main scoring script
├── wallet_risk_scores.csv      # Output file with wallet_id and score
└── README.md                   # Documentation and setup guide
