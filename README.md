# Texas Daily 4 Payouts & Odds Dataset (2026 Statutory Rules)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Verified Data: 16 TAC 401.316](https://img.shields.io/badge/Verified-16_TAC_§401.316-emerald)](https://texreg.sos.state.tx.us/public/readtac$ext.TacPage?sl=R&app=9&p_dir=&p_rloc=&p_tloc=&p_ploc=&pg=1&p_tac=&ti=16&pt=9&ch=401&rl=316)

A curated, machine-readable JSON dataset containing the complete statutory payout structures, odds, and FIREBALL replacement prize matrices for the **Texas Daily 4** draw game, verified against the official **Texas Administrative Code (16 TAC §401.316)**.

## Dataset Coverage
- **Game Authority**: Texas Lottery Commission
- **Draw Schedule**: 4x Daily (Morning 10:00 AM, Day 12:27 PM, Evening 6:00 PM, Night 10:12 PM CT) • Monday through Saturday (Sunday blackout)
- **Supported Play Types**:
  - Straight (Exact Order)
  - Box (24-Way, 12-Way, 6-Way, 4-Way)
  - Straight/Box (50/50 split play)
  - Combo (All straight permutations)
  - Pairs (Front Pair, Mid Pair, Back Pair)
- **Wager Tiers**: $0.50, $1.00, $2.00, $3.00, $4.00, $5.00
- **Multi-Draw Range**: 1 to 24 consecutive drawings

## Live Interactive Utilities
This dataset powers the free, verified calculation suite on PickPayouts:
- 🎯 **[Texas Daily 4 Payout Calculator](https://pickpayouts.com/texas/daily-4-payout-calculator/)** (Straight, Box, Combo, Pairs & Fireball)
- 🎲 **[Texas Pick 3 Payout Calculator](https://pickpayouts.com/texas/pick-3-payout-calculator/)** (Exact Order, Any Order, Combo & Fireball)
- 💰 **[Texas Cash Five Payout Calculator](https://pickpayouts.com/texas/cash-five-payout-calculator/)** (5/35 Matrix, Match 2 Free Ticket & $25K Top Prize)

The live tool calculates real-time ticket costs, base game prizes, Fireball replacement tiers, and IRS W-2G threshold notices.

## Data Schema & Usage
The primary truth data resides in [`texas-daily-4.json`](./texas-daily-4.json).

```json
{
  "state": "TX",
  "game_name": "Daily 4",
  "statutory_source": "Texas Administrative Code (16 TAC §401.316)",
  "wager_options": [0.5, 1.0, 2.0, 3.0, 4.0, 5.0],
  "retailer_cash_limit": 599.99,
  "w2g_threshold": 600.00
}
