Certainly! Here's a list of 15 medium-level practice problems along with solutions and explanations to reinforce understanding of NumPy:

1. **Problem 1: Matrix Multiplication**
   - Perform matrix multiplication between two given 2D arrays.

   ```python
   import numpy as np

   A = np.array([[1, 2], [3, 4]])
   B = np.array([[5, 6], [7, 8]])
   result = np.dot(A, B)
   print(result)
   ```

2. **Problem 2: Array Broadcasting with Different Shapes**
   - Add a 1D array to each column of a 2D array with broadcasting.

   ```python
   import numpy as np

   A = np.array([[1, 2], [3, 4], [5, 6]])
   B = np.array([10, 20])
   result = A + B[:, np.newaxis]
   print(result)
   ```

3. **Problem 3: Array Masking**
   - Replace negative elements in a given array with zero.

   ```python
   import numpy as np

   arr = np.array([-1, 2, -3, 4, -5])
   arr[arr < 0] = 0
   print(arr)
   ```

4. **Problem 4: Array Splitting**
   - Split a given array into multiple sub-arrays along the horizontal axis.

   ```python
   import numpy as np

   arr = np.arange(12).reshape(2, 6)
   result = np.hsplit(arr, 3)
   print(result)
   ```

5. **Problem 5: Reshaping with Unknown Dimension**
   - Reshape a given array into a 3x3 matrix with an unknown dimension.

   ```python
   import numpy as np

   arr = np.arange(9)
   result = arr.reshape(3, -1)
   print(result)
   ```

6. **Problem 6: Array Filtering**
   - Extract even numbers from a given 1D array.

   ```python
   import numpy as np

   arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
   even_numbers = arr[arr % 2 == 0]
   print(even_numbers)
   ```

7. **Problem 7: Array Concatenation with Axis**
   - Concatenate two 2D arrays along the vertical axis.

   ```python
   import numpy as np

   A = np.array([[1, 2], [3, 4]])
   B = np.array([[5, 6], [7, 8]])
   result = np.concatenate((A, B), axis=0)
   print(result)
   ```

8. **Problem 8: Array Sorting with Multiple Keys**
   - Sort a 2D array based on the second column in ascending order.

   ```python
   import numpy as np

   arr = np.array([[3, 2], [1, 4], [5, 6]])
   sorted_array = arr[arr[:, 1].argsort()]
   print(sorted_array)
   ```

9. **Problem 9: Matrix Inversion**
   - Calculate the inverse of a given 2x2 matrix.

   ```python
   import numpy as np

   A = np.array([[4, 7], [2, 6]])
   inverse = np.linalg.inv(A)
   print(inverse)
   ```

10. **Problem 10: Singular Value Decomposition (SVD)**
    - Perform singular value decomposition on a given matrix.

    ```python
    import numpy as np

    A = np.array([[1, 2], [3, 4], [5, 6]])
    U, S, V = np.linalg.svd(A)
    print("U:\n", U)
    print("S:\n", S)
    print("V:\n", V)
    ```

11. **Problem 11: Polynomial Fitting**
    - Fit a polynomial curve to a set of data points using NumPy's polyfit function.

    ```python
    import numpy as np

    x = np.array([0, 1, 2, 3, 4])
    y = np.array([0, 0.8, 0.9, 0.1, -0.8])
    coefficients = np.polyfit(x, y, 3)
    print(coefficients)
    ```

12. **Problem 12: Random Sampling**
    - Generate a random sample from a given 1D array.

    ```python
    import numpy as np

    arr = np.array([1, 2, 3, 4, 5])
    sample = np.random.choice(arr, size=3, replace=False)
    print(sample)
    ```

13. **Problem 13: Array Interpolation**
    - Interpolate missing values in a given 1D array using linear interpolation.

    ```python
    import numpy as np

    arr = np.array([1, np.nan, 3, np.nan, 5])
    interpolated_values = np.interp(np.arange(len(arr)), np.where(~np.isnan(arr))[0], arr[~np.isnan(arr)])
    print(interpolated_values)
    ```

14. **Problem 14: Extract Diagonal Elements**
    - Extract diagonal elements from a given 2D array.

    ```python
    import numpy as np

    arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
    diagonal_elements = np.diag(arr)
    print(diagonal_elements)
    ```

15. **Problem 15: Boolean Indexing with Multiple Conditions**
    - Select elements from a given array that are divisible by 3 and greater than 5.

    ```python
    import numpy as np

    arr = np.arange(10)
    selected_elements = arr[(arr % 3 == 0) & (arr > 5)]
    print(selected_elements)
    ```

These medium-level practice problems cover a broader range of concepts in NumPy and provide opportunities for intermediate programmers to enhance their skills. Happy coding!
