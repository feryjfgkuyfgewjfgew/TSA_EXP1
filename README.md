# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("tsa.csv", parse_dates=["Date"])

plt.figure(figsize=(12, 6))
plt.plot(df["Date"], df["High"], label="Price", color="red")

plt.title("Microsoft stock High Price Over Time")
plt.xlabel("Date")
plt.ylabel("Price")
plt.grid(True)
plt.legend()
plt.tight_layout()

plt.show()
```
# OUTPUT:
<img width="1451" height="696" alt="Screenshot 2025-08-18 160955" src="https://github.com/user-attachments/assets/59977f9b-ed0a-4238-8912-a4026677906b" />







# RESULT:
Thus we have created the python code for plotting the time series of given data.
