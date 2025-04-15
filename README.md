# Solana MEV Sandwich Bot – Experimental Simulation

This project is an experimental Python-based simulator of a **sandwich attack bot** tailored for the **Solana blockchain**.

It focuses on modeling the logic behind MEV strategies—specifically **sandwich attacks**—by scanning a stream of simulated pending transactions and identifying patterns that might be exploited by a searcher.

---

## What This Project Does

- Simulates a transaction feed similar to what a Solana searcher would see using tools like Jito’s Shred Stream.
- Identifies high-value swap transactions.
- Logs moments where front-run/back-run logic would be triggered.

---

## Why This Exists

In real-world Solana MEV, latency and transaction ordering are everything.  
This project breaks down the logic to a **pure educational core** for research and prototyping purposes.

---

## Features

- Simple structure using native Python
- No real RPC calls – safe to run anywhere
- Easy to customize swap patterns, token filters, thresholds, etc.

---

## Getting Started

### Requirements
- Python 3.8 or higher

### Run the bot
```bash
python main.py
