import pandas as pd
df = pd.read_csv("Pollution_TTest_Dataset.csv")
stats = df.groupby("Category")["Pollution"].agg(["count", "mean", "std", "min", "max"])
print("Pollution Statistics by Category")
print(stats)
<img width="612" height="172" alt="Screenshot 2026-09-08 224501" src="https://github.com/user-attachments/assets/a0c1b078-32f0-4fcc-8e5b-41e02d790b41" />
