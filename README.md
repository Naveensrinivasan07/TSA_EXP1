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

# Example time series data
data = {
    'Date': pd.date_range(start='2023-01-01', periods=10, freq='D'),
    'Value': [10, 12, 9, 15, 18, 20, 17, 22, 25, 24]
}

# Create DataFrame
df = pd.DataFrame(data)

# Plot time series
plt.figure(figsize=(8,5))
plt.plot(df['Date'], df['Value'], marker='o', linestyle='-', color='blue')
plt.title('Time Series Plot')
plt.xlabel('Date')
plt.ylabel('Value')
plt.grid(True)
plt.show() 
```

# OUTPUT:

<img width="890" height="605" alt="image" src="https://github.com/user-attachments/assets/79e2e2ab-c19c-4b19-addc-406c47a7dc63" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
