## Quick Introduction

## Problem Statement
- Objective:
    - At a given time and location in NYC we want to predict the number of pickups in a 10 minutes interval.
- Constraints:
    - Latency, we expect the ML model to give us the result in a few seconds. Imagine a senario where you are a cab driver in NYC, you wouldn't want to wait 5 minutes to see the number of pickups in the region surrounding your current location.
    - Interpretability is not very important.
    - Relative errors:
      Example: 
        r1 -> 5:40 - 5:50 -> 100 pick ups, actual -> 102 -> error -> 2%
        r2 -> 5:40 - 5:50 -> 10 pick ups, actual -> 12 -> error -> 20%
        we care about the % error not the absolute error.
 
## Approach
Our problem is a regression task with temporal data, essentially time-series prediction.

**Data Cleaning:**

**Performace Metrics:**
  - Mean Absolute Percentage Error(MAPE)
  - Mean Squared Error(MSE)
## Results 
- Used dask to handle massive datasets in this project.

## Interesting Plots
