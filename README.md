# series_to_supervised
Simple function to turn a time series into an ML ready dataset.

Originally sourced from:
https://machinelearningmastery.com/convert-time-series-supervised-learning-problem-python/

---

This Python function named takes a univariate or multivariate time series and frames it as a supervised learning dataset.

The function takes four arguments:
* __data__: Sequence of observations as a list or 2D NumPy array. Required.
* __n_in__: Number of lag observations as input (X). Values may be between [1..len(data)] Optional. Defaults to 1.
* __n_out__: Number of observations as output (y). Values may be between [0..len(data)-1]. Optional. Defaults to 1.
* __dropnan__: Boolean whether or not to drop rows with NaN values. Optional. Defaults to True.

The function returns a single value:
* __return__: Pandas DataFrame of series framed for supervised learning.
