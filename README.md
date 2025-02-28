# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: NAVEENKUMAR V
### Register Number: 212221230068
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('sun2.jpg',1)
cv2.imshow('sun2',color_image)
cv2.waitKey(0)  

```
ii) #To write the image
```
import cv2
color_image = cv2.imread('sun2.jpg',1)
h = cv2.imwrite('sun2.jpg',color_image)
cv2.imshow('hari',color_image)
cv2.waitKey(0) 


```
iii) #Find the shape of the Image
```
import cv2
color_image = cv2.imread('sun2.jpg',1)
print(color_image.shape)


```
iv) #To access rows and columns

```
import random
import cv2
color_image = cv2.imread('sun2.jpg',1)
for i in range(150):
    for j in range(color_image.shape[1]):
        color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('sun2.jpg',color_image)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
color_image = cv2.imread('sun2.jpg',1)
part = color_image[300:400,300:400]
color_image[50:150,50:150] = part
cv2.imshow("hari",color_image)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image
![image](https://user-images.githubusercontent.com/94165322/232280001-5322f660-6c5c-452f-81d0-016c0dc41ba7.png)
![image](https://user-images.githubusercontent.com/94165322/232280011-4ee13efc-727b-44d0-a256-bd1304a0d9eb.png)




### ii)Write the image
![image](https://user-images.githubusercontent.com/94165322/232280018-fa13d6d0-7902-4d1a-aed2-68964d5dad17.png)




### iii)Shape of the Image

![image](https://user-images.githubusercontent.com/94165322/232280024-d211a2f1-27b7-41c0-81f0-38ee75709c6f.png)




### iv)Access rows and columns
![image](https://user-images.githubusercontent.com/94165322/232280031-d8e2e5a6-b6b9-4b2e-a80c-fcade59d8c7c.png)




### v)Cut and paste portion of image

![image](https://user-images.githubusercontent.com/94165322/232280037-58d3a471-a0bf-4bc0-b216-54acdf1253cc.png)



## Result:
Thus the images are read, displayed, and written successfully using the python program.


