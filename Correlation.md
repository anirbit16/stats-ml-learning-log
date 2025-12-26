 
# Correlation
## 1. What it is
Correlation measures the **strength and direction of a linear**</br>
**relationship** between 2 numerical variables.
- **Direction**:
  - Positive (`r > 0`) → variables increase/decrease together.
  - Negative (`r < 0`) → one increases while the other decreases.
- **Strength** (magnitude of `r`)
   - `|r| = 1` → perfectly linear relationship
   - `|r| ≥ 0.7` → strong linear trend
   - `|r| ≈ 0.3 to 0.6` → moderate trend
   - `|r| < 0.3` → weak linear trend
   - `|r| = 0` → no linear relationship
## 2. Formula (Pearson Correlation Coefficient)
$$
r = cov(X, Y) / (σₓ · σᵧ)
$$

where:
- `cov(X, Y)` = covariance between X and Y
- `σₓ` = standard deviation of X
- `σy` = standard deviation of Y

Expanded view:

$$
r = [ Σ (xᵢ − μₓ)(yᵢ − μᵧ) ] / √[ Σ (xᵢ − μₓ)² · Σ (yᵢ − μᵧ)² ]
$$

## 3.Simple Intuition
It tells how consistently **two variables form a straight-line pattern** without being affected by units.   

## 4. Example
Dataset:
- X = 2, 4, 6, 8
- Y = 1, 2, 3, 4

### Step 1: Compute Means
```
μₓ = (2 + 4 + 6 + 8)/4  = 20/4 = 5
μᵧ = (1 + 2 + 3 + 4)/4 = 10/4 = 2.5

```
### Step 2: Compute standard deviations
```
σₓ = √[ Σ(xᵢ − μₓ)² / N ]
   = √[((2-5)² + (4-5)² + (6-5)² + (8-5)²)/4]
   = √[(9 + 1  + 1 + 9)/4]
   = √[5]
   =  2.236
σᵧ = √[ Σ(yᵢ − μᵧ)² / N ]
   = √[ ((1 − 2.5)² + (2 − 2.5)² + (3 − 2.5)² + (4 − 2.5)²/ 4 ]
   = √[(2.25 + 0.25 + 0.25 + 2.25)/4]
   = √[5/4]
   = √1.25
   =  1.118
```
### Step 3: Compute covariance
```
cov(X, Y) = Σ (xᵢ − μₓ)(yᵢ − μᵧ) / N
          = [(2-5)(1-2.5) + (4-5)(2-2.5) + (6-5)(3-2.5) + (8-5)(4-2.5)]/4
          = [4.5 + 0.5 + 0.5 + 4.5]/4
          = 10/4
          = 2.5
```
### Step 4 — Compute Pearson correlation
```
r = cov(X, Y) / (σₓ * σᵧ)
  = 2.5/(2.236 * 1.118)
  = 2.5/2.5000
  =  1
```
- Both increase together → **positive correlation**
- They form a clean straight-line trend → `r = 1` (perfect linear correlation)

