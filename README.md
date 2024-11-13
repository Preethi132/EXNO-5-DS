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
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1, y1, label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2, y2, label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
```
![image](https://github.com/user-attachments/assets/34420fd0-0026-4389-98e3-2f8b77e1c919)
```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y, color='blue', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='red', markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customization')
```
![image](https://github.com/user-attachments/assets/a0a90847-f2a9-406e-bbec-f79d2d76f6c7)
```
years=range(2000, 2012)
apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges=[0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectre)')
plt.title('Crops yield in Kento')
plt.legend(['Apples', 'Oranges'])
```
![image](https://github.com/user-attachments/assets/d9425c55-68ec-4c4e-887a-7d787d3f07e8)
```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
![image](https://github.com/user-attachments/assets/e13fa93c-b75b-44ca-b8e8-f3724b1e5d76)
```
import numpy as np
np.pi
```
![image](https://github.com/user-attachments/assets/0d618eb1-57fb-40ed-b3f6-17a83c0d9a95)
```
x=np.arange(0,4 * np.pi, 0.1)
y=np.sin(x)
plt.title('Sine Wave form')
plt.plot(x,y,'g--', linewidth=3)
```
![image](https://github.com/user-attachments/assets/76548834-ec0d-4ef0-8f62-238b853784b1)
```
import matplotlib.pyplot as plt
import numpy as np
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.fill_between(x,y1, color='blue')
plt.fill_between(x,y2, color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/fcc2d26b-7e55-4a3f-ba64-93fedfb662f4)
```
plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2', 'Line3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.xlabel('Y-axis')
```
![image](https://github.com/user-attachments/assets/ea2523fd-88b0-48c6-8f7f-3716229a6409)
```
height = [10,24,36,40,5]
names = ['one', 'two', 'three', 'four', 'five']
c1 = ['red', 'green']
c2 = ['b','g']
plt.bar(names, height, width=0.8, color=c1)

plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')

plt.show()
```
![image](https://github.com/user-attachments/assets/d6b9fc8c-d0ba-45d2-998a-e1f02ad0fc1c)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,label='Bars1',color='r')
plt.bar(x2,y2,label='Bars2',color='g')
plt.xlabel('Bar Number')
plt.ylabel('Bar Height')
plt.title('Bar Chart')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/0ddbcfef-900c-44bb-84ba-365deabf9cb0)
```
ages = [2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0,100)
bins = 10
plt.hist(ages, bins, range, color='g', histtype='bar', rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/5e83f990-775a-4db2-8153-bb4bf9ca7d32)
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
#plot for a histogram
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/427325b0-be27-4cca-834a-0fd868d24edc)
```
np.random.seed(0)
data = np.random.normal(loc=0, scale=1, size=100)
data
```
![image](https://github.com/user-attachments/assets/8dcbf297-ea2b-4432-8170-e12cb7d72382)
```
fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
plt.show()
```
![image](https://github.com/user-attachments/assets/769989bf-643a-43c0-85fa-e5f752180b4c)
```
activities = ['eat', 'sleep', 'work', 'play']
slices = [3, 7, 8, 6]
colors = ['r', 'y', 'g', 'b']
plt.pie (slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius= 1.2, autopct = '%1.1f%%')
plt.legend ()
plt.show()
```
![image](https://github.com/user-attachments/assets/39600b48-fdde-4377-8812-d02772d3246e)
```
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0.1, 0, 0, 0.2)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.2f%%', shadow=True)
# plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/3a943a9b-6fc3-4937-9f10-f919c5184d71)


# Result:
  We have performed Data Visualization using matplot python library for the given datas successfully.
