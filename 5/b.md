import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
# Load dataset
df = pd.read_csv("student_data.csv")
# Select numerical columns
num_data = df.select_dtypes(include=['number'])
# Correlation Matrix
corr_matrix = num_data.corr()
# Heatmap
plt.figure(figsize=(10,8))
sns.heatmap(corr_matrix,
annot=True,
cmap="coolwarm",
fmt=".2f")
plt.title("Student Performance Correlation Matrix")
plt.show()
<img width="770" height="695" alt="image" src="https://github.com/user-attachments/assets/94d8a7cd-8471-4327-aa07-18a854d0b678" />
