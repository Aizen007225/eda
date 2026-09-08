import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv("Pollution_Dataset_7x7.csv")
df["Date"] = pd.to_datetime(df["Date"], dayfirst=True)
df.set_index("Date", inplace=True)
df["Rolling_SD"] = df["Pollution"].rolling(window=7).std()
plt.figure(figsize=(10,5))
plt.plot(df.index, df["Rolling_SD"], linewidth=3)
plt.title("7-Day Rolling Standard Deviation of Pollution")
plt.xlabel("Date")
plt.ylabel("Standard Deviation")
plt.show()
<img width="581" height="327" alt="image" src="https://github.com/user-attachments/assets/edd32839-5c79-4973-a0e1-233369f23463" />
