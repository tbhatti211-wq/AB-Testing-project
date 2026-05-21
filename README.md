# Pricing A/B Test Analysis

Analysis of a pricing experiment run by Company XYZ to determine whether 
raising software price from $39 to $59 would increase revenue. 66% of users 
saw the original price, 33% saw the higher price.

## Objectives
- Recommend the optimal price point ($39 vs $59) based on revenue, not just conversion
- Identify user segments with distinct price sensitivity (by source, device, OS, geography)
- Evaluate whether the test ran long enough to draw reliable conclusions

## Approach
- Data validation and randomization checks (sample ratio, group balance)
- Conversion rate and revenue-per-user comparison with statistical testing
- Segment-level analysis across marketing channel, device, OS, and country
- Time-series review of conversion stability and novelty effects

## Tech Stack
Python · pandas · NumPy · SciPy · statsmodels · matplotlib · seaborn

## Key Questions Answered
1. Which price drives higher revenue per user?
2. Are there segments where the higher price actually wins?
3. Was the test duration sufficient, and when should it have been concluded?

## Dataset
Two tables: user-level test assignments (price shown, conversion outcome, 
traffic source, device, OS) joined with user geography (city, country, lat/long).
