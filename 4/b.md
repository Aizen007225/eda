import pandas as pd
# Load the student dataset
df = pd.read_csv("student_data.csv")
# Rename columns
df.rename(columns={
'Medu': 'Mother_Education',
'Fedu': 'Father_Education',
'Mjob': 'Mother_Job',
'Fjob': 'Father_Job',
'G1': 'First_Period_Grade',
'G2': 'Second_Period_Grade',
'G3': 'Final_Grade'
}, inplace=True)
# Display data types before conversion
print("Before Conversion:")
print(df.dtypes)
# Convert numerical columns to appropriate data types
df["age"] = df["age"].astype(int)
df["studytime"] = df["studytime"].astype(int)
df["failures"] = df["failures"].astype(int)
df["absences"] = df["absences"].astype(int)
df["First_Period_Grade"] = df["First_Period_Grade"].astype(int)
df["Second_Period_Grade"] = df["Second_Period_Grade"].astype(int)
df["Final_Grade"] = df["Final_Grade"].astype(int)
# Display data types after conversion
print("\nAfter Conversion:")
print(df.dtypes)
<img width="310" height="601" alt="Screenshot 2026-09-08 232907" src="https://github.com/user-attachments/assets/06a225c1-35d7-4eba-b363-f531d599f832" />
<img width="310" height="755" alt="image" src="https://github.com/user-attachments/assets/aea877fb-fe0c-4bc2-bcac-74cb62f9535b" />
