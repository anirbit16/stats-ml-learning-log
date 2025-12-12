# Variance
## 1. Defination
Variance measures how the spread out the data values are from the mean.</br>
It is the squared differences between each value and mean.</br></br>

In simpler terms,variance tells **how much the data varies**.

## 2. Why Variance exists
Means tells us where the center is, but it doesn't tell us:
- how far the values are from the center
- whether the data points are tightly packed or widely scattered.</br>

Variance solves this problem by estimating the **deviation from mean**.

## 3. How variance is calculated
For a population:
> $$
> \sigma^2 = \frac{1}{N}\sum (x_i - \mu)^2
> $$

where:
- N = total number of data points
- xᵢ = each individual value
- μ = mean of the data
- Σ = summation over all data point </br>

Steps:
1. Find the mean of the data.
2. Subtract the mean from each value (deviation).
3. Square each derivation.
4. Take the average of squared deviations. </br>

Squaring is used because:
- positive and negative deviations shouldn't cancel out each other
- larger deviations shouldn't be penalised more.
## 4. Example
Data: 10, 12, 14, 18 </br>

Mean = 13 </br>

Deviations:
- 10 - 13 = -3
- 12 - 13 = -1
- 14 - 13 =  1
- 18 - 13 =  5 </br>

Squared Deviations:
- 9, 1, 1, 25

> **Variance calculation**
>
> (9 + 1 + 1 + 25) / 4 = **9**

## 5. Example
Variance is used to measure data spread,noise and uncertainty.</br>
It appears directly in loss functions, outlier detections, and regression math.</br>
Understanding variance is essential for understanding model error.

 
