import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv("Pollution_Dataset_7x7.csv")
df["Date"] = pd.to_datetime(df["Date"], dayfirst=True)
df.set_index("Date", inplace=True)
df["Rolling_Mean"] = df["Pollution"].rolling(window=7).mean()
plt.figure(figsize=(10,5))
plt.plot(df.index, df["Pollution"], label="Original Pollution")
plt.plot(df.index, df["Rolling_Mean"], linewidth=3, label="7-Day Rolling Mean")
plt.title("Pollution vs 7-Day Rolling Mean")
plt.xlabel("Date")
plt.ylabel("Pollution")
plt.legend()
plt.show()
<img width="605" height="305" alt="image" src="https://github.com/user-attachments/assets/8c4907ba-247e-4a85-8056-48ec9cb304a0" />
