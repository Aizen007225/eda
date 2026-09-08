import pandas as pd
df = pd.read_csv("student_data.csv")
print(df[df.duplicated()])
<img width="605" height="160" alt="image" src="https://github.com/user-attachments/assets/6df98926-0aff-4ca8-aaf7-f5d701b861ed" />
