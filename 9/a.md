import pandas as pd
from scipy.stats import ttest_ind
df = pd.read_csv("Pollution_TTest_Dataset.csv")
urban = df[df["Category"] == "Urban"]["Pollution"]
rural = df[df["Category"] == "Rural"]["Pollution"]
t_value, p_value = ttest_ind(urban, rural)
print("t-value :", t_value)
print("p-value :", p_value)
<img width="792" height="77" alt="Screenshot 2026-09-08 224257" src="https://github.com/user-attachments/assets/de260c38-f912-48cc-aa7b-3a7d9b7b167a" />
