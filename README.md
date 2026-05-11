# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries and create the dataset.

2. Select the input features for clustering.

3. Create the K-Means clustering model.

4. Train the model using the dataset.

5. Predict the clusters and display the clustered output.
 

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: Ranjani S
RegisterNumber:212225230224

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

# Employee dataset
data = {
    'EmployeeID': [1,2,3,4,5,6,7,8,9,10],
    'Salary': [25000,30000,35000,40000,45000,50000,55000,60000,65000,70000],
    'Experience': [1,2,2,3,4,5,6,7,8,9]
}

# Create DataFrame
df = pd.DataFrame(data)

# Features
X = df[['Salary', 'Experience']]

# K-Means Model
model = KMeans(n_clusters=3, random_state=42)
df['Cluster'] = model.fit_predict(X)

# Print clustered data
print(df)

# Visualization
plt.scatter(df['Salary'], df['Experience'],
            c=df['Cluster'], cmap='viridis')

plt.scatter(model.cluster_centers_[:,0],
            model.cluster_centers_[:,1],
            s=200, c='red', marker='X')

plt.title("Employee Segmentation using K-Means")
plt.xlabel("Salary")
plt.ylabel("Experience")
plt.show()

*/
```

## Output:

<img width="780" height="726" alt="Screenshot 2026-05-11 210351" src="https://github.com/user-attachments/assets/3b758c63-0cf2-4ccb-805a-beb9d8a98014" />


## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
