# StockTrader reports

Published reports from an evidence-driven **paper-trading** research project on Indian stocks (Nifty 500, NSE).
**No real money is traded. Nothing here is investment advice.**

**Site:** https://shanki200801.github.io/stocktrader-reports/

| Page | What it shows |
|---|---|
| [Weekly digest](https://shanki200801.github.io/stocktrader-reports/weekly/index.html) · [all weeks](https://shanki200801.github.io/stocktrader-reports/weekly/all.html) | **Recommended read.** Book performance vs Nifty 500, holdings and their contribution, prediction progress, regime and breadth, VIX and FII/DII, news of the week, and a sortable table of every Nifty 500 stock with its indicators |
| [Monthly report](https://shanki200801.github.io/stocktrader-reports/monthly/index.html) · [all months](https://shanki200801.github.io/stocktrader-reports/monthly/all.html) | Equity curve, the month-end rebalance (buys and sells with reasons and costs), per-stock P&L attribution, costs, closed trades, scorecard and learning update |
| [Daily brief](https://shanki200801.github.io/stocktrader-reports/) | Full daily log: ₹1,00,000 paper book vs Nifty 500, positions history, orders, shadow books, prediction tracker, news flags, data checks, learning state |
| [Archive](https://shanki200801.github.io/stocktrader-reports/archive.html) | Every trading day with its paper NAV, plus links to that day's brief and screen |
| [How to use](https://shanki200801.github.io/stocktrader-reports/how-to-use.html) | Plain-language guide: what each page means, how to judge whether it works, risks |
| [Stock screen](https://shanki200801.github.io/stocktrader-reports/screen/index.html) | Today's top-ranked stocks per candidate method, with every formula input (returns, volatility, z-scores, momentum score, trend, β) and market regime |
| [Evidence v2, survivorship-free](https://shanki200801.github.io/stocktrader-reports/evidence/v2_pit.html) | Backtest of each method on a point-in-time universe built from NSE bhavcopies (2010–2026), net of Indian trading costs |
| [Evidence v2, all methods](https://shanki200801.github.io/stocktrader-reports/evidence/v2_cur.html) | All 85 method variants on today's constituents (survivorship-biased; read with v2_pit) |
| [Evidence v1](https://shanki200801.github.io/stocktrader-reports/evidence/v1.html) | First evidence run, sealed-holdout results and news-bias checks |

## How to read the numbers

- Every number is computed by code from public data (NSE bhavcopies, Yahoo Finance prices, NSE RSS). No figure is written by hand or by an LLM.
- Backtest figures are **historical averages, not forecasts**. The strategy's worst historical drawdown was −67%.
- A method is **CANDIDATE** when it passes every statistical gate except the multiple-testing (Deflated Sharpe) gate. It is paper-traded to collect live evidence. **REJECTED** methods failed after costs. **INSUFFICIENT_DATA** means there is too little history to judge.
- Predictions are recorded before their outcomes exist and are scored when their horizon (63 or 126 trading days) ends.

Every page has the same navigation bar (Today · Screen · Weekly · Monthly · Archive · Evidence · How to use) and works on phones, in light and dark mode. The pages update automatically every weekday around 19:00 IST; weekly digests appear after each week's last trading day and monthly reports after each month end. This repository only holds the generated HTML; the code is private.
