import pandas as pd
df = pd.read_csv("student_data.csv")
# Fill missing numerical values with mean
df["age"] = df["age"].fillna(df["age"].mean())
df["G1"] = df["G1"].fillna(df["G1"].mean())
df["G2"] = df["G2"].fillna(df["G2"].mean())
df["G3"] = df["G3"].fillna(df["G3"].mean())
print(df)
<img width="612" height="646" alt="image" src="https://github.com/user-attachments/assets/226a48ab-6fef-467e-9583-872bafca67ce" />
