# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY
# NAME: HARI PRASATH.P
# REG NO: 212224230084

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

# LINE PLOT:

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
<img width="521" height="733" alt="Screenshot 2025-10-29 031848" src="https://github.com/user-attachments/assets/06c8a1b5-3505-4b51-a328-af0aecfb239c" />




# Scatter Plot:
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
<img width="561" height="816" alt="Screenshot 2025-10-29 033550" src="https://github.com/user-attachments/assets/215df134-f5e0-4fd2-9bc4-a9a54556b528" />


# Pie Chart:
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

<img width="435" height="708" alt="Screenshot 2025-10-29 032016" src="https://github.com/user-attachments/assets/9c8b63f0-4485-404b-b391-6a6b38305a49" />



# Area Chart:
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
<img width="558" height="409" alt="Screenshot 2025-10-29 033753" src="https://github.com/user-attachments/assets/0e597aba-5649-43da-8ec9-2471626fc1c7" />




# Bar Chart:
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

<img width="524" height="383" alt="Screenshot 2025-10-29 032237" src="https://github.com/user-attachments/assets/a324c0aa-2fd1-4814-bc3a-21c244536bca" />

# Histogram:
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```
<img width="482" height="360" alt="Screenshot 2025-10-29 032321" src="https://github.com/user-attachments/assets/cfb0b85e-bfc6-4277-a5ca-9f6ccc6e0044" />


# Box Plot:
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```
<img width="717" height="443" alt="Screenshot 2025-10-29 091018" src="https://github.com/user-attachments/assets/a613ab98-4fd4-40fe-b6e7-664a8e375d7e" />




```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
<img width="617" height="461" alt="Screenshot 2025-10-29 032554" src="https://github.com/user-attachments/assets/f84f10b3-e6a7-4335-99e8-7c5e0a20c5d7" />



# Result:
  Thus, all the data visualization techniques of matplotlib has been implemented.
