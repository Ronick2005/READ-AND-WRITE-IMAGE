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
img = cv2.imread('ai_dog.jpg', 1)
cv2.imshow('212222240084_Ronick', img)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
img = cv2.imread('ai_dog.jpg', 1)
new_img = cv2.imwrite('ai_dog_copy.jpg', img)
cv2.imshow('212222240084_Ronick', img)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```
import cv2
img = cv2.imread('ai_dog.jpg', 1)
print(img.shape)
```
iv) #To access rows and columns
```
import cv2
import random
img = cv2.imread('ai_dog.jpg', 1)
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
cv2.imshow('part image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) #To cut and paste portion of image
```
import cv2
img = cv2.imread('ai_dog.jpg', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('212222240084_Ronick', img)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image
![](ep1_op1.png)
### ii)Write the image
![](ep1_op2.png)
### iii)Shape of the Image
![](ep1_op3.png)
### iv)Access rows and columns
![](ep1_op4.png)
### v)Cut and paste portion of image
![](ep1_op5.png)
## Result:
Thus the images are read, displayed, and written successfully using the python program.
