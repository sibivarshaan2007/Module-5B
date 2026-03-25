# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
Add code here
```
import pandas as pd
import numpy as np

exam_data = {
    'name': ['Ankit', 'Riya', 'Karan', 'Sneha', 'Rahul'],
    'score': [85, 90, 78, 92, 88],
    'attempts': [1, 1, 2, 1, 2],
    'qualify': ['Yes', 'Yes', 'No', 'Yes', 'Yes']
}

labels = ['a', 'b', 'c', 'd', 'e']

df = pd.DataFrame(exam_data, index=labels)

print(df)
```

## Output
<img width="549" height="337" alt="image" src="https://github.com/user-attachments/assets/7ca2e40b-bde5-49b6-88e7-81aa065be1b4" />


## Result
The program successfully created a DataFrame using the given dictionary and applied custom index labels to the rows using Pandas. The DataFrame was displayed with the specified labels and data correctly formatted.
