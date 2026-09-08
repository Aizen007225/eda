import pandas as pd
# Load dataset
df = pd.read_csv("student_data.csv")
# Select numerical columns
num_data = df.select_dtypes(include=['number'])
# Correlation Matrix
corr_matrix = num_data.corr()
print("Highly Correlated Variable Pairs\n")
for i in range(len(corr_matrix.columns)):
for j in range(i + 1, len(corr_matrix.columns)):
value = corr_matrix.iloc[i, j]
if value > 0.8 or value < -0.8:
Highly Correlated Variable Pairs
G1 <--> G2 = 0.85
G1 <--> G3 = 0.8
G2 <--> G3 = 0.9
print(corr_matrix.columns[i], "<-->", corr_matrix.columns[j])
<img width="252" height="95" alt="image" src="https://github.com/user-attachments/assets/cee7429f-8b37-4a4d-961b-44d21660af09" />
