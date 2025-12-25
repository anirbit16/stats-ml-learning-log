# Covarariance
## 1. Defination
Covariance tells us **whether two numerical values move together** and in what **direction**.
- Positive value → both increase/decrease together
- Negative value → one increases while the other decreases
- Value magntitude depends on units, so it's **not standardized**
## 2. Formula
$$
σ(X, Y) = (1 / N) Σ (xᵢ − μₓ)(yᵢ − μᵧ)
$$

Where:
- `σ(X, Y)` = Covariance between X and Y
- `N` = Number of paired data points
- `xᵢ`= Individual values of variable X
- `yᵢ`= Individual values of variable Y
## 3. Intuition
It measures the direction of **direction of joint variation**,not strength.

## 4. Quick Example
Heights (X): 150, 160, 170, 180 → `μₓ=165`

Heights (Y) : 50, 60, 70, 80 → `μᵧ=65`


$$
σ(X, Y) = (1 / 4) Σ (xᵢ − 165)(yᵢ − 65)
$$

Result will be positive, meaning height and weight move together.

## 5. In ML
Covarariance helps you check **check if features trend together** before scaling.

## 6. Limitations
- Not scaled to a fixed range
- Not comparable accross different unit scales
- Direction only,no strength measure.
