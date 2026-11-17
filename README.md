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
