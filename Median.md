# Median
## 1. Defination
Median is the middle value of a dataset after sorting. 

It divides the data into 2 equal halves.
### 1.1 How to find median (using positions)
Let n = number of observations and the data be sorted
- If the number of values is **odd**:
      Median is  the value at the position of **(n+1)/2**
- If the number of values is **even**:
      Median is the average of the values at positions **n/2** and  **(n+1)/2**
## 2. Why it matters

Median represents the **typical value** when the data has extremely high or low values.

It is much less affected by outliers than mean.

##  3. Examples
### 3.1   Odd number of values
Data: 5, 10, 14, 200, 12

Sorted:  5, 10, 12, 14, 200

Median=  **12**,(the middle value)

### 3.2   Even number of values
Data:    10, 100, 12, 14

Sorted:  5, 10, 12, 14, 200

Median=  (12 + 14)/2 = **13**

**In both cases, most values are around 10–15, not 100 or 200.**

##  4. When median wins
Median is much better when the data is **skewed** or has **outliers**.

Typical examples:
 - Salaries
 - House Prices
 - marks when one topper scores extremely high
##  5. In ML
Median is used to fill missing values when the data has outliers or a skewed distribution.

It gives a more **robust central value** compared to the mean.
