: import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv("student_data.csv")
gender = df["sex"].value_counts()
plt.pie(gender, labels=gender.index, autopct="%1.1f%%")
plt.title("Pie Chart - Gender Distribution")
plt.show()
<img width="616" height="466" alt="image" src="https://github.com/user-attachments/assets/42d29b40-2d25-4fd5-b0c3-af3b63504711" />
