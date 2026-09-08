import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = pd.read_csv("student_dataset.csv")
sns.pairplot(df, vars=["Age","Marks"], hue="Gender", diag_kind="hist")
plt.show()
<img width="791" height="560" alt="image" src="https://github.com/user-attachments/assets/31e9361c-4458-49ef-84c3-4b68cbf0634a" />
