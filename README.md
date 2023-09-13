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
```python
# Developed By: AMURTHA VAAHINI KN
# Register Number:212222240008
# To Read,display the image
import cv2
colorImage = cv2.imread('/Users/lenovo/Pictures/pic.jpg',1)
cv2.imshow('212221240033-Read&Display',colorImage)
cv2.waitKey(0)



# To write the image
import cv2
colorImage = cv2.imread('/Users/lenovo/Pictures/pic.jpg',1)
cv2.imwrite('/Users/lenovo/Pictures/written.jpg',colorImage)
writtenImage = cv2.imread('/Users/lenovo/Pictures/written.jpg',1)
cv2.imshow('212221240033-WrittenImage',writtenImage)
cv2.waitKey(0)




# Find the shape of the Image

import cv2
color=cv2.imread('/Users/lenovo/Pictures/pic.jpg',1)
print(color.shape)



# To access rows and columns
import cv2
import random
colorImage = cv2.imread('/Users/lenovo/Pictures/pic.jpg',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240033-AccessingRowsAndColumns',colorImage)
cv2.waitKey(0)





# To cut and paste portion of image
import cv2
color_img = cv2.imread('/Users/lenovo/Pictures/pic.jpg',1)
tag = color_img[20:80,20:80]
color_img[90:150,90:150] = tag
cv2.imshow('212221240033-CutAndPaste',color_img)
cv2.waitKey(0)









```
## Output:

### i) Read and display the image

![o](212221240033Read&Display.png)

### ii)Write the image
![o](212221240033-WrittenImage.png)


### iii)Shape of the Image
![o](shape.jpg)

### iv)Access rows and columns
![o](212221240033-AccessingRowsAndColumns.png)
### v)Cut and paste portion of image

![o](212221240033-CutAndPaste.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


