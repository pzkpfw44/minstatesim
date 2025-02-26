# Minimal-State Society Simulation

## Overview
This project simulates a **Minimal-State Society**, where individuals engage in **work, trade, and taxation** under a minimal government that only provides essential services like **Security** and a **Legal System**. The goal is to explore how a minimalist government interacts with an economy of self-reliant citizens.

## Features
✅ Citizens with **different ideologies** and productivity levels  
✅ **Work and trade system** that affects individual wealth  
✅ **Taxation system** with a small tax rate (default 10%)  
✅ **State-provided services** when funds allow  
✅ **Randomized economic outcomes** to simulate unpredictability

## Installation
### 1️⃣ Install Python Dependencies
```sh
pip install random
```
(Note: The `random` module is built into Python, so no extra install is needed.)

### 2️⃣ Run the Simulation
```sh
python minimal_state_simulation.py
```

## How It Works
1. Citizens **work and earn income** based on their productivity.
2. They **trade with each other**, exchanging wealth.
3. The **Minimal State** collects a **small tax** and funds essential services.
4. If the state lacks funds, services **may not be provided**.
5. The simulation runs for **10 rounds**, showing economic evolution.

## Example Output
```
--- Round 1 ---
Alice worked and earned 18.24, now has 118.24
Bob worked and earned 25.87, now has 175.87
Charlie worked and earned 29.32, now has 229.32
State collected 52.94 in taxes. State funds: 52.94
State funds too low for services.
```

## Future Enhancements
- 🔹 **Private security & arbitration** instead of a state-run system
- 🔹 **AI-driven decision-making** for citizen interactions
- 🔹 **Advanced economic modeling** for market simulations

---

🛠 **Contributions are welcome!** Fel free to fork the project and suggest improvements. 🚀

