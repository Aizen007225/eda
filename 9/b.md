import pandas as pd
from scipy.stats import ttest_ind
df = pd.read_csv("Pollution_TTest_Dataset.csv")
urban = df[df["Category"]=="Urban"]["Pollution"]
rural = df[df["Category"]=="Rural"]["Pollution"]
t, p = ttest_ind(urban, rural)
alpha = 0.05
print("t-value:", t)
print("p-value:", p)
if p < alpha:
    print("Reject H0")
    print("Significant difference in Urban and Rural pollution.")
else:
    print("Fail to Reject H0")
    print("No significant difference in Urban and Rural pollution.")
    <img width="805" height="196" alt="Screenshot 2026-09-08 224409" src="https://github.com/user-attachments/assets/7da18156-fabe-4042-9fa1-951a165eec43" />
