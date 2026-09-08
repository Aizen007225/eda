import pandas as pd
# Load the student dataset
df = pd.read_csv("student_data.csv")
# Equal-Width Binning
df["Age_EqualWidth"] = pd.cut(
df["age"],
bins=4,
labels=["Young", "Adult", "Middle Age", "Older"]
)
# Equal-Frequency Binning
df["Age_EqualFrequency"] = pd.qcut(
df["age"],
q=4,
labels=["Young", "Adult", "Middle Age", "Older"]
)
# Display the result
print(df[[
"age",
"Age_EqualWidth",
"Age_EqualFrequency"
]])
<img width="427" height="290" alt="image" src="https://github.com/user-attachments/assets/5850a4e7-5abf-4f20-a232-1ebd8e3d4a4d" />
