import pandas as pd
df = pd.read_csv("student_data.csv")
# Fill missing categorical values with mode
df["sex"] = df["sex"].fillna(df["sex"].mode()[0])
df["school"] = df["school"].fillna(df["school"].mode()[0])
print(df)
<img width="646" height="656" alt="image" src="https://github.com/user-attachments/assets/75f5d0b9-9d54-43e8-8a57-863580f33151" />
