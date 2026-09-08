import pandas as pd
df = pd.read_csv("student_data.csv")
print(df[df.duplicated()])
<img width="616" height="110" alt="image" src="https://github.com/user-attachments/assets/75c46bb0-866a-4f23-80d6-51851c26be40" />
