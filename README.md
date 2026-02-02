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

import pandas as pd
import matplotlib.pyplot as plt


df = pd.read_csv(r"/content/car_price.csv")

df_clean = df.dropna(subset=["Year", "Mileage"])


plt.figure()
plt.scatter(df_clean["Year"], df_clean["Mileage"])
plt.xlabel("Year")   
plt.ylabel("Mileage")
plt.title("Year vs Mileage")

plt.show()








# OUTPUT:
![Uploading image.png…]()






# RESULT:
Thus we have created the python code for plotting the time series of given data.
