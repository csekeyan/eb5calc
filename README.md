# EB-5 Opportunity Cost Calculator

**Live:** [eb5calc.pages.dev](https://eb5calc.pages.dev/)

A client-side calculator that helps you evaluate the financial trade-off between investing $800K in EB-5 vs waiting for your Green Card via other means (EB-2/EB-3/EB-1A).

## What It Does

Compares two paths side-by-side:

- **Path A (No EB-5):** Your full capital stays in the market, compounding. You wait longer for GC.
- **Path B (EB-5):** $800K is locked in a Regional Center. You get EAD+AP sooner (work and travel freedom), but lose years of market growth on that capital.

## How It Works

### Core Calculation

1. **Path A:** Total capital ($800K + fees) grows at market rate for the full projection period. Side income starts from your non-EB-5 GC date.

2. **Path B:** $800K is locked until the RC returns it. During that time, it earns simple interest (typically 0-2%). Once returned, it goes back into the market. Side income starts earlier (from EAD+AP date). Intangible benefits (peace of mind, travel freedom) are added for the early-freedom window.

### Optional Layers

- **Loan (HELOC/Margin):** If you borrow part of the $800K, your collateral (stocks/home) keeps appreciating. You pay interest, but reduce opportunity cost.
- **Additional Earning Potential:** Earlier work freedom lets you freelance, start a business, or join a better company. Compounds with market returns.
- **Peace of Mind & Freedom:** Assign dollar value to travel freedom (no stamping), stability, and peace of mind. Grows annually.

### Key Variables

| Input | What it affects |
|-------|----------------|
| Market return % | How much you lose by locking $800K (opportunity cost) |
| RC return % | Simple interest earned while locked |
| Money-back date | How long your capital is locked |
| EB-2/3 GC date | How long the "advantage window" is for EB-5 |
| Loan % | Reduces opportunity cost but adds interest expense |
| Side income | Earlier start = more compounding years |
| Intangible growth | Value of freedom compounds as career grows |

### What Tips the Balance

- **EB-5 wins when:** Long gap between EB-5 EAD and EB-2/3 GC (5+ years), moderate market returns (4-6%), side income factored in, or high intangible value assigned.
- **No EB-5 wins when:** Short gap (1-2 years), high market returns (10%+), no side income plans, or purely financial comparison.

## Technical Details

- 100% client-side JavaScript. No server, no database, no tracking.
- Single `index.html` file. No build step.
- Chart.js for visualization.
- Shareable URLs: all inputs encode into query parameters.
- Hosted on Cloudflare Pages (auto-deploys from GitHub).

## Sharing

Click "Copy Shareable Link" to generate a URL with all your settings. Anyone opening it will see your exact scenario pre-filled.

## Disclaimer

This is a decision-support tool, not financial or immigration advice. Every situation is unique. Consult qualified professionals before making investment or immigration decisions.

## Author

Built by [Karthikeyan Gopal](https://www.linkedin.com/in/kgnmzn/)
