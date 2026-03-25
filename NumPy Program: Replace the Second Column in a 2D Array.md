# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

Add code here
```
import numpy as np

rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements row-wise:")
data = []
for i in range(rows):
    row = list(map(int, input().split()))
    data.append(row)

arr = np.array(data)

print("Enter elements of new column:")
new_col = list(map(int, input().split()))

new_col = np.array(new_col).reshape(rows, 1)

arr_deleted = np.delete(arr, 1, axis=1)

updated_arr = np.insert(arr_deleted, 1, new_col, axis=1)

print("\nOriginal Array:")
print(arr)

print("\nUpdated Array (Second column replaced):")
print(updated_arr)
```

## Output
<img width="622" height="293" alt="image" src="https://github.com/user-attachments/assets/a4158715-f4c8-4b80-8b4a-5bf597ebed97" />


## Result
code executed well
