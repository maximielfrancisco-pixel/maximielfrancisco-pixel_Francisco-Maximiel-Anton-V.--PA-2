# maximielfrancisco-pixel_Francisco-Maximiel-Anton-V.--PA-2
------
### 1) Normalization Problem:  - Creating a function for normalization it preprocess data by centering it through mean subtraction and scaling it by dividing with the standard deviation
```python
  # GENERATES RANDOM 5 BY 5 NUMBERS
X = np.random.random((5,5))

# VISUALIZE EQUATION: Z = (X - mean) / σ)
X_normalized = (X - X.mean()) / X.std()
```
##### Step-by-Step Procedure of Functions:
- `np.random.random((5,5))` → Creates a 5x5 array of random floats from 0 up to 1 but less than 1
- `X.mean()` → function that proccess the average value of all numbers inside the array
- `X.std()` → function that computes the standard deviation
- `X-X.mean()` →  shift all numbers so new mean centers 
- `X_normalized` → stores the final formula of the normalized arrary wehre all values are scaled by variable and centered
- `print()` → shows all the data that was stored and needed to be printed
------
### 2) Divisible By 3 Problem - Creates a function that generates a 10×10 array of the squares of the first 100 positive integers, extracts all elements divisible by 3

```python
  # CREATE 10 BY 10 N-DIMENSIONAL ARRAY 
A = np.arange(1, 101).reshape(10, 10) ** 2

# FIND ALL DIVISIBLE BY 3 FROM THE ARRAY
div_by_3 = A[A % 3 == 0]
```
##### Step-by-Step Procedure of Functions:
- `np.arange(1, 101)` → creates array of numbers from 1 to 100 
- `.reshape(10, 10)` → reshapes the array into 10x10 2d array 
- `** 2` → putting this after the arrays formation makes the each element squared
- `A[A % 3 == 0]` → with the use of boolean mask to extract only the elements divisible by 3
- `div_by_3.npy` → stores the condition of divisible by 3
- `print()` → shows all the data that was stored and needed to be printed
------
