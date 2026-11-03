# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 13/10/2026

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
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```
```
df = pd.read_csv("yahoo_stock.csv")
df.head()
```
```
x = pd.to_datetime(df['Date'])
y = df['Volume']
```
```
plt.plot(x, y, color="Blue")
plt.xlabel("Date")
plt.ylabel("Volume")
plt.title("Yahoo Stock Trading Volume")
plt.show()
```

# OUTPUT:
<img width="867" height="294" alt="image" src="https://github.com/user-attachments/assets/c97741cd-5d42-4c3d-b8a1-39c0328b5ce0" />

<img width="559" height="455" alt="image" src="https://github.com/user-attachments/assets/eae14a48-12ae-4928-80aa-5999e71bce27" />




# RESULT:
Thus we have created the python code for plotting the time series of given data.
