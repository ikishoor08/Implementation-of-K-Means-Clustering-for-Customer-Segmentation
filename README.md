# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: KISHOOR I
RegisterNumber:  212225040190
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv(r"C:\College\SEM 2\Machine Learning\Exp10\Mall_Customers.csv")

print(data.head())

print(data.info())

data.isnull().sum()

from sklearn.cluster import KMeans
wcss = []

for i in range(1,11):
    kmeans = KMeans(n_clusters = i,init = "k-means++")
    kmeans.fit(data.iloc[:,3:])
    wcss.append(kmeans.inertia_)

plt.plot(range(1,11),wcss)
plt.xlabel("No of Cluster")
plt.ylabel("wcss")
plt.title("Elbow Method")
plt.figure()

km = KMeans(n_clusters = 5)
km.fit(data.iloc[:,3:])

KMeans(n_clusters=5)

y_pred = km.predict(data.iloc[:,3:])
print("Predicted values: \n",y_pred)

data["cluster"]=y_pred
df0 = data[data["cluster"]==0]
df1 = data[data["cluster"]==1]
df2 = data[data["cluster"]==2]
df3 = data[data["cluster"]==3]
df4 = data[data["cluster"]==4]
plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="black",label="cluster1")
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="blue",label="cluster2")
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")
plt.legend()
plt.title("Customer Segments")
plt.show()
*/

## Output:
```

<img width="692" height="128" alt="image" src="https://github.com/user-attachments/assets/90178dc2-b109-4abe-85e6-5d599ba00b51" />

<img width="692" height="128" alt="image" src="https://github.com/user-attachments/assets/9ee75edc-fb88-4666-b342-6e816f0e6f08" />

<img width="717" height="157" alt="image" src="https://github.com/user-attachments/assets/14368aab-ce37-4eb4-a1cb-b02488db233b" />

<img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/f60ed7b3-41b3-43df-8ad6-938838082101" /><img width="640" height="480" alt="image" src="https://github.com/user-attachments/assets/bfdb09cd-ab2b-46ff-8936-892769fb7d0f" />




```
## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
