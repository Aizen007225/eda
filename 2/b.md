import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv("student_data.csv")
data = df.head(7)
plt.bar(range(1, 8), data["G3"])
plt.xlabel("Student Number")
plt.ylabel("Final Grade")
plt.title("Bar Chart - Final Grades")
plt.show()
<img width="547" height="547" alt="image" src="https://github.com/user-attachments/assets/8c5580a8-913a-4d79-8fd7-cb9e60302a54" />
