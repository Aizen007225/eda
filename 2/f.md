import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv("student_data.csv")
plt.hist(df["G3"], bins=10, edgecolor="black")
plt.xlabel("Final Grade")
plt.ylabel("Number of Students")
plt.title("Histogram - Final Grade Distribution")
plt.show()
<img width="711" height="506" alt="image" src="https://github.com/user-attachments/assets/59dc3bd8-ab08-432a-92da-cabdc6a37ab7" />
