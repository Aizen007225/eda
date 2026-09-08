import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv("student_data.csv")
plt.boxplot(df["G3"])
plt.xlabel("Final Grade")
plt.ylabel("Marks")
plt.title("Box Plot - Final Grades")
plt.show()
<img width="822" height="630" alt="Screenshot 2026-09-08 231730" src="https://github.com/user-attachments/assets/2f7fb5ba-f011-4078-b8bb-2870717dc8aa" />
