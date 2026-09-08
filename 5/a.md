import pandas as pd
# Load dataset
df = pd.read_csv("student_data.csv")
# Select numerical columns
num_data = df.select_dtypes(include=['number'])
# Correlation Matrix
corr_matrix = num_data.corr()
print("Correlation Matrix")
print(corr_matrix)
<img width="738" height="730" alt="Screenshot 2026-09-08 233110" src="https://github.com/user-attachments/assets/bbf06e9b-277d-4973-85bb-149959bbcf3c" />
<img width="502" height="337" alt="image" src="https://github.com/user-attachments/assets/34760b9e-eaa9-4c7f-af85-2a29d5094641" />
