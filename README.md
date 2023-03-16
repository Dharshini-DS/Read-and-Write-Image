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
### Developed By: DHARSHINI.D.S
### Register Number: 212221230022
i) #To Read,display the image
```
import cv2
A=cv2.imread("img1.png",1)
cv2.imshow("Dharshini.DS",A)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
A=cv2.imread("img1.png",1)
cv2.imshow("Dharshini.DS",A)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```
import cv2
color_image = cv2.imread('img1.png',1)
print(color_image.shape)


```
iv) #To access rows and columns

```
import random
import cv2
A=cv2.imread("img1.png",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221230022",A)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```
import cv2
color_image = cv2.imread('img1.png',1)
part = color_image[300:400,300:400]
color_image[50:150,50:150] = part
cv2.imshow("dharshini.ds",color_image)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image

![exp1a](https://user-images.githubusercontent.com/93427345/225704699-41fa3530-49b1-444c-9e67-b61123c8fbf2.png)

### ii)Write the image

![exp1a](https://user-images.githubusercontent.com/93427345/225704794-ed8a26bb-fff6-4cef-9fa6-c292191796af.png)

### iii)Shape of the Image

![exp1b](https://user-images.githubusercontent.com/93427345/225704861-31b2ecdd-5bbc-4b88-a6fd-c1dbcd761a24.png)

### iv)Access rows and columns

![exp1c](https://user-images.githubusercontent.com/93427345/225704954-8458c424-1bcc-41d3-bd9b-3143defe0209.png)

### v)Cut and paste portion of image

![exp1d](https://user-images.githubusercontent.com/93427345/225705006-e368b2b0-6d15-4b80-8b05-73f874aa6903.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


