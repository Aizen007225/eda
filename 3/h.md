import pandas as pd
df = pd.read_csv("student_data.csv")
df = df.drop_duplicates()
print(df)
<img width="680" height="660" alt="image" src="https://github.com/user-attachments/assets/eae2e454-b569-4351-9238-a85d0d9c0ea3" />
