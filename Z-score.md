# Z-Score
## 1. Defination
Z-score measures how much standard deviations is away from the mean.</br>
It tells whether the value is typical or unusual in a dataset.

## 2. Formula
Z-score is defined as:
>
$$
Z = \frac{x - \mu}{\sigma}
$$

WHERE:
- x = the individual data point
- μ (mu) = the mean of the dataset
- σ (sigma) = the standard deviation of the dataset

## 3. Meaning of Z-score
- Z = 0 → value is exactly at the mean.
- Z > 0 → value is above the mean.
- Z < 0 → value is above the mean.</br>

The magnitude of Z tells how unusual the value is.</br>

## 4. Example
Mean (μ) = 50 </br></br>
Standard Deviation (σ) = 10  </br></br>
Value (x) = 70  </br></br>
Z = (70-50)/10 = **2** </br>

This means the value is **2 standard deviations above the mean**.</br>

## 5. Interpretation
- |Z| < 1 → Very common value
- 1 ≤ |Z| ≤ 2  → somewhat unusual
- |Z| ≥ 3 very rare (potential outlier)</br>

## 6. In ML
Z-score is used for feature standardization and outlier detection.</br>
It helps models converge by putting features on a comparable scale.</br>
Z-score normalization is common in regression and distance-based algorithms.


