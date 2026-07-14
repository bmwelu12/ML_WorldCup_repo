# ML_WorldCup_repo
# WC26 Prediction Model

Predicting the 2026 World Cup semifinals and final — forecast locked before kickoff.

## The claim that matters
Computed **before** either semifinal was played:
**France 57.7% · Argentina 26.3% · England 10.1% · Spain 6.0%** to win it all.

## What's inside
- Static rating model (2022 FAR + FIFA fallback): 64.3% accuracy
- + 2026 form + fitted scale: 71.4% accuracy
- Sequential Elo comparison: 85.7% accuracy
- Logistic regression (leave-one-out CV): 82.1% accuracy
- Player-continuity signal — includes a real error, caught and fixed (see notebook §9)
- Full bracket simulation → semifinal, final, and overall champion probabilities

## Honest limitations
- Tests whether 2022 tactical data predicts 2026 — not current form or new talent (e.g. Lamine Yamal has zero 2022 footprint)
- Small samples throughout (28 matches, 4 teams in the final sim)
- Some parameters fit and graded on the same data — named explicitly, not hidden

