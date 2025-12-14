# Standard Deviation
## 1. Defination
Standard deviation measures the typical distance from the mean. </br>
It is the square root of the variance and is expressed in **original units** of data.</br>
In simple terms, it means **how far values deviate from the mean**

## 2. Why standard deviation exists?
Variance measures spread but is interpret to spread because it uses **squared units**.</br>
Standard deviation fixes this by converting variance back to **original units**.</br></br>
This makes spread easier to interpret and communicate.

## 3. Relationship with variance
Standard deviation is defined as:

$$
\sigma = \sqrt{\sigma^2}
$$

Where:
- σ² = variance  
- σ = population standard deviation </br>

Variance focuses on mathematical convenience while standard deviation focuses on human interpetability

## 4. Example

From the previous variance example:</br></br>
Variance=9 </br></br>
Standard deviation = √9 = 3 </br></br>
This means data points lie about **3 units from mean**.

## 5. Interpretation
- Small standard deviation → Data is tightly clustered around mean
- Large standard deviation → Data is widely spread out.</br></br>

  Standard deviation gives a sense of consistency V/s variability.
## 6. Key properties
   - Standard deviation is always **non negative**
   - It has the same unit as **original data**
   - It is sensitive to **outliers**.
## 7. In ML
Standard deviation is used for z-score calculation, outlier detection,data normalization.</br>
It helps models learn efficiently by keeping data on comparable scales.</br>
Understanding standard deviation is essential for regression and probabilistic models
 

