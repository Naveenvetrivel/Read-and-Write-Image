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
![image](https://user-images.githubusercontent.com/94165322/226805575-67ebda91-19d3-465c-ba1b-3d96a94dde0a.png)



### ii)Write the image
![image](https://user-images.githubusercontent.com/94165322/226805648-97a383e1-7f8d-4566-a32b-e73cd392110f.png)



### iii)Shape of the Image

![image](https://user-images.githubusercontent.com/94165322/226805695-3c31c4ee-5672-43e7-8f58-d2702714fc68.png)



### iv)Access rows and columns
![image](https://user-images.githubusercontent.com/94165322/226805712-a5235664-76f1-47e4-9be4-1fb9840d6e5f.png)




### v)Cut and paste portion of image
![image](https://user-images.githubusercontent.com/94165322/226805752-011832c5-5909-4e33-a04c-1a2f1eed3875.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


