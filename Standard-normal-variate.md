# Standard Normal Variate

## Defination
A **Standard Normal Variate** is a transformed value from a normal distribution </br>
that has:
- Mean (μ) = **0**
- Standard deviation (σ) = **1**

## Formula

$$
z = \frac{x - \mu}{\sigma}
$$

Where:
- **X** = original data point
- **μ (mean)** = population mean of original distribution
- **σ (sigma)** = population standard deviation of standard deviation

## Intuition
- SNV converts any normal distribution into a common scale (**μ=0, σ=1**) so values can be compared easily
- The **Z-table** then tells you the probability of a value being below a given Z-score

## Empirical Rule (68–95–99.7 rule)
In a normal distribution:</br>
- 68% of the data lies within ±1σ
- 95% of the data lies within ±2σ
- 99.7% of the data lies within ±3σ

In SNV terms, this becomes:
- P(Z < 1) ≈ 0.84
- P(Z < 2) ≈ 0.977
- P(Z < 3) ≈ 0.9987 </br>

These are right-tail cumulative values from standard normal Z-table.

## ML Applications (1–2 lines)
- Used for **outlier detection** (flag values with |Z| > 3 as extreme).
- Helps in **feature standardization** before linear models so all features behave on the same probability scale.

## Limitations
- Works only if the original data is **approximately normal**.
- If data is **heavily skewed or non-Gaussian**, SNV interpretation becomes unreliable without transformations.
