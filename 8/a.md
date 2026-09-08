import pandas as pd
df = pd.read_csv("Pollution_Dataset.csv")
df["Date"] = pd.to_datetime(df["Date"], dayfirst=True)
df.set_index("Date", inplace=True)
df["Rolling_Mean"] = df["Pollution"].rolling(window=7).mean()
df["Rolling_SD"] = df["Pollution"].rolling(window=7).std()
print(df[["Pollution", "Rolling_Mean", "Rolling_SD"]])
<img width="480" height="251" alt="image" src="https://github.com/user-attachments/assets/72141e5d-a3d7-47b0-a27c-add508020c37" />
