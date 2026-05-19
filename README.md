# COVID-19 State Clustering and Virus Spread Analysis

A clustering analysis project that groups US states based on COVID-19 death patterns from January 2020 onward. Uses parametric modeling to characterize each state's virus spread, then applies hierarchical and K-means clustering to identify states with similar epidemic trajectories.

## Features

- Cumulative time series extraction for all 50 US states
- Daily death rate calculations (per million population)
- Parametric modeling using 5 statistical features:
  - Mean daily deaths
  - Standard deviation
  - Median
  - Linear trend coefficient (beta)
  - Autocorrelation coefficient (rho)
- Hierarchical clustering with single linkage
- Hierarchical clustering with complete linkage
- K-means clustering with custom implementation
- Cluster distortion calculation

## Tech Stack

- Python
- Pandas (data manipulation)
- NumPy (numerical computation)
- Johns Hopkins University COVID-19 dataset

## Methodology

1. **Data Processing:** Extract cumulative death time series and compute daily differences
2. **Feature Engineering:** Calculate 5 statistical parameters per state characterizing the virus spread pattern
3. **Normalization:** Min-max scale all features to [0,1] range
4. **Distance Matrix:** Compute Euclidean distances between state feature vectors
5. **Clustering:** Apply three clustering approaches (single linkage, complete linkage, K-means)

## Key Concepts Demonstrated

- Time series analysis and feature engineering
- Hierarchical clustering algorithms (single vs complete linkage)
- K-means clustering from scratch
- Statistical parameter estimation
- Distance metrics (Euclidean)
- Min-max normalization
- Cluster validation through distortion metrics
- Real-world public health data analysis

## Dataset

Time series COVID-19 deaths data for US states from Johns Hopkins University CSSE.
