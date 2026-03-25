# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd

student_data1 = {
    'name': ['Arun', 'Bala', 'Charan'],
    'marks': [85, 90, 78]
}

student_data2 = {
    'name': ['Divya', 'Esha', 'Farhan'],
    'marks': [88, 76, 95]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

new_df = pd.concat([df1, df2], axis=0)

print(new_df)
```
## Output
<img width="634" height="385" alt="image" src="https://github.com/user-attachments/assets/046b458b-e392-44ac-b104-d529b5334665" />


## Result
The program successfully joined two DataFrames along rows using the Pandas concat() function with axis = 0. The combined DataFrame was created and displayed correctly with all rows from both DataFrames.
