# DSAC-Project: Fourth Down Decision-Making in the NFL

**Team:** Grady, Grant, Will, Robert, Max

## Question
For every 4th down situation (yard line + yards to go), which call
maximizes expected points: going for it, kicking a field goal, or punting?
The end product is a decision chart coaches could actually use.

## Data
NFL play-by-play data from nflverse. Seasons: TBD.

## Approach
For each situation, estimate the expected points (EP) of each option:
- **Go for it:** P(convert) × EP if converted + P(fail) × EP if turnover on downs
- **Field goal:** P(make) × 3 + P(miss) × EP for opponent at the spot
- **Punt:** EP for opponent after an average net punt

Pick the option with the highest EP, then plot it as a grid
(yard line on one axis, yards to go on the other).
