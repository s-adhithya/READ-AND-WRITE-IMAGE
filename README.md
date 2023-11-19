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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('kratos.jpeg',1)
cv2.imshow('212222240030',color_img)
cv2.waitKey(0) 

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('kratos.jpeg',1)
w= cv2.imwrite('0.png',color_img)
cv2.imshow('0',color_img)
cv2.waitKey(0)



```
iii) #Find the shape of the Image
```python3
import cv2
import random
color_img=cv2.imread('kratos.jpeg',1)
print(color_img.shape)



```
iv) #To access rows and columns

```python3
import cv2
import random
color_img=cv2.imread('kratos.jpeg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222240030',color_img)
cv2.waitKey(0)





```
v) #To cut and paste portion of image
```python3

import cv2
color_image=cv2.imread('kratos.jpeg',1)
tag=color_image[20:80,20:80]
color_image[90:150,90:150]=tag
cv2.imshow("212222240030",color_image)
cv2.waitKey(0)




```

## Output:

### i) Read and display the image
![image](https://github.com/s-adhithya/READ-AND-WRITE-IMAGE/assets/113497423/46dc3b8a-8b41-44f2-acb5-718535041d00)


### ii)Write the image
![image](https://github.com/s-adhithya/READ-AND-WRITE-IMAGE/assets/113497423/615ba75e-8449-4f87-8d08-61b61b0c6246)

### iii)Shape of the Image
![image](https://github.com/s-adhithya/READ-AND-WRITE-IMAGE/assets/113497423/c09555e4-13bc-48ee-b9a7-269a02d4b748)

### iv)Access rows and columns
![image](https://github.com/s-adhithya/READ-AND-WRITE-IMAGE/assets/113497423/0acbb267-3b47-4807-a067-b7c68f71e96b)

### v)Cut and paste portion of image
![image](https://github.com/s-adhithya/READ-AND-WRITE-IMAGE/assets/113497423/bed2924e-f9cc-457e-91e1-ce1566c90e7f)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
