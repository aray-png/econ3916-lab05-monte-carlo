# Abigail Ray | Monte Carlo Engine — Probability & Simulation

## Objective
I used random simulation to test probability concepts and estimate financial risk, checking each simulated result against its known theoretical answer.

## Methodology
- Simulated 10,000 fair coin flips and tracked the running share of heads to show how a sample proportion settles toward its true probability as sample size grows
- Simulated 10,000 Monty Hall games under the "always switch" strategy to test whether switching doors actually improves your odds
- Simulated a disease screening test across 100,000 people, using a 1% disease prevalence, 95% sensitivity, and 90% specificity, to see what share of positive test results actually came from sick people
- Simulated 10,000 days of portfolio returns and computed Value at Risk (VaR) and Expected Shortfall (ES) at the 95% and 99% confidence levels for a $1,000,000 portfolio
- Estimated pi at several sample sizes to check that Monte Carlo error shrinks at the rate of 1 divided by the square root of the sample size
- Wrote a function with AI assistance to recompute VaR and ES, then checked its output against my own numbers

## Key Findings
- Switching doors in the Monty Hall simulation won 6,694 out of 10,000 games, close to the theoretical two-thirds win rate
- Only 9.2% of positive disease test results actually came from sick people, showing that even a test with 95% sensitivity gives mostly false alarms when the disease itself is rare
- On the $1,000,000 portfolio, the 95% VaR was $19,494 and the 95% ES was $24,230, meaning losses exceed $19,494 on the worst 5% of days, and average $24,230 on those days specifically
- The pi estimation confirmed that Monte Carlo error shrinks proportionally to 1 divided by the square root of the sample size, meaning four times as many simulations are needed to cut the error in half
