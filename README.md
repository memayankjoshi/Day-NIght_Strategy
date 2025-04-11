# Day and Night Trading Strategy
## ✨ What is the Day & Night Strategy?

The "Day & Night" strategy comes from a research paper that found something surprising:

> **Most of the gains in the U.S. stock market happen overnight, not during the day.**

In other words:
- When the market is **closed** (from the previous day's close to the next day's open), stocks tend to go **up**.
- When the market is **open** (from open to close during the trading day), returns are usually **flat or even negative**.

This is the opposite of what many people expect. 

This strategy looks to **capture those overnight gains** by:
- Buying a stock at the **market close** (e.g., 4:00 PM)
- Selling it at the **next day’s open** (e.g., 9:30 AM)

---

## 🚀 Why Does the Strategy Work?

The exact reason isn’t fully clear, but here are a few ideas:

- **Good news** often comes out after markets close (e.g., earnings announcements), causing stocks to gap up the next morning.
- **Investors can't react overnight**, so prices adjust suddenly at the open.
- **Lower liquidity** overnight may lead to price jumps.
- The **risk premium** might be paid to those who hold stocks during off-hours.

Surprisingly, even though the **daytime has more trading volume and volatility**, it doesn't lead to better returns.

---

## 🌌 What Strategy Did I Implement?

I tested this strategy on **Apple (AAPL)** and **Amazon (AMZN)** stocks using Python and historical data.

### Steps:
1. Pulled historical stock data from Yahoo Finance.
2. Calculated:
   - **Night Return**: (Next day's Open / Previous day's Close) - 1
   - **Day Return**: (Close / Open) - 1
3. Created a slider to adjust the weight (e.g., 50% Apple, 50% Amazon or any mix).
4. Simulated and plotted the **cumulative returns** of both strategies.
5. Calculated **Sharpe Ratio** to compare risk-adjusted performance.

---

## ⚖️ Pros and Cons

### Pros:
- Simple and rules-based
- Historically strong returns
- Easily applicable to many stocks or ETFs

### Cons:
- Doesn’t work well for all stocks
- Can be affected by **slippage**, **taxes**, and **overnight news risks**
- Requires holding positions overnight (some traders avoid this)

---

## 🙋 How Can It Be Improved?
- Combine this with **volatility filters** or **volume confirmation**
- Use it only during **earnings seasons** or specific days
- Apply **machine learning** to predict strong overnight candidates
- Add **stop-loss rules** or pair with hedges

---

## 📊 Performance Summary
- **Night strategy (AAPL + AMZN)** significantly outperformed the **day strategy**.
- Sharpe Ratio for night strategy was higher, meaning **better return per unit of risk**.
- Results matched the original paper: **overnight = alpha**!

---

## 📅 Similar Strategies
- **Weekend Effect**: Returns from Friday close to Monday open
- **Earnings Drift**: Buying after positive earnings surprises
- **Opening Range Breakout**: Using first 30 mins to set entry/exit

---

## 🚀 Summary
This strategy shows that sometimes, **doing nothing overnight** beats trading all day. It challenges traditional thinking and shows the value of digging into data.

If you’re curious about trading strategies, backtesting, or market anomalies — this is a great place to start!

---

Thanks for reading! Feel free to check the code and visuals in the repo.
