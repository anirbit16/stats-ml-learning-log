# Outlier Detection

## 1. Outlier Detection
An outlier is data point that significantly deviates from the majority of the observations.</br>
It may represent a noise,error or a rare but valid event.

## 2. Why outlier detection matters
Outliers can:
- skew mean and standard deviation.</br>
- distort regression models
- affect distance based algorithms
- reduce model reliability

Detecting outliers is a potential step in data cleaning.

## 3. Z-score method
### Idea
A data point is considered an outlier if it lies many standard deviations away from the mean.</br>
### Formula
$$
Z = \frac{x - \mu}{\sigma}
$$

𝑍: the z-score (standardized value)

𝑥: the observed data value

𝜇: the mean (average) of the population or dataset

𝜎: the standard deviation of the population


### Rule of thumb
- |Z| ≥ 3 → potential outlier </br>

### Example
Mean = 50

Standard Deviaition = 10

Value = 85

Z = (85-50)/10 = 3.5

### Limitations
- Assumes data is normally distributed 
- Performs poorly on skewed data

## 4. IQR (Inter-Quartile Range method)

### Idea
IQR focused on the middle 50% of the data is robust to skewness.</br>

### Steps
1. Compute Q1 (25th percentile)
2. Compute Q3 (75th perecentile)
3. IQR = Q3 - Q1

### Fences
- Lower bound = Q1 - 1.5 x IQR
- Upper bound = Q3 + 1.5 x IQR

Any values outside this bounds is an outlier

### Why IQR works well
- Does not assume normal distribution
- Resistant to extreme values
- Commpnly used with boxplots
  
## 5. Z-score vs IQR
| Method | Best used when |
|------|---------------|
| Z-score | Data is roughly normal |
| IQR | Data is skewed or unknown |


## 6. In ML
Outlier detection improves model stability and performance. </br>
Outliers maybe removed, capped or treated separetly depending on the problem.</br>
Understanding outliers helps preventing misleading predictions.
















