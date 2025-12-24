# Random Variable
A random variable is a numerical quantity whose value depends on the </br>
outcome of a random process.

Random variables allow us to:
- assign numbers to uncertain outcomes
- define probabilities mathematically
- describe distributions

Random variables can be:
- discrete (countable values)
- continuous (any value within a range)

# 1. Cumulative Distribution Function (CDF)
## What is CDF?
The cumulative distribution function (CDF) gives us the probability that a </br>
random variable takes a value less than or equal to x.

Formally, it answers:

**P(X ≤ x)**

For continuous distributions, probablity is accumulated </br>
over a range, not a single point.

 ## 2. CDF in plain english
 CDF can be interpreted as a **running total of the probability** from the far left of the </br>
 distribution, to the far right of the distribution.
 - Far left probability → 0
 - Far right probability → 1

 As `x` increases, the CDF **never decreases**.

## 3. Relationship between PDF and CDF
- **PDF** tells how dense the data is that point
-  **CDF** tells how much probaility has accumulated upto that point.

Conceptually:

$$
\text{CDF}(x) = \text{Area under the PDF curve from } -\infty \text{ to } x
$$

The PDF is the **slope** of the CDF.

## 4. Shape of the CDF for a normal distribution
For a normal distribution, the CDF has an **S-shape**.

- Flat at the left tail (no probability accumulation)
- Steep near the mean (rapid accumulation)
- flat again at the right tail
- 
This reflects where data is most concentrated.

## 5. Why proability at a single point is 0?
For continuos distribution:
- P(X=x) = 0
- Probability exists only over intervals

That is why we always compute:
- P(X ≤ x)
- P(a ≤ X ≤ b)
## 6. Z-score and CDF
When we convert a value to `x` to a Z-score:

$$
Z = \frac{x - \mu}{\sigma}
$$

- We are nmapping `x` onto the standard normal distribution
- The **Z-table** is simply a lookup table for the CDF of the standard normal distribution.

## 7. Using the CDF to compute probabilities
Examples:
- P(X ≤ x) → directly from the CDF
- P(X > x) = 1 - CDF(x)
- P(a ≤ X b) = CDF(b)-CDF(a)
## 8. Why the CDF matters in Machine Learning
CDF is used when:
- setting probability thresholds
- interpreting model confidence
- computing risk and tail proabilities
- working with probilistic models

Many ML decisions are based on **cumulative probability**, not point estimates

## 9. Key takeaways
- PDF describes density, not probability
- CDF converts density into probability
- Probability is always an area
- Z-tables are CDF lookups
- CDF is essential for probabilistic reasoning
