# REF Track Record

Public, outcomes-only track record for the **Reference Exposure Framework (REF)** unlevered weekly strategy, across 21 investor-grade assets from 2006 to present.

---

## What this repository contains

**Historical**: one Excel file per calendar year, 2006–2025.
Example: `REF_yearly_2018.xlsx`

**Current**: one Excel file per week, published after Friday's close, starting 2026-01-02.
Example: `REF_weekly_2026-W16.xlsx` (week ending 2026-04-17, ISO week 16).
Each weekly file carries forward the prior week's ending balance — it is a cumulative year-to-date record, not a single-week snapshot.

**Cross-year summary**: `REF_all_years_summary.xlsx` — one sheet per asset class, showing year-by-year performance plus $100,000 compounded through the full period (REF vs Buy & Hold).

Every Excel file has the same 5-tab structure — one tab per asset class:
1. Broad Index
2. Sector ETFs
3. International
4. Bonds
5. Commodities

---

## Strategy

REF is a **weekly, unlevered, long-or-flat** strategy. Every asset is held at 0% to 100% exposure, never leveraged, never shorted. The strategy moves to cash when its gate logic signals risk-off and re-enters when conditions turn favourable.

- **Starting capital**: $100,000 per asset at period start.
- **Rebalance**: weekly, on Friday close.
- **Costs**: Interactive Brokers Pro commissions ($0.005/share, $1 min) + asset-tier slippage, netted from the NAV.
- **Cash yield**: while flat, the strategy earns the **IBKR Pro rate (Fed Funds − 50 bps)** on uninvested capital, with weekly compounding. This is shown explicitly on every sheet (**REF Cash Yield $** column and **Cash yield contribution** summary line).

The algorithm is **not** disclosed publicly. What is disclosed is the outcomes: returns, drawdowns, time in market, cash yield, and the $ end-value of a $100k investment.

---

## Universe

21 assets, chosen as an **investor-grade baseline** — what a suitability file could justify holding:

| Bucket | Tickers | Count |
|---|---|---|
| **Broad Index** | NDX, SPX | 2 |
| **Sector ETFs** | XLB, XLC, XLE, XLF, XLI, XLK, XLP, XLRE, XLU, XLV, XLY | 11 |
| **Investment-Grade Bonds** | IEF, LQD, TLT | 3 |
| **International** | EEM, VEA | 2 |
| **Commodities** | GLD, SLV, DBC | 3 |

Assets excluded from this published universe because they are speculative, single-issue, or redundant to a cleaner ticker in the same bucket: HYG, FXI, PPLT, PALL, USO, BNO, UGA, UNG, JO, CPER, DBB, WEAT, CORN, SOYB, CANE, REMX, URA, GSG, PDBC.

---

## Buy & Hold comparison

Every REF return is shown side-by-side with a **Buy & Hold** baseline for the same asset, over the same dates. B&H includes **10 bps round-trip cost parity** (entry + exit) so the comparison is fair against REF's own commission/slippage treatment.

---

## Publication cadence

- **Historical 2006–2025**: published once, one file per year.
- **Weekly from 2026**: new file every Friday after close, datestamped by ISO week.
- Files are immutable once published. If an underlying data correction materially changes a prior period's numbers, a dated correction note will be added.

---

## Honest framing

Some things a reader should understand:

- **REF wins most in crisis years, lags in bull years**. 2008, 2011, 2015, 2018, 2022 — big positive alpha. 2009, 2017, 2019, 2021 — negative alpha (strategy stayed in cash or low exposure while B&H ran hot).
- **Drawdown protection is the real product**, not alpha. Across 20 years the worst single-year REF drawdown (equal-weight bucket mean) was under 2%; B&H hit −49% in 2008.
- **Cash yield is a large share of returns when rates are high and gates are closed** (e.g. Bonds 2023–2025). This is shown transparently on every sheet.
- **Past performance is backtested.** Live results will differ.

---

## Contact

Colin Larcombe — <colinlarcombe@gmail.com>
