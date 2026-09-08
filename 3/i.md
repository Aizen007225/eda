import pandas as pd
df = pd.read_csv("student_data.csv")
df = df.drop_duplicates()
print("Missing Values:")
print(df.isnull().sum())
print("\nDuplicate Records:")
print(df.duplicated().sum())
print("\nCleaned Dataset:")
print(df)
<img width="583" height="732" alt="Screenshot 2026-09-08 232649" src="https://github.com/user-attachments/assets/a54abb1b-de7a-4c8b-8be0-046927447677" />
<img width="551" height="543" alt="image" src="https://github.com/user-attachments/assets/779a731b-ea6b-4d8e-aa0f-40ba7af9bf38" />
