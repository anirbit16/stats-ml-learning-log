# Types of Variable
## 1. Categorical
- Nominal
- Ordinal
  ### 1.1 Nominal
  **Defination**:
  There is no specific order between categories

  **Examples**:
  - Gender
  - Blood Group
  - City
  - Color
  
  **Properties**:
  - You cannot rank categories
  - You cannot calculate mean,median,mode
  - Only Counts & Proportions make sense
    
  **In ML**:
   - Encode using One Hot Encoding
   - Label encoding creates fake order — don’t do it
   - Good for tree models, linear models after encoding
  ### 1.2 Ordinal
  **Defination**:
    Categories with order but gaps between levels and not equal

  **Examples**:
  - Size:S, M,L,XL
  - Satisfaction: Low,Medium,High
  - Ranking: Low, Medium, High


  **Properties**:
  - Order exists (L>M)
  - But differnence between S-->M is not equal to M--->L
  - Medium is meaningful,mean is not.
  
  **In ML**
  - Encode using Ordinal Encoding (integers)
  - One Hot is okay if you don’t care about order
  - Don’t treat values as numeric distances in KNN/SVM

 
 
## 2. Numerical (Quantitative)
- Discrete
- Continous
  ### 2.1 Discrete
  **Defination**
  Discrete numbers are countable numbers with no decimals

  **Examples**
  - No. of students: 42
  - Tickets sold:120

  **Properties**
  - Comes from counting
  - Difference is meaningful
  - Mean,median & mode are meaningful
  
  **In ML**
  - Treat as numeric
  - Scaling is optional
  - Works directly with most algorithms
 
  ### 2.2 Continuous
  **Defination**
  Continuous data are measurable values and can include decimals

  **Examples**
  - Height: 170.4 cm
  - Weight: 67.21 kg

  **Properties**
  - Comes from measurement
  - Infinite possible values
  - Mean,median & SD are meaningful
  
  **In ML**
  - Always apply scaling (StandardScaler/MinMax)
  - Distance-based models depend heavily on it
  - Good for linear regression, KNN, SVM
  ## 3. In Machine Learning
  Identifying variable types guides how to encode and scale data. Nominal data require one-hot encoding, ordinal data need ordered encoding, discrete and continuous data are treated as numeric, with continuous variables usually scaled before modeling.
  ## 4. Examples
  Nominal: Class section (A, B, C), blood group

  Ordinal: Grade level (1st, 2nd, 3rd), rating (low, medium, high)

  Discrete: Number of books issued, number of absences

  Continuous: Student height, student weight, annual fees
 



 


