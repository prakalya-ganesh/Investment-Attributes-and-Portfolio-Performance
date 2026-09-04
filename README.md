# Investment Attributes and Portfolio Performance

## An Empirical Analysis of Size, Beta and Value Effects in Indian Equities

This project investigates whether three widely used investment attributes — **market capitalization (size), beta (systematic risk), and P/E ratio (valuation)** — explain differences in portfolio performance in the Indian equity market.

Using a sample of **39 non-financial Nifty constituents** over the **2016–2025** period, stocks are sorted annually into Low, Medium, and High tercile portfolios based on each attribute.

Portfolio performance is evaluated using **annualized returns, volatility, Sharpe ratios, and Jensen's alpha**, while statistical significance is examined through **High-minus-Low t-tests** and **Fama-MacBeth cross-sectional regressions**.

---

## Research Question

**Do size, systematic risk, and valuation characteristics explain differences in risk-adjusted equity returns in the Indian market?**

The study examines three hypotheses:

- **H1 — Size Effect:** Small-cap portfolios generate higher risk-adjusted returns than large-cap portfolios.
- **H2 — Low-Beta Anomaly:** High-beta portfolios do not generate proportionally higher risk-adjusted returns than low-beta portfolios.
- **H3 — Value Effect:** Low P/E (value) portfolios outperform high P/E (growth) portfolios on a risk-adjusted basis.

---

## Investment Attributes

### 1. Size — Market Capitalization

Market capitalization is used as the proxy for firm size.

The study uses:

**ln(Market Capitalization)**

to reduce the influence of extreme values and provide a suitable continuous measure for cross-sectional regression.

Stocks are sorted into Low, Medium, and High market-cap portfolios.

---

### 2. Beta — Systematic Risk

Beta measures the sensitivity of a stock's returns to movements in the overall market.

Beta is estimated using an OLS regression of monthly excess stock returns against monthly excess market returns:

```text
(Ri,t − Rf,t) = α + βi(Rm,t − Rf,t) + εt
