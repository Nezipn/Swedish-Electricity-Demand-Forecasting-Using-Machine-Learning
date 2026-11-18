# Electricity Demand Forecasting in Sweden (SE3)

This project explores hourly electricity demand in Sweden’s SE3 bidding zone.
The goal is to forecast future demand using historical observations.

## Data

The analysis uses hourly electricity demand readings published by
ENTSO-E and distributed by Open Power System Data. Demand is measured
in megawatts (MW), and timestamps are stored in UTC.

## Work completed

- Loaded the SE3 demand series and sorted observations by timestamp.
- Identified 80 missing demand readings across 50,401 rows.
- Explored the time series in a Jupyter notebook.
- [View the SE3 electricity demand notebook](01_explore_se3_demand.ipynb)

## Next step

Build a weekly forecasting baseline using electricity demand from the
same hour seven days earlier, and evaluate its mean absolute error (MAE).

## Key findings (18 nov)

This project analyzes hourly electricity demand in Sweden’s SE3 bidding
zone using Swedish local time. The overall weekday and weekend profiles
use all months and years available in the dataset.

- **Weekday vs. weekend:** The largest difference occurs around 07:00,
  when average weekday demand is about 2,300 MW higher than weekend demand.
- **June vs. November:** From 14:00 to 18:00, average weekday demand fell
  by 4.2% in June and rose by 2.8% in November. Weekend demand rose by
  1.0% in June and 6.6% in November.

The notebook includes both plots and the calculations behind these results.
