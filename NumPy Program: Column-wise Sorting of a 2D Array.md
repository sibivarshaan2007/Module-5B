# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
Add code here
```# Import NumPy
import numpy as np

# Get input from user
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements row-wise:")

# Create empty list
data = []

for i in range(rows):
    row = list(map(int, input().split()))
    data.append(row)

# Convert to NumPy array
arr = np.array(data)

# Sort column-wise (axis = 0)
sorted_arr = np.sort(arr, axis=0)

# Display output
print("\nOriginal Array:")
print(arr)

print("\nColumn-wise Sorted Array:")
print(sorted_arr)
```

## Output
<img width="754" height="765" alt="image" src="https://github.com/user-attachments/assets/becb02e9-457e-44f8-8ea4-1902dbcdbd4e" />


## Result
The given 2D array was successfully sorted column-wise in ascending order using NumPy. Each column of the array was arranged independently from smallest to largest value by using the np.sort() function with axis = 0. The output confirms that column-wise sorting was performed correctly.
