# Normal Distribution
## 1. What is normal distribution?
A normal distribution is a continous probability distribution in which data is </br>
symmetrically distributed around a central value.It has a bell-shaped curve and </br> commonly
arises in natural and measurement-driven phenomena.</br>

In a normal distribution:
- Mean = median = mode

## 2. Why is normal distribution important?
Normal distribution because many small independent random effects </br>
combine to produce it. This intuition is often associated with central </br>
limit effect.

It is commonly observed in:
- heights and weights
- measurement noise
- exam scores
- residual (errors) in regression models
  
## 3. Parameters of normal distribution
A normal distribution is defined by 2 parameters:
-  **μ (mu)** → mean, which determines the center of distribution </br>
-  **σ (sigma)** → standard deviation, which determines the spread of deviation

## 4. Shape and symmetry 
- The distribution is perfectly symmetric about mean.
-  Left and right are mirror images </br></br>

   Tails extend indefinetly, but probabilities decrease rapdily way from the mean.</br>
   This symmetry makes the mean and standard deviation reliable descriptive measures.
## 5. Empirical Rule (68-95-99.7 rule)
In a normal distribution:
- Approximately 68% of the data lies within ±1σ of the mean
- Approxinmately 95% of the data lies within the ±2σ of the mean
- Approximately 99.7% of the data lies within the ±3σ </br>

This explains why the values far from the mean are considered rare.
## 6. Standard Normal distribution
The probability distriubtion function (PDF) of a normal distribution is given by:


$$
f(x) = \frac{1}{\sigma \sqrt{2\pi}} \ e^{-\frac{1}{2}\left(\frac{x - \mu}{\sigma}\right)^2}
$$

The PDF describes how **dense** is the data around `x`.</br>
It does not give probability at a single point.

For continuous distributions:
- Probability is obtained by calculating the area under the curve
- Height of the curve represents density not probability.

## Effects on the parameter on the PDF
- Increasing **μ** shifts the curve horizontally
- Increasing **σ** spreads the curve wider and lowers the peak
- Decreasing **σ** makes the curve narrower and increases the peak

The total area under the curve always remains equal to 1.

## 7. Cumulative Distribution Function (CDF)


