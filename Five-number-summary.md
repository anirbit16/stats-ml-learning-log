# Five Number Summary

## Defination
The five-number-summary is a statistical representation of a dataset using 5 key values: </br>
- **Minimum**: Smallest value in the dataset
- **First quartile (Q1)**: 25th percentile (value below which 25% of data lies)
- **Median (Q2)**: 50th percentile (middle value after sorting)
- **Third Quartile (Q3)**:75th percentile (below which 75% of data lies)
- **Maximum (max)**:Largest value in the data
## Intuition 
- It gives a quick sense of **spread and range** of the data
- The quartiles **Q1 and Q3** describe the **midddle 50% of the values** reducing sensitivity to extreme outliers
- Unlike the mean, it helps us to understand data behaviour even  when the dataset  </br> contains **outliers**  or is skewed
## How to calulate
1. Sort the data in ascending order.</br>
2. Identify the minimum and maximum correctly.</br>
3. Compute quartiles
   - If `n` is **odd**

     ```
      Median = x[(n+1) / 2]

      Q1 = Median of left half

      Q2 = Median of right half
 
      ```
   - If `n` is **even**
       ```
       Median = (x[n/2] + x[n/2 + 1])/2

       Q1 = median of first n/2 values

       Q2 =  median of last n/2 values

    ## Example
    Dataset:   `42, 15, 7, 49, 39, 43, 36, 47, 40, 41`
   
    Sorted : `7, 15, 36, 39, 40, 41, 42, 43, 47, 49`
   ```
    Min = 7

    Median(Q2) =  (40+41)/2 = 40.5

    Q1 = median of [7, 15, 36, 39, 40] = 36

    Q3 = median of [41, 42, 43, 47, 49] = 43

    Max = 49
   ```
    ## Use in Machine Learning (applied scenarios)
   - Frequently used during **Exploratory Data Analysis (EDA)** to summarize feature distributions.
   - Forms the basis of **boxplots**, which visually show quartiles and outliers.
   - Helps choose robust strategies like using **median or IQR** instead of mean-based </br>
     approaches when features contain extreme values.
      
