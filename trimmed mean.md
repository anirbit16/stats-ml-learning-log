# Trimmed Mean
## 1. Defination
Trimmed mean is the mean calculated after removing a fixed percentage of the smallest and largest values from the dataset.</br>
It reduces the influence of extreme values (outliers).</br>

## 2. Why it matters?
Mean is senstitive to outliers.</br>
Trimmed mean keeps the simplicity while becoming more robust to extreme values.</br> 

## 3. How it works
    1. Sort the data
    2. Remove the lowest and highest k% values
    3. Compute the mean of the remaining values
## 4. Example
Data: 2, 3, 4, 5, 100</br>
Trim: Remove 20% from each end (2 and 100) → 3, 4, 5   </br></br>

Trimmed mean: (3 + 4 + 5)/3 = **4** </br></br>

## 5. In ML
Trimmed mean helps summarizing noisy data where a few noisy values can distort the average.</br>
It can be useful in robust preprocessing or exploratory analysis. 

