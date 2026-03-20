**ATP Tennis Betting Model**

A quantitative sports betting model built in Python that uses Elo ratings and historical bookmaker odds to identify mispriced matches in the ATP tennis tour.

**How It Works**

The model builds a dynamic Elo rating system trained on 70,000+ ATP matches from 2000–2024. For each match, it calculates the implied win probability from Bet365 odds and compares it against the Elo-derived probability. When the model's estimate exceeds the bookmaker's implied probability by more than 20%, a value bet is identified.

**Strategy**

This is a value betting strategy — the goal is not to predict winners, but to find matches where the bookmaker has underpriced a player relative to their true probability of winning. Over time, consistently finding these edges produces positive expected value.

**Results (Backtested 2020–2024)**

Bets placed: 106
ROI: 34.72%
Stake: $20 flat per bet
Total profit: $736
Edge threshold: 20%

A Monte Carlo simulation of 1,000 paths over 250 bets confirms positive expected value with realistic downside scenarios.

**Tech Stack**
Python, Pandas, NumPy, Matplotlib

**Data: tennis_atp by Jeff Sackmann, historical odds from tennis-data.co.uk**
