import pandas as pd
# Load the student dataset
df = pd.read_csv("student_data.csv")
# Display original column names
print("Original Column Names:")
print(df.columns)
# Rename ambiguous column names
df.rename(columns={
'Medu': 'Mother_Education',
'Fedu': 'Father_Education',
'Mjob': 'Mother_Job',
'Fjob': 'Father_Job',
'G1': 'First_Period_Grade',
'G2': 'Second_Period_Grade',
'G3': 'Final_Grade'
}, inplace=True)
# Display updated column names
print("\nRenamed Column Names:")
print(df.columns)
<img width="787" height="467" alt="image" src="https://github.com/user-attachments/assets/7ff2c97c-df75-4daa-a702-9f67cfc10d0b" />
