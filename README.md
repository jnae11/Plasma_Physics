# Plasma_Physics
Exploring the Dynamics of Geomagnetic Activity: A Comprehensive Analysis of Linear, Nonlinear, and Time-Lagged Correlations with Solar Wind Parameters                                                       
EXPLORATORY DATA ANALYSIS WITH THIS DATA FROM OMNI
The data is resampled for various time intervals: hourly (H), daily (D), weekly (W), monthly (M), quarterly (Q), and annually (Y). This step aggregates the data to these specific time frames.
Basic Calculations:

Percentage Change: Calculates the percent change in each column's value compared to the previous period in the time window. This helps identify trends or sudden changes over time.
Logarithmic Transformation: Applies a logarithmic transformation to the data (np.log(1 + value)) to normalize large range values, making trends more apparent and stabilizing variance.
Difference Calculations:

Calculates the difference of the logarithmically transformed values over a specified period. For instance, the 24-hour log difference for hourly data. This highlights the rate of change from one period to another.
Rolling Window Calculations:

Rolling Window Mean and Standard Deviation: Computes the mean and standard deviation over a rolling window (7 days for shorter periods like hourly, daily, and weekly; 4 periods for longer ones like monthly, quarterly, and annually). These metrics smooth out short-term fluctuations and highlight longer-term trends and variability.
Cumulative Sum:

Calculates the cumulative sum of each column over time, providing a sense of the total accumulation of the measured parameter.
