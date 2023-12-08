Collaboration to detect sleep states with accelerometer data for the following Kaggle competition:
https://www.kaggle.com/competitions/child-mind-institute-detect-sleep-states/overview

Our solution includes:
1. Creating a solution for re-organizing the parquet files. This was necessary because the default DateTime was unusable, and any native conversion was too memory-intensive (even with Dask).
2. Basic EDA, with comparative plots of the data during sleep/wake sessions.
3. Feature engineering, primarily for chunking the accelerometer data with varying window sizes.
4. Training a single model using Dask-ML.

A whole lot was learned from going over the winning solution:
https://www.kaggle.com/competitions/child-mind-institute-detect-sleep-states/discussion/459715
