# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.



# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

```
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
```
 Line Plot:
 ```
 marks=[13,45,63,78]
 student=['ABC','QOR','EFB','TOB']
 plt.plot(marks,student)
 plt.xlabel('Marks')
 plt.ylabel('Student name')
 plt.show()
 student=['A','B','C','D']
 attendence=[90,85,73,88]
 plt.plot(attendence,student)
 plt.xlabel('Attendence')
 plt.ylabel('Student name')
 plt.show()
```
<img width="594" height="734" alt="image" src="https://github.com/user-attachments/assets/20859879-e76c-4d0a-9de5-6da8d40e9b0c" />

 Scatter Plot:
 ```
 x=[10,20,30,40,50]
 y=[100,200,300,400,500]
 plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
 plt.show()
 x=np.arange(0,15)
 y=np.arange(0,15)
 x
 y
 plt.scatter(x,y,c='r')
 plt.xlabel('X axis')
 plt.ylabel('y axis')
 plt.title('Scatter plot')
 plt.show()
```

<img width="563" height="744" alt="image" src="https://github.com/user-attachments/assets/00136e87-3b45-4eb5-94a1-8847fe440de4" />

 Pie Chart:
 ```
 act=['eat','sleep','work','play']
 slices=[3,7,8,6]
 color=['r','y','g','b']
 plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
 plt.legend()
 plt.show()
 feedback=['Good','excellent','Perfect','Ok']
 slices=[4,10,3,8]
 color=['y','r','b','g']
 plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
 plt.legend()
 plt.show()
```
<img width="520" height="696" alt="image" src="https://github.com/user-attachments/assets/61677510-a404-40bc-86cf-030c18fd21cf" />


 Area Chart:
 ```
 x = [1, 2, 3, 4, 5]
 y1 = [10, 12, 14, 16, 18]
 y2 = [5, 7, 9, 11, 13]
 y3 = [2, 4, 6, 8, 10]
 plt.fill_between(x, y1, color='blue')
 plt.fill_between(x, y2, color='green')
 plt.plot(x, y1, color='red')
 plt.plot(x, y2, color='black')
 plt.legend(['y1','y2'])
 plt.show()
```

<img width="592" height="362" alt="image" src="https://github.com/user-attachments/assets/18ef38b6-2e63-4d35-b9c8-dbd1910d08f8" />


 Bar Chart:
 ```
 height = [10, 24, 36, 40, 5]
 names = ['one', 'two', 'three', 'four', 'five']
 c1=['red', 'green'] 
 c2=['b', 'g']
 plt.bar (names, height, width=0.8, color=c1)
 plt.xlabel('x - axis')
 plt.ylabel('y - axis')
 plt.title('My bar chart!')
 plt.show()
```
<img width="537" height="396" alt="image" src="https://github.com/user-attachments/assets/304cfc49-1af1-4f66-b275-9c120c9fbe2c" />


 Histogram:
 ```
 x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
 plt.hist(x, bins = 10, color='blue', alpha=0.5)
 plt.show()
```
<img width="537" height="354" alt="image" src="https://github.com/user-attachments/assets/db2ba0ac-3496-4aa0-8e65-a584dc085e8c" />

 Box Plot:
 ```
 np.random.seed(0)
 data=np.random.normal(loc=0, scale=1, size=100)
 data
```
<img width="534" height="306" alt="image" src="https://github.com/user-attachments/assets/7cf03619-586b-4e1e-9e0a-78cef8d7d017" />

```
 fig, ax= plt.subplots()
 ax.boxplot(data)
 ax.set_xlabel('Data')
 ax.set_ylabel('Values')
 ax.set_title('Box Plot')
```

<img width="543" height="404" alt="image" src="https://github.com/user-attachments/assets/36f3636c-bae0-4c1c-bd86-2f4ff6d29a3f" />

# Summary:
In this experiment, various data visualization techniques were implemented using the Matplotlib library in Python. Different types of charts such as line plots, scatter plots, pie charts, area charts, bar charts, histograms, and box plots were created to represent and analyze data visually. These visualizations help in understanding patterns, trends, and relationships within the data more effectively. Thus, the experiment successfully demonstrated the use of Matplotlib for effective data visualization.

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
