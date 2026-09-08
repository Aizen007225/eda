import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv("student_data.csv")
plt.scatter(df["studytime"], df["G3"])
plt.xlabel("Study Time")
plt.ylabel("Final Grade")
plt.title("Scatter Plot - Study Time vs Final Grade")
plt.show()
<img width="790" height="602" alt="image" src="https://github.com/user-attachments/assets/561eebbb-ded8-48d5-bead-e9a62cfdba8e" />
