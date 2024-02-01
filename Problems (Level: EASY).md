Certainly! Here's a list of 15 beginner-level practice problems along with solutions to reinforce understanding of NumPy:

1. **Problem 1: Array Creation**
   - Create a 3x3 NumPy array filled with zeros.

   ```python
   import numpy as np

   zeros_array = np.zeros((3, 3))
   print(zeros_array)
   ```

2. **Problem 2: Array Indexing**
   - Access the element at the second row and third column of a given 2D array.

   ```python
   import numpy as np

   arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
   element = arr[1, 2]
   print(element)
   ```

3. **Problem 3: Array Operations**
   - Perform element-wise addition of two 2x2 NumPy arrays.

   ```python
   import numpy as np

   arr1 = np.array([[1, 2], [3, 4]])
   arr2 = np.array([[5, 6], [7, 8]])
   result = arr1 + arr2
   print(result)
   ```

4. **Problem 4: Array Slicing**
   - Extract the first two elements of a given 1D array.

   ```python
   import numpy as np

   arr = np.array([1, 2, 3, 4, 5])
   sliced_array = arr[:2]
   print(sliced_array)
   ```

5. **Problem 5: Array Reshaping**
   - Reshape a 1D array of 12 elements into a 3x4 array.

   ```python
   import numpy as np

   arr = np.arange(12)
   reshaped_array = arr.reshape(3, 4)
   print(reshaped_array)
   ```

6. **Problem 6: Array Concatenation**
   - Concatenate two 1D arrays horizontally.

   ```python
   import numpy as np

   arr1 = np.array([1, 2, 3])
   arr2 = np.array([4, 5, 6])
   concatenated_array = np.concatenate((arr1, arr2))
   print(concatenated_array)
   ```

7. **Problem 7: Array Transposition**
   - Transpose a given 2D array.

   ```python
   import numpy as np

   arr = np.array([[1, 2], [3, 4], [5, 6]])
   transposed_array = arr.T
   print(transposed_array)
   ```

8. **Problem 8: Array Iteration**
   - Iterate over elements of a 2D array and print each element.

   ```python
   import numpy as np

   arr = np.array([[1, 2], [3, 4]])
   for row in arr:
       for element in row:
           print(element)
   ```

9. **Problem 9: Array Stacking**
   - Stack two 1D arrays vertically.

   ```python
   import numpy as np

   arr1 = np.array([1, 2, 3])
   arr2 = np.array([4, 5, 6])
   stacked_array = np.vstack((arr1, arr2))
   print(stacked_array)
   ```

10. **Problem 10: Array Arithmetic Operations**
    - Multiply each element of a given 2D array by 2.

    ```python
    import numpy as np

    arr = np.array([[1, 2], [3, 4]])
    multiplied_array = arr * 2
    print(multiplied_array)
    ```

11. **Problem 11: Array Comparison**
    - Compare two 1D arrays element-wise and return True for elements that are equal.

    ```python
    import numpy as np

    arr1 = np.array([1, 2, 3])
    arr2 = np.array([1, 4, 3])
    comparison_result = arr1 == arr2
    print(comparison_result)
    ```

12. **Problem 12: Array Broadcasting**
    - Add a scalar value to each element of a given 2D array.

    ```python
    import numpy as np

    arr = np.array([[1, 2], [3, 4]])
    scalar_value = 2
    result_array = arr + scalar_value
    print(result_array)
    ```

13. **Problem 13: Array Mean Calculation**
    - Calculate the mean of elements in a given 1D array.

    ```python
    import numpy as np

    arr = np.array([1, 2, 3, 4, 5])
    mean_value = np.mean(arr)
    print(mean_value)
    ```

14. **Problem 14: Array Max Value Extraction**
    - Find the maximum value in a given 2D array.

    ```python
    import numpy as np

    arr = np.array([[1, 2, 3], [4, 5, 6]])
    max_value = np.max(arr)
    print(max_value)
    ```

15. **Problem 15: Array Sorting**
    - Sort elements of a given 1D array in ascending order.

    ```python
    import numpy as np

    arr = np.array([3, 1, 2, 5, 4])
    sorted_array = np.sort(arr)
    print(sorted_array)
    ```

These practice problems cover a range of fundamental concepts in NumPy and provide opportunities for hands-on learning and skill-building for beginner programmers. Happy coding!
